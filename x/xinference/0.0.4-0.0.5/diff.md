# Comparing `tmp/xinference-0.0.4.tar.gz` & `tmp/xinference-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.0.4.tar", last modified: Fri Jul 14 12:15:56 2023, max compression
+gzip compressed data, was "xinference-0.0.5.tar", last modified: Wed Jul 19 11:33:37 2023, max compression
```

## Comparing `xinference-0.0.4.tar` & `xinference-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-14 12:15:47.000000 xinference-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-14 12:15:47.000000 xinference-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-14 12:15:56.718407 xinference-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-14 12:15:47.000000 xinference-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 12:15:47.000000 xinference-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-14 12:15:56.718407 xinference-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-14 12:15:47.000000 xinference-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-14 12:15:47.000000 xinference-0.0.4/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/locale/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/locale/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.714407 xinference-0.0.4/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-19 11:33:27.000000 xinference-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-19 11:33:27.000000 xinference-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-19 11:33:37.533058 xinference-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-19 11:33:27.000000 xinference-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-19 11:33:27.000000 xinference-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-19 11:33:37.537058 xinference-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-19 11:33:27.000000 xinference-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-19 11:33:27.000000 xinference-0.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.537058 xinference-0.0.5/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-19 11:33:37.537058 xinference-0.0.5/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.529058 xinference-0.0.5/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/orca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.533058 xinference-0.0.5/xinference/model/llm/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/pytorch/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/model/llm/wizardlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-19 11:33:27.000000 xinference-0.0.5/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:33:37.529058 xinference-0.0.5/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 11:33:37.000000 xinference-0.0.5/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.0.4/LICENSE` & `xinference-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/PKG-INFO` & `xinference-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.4
+Version: 0.0.5
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -16,26 +16,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: doc
 License-File: LICENSE
 
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
+
+English | [中文介绍](README_zh_CN.md)
 </div>
 <br />
 
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
@@ -73,15 +76,15 @@
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
 ```bash
 $ pip install "xinference[all]"
 ```
-"xinference[all]" installs all the necessary packages for serving models. If you want to achieve acceleration on 
+`xinference[all]` installs all the necessary packages for serving models. If you want to achieve acceleration on 
 different hardware, refer to the installation documentation of the corresponding package.
 - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
 - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
 
 
 ### Deployment
 You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
@@ -179,28 +182,31 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
-| Name                 | Type             | Language | Format | Size (in billions) | Quantization                           |
-| -------------------- |------------------|----------|--------|--------------------|----------------------------------------|
-| baichuan             | Foundation Model | en, zh   | ggmlv3 | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| chatglm              | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-| chatglm2             | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-| wizardlm-v1.0        | SFT Model        | en       | ggmlv3 | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| vicuna-v1.3          | SFT Model        | en       | ggmlv3 | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| orca                 | SFT Model        | en       | ggmlv3 | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| Name          | Type             | Language | Format  | Size (in billions) | Quantization                            |
+|---------------|------------------|----------|---------|--------------------|-----------------------------------------|
+| llama-2       | Foundation Model | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| baichuan      | Foundation Model | en, zh   | ggmlv3  | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| chatglm       | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
+| chatglm2      | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
+| wizardlm-v1.0 | SFT Model        | en       | ggmlv3  | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| wizardlm-v1.1 | SFT Model        | en       | ggmlv3  | 13                 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| vicuna-v1.3   | SFT Model        | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
-- SFT models provide both `generate` and `chat`.
+- RLHF and SFT models provide both `generate` and `chat`.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
 With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.4 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.0.5 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Software Development :: Libraries Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all License-
-File: LICENSE
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all Provides-
+Extra: doc License-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
   xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
   t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
  (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
-                    badge)](https://twitter.com/xorbitsio)
+        badge)](https://twitter.com/xorbitsio) English | [ä¸­æä»ç»]
+                               (README_zh_CN.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
 full potential of cutting-edge AI models. ![demo](assets/demo.gif)
@@ -44,15 +45,15 @@
 WebUI for seamless management and monitoring. ð **Distributed Deployment**:
 Excel in distributed deployment scenarios, allowing the seamless distribution
 of model inference across multiple devices or machines. ð **Built-in
 Integration with Third-Party Libraries**: Xorbits Inference seamlessly
 integrates with popular third-party libraries like LangChain and LlamaIndex.
 (Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
 It is highly recommended to create a new virtual environment to avoid
-conflicts. ```bash $ pip install "xinference[all]" ``` "xinference[all]"
+conflicts. ```bash $ pip install "xinference[all]" ``` `xinference[all]`
 installs all the necessary packages for serving models. If you want to achieve
 acceleration on different hardware, refer to the installation documentation of
 the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
 llama-cpp-python#installation-from-pypi-recommended) is required to run
 `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
 (https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
 `chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
@@ -95,25 +96,29 @@
 known to science may be larger still. Some scientists believe that the largest
 animals may not have a clear \"size\" in the same way that humans do, as their
 size can vary depending on the environment and the stage of their life." },
 "finish_reason": "None" } ], "usage": { "prompt_tokens": -1,
 "completion_tokens": -1, "total_tokens": -1 } } ``` See [examples](examples)
 for more examples. ## Builtin models To view the builtin models, run the
 following command: ```bash $ xinference list --all ``` | Name | Type | Language
-| Format | Size (in billions) | Quantization | | -------------------- |--------
-----------|----------|--------|--------------------|---------------------------
--------------| | baichuan | Foundation Model | en, zh | ggmlv3 | 7 | 'q2_K',
-'q3_K_L', ... , 'q6_K', 'q8_0' | | chatglm | SFT Model | en, zh | ggmlv3 | 6 |
-'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | chatglm2 | SFT Model | en, zh |
-ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT
-Model | en | ggmlv3 | 7, 13, 33 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
-vicuna-v1.3 | SFT Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K',
-'q8_0' | | orca | SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0',
-'q5_1', 'q8_0' | **NOTE**: - Xinference will download models automatically for
-you, and by default the models will be saved under `${USER}/.xinference/cache`.
-- Foundation models only provide interface `generate`. - SFT models provide
-both `generate` and `chat`. ## Roadmap Xinference is currently under active
-development. Here's a roadmap outlining our planned developments for the next
-few weeks: ### PyTorch Support With PyTorch integration, users will be able to
-seamlessly utilize PyTorch models from Hugging Face within Xinference. ###
-Langchain & LlamaIndex integration With Xinference, it will be much easier for
-users to use these libraries and build applications with LLMs.
+| Format | Size (in billions) | Quantization | |---------------|---------------
+---|----------|---------|--------------------|---------------------------------
+--------| | llama-2 | Foundation Model | en | ggmlv3 | 7, 13 | 'q2_K',
+'q3_K_L', ... , 'q6_K', 'q8_0' | | baichuan | Foundation Model | en, zh |
+ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | llama-2-chat | RLHF
+Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
+chatglm | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1',
+'q8_0' | | chatglm2 | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0',
+'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT Model | en | ggmlv3 | 7, 13, 33 |
+'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
+ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
+Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
+SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+**NOTE**: - Xinference will download models automatically for you, and by
+default the models will be saved under `${USER}/.xinference/cache`. -
+Foundation models only provide interface `generate`. - RLHF and SFT models
+provide both `generate` and `chat`. ## Roadmap Xinference is currently under
+active development. Here's a roadmap outlining our planned developments for the
+next few weeks: ### PyTorch Support With PyTorch integration, users will be
+able to seamlessly utilize PyTorch models from Hugging Face within Xinference.
+### Langchain & LlamaIndex integration With Xinference, it will be much easier
+for users to use these libraries and build applications with LLMs.
```

### Comparing `xinference-0.0.4/README.md` & `xinference-0.0.5/xinference.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,44 @@
+Metadata-Version: 2.1
+Name: xinference
+Version: 0.0.5
+Summary: Model Serving Made Easy
+Home-page: https://github.com/xorbitsai/inference
+Author: Qin Xuye
+Author-email: qinxuye@xprobe.io
+Maintainer: Qin Xuye
+Maintainer-email: qinxuye@xprobe.io
+License: Apache License 2.0
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: all
+Provides-Extra: doc
+License-File: LICENSE
+
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
+
+English | [中文介绍](README_zh_CN.md)
 </div>
 <br />
 
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
@@ -49,15 +76,15 @@
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
 ```bash
 $ pip install "xinference[all]"
 ```
-"xinference[all]" installs all the necessary packages for serving models. If you want to achieve acceleration on 
+`xinference[all]` installs all the necessary packages for serving models. If you want to achieve acceleration on 
 different hardware, refer to the installation documentation of the corresponding package.
 - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
 - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
 
 
 ### Deployment
 You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
@@ -155,28 +182,31 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
-| Name                 | Type             | Language | Format | Size (in billions) | Quantization                           |
-| -------------------- |------------------|----------|--------|--------------------|----------------------------------------|
-| baichuan             | Foundation Model | en, zh   | ggmlv3 | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| chatglm              | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-| chatglm2             | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-| wizardlm-v1.0        | SFT Model        | en       | ggmlv3 | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| vicuna-v1.3          | SFT Model        | en       | ggmlv3 | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| orca                 | SFT Model        | en       | ggmlv3 | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| Name          | Type             | Language | Format  | Size (in billions) | Quantization                            |
+|---------------|------------------|----------|---------|--------------------|-----------------------------------------|
+| llama-2       | Foundation Model | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| baichuan      | Foundation Model | en, zh   | ggmlv3  | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| chatglm       | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
+| chatglm2      | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
+| wizardlm-v1.0 | SFT Model        | en       | ggmlv3  | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| wizardlm-v1.1 | SFT Model        | en       | ggmlv3  | 13                 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| vicuna-v1.3   | SFT Model        | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
-- SFT models provide both `generate` and `chat`.
+- RLHF and SFT models provide both `generate` and `chat`.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
 With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
```

#### html2text {}

```diff
@@ -1,19 +1,32 @@
+Metadata-Version: 2.1 Name: xinference Version: 0.0.5 Summary: Model Serving
+Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
+Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
+qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Software Development :: Libraries Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all Provides-
+Extra: doc License-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
   xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
   t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
  (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
-                    badge)](https://twitter.com/xorbitsio)
+        badge)](https://twitter.com/xorbitsio) English | [ä¸­æä»ç»]
+                               (README_zh_CN.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
 full potential of cutting-edge AI models. ![demo](assets/demo.gif)
@@ -32,15 +45,15 @@
 WebUI for seamless management and monitoring. ð **Distributed Deployment**:
 Excel in distributed deployment scenarios, allowing the seamless distribution
 of model inference across multiple devices or machines. ð **Built-in
 Integration with Third-Party Libraries**: Xorbits Inference seamlessly
 integrates with popular third-party libraries like LangChain and LlamaIndex.
 (Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
 It is highly recommended to create a new virtual environment to avoid
-conflicts. ```bash $ pip install "xinference[all]" ``` "xinference[all]"
+conflicts. ```bash $ pip install "xinference[all]" ``` `xinference[all]`
 installs all the necessary packages for serving models. If you want to achieve
 acceleration on different hardware, refer to the installation documentation of
 the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
 llama-cpp-python#installation-from-pypi-recommended) is required to run
 `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
 (https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
 `chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
@@ -83,25 +96,29 @@
 known to science may be larger still. Some scientists believe that the largest
 animals may not have a clear \"size\" in the same way that humans do, as their
 size can vary depending on the environment and the stage of their life." },
 "finish_reason": "None" } ], "usage": { "prompt_tokens": -1,
 "completion_tokens": -1, "total_tokens": -1 } } ``` See [examples](examples)
 for more examples. ## Builtin models To view the builtin models, run the
 following command: ```bash $ xinference list --all ``` | Name | Type | Language
-| Format | Size (in billions) | Quantization | | -------------------- |--------
-----------|----------|--------|--------------------|---------------------------
--------------| | baichuan | Foundation Model | en, zh | ggmlv3 | 7 | 'q2_K',
-'q3_K_L', ... , 'q6_K', 'q8_0' | | chatglm | SFT Model | en, zh | ggmlv3 | 6 |
-'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | chatglm2 | SFT Model | en, zh |
-ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT
-Model | en | ggmlv3 | 7, 13, 33 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
-vicuna-v1.3 | SFT Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K',
-'q8_0' | | orca | SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0',
-'q5_1', 'q8_0' | **NOTE**: - Xinference will download models automatically for
-you, and by default the models will be saved under `${USER}/.xinference/cache`.
-- Foundation models only provide interface `generate`. - SFT models provide
-both `generate` and `chat`. ## Roadmap Xinference is currently under active
-development. Here's a roadmap outlining our planned developments for the next
-few weeks: ### PyTorch Support With PyTorch integration, users will be able to
-seamlessly utilize PyTorch models from Hugging Face within Xinference. ###
-Langchain & LlamaIndex integration With Xinference, it will be much easier for
-users to use these libraries and build applications with LLMs.
+| Format | Size (in billions) | Quantization | |---------------|---------------
+---|----------|---------|--------------------|---------------------------------
+--------| | llama-2 | Foundation Model | en | ggmlv3 | 7, 13 | 'q2_K',
+'q3_K_L', ... , 'q6_K', 'q8_0' | | baichuan | Foundation Model | en, zh |
+ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | llama-2-chat | RLHF
+Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
+chatglm | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1',
+'q8_0' | | chatglm2 | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0',
+'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT Model | en | ggmlv3 | 7, 13, 33 |
+'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
+ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
+Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
+SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+**NOTE**: - Xinference will download models automatically for you, and by
+default the models will be saved under `${USER}/.xinference/cache`. -
+Foundation models only provide interface `generate`. - RLHF and SFT models
+provide both `generate` and `chat`. ## Roadmap Xinference is currently under
+active development. Here's a roadmap outlining our planned developments for the
+next few weeks: ### PyTorch Support With PyTorch integration, users will be
+able to seamlessly utilize PyTorch models from Hugging Face within Xinference.
+### Langchain & LlamaIndex integration With Xinference, it will be much easier
+for users to use these libraries and build applications with LLMs.
```

### Comparing `xinference-0.0.4/setup.cfg` & `xinference-0.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 	click
 	tqdm
 	tabulate
 	requests
 	pydantic
 	fastapi
 	uvicorn
+	sse_starlette
 
 [options.packages.find]
 exclude = 
 	*.conftest*
 	*.tests.*
 	*.tests
 
@@ -45,19 +46,35 @@
 dev = 
 	cython>=0.29
 	pytest>=3.5.0
 	pytest-cov>=2.5.0
 	pytest-timeout>=1.2.0
 	pytest-forked>=1.0
 	pytest-asyncio>=0.14.0
+	ipython>=6.5.0
+	sphinx>=3.0.0,<5.0.0
+	pydata-sphinx-theme>=0.3.0
+	sphinx-intl>=0.9.9
+	jieba>=0.42.0
 	flake8>=3.8.0
 	black
 all = 
 	chatglm-cpp
 	llama-cpp-python
+	transformers
+	torch
+	accelerate
+	sentencepiece
+	transformers_stream_generator
+	cpm_kernels
+doc = 
+	ipython>=6.5.0
+	sphinx>=3.0.0,<5.0.0
+	pydata-sphinx-theme>=0.3.0
+	sphinx-intl>=0.9.9
 
 [options.entry_points]
 console_scripts = 
 	xinference = xinference.deploy.cmdline:cli
 	xinference-supervisor = xinference.deploy.cmdline:supervisor
 	xinference-worker = xinference.deploy.cmdline:worker
```

### Comparing `xinference-0.0.4/setup.py` & `xinference-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/versioneer.py` & `xinference-0.0.5/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/__init__.py` & `xinference-0.0.5/xinference/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/client.py` & `xinference-0.0.5/xinference/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,63 +9,76 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
+import json
 import uuid
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union
 
 import requests
 import xoscar as xo
 
 from .core.model import ModelActor
 from .core.service import SupervisorActor
 from .isolation import Isolation
 
 if TYPE_CHECKING:
     from .model import ModelSpec
     from .model.llm.chatglm import ChatglmCppGenerateConfig
     from .model.llm.core import LlamaCppGenerateConfig
+    from .model.llm.pytorch.core import PytorchGenerateConfig
     from .types import (
         ChatCompletion,
         ChatCompletionChunk,
         ChatCompletionMessage,
         Completion,
         CompletionChunk,
+        Embedding,
     )
 
 
 class ModelHandle:
     """
     A sync model interface (for rpc client) which provides type hints that makes it much easier to use xinference
     programmatically.
     """
 
     def __init__(self, model_ref: xo.ActorRefType["ModelActor"], isolation: Isolation):
         self._model_ref = model_ref
         self._isolation = isolation
 
 
-class LlamaCppModelHandle(ModelHandle):
+class GenerateModelHandle(ModelHandle):
     def generate(
-        self, prompt: str, generate_config: Optional["LlamaCppGenerateConfig"] = None
+        self,
+        prompt: str,
+        generate_config: Optional[
+            Union["LlamaCppGenerateConfig", "PytorchGenerateConfig"]
+        ] = None,
     ) -> Union["Completion", Iterator["CompletionChunk"]]:
         coro = self._model_ref.generate(prompt, generate_config)
         return self._isolation.call(coro)
 
+    def create_embedding(self, input: Union[str, List[str]]) -> "Embedding":
+        coro = self._model_ref.create_embedding(input)
+        return self._isolation.call(coro)
+
 
-class LlamaCppChatModelHandle(LlamaCppModelHandle):
+class ChatModelHandle(GenerateModelHandle):
     def chat(
         self,
         prompt: str,
         system_prompt: Optional[str] = None,
         chat_history: Optional[List["ChatCompletionMessage"]] = None,
-        generate_config: Optional["LlamaCppGenerateConfig"] = None,
+        generate_config: Optional[
+            Union["LlamaCppGenerateConfig", "PytorchGenerateConfig"]
+        ] = None,
     ) -> Union["ChatCompletion", Iterator["ChatCompletionChunk"]]:
         coro = self._model_ref.chat(
             prompt, system_prompt, chat_history, generate_config
         )
         return self._isolation.call(coro)
 
 
@@ -76,28 +89,53 @@
         chat_history: Optional[List["ChatCompletionMessage"]] = None,
         generate_config: Optional["ChatglmCppGenerateConfig"] = None,
     ) -> Union["ChatCompletion", Iterator["ChatCompletionChunk"]]:
         coro = self._model_ref.chat(prompt, chat_history, generate_config)
         return self._isolation.call(coro)
 
 
+def streaming_response_iterator(
+    response_lines: Iterator[bytes],
+) -> Iterator["CompletionChunk"]:
+    for line in response_lines:
+        line = line.strip()
+        if line.startswith(b"data:"):
+            data = json.loads(line.decode("utf-8").replace("data: ", "", 1))
+            yield data
+
+
+# Duplicate code due to type hint issues
+def chat_streaming_response_iterator(
+    response_lines: Iterator[bytes],
+) -> Iterator["ChatCompletionChunk"]:
+    for line in response_lines:
+        line = line.strip()
+        if line.startswith(b"data:"):
+            data = json.loads(line.decode("utf-8").replace("data: ", "", 1))
+            yield data
+
+
 class RESTfulModelHandle:
     """
     A sync model interface (for RESTful client) which provides type hints that makes it much easier to use xinference
     programmatically.
     """
 
     def __init__(self, model_uid: str, base_url: str):
         self._model_uid = model_uid
         self._base_url = base_url
 
 
-class RESTfulLlamaCppModelHandle(RESTfulModelHandle):
+class RESTfulGenerateModelHandle(RESTfulModelHandle):
     def generate(
-        self, prompt: str, generate_config: Optional["LlamaCppGenerateConfig"] = None
+        self,
+        prompt: str,
+        generate_config: Optional[
+            Union["LlamaCppGenerateConfig", "PytorchGenerateConfig"]
+        ] = None,
     ) -> Union["Completion", Iterator["CompletionChunk"]]:
         url = f"{self._base_url}/v1/completions"
         if generate_config is None:
             request_body = {"model": self._model_uid, "prompt": prompt}
         else:
             generate_config_dict = {}
             for key, value in generate_config.items():
@@ -109,25 +147,43 @@
             }
 
         response = requests.post(url, json=request_body)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to generate completion, detail: {response.json()['detail']}"
             )
+
+        if generate_config and generate_config.get("stream"):
+            return streaming_response_iterator(response.iter_lines())
+
+        response_data = response.json()
+        return response_data
+
+    def create_embedding(self, input: Union[str, List[str]]) -> "Embedding":
+        url = f"{self._base_url}/v1/embeddings"
+        request_body = {"model": self._model_uid, "input": input}
+        response = requests.post(url, json=request_body)
+        if response.status_code != 200:
+            raise RuntimeError(
+                f"Failed to create the embeddings, detail: {response.json()['detail']}"
+            )
+
         response_data = response.json()
         return response_data
 
 
-class RESTfulLlamaCppChatModelHandle(RESTfulLlamaCppModelHandle):
+class RESTfulChatModelHandle(RESTfulGenerateModelHandle):
     def chat(
         self,
         prompt: str,
         system_prompt: Optional[str] = None,
         chat_history: Optional[List["ChatCompletionMessage"]] = None,
-        generate_config: Optional["LlamaCppGenerateConfig"] = None,
+        generate_config: Optional[
+            Union["LlamaCppGenerateConfig", "PytorchGenerateConfig"]
+        ] = None,
     ) -> Union["ChatCompletion", Iterator["ChatCompletionChunk"]]:
         url = f"{self._base_url}/v1/chat/completions"
 
         if chat_history is None:
             chat_history = []
 
         if chat_history and chat_history[0]["role"] == "system":
@@ -153,14 +209,18 @@
             }
 
         response = requests.post(url, json=request_body)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to generate chat completion, detail: {response.json()['detail']}"
             )
+
+        if generate_config and generate_config.get("stream"):
+            return chat_streaming_response_iterator(response.iter_lines())
+
         response_data = response.json()
         return response_data
 
 
 class RESTfulChatglmCppChatModelHandle(RESTfulModelHandle):
     def chat(
         self,
@@ -188,14 +248,18 @@
             }
 
         response = requests.post(url, json=request_body)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to generate chat completion, detail: {response.json()['detail']}"
             )
+
+        if generate_config and generate_config.get("stream"):
+            return chat_streaming_response_iterator(response.iter_lines())
+
         response_data = response.json()
         return response_data
 
 
 class Client:
     def __init__(self, endpoint: str):
         restful_client = RESTfulClient(endpoint)
@@ -245,18 +309,18 @@
         model_spec: "ModelSpec" = self._isolation.call(
             self._supervisor_ref.describe_model(model_uid)
         )
         model_ref = self._isolation.call(self._supervisor_ref.get_model(model_uid))
 
         if model_spec.model_name == "chatglm" or model_spec.model_name == "chatglm2":
             return ChatglmCppChatModelHandle(model_ref, self._isolation)
-        elif model_spec.model_name == "baichuan":
-            return LlamaCppModelHandle(model_ref, self._isolation)
+        elif model_spec.model_name in ["baichuan", "baichuan-base", "llama-2"]:
+            return GenerateModelHandle(model_ref, self._isolation)
         else:
-            return LlamaCppChatModelHandle(model_ref, self._isolation)
+            return ChatModelHandle(model_ref, self._isolation)
 
 
 class RESTfulClient:
     def __init__(self, base_url):
         self.base_url = base_url
 
     @classmethod
@@ -266,15 +330,15 @@
 
     def list_models(self) -> Dict[str, Dict[str, Any]]:
         url = f"{self.base_url}/v1/models"
 
         response = requests.get(url)
         if response.status_code != 200:
             raise RuntimeError(
-                f"Failed to launch model, detail: {response.json()['detail']}"
+                f"Failed to list model, detail: {response.json()['detail']}"
             )
 
         response_data = response.json()
         return response_data
 
     def launch_model(
         self,
@@ -283,22 +347,26 @@
         model_format: Optional[str] = None,
         quantization: Optional[str] = None,
         **kwargs,
     ) -> str:
         url = f"{self.base_url}/v1/models"
 
         model_uid = self.gen_model_uid()
+
         payload = {
             "model_uid": model_uid,
             "model_name": model_name,
             "model_size_in_billions": model_size_in_billions,
             "model_format": model_format,
             "quantization": quantization,
-            "kwargs": kwargs,
         }
+
+        for key, value in kwargs.items():
+            payload[str(key)] = value
+
         response = requests.post(url, json=payload)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to launch model, detail: {response.json()['detail']}"
             )
 
         response_data = response.json()
@@ -332,11 +400,11 @@
         model_spec = response.json()
 
         if (
             model_spec["model_name"] == "chatglm"
             or model_spec["model_name"] == "chatglm2"
         ):
             return RESTfulChatglmCppChatModelHandle(model_uid, self.base_url)
-        elif model_spec["model_name"] == "baichuan":
-            return RESTfulLlamaCppModelHandle(model_uid, self.base_url)
+        elif model_spec["model_name"] in ["baichuan", "baichuan-base", "llama-2"]:
+            return RESTfulGenerateModelHandle(model_uid, self.base_url)
         else:
-            return RESTfulLlamaCppChatModelHandle(model_uid, self.base_url)
+            return RESTfulChatModelHandle(model_uid, self.base_url)
```

### Comparing `xinference-0.0.4/xinference/constants.py` & `xinference-0.0.5/xinference/constants.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/core/__init__.py` & `xinference-0.0.5/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/core/api.py` & `xinference-0.0.5/xinference/core/api.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/core/gradio.py` & `xinference-0.0.5/xinference/core/gradio.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 if TYPE_CHECKING:
     from ..types import ChatCompletionChunk, ChatCompletionMessage
 
 MODEL_TO_FAMILIES = dict(
     (model_family.model_name, model_family)
     for model_family in MODEL_FAMILIES
-    if model_family.model_name != "baichuan"
+    if model_family.model_name not in ["baichuan", "baichuan-base", "llama-2"]
 )
 
 
 class GradioApp:
     def __init__(
         self,
         supervisor_address: str,
@@ -399,29 +399,29 @@
 
         model_selection.change(
             select_model, inputs=[model_selection], outputs=[chat, model_uid]
         )
         return chat, model_text
 
     def _build_arena_with_launched(self, models: List[Tuple[str, ModelSpec]]):
-        with gr.Box():
-            with gr.Row():
-                chat_and_text = [
-                    self._build_single_with_launched(models, i)
-                    for i in range(self._gladiator_num)
-                ]
-                chats = [c[0] for c in chat_and_text]
-                texts = [c[1] for c in chat_and_text]
+        chat_and_text = []
+        with gr.Row():
+            for i in range(self._gladiator_num):
+                with gr.Column():
+                    chat_and_text.append(self._build_single_with_launched(models, i))
 
-            msg = gr.Textbox(label=self._locale("Input"))
+        chats = [c[0] for c in chat_and_text]
+        texts = [c[1] for c in chat_and_text]
 
-            def update_message(text_in: str):
-                return "", text_in, text_in
+        msg = gr.Textbox(label=self._locale("Input"))
 
-            msg.submit(update_message, inputs=[msg], outputs=[msg] + texts)
+        def update_message(text_in: str):
+            return "", text_in, text_in
+
+        msg.submit(update_message, inputs=[msg], outputs=[msg] + texts)
 
         gr.ClearButton(components=[msg] + chats + texts)
 
     def build(self):
         if self._use_launched_model:
             models = self._api.list_models()
             with gr.Blocks() as blocks:
@@ -430,15 +430,15 @@
                     msg = gr.Textbox(label=self._locale("Input"))
 
                     def update_message(text_in: str):
                         return "", text_in
 
                     msg.submit(update_message, inputs=[msg], outputs=[msg, model_text])
                     gr.ClearButton(components=[chat, msg, model_text])
-                if len(models) > 2:
+                if len(models) >= 2:
                     with gr.Tab(self._locale("Arena")):
                         self._build_arena_with_launched(models)
         else:
             with gr.Blocks() as blocks:
                 with gr.Tab(self._locale("Chat")):
                     self._build_single()
                 with gr.Tab(self._locale("Arena")):
```

### Comparing `xinference-0.0.4/xinference/core/model.py` & `xinference-0.0.5/xinference/core/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
-from typing import TYPE_CHECKING, Any, Generic, Iterator, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Generic, Iterator, List, Optional, TypeVar, Union
 
 import xoscar as xo
 
 if TYPE_CHECKING:
     from ..model.llm.core import Model
     from ..types import ChatCompletionChunk, CompletionChunk
 
@@ -88,14 +88,22 @@
         if not hasattr(self._model, "chat"):
             raise AttributeError(f"Model {self._model.model_spec} is not for chat.")
 
         return self._wrap_generator(
             getattr(self._model, "chat")(prompt, *args, **kwargs)
         )
 
+    async def create_embedding(self, input: Union[str, List[str]], *args, **kwargs):
+        if not hasattr(self._model, "create_embedding"):
+            raise AttributeError(
+                f"Model {self._model.model_spec} is not for creating embedding."
+            )
+
+        return getattr(self._model, "create_embedding")(input, *args, **kwargs)
+
     async def next(self) -> Union["ChatCompletionChunk", "CompletionChunk"]:
         try:
             assert self._generator is not None
             return next(self._generator)
         except StopIteration:
             self._generator = None
             raise Exception("StopIteration")
```

### Comparing `xinference-0.0.4/xinference/core/resource.py` & `xinference-0.0.5/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/core/restful_api.py` & `xinference-0.0.5/xinference/core/restful_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
 import logging
 import socket
 import threading
+from functools import partial
 from typing import Any, Dict, List, Literal, Optional, Union
 
+import anyio
 import gradio as gr
 import xoscar as xo
+from anyio.streams.memory import MemoryObjectSendStream
 from fastapi import APIRouter, FastAPI, HTTPException, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, Field
+from sse_starlette.sse import EventSourceResponse
 from typing_extensions import NotRequired, TypedDict
 from uvicorn import Config, Server
 
-from ..types import ChatCompletion, Completion
+from ..types import ChatCompletion, Completion, Embedding
 from .service import SupervisorActor
 
 logger = logging.getLogger(__name__)
 
 max_tokens_field = Field(
     default=128, ge=1, le=2048, description="The maximum number of tokens to generate."
 )
@@ -64,15 +69,15 @@
 top_k_field = Field(
     default=40,
     ge=0,
     description="Limit the next token selection to the K most probable tokens.\n\n"
     + "Top-k sampling is a text generation method that selects the next token only from the top k most likely tokens predicted by the model. It helps reduce the risk of generating low-probability or nonsensical tokens, but it may also limit the diversity of the output. A higher value for top_k (e.g., 100) will consider more tokens and lead to more diverse text, while a lower value (e.g., 10) will focus on the most probable tokens and generate more conservative text.",
 )
 
-repeat_penalty_field = Field(
+repetition_penalty_field = Field(
     default=1.1,
     ge=0.0,
     description="A penalty applied to each token that is already generated. This helps prevent the model from repeating itself.\n\n"
     + "Repeat penalty is a hyperparameter used to penalize the repetition of token sequences during text generation. It helps prevent the model from generating repetitive or monotonous text. A higher value (e.g., 1.5) will penalize repetitions more strongly, while a lower value (e.g., 0.9) will be more lenient.",
 )
 
 presence_penalty_field = Field(
@@ -135,31 +140,30 @@
     model: str
     n: Optional[int] = 1
     best_of: Optional[int] = 1
     user: Optional[str] = Field(None)
 
     # llama.cpp specific parameters
     top_k: int = top_k_field
-    repeat_penalty: float = repeat_penalty_field
+    repetition_penalty: float = repetition_penalty_field
     logit_bias_type: Optional[Literal["input_ids", "tokens"]] = Field(None)
 
     class Config:
         schema_extra = {
             "example": {
                 "prompt": "\n\n### Instructions:\nWhat is the capital of France?\n\n### Response:\n",
                 "stop": ["\n", "###"],
             }
         }
 
 
-# TODO: create embedding request and response
 class CreateEmbeddingRequest(BaseModel):
     model: str
     input: Union[str, List[str]] = Field(description="The input to embed.")
-    user: Optional[str]
+    user: Optional[str] = None
 
     class Config:
         schema_extra = {
             "example": {
                 "input": "The food was delicious and the waiter...",
             }
         }
@@ -189,15 +193,15 @@
 
     model: str
     n: Optional[int] = 1
     user: Optional[str] = Field(None)
 
     # llama.cpp specific parameters
     top_k: int = top_k_field
-    repeat_penalty: float = repeat_penalty_field
+    repetition_penalty: float = repetition_penalty_field
     logit_bias_type: Optional[Literal["input_ids", "tokens"]] = Field(None)
 
     class Config:
         schema_extra = {
             "example": {
                 "messages": [
                     {"role": "system", "content": "you are a helpful AI assistant"},
@@ -247,15 +251,18 @@
         self._router.add_api_route(
             "/v1/completions",
             self.create_completion,
             methods=["POST"],
             response_model=Completion,
         )
         self._router.add_api_route(
-            "/v1/embeddings", self.create_embedding, methods=["POST"]
+            "/v1/embeddings",
+            self.create_embedding,
+            methods=["POST"],
+            response_model=Embedding,
         )
         self._router.add_api_route(
             "/v1/chat/completions",
             self.create_chat_completion,
             methods=["POST"],
             response_model=ChatCompletion,
         )
@@ -290,44 +297,78 @@
                 "quantization": model_spec.quantization,
             }
         return models_dict
 
     async def describe_model(self, model_uid: str):
         try:
             return await self._supervisor_ref.describe_model(model_uid)
+
+        except ValueError as ve:
+            logger.error(str(ve), exc_info=True)
+            raise HTTPException(status_code=400, detail=str(ve))
+
         except Exception as e:
             logger.error(e, exc_info=True)
             raise HTTPException(status_code=500, detail=str(e))
 
     async def launch_model(self, request: Request) -> JSONResponse:
         payload = await request.json()
         model_uid = payload.get("model_uid")
         model_name = payload.get("model_name")
         model_size_in_billions = payload.get("model_size_in_billions")
         model_format = payload.get("model_format")
         quantization = payload.get("quantization")
-        kwargs = payload.get("kwargs", {}) or {}
+
+        exclude_keys = {
+            "model_uid",
+            "model_name",
+            "model_size_in_billions",
+            "model_format",
+            "quantization",
+        }
+
+        kwargs = {
+            key: value for key, value in payload.items() if key not in exclude_keys
+        }
+
+        if model_uid is None or model_uid is None:
+            raise HTTPException(
+                status_code=400,
+                detail="Invalid input. Please specify the model UID and the model name",
+            )
 
         try:
             await self._supervisor_ref.launch_builtin_model(
                 model_uid=model_uid,
                 model_name=model_name,
                 model_size_in_billions=model_size_in_billions,
                 model_format=model_format,
                 quantization=quantization,
                 **kwargs,
             )
+
+        except ValueError as ve:
+            logger.error(str(ve), exc_info=True)
+            raise HTTPException(status_code=400, detail=str(ve))
+        except RuntimeError as re:
+            logger.error(str(re), exc_info=True)
+            raise HTTPException(status_code=503, detail=str(re))
         except Exception as e:
-            logger.error(e, exc_info=True)
+            logger.error(str(e), exc_info=True)
             raise HTTPException(status_code=500, detail=str(e))
+
         return JSONResponse(content={"model_uid": model_uid})
 
     async def terminate_model(self, model_uid: str):
         try:
             await self._supervisor_ref.terminate_model(model_uid)
+        except ValueError as ve:
+            logger.error(str(ve), exc_info=True)
+            raise HTTPException(status_code=400, detail=str(ve))
+
         except Exception as e:
             logger.error(e, exc_info=True)
             raise HTTPException(status_code=500, detail=str(e))
 
     async def get_address(self):
         return self.address
 
@@ -340,34 +381,85 @@
             "logit_bias",
             "logit_bias_type",
             "user",
         }
         kwargs = body.dict(exclude=exclude)
 
         if body.logit_bias is not None:
-            raise NotImplementedError
+            raise HTTPException(status_code=501, detail="Not implemented")
+
         model_uid = body.model
 
         try:
             model = await self._supervisor_ref.get_model(model_uid)
+        except ValueError as ve:
+            logger.error(str(ve), exc_info=True)
+            raise HTTPException(status_code=400, detail=str(ve))
+
         except Exception as e:
             logger.error(e, exc_info=True)
             raise HTTPException(status_code=500, detail=str(e))
 
         if body.stream:
-            raise NotImplementedError
+            # create a pair of memory object streams
+            send_chan, recv_chan = anyio.create_memory_object_stream(10)
+
+            async def event_publisher(inner_send_chan: MemoryObjectSendStream):
+                async with inner_send_chan:
+                    try:
+                        iterator = await model.generate(body.prompt, kwargs)
+                        async for chunk in iterator:
+                            await inner_send_chan.send(dict(data=json.dumps(chunk)))
+                            if await request.is_disconnected():
+                                raise anyio.get_cancelled_exc_class()()
+                    except anyio.get_cancelled_exc_class() as e:
+                        logger.warning("disconnected")
+                        with anyio.move_on_after(1, shield=True):
+                            logger.warning(
+                                f"Disconnected from client (via refresh/close) {request.client}"
+                            )
+                            await inner_send_chan.send(dict(closing=True))
+                            raise e
+                    except Exception as e:
+                        raise HTTPException(status_code=500, detail=str(e))
+
+            return EventSourceResponse(
+                recv_chan, data_sender_callable=partial(event_publisher, send_chan)
+            )
+
         else:
             try:
                 return await model.generate(body.prompt, kwargs)
             except Exception as e:
                 logger.error(e, exc_info=True)
                 raise HTTPException(status_code=500, detail=str(e))
 
     async def create_embedding(self, request: CreateEmbeddingRequest):
-        raise NotImplementedError
+        model_uid = request.model
+
+        try:
+            model = await self._supervisor_ref.get_model(model_uid)
+        except ValueError as ve:
+            logger.error(str(ve), exc_info=True)
+            raise HTTPException(status_code=400, detail=str(ve))
+        except Exception as e:
+            logger.error(e, exc_info=True)
+            raise HTTPException(status_code=500, detail=str(e))
+
+        input = request.input
+
+        try:
+            embedding = await model.create_embedding(input)
+            return embedding
+        except RuntimeError as re:
+            logger.error(re, exc_info=True)
+            raise HTTPException(status_code=400, detail=str(re))
+        except Exception as e:
+            logger.error(e, exc_info=True)
+            raise HTTPException(status_code=500, detail=str(e))
 
     async def create_chat_completion(
         self,
         request: Request,
         body: CreateChatCompletionRequest,
     ):
         exclude = {
@@ -377,37 +469,73 @@
             "logit_bias",
             "logit_bias_type",
             "user",
         }
         kwargs = body.dict(exclude=exclude)
 
         if body.logit_bias is not None:
-            raise NotImplementedError
+            raise HTTPException(status_code=501, detail="Not implemented")
+
+        if (
+            not body.messages
+            or body.messages[-1].get("role") != "user"
+            or not body.messages[-1].get("content")
+        ):
+            raise HTTPException(
+                status_code=400, detail="Invalid input. Please specify the prompt."
+            )
+
+        prompt = body.messages[-1]["content"]
 
-        user_messages = [
-            msg["content"] for msg in body.messages if msg["role"] == "user"
-        ]
-        if user_messages:
-            prompt = user_messages[-1]
-        else:
-            raise HTTPException(status_code=400, detail="No prompt given")
         system_prompt = next(
             (msg["content"] for msg in body.messages if msg["role"] == "system"), None
         )
 
         chat_history = body.messages
 
         model_uid = body.model
+
         try:
             model = await self._supervisor_ref.get_model(model_uid)
+
+        except ValueError as ve:
+            logger.error(str(ve), exc_info=True)
+            raise HTTPException(status_code=400, detail=str(ve))
         except Exception as e:
             logger.error(e, exc_info=True)
             raise HTTPException(status_code=500, detail=str(e))
 
         if body.stream:
-            raise NotImplementedError
+            # create a pair of memory object streams
+            send_chan, recv_chan = anyio.create_memory_object_stream(10)
+
+            async def event_publisher(inner_send_chan: MemoryObjectSendStream):
+                async with inner_send_chan:
+                    try:
+                        iterator = await model.chat(
+                            prompt, system_prompt, chat_history, kwargs
+                        )
+                        async for chunk in iterator:
+                            await inner_send_chan.send(dict(data=json.dumps(chunk)))
+                            if await request.is_disconnected():
+                                raise anyio.get_cancelled_exc_class()()
+                    except anyio.get_cancelled_exc_class() as e:
+                        logger.warning("disconnected")
+                        with anyio.move_on_after(1, shield=True):
+                            logger.warning(
+                                f"Disconnected from client (via refresh/close) {request.client}"
+                            )
+                            await inner_send_chan.send(dict(closing=True))
+                            raise e
+                    except Exception as e:
+                        raise HTTPException(status_code=500, detail=str(e))
+
+            return EventSourceResponse(
+                recv_chan, data_sender_callable=partial(event_publisher, send_chan)
+            )
+
         else:
             try:
                 return await model.chat(prompt, system_prompt, chat_history, kwargs)
             except Exception as e:
                 logger.error(e, exc_info=True)
                 raise HTTPException(status_code=500, detail=str(e))
```

### Comparing `xinference-0.0.4/xinference/core/service.py` & `xinference-0.0.5/xinference/core/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,16 @@
             model_uid,
             model_name,
             str(model_size_in_billions) if model_size_in_billions else "",
             model_format,
             quantization,
         )
 
-        assert model_uid not in self._model_uid_to_worker
+        if model_uid in self._model_uid_to_worker:
+            raise ValueError(f"Model is already in the model list, uid: {model_uid}")
 
         worker_ref = await self._choose_worker()
         model_ref = yield worker_ref.launch_builtin_model(
             model_uid=model_uid,
             model_name=model_name,
             model_size_in_billions=model_size_in_billions,
             model_format=model_format,
@@ -142,27 +143,34 @@
                     )
                     self._worker_status.pop(address)
                     self._worker_address_to_worker.pop(address)
             await asyncio.sleep(5)
 
     @log
     async def terminate_model(self, model_uid: str):
-        assert model_uid in self._model_uid_to_worker
+        if model_uid not in self._model_uid_to_worker:
+            raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
         worker_ref = self._model_uid_to_worker[model_uid]
         await worker_ref.terminate_model(model_uid=model_uid)
         del self._model_uid_to_worker[model_uid]
 
     @log
     async def get_model(self, model_uid: str) -> xo.ActorRefType["ModelActor"]:
+        if model_uid not in self._model_uid_to_worker:
+            raise ValueError(f"Model not found in the model list, uid: {model_uid}")
+
         worker_ref = self._model_uid_to_worker[model_uid]
         return await worker_ref.get_model(model_uid=model_uid)
 
     @log
     async def describe_model(self, model_uid: str):
+        if model_uid not in self._model_uid_to_worker:
+            raise ValueError(f"Model not found in the model list, uid: {model_uid}")
+
         worker_ref = self._model_uid_to_worker[model_uid]
         return await worker_ref.describe_model(model_uid=model_uid)
 
     @log
     async def list_models(self) -> List[Tuple[str, ModelSpec]]:
         ret = []
         for worker in self._worker_address_to_worker.values():
@@ -284,17 +292,19 @@
         raise ValueError(
             f"Model not found, name: {model_name}, format: {model_format},"
             f" size: {model_size_in_billions}, quantization: {quantization}"
         )
 
     @log
     async def terminate_model(self, model_uid: str):
-        assert model_uid in self._model_uid_to_model
+        if model_uid not in self._model_uid_to_model:
+            raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
         model_ref = self._model_uid_to_model[model_uid]
+
         await xo.destroy_actor(model_ref)
         del self._model_uid_to_model[model_uid]
         del self._model_uid_to_model_spec[model_uid]
         for subpool_address in self._subpool_address_to_model_uids:
             if model_uid in self._subpool_address_to_model_uids[subpool_address]:
                 self._subpool_address_to_model_uids[subpool_address].remove(model_uid)
 
@@ -303,18 +313,24 @@
         ret = []
         for k, v in self._model_uid_to_model_spec.items():
             ret.append((k, v))
         return ret
 
     @log
     async def get_model(self, model_uid: str) -> xo.ActorRefType["ModelActor"]:
+        if model_uid not in self._model_uid_to_model:
+            raise ValueError(f"Model not found in the model list, uid: {model_uid}")
+
         return self._model_uid_to_model[model_uid]
 
     @log
     async def describe_model(self, model_uid: str) -> ModelSpec:
+        if model_uid not in self._model_uid_to_model:
+            raise ValueError(f"Model not found in the model list, uid: {model_uid}")
+
         return self._model_uid_to_model_spec[model_uid]
 
     async def report_status(self):
         status = await asyncio.to_thread(gather_node_info)
         await self._supervisor_ref.report_worker_status(self.address, status)
 
     async def _periodical_report_status(self):
```

### Comparing `xinference-0.0.4/xinference/deploy/__init__.py` & `xinference-0.0.5/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/deploy/cmdline.py` & `xinference-0.0.5/xinference/deploy/cmdline.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/deploy/local.py` & `xinference-0.0.5/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/deploy/supervisor.py` & `xinference-0.0.5/xinference/deploy/supervisor.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/deploy/test/__init__.py` & `xinference-0.0.5/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/deploy/utils.py` & `xinference-0.0.5/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/deploy/worker.py` & `xinference-0.0.5/xinference/deploy/worker.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/isolation.py` & `xinference-0.0.5/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/locale/__init__.py` & `xinference-0.0.5/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/locale/utils.py` & `xinference-0.0.5/xinference/locale/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/locale/zh_CN.json` & `xinference-0.0.5/xinference/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/model/__init__.py` & `xinference-0.0.5/xinference/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,17 @@
             model_size_in_billions or self.model_sizes_in_billions[0]
         )
         # by default, choose the most coarse-grained quantization.
         quantization = quantization or self.quantizations[0]
 
         url = self.url_generator(model_size_in_billions, quantization)
 
+        if self.model_format == "pytorch":
+            return url
+
         full_name = f"{str(self)}-{model_size_in_billions}b-{quantization}"
         save_path, meta_path = self.generate_cache_path(
             model_size_in_billions, quantization
         )
         if os.path.exists(meta_path) and os.path.exists(save_path):
             # TODO: verify the integrity.
             return save_path
```

### Comparing `xinference-0.0.4/xinference/model/llm/chatglm.py` & `xinference-0.0.5/xinference/model/llm/chatglm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/model/llm/core.py` & `xinference-0.0.5/xinference/model/llm/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import logging
 import platform
 from abc import abstractmethod
-from typing import TYPE_CHECKING, Any, Iterator, List, Optional, TypedDict, Union
+from typing import TYPE_CHECKING, Iterator, List, Optional, TypedDict, Union
 
 from ...types import (
     ChatCompletion,
     ChatCompletionChunk,
     ChatCompletionMessage,
     Completion,
     CompletionChunk,
+    Embedding,
 )
+from .utils import ChatModelDataProcessorMixin
 
 if TYPE_CHECKING:
     from llama_cpp import LogitsProcessorList, StoppingCriteriaList
 
     from .. import ModelSpec
 
 logger = logging.getLogger(__name__)
@@ -38,40 +40,25 @@
     7: 32,
     13: 40,
     30: 60,
     65: 80,
 }
 
 
-class StrictTypedDict(TypedDict):
-    def __setitem__(self, key: str, value: Any):  # type: ignore
-        if key not in self.__annotations__:
-            raise KeyError(f"Key '{key}' is not allowed in {self.__class__.__name__}")
-
-        expected_type = self.__annotations__[key]
-        if not isinstance(value, expected_type):
-            raise TypeError(
-                f"Value for key '{key}' must be of type '{expected_type.__name__}', "
-                f"not '{type(value).__name__}'"
-            )
-
-        super().__setitem__(key, value)
-
-
 class LlamaCppGenerateConfig(TypedDict, total=False):
     suffix: Optional[str]
     max_tokens: int
     temperature: float
     top_p: float
     logprobs: Optional[int]
     echo: bool
     stop: Optional[Union[str, List[str]]]
     frequency_penalty: float
     presence_penalty: float
-    repeat_penalty: float
+    repetition_penalty: float
     top_k: int
     stream: bool
     tfs_z: float
     mirostat_mode: int
     mirostat_tau: float
     mirostat_eta: float
     model: Optional[str]
@@ -100,14 +87,22 @@
 
 
 class Model(abc.ABC):
     def __init__(self, model_uid: str, model_spec: "ModelSpec", *args, **kwargs):
         self.model_uid = model_uid
         self.model_spec = model_spec
 
+    @staticmethod
+    def _is_darwin_and_apple_silicon():
+        return platform.system() == "Darwin" and platform.processor() == "arm"
+
+    @staticmethod
+    def _is_linux():
+        return platform.system() == "Linux"
+
     @abstractmethod
     def load(self):
         pass
 
 
 class LlamaCppModel(Model):
     def __init__(
@@ -126,22 +121,14 @@
         self._gpu_layers = SIZE_TO_GPU_LAYERS[closest_size]
         self._model_path = model_path
         self._llamacpp_model_config: LlamaCppModelConfig = self._sanitize_model_config(
             llamacpp_model_config
         )
         self._llm = None
 
-    @staticmethod
-    def _is_darwin_and_apple_silicon():
-        return platform.system() == "Darwin" and platform.processor() == "arm"
-
-    @staticmethod
-    def _is_linux():
-        return platform.system() == "Linux"
-
     def _can_apply_metal(self):
         return (
             self.model_spec.quantization == "q4_0"
             or self.model_spec.quantization == "q4_1"
         )
 
     def _can_apply_cublas(self):
@@ -154,14 +141,17 @@
         if llamacpp_model_config is None:
             llamacpp_model_config = LlamaCppModelConfig()
         if platform.system() == "Windows":
             llamacpp_model_config.setdefault("n_ctx", 512)
         else:
             llamacpp_model_config.setdefault("n_ctx", 2048)
 
+        llamacpp_model_config.setdefault("use_mmap", False)
+        llamacpp_model_config.setdefault("use_mlock", True)
+
         if self._is_darwin_and_apple_silicon() and self._can_apply_metal():
             llamacpp_model_config.setdefault("n_gpu_layers", 1)
         elif self._is_linux() and self._can_apply_cublas():
             llamacpp_model_config.setdefault("n_gpu_layers", self._gpu_layers)
 
         return llamacpp_model_config
 
@@ -192,125 +182,79 @@
             **self._llamacpp_model_config,
         )
 
     def generate(
         self, prompt: str, generate_config: Optional[LlamaCppGenerateConfig] = None
     ) -> Union[Completion, Iterator[CompletionChunk]]:
         def generator_wrapper(
-            _prompt: str, _generate_config: LlamaCppGenerateConfig
+            _prompt: str,
+            repeat_penalty: float,
+            _generate_config: LlamaCppGenerateConfig,
         ) -> Iterator[CompletionChunk]:
             assert self._llm is not None
-            for _completion_chunk in self._llm(prompt=_prompt, **_generate_config):
+            for _completion_chunk in self._llm(
+                prompt=_prompt, repeat_penalty=repeat_penalty, **_generate_config
+            ):
                 yield _completion_chunk
 
         logger.debug(
             "Enter generate, prompt: %s, generate config: %s", prompt, generate_config
         )
 
         generate_config = self._sanitize_generate_config(generate_config)
 
+        repeat_penalty = 1.1
+        if "repetition_penalty" in generate_config:
+            repeat_penalty = generate_config["repetition_penalty"]
+            generate_config.pop("repetition_penalty")
+
         stream = generate_config.get("stream", False)
         if not stream:
             assert self._llm is not None
-            completion = self._llm(prompt=prompt, **generate_config)
+            completion = self._llm(
+                prompt=prompt, repeat_penalty=repeat_penalty, **generate_config
+            )
 
             return completion
         else:
-            return generator_wrapper(prompt, generate_config)
+            return generator_wrapper(prompt, repeat_penalty, generate_config)
 
+    def create_embedding(self, input: Union[str, List[str]]) -> Embedding:
+        assert self._llm is not None
+        embedding = self._llm.create_embedding(input)
+        return embedding
 
-class LlamaCppChatModel(LlamaCppModel):
+
+class LlamaCppChatModel(LlamaCppModel, ChatModelDataProcessorMixin):
     def __init__(
         self,
         model_uid: str,
         model_spec: "ModelSpec",
         model_path: str,
         system_prompt: str,
         sep: str,
         user_name: str,
         assistant_name: str,
+        stop: Optional[Union[str, List[str]]] = None,
         llamacpp_model_config: Optional[LlamaCppModelConfig] = None,
     ):
         super().__init__(model_uid, model_spec, model_path, llamacpp_model_config)
         self._system_prompt: str = system_prompt
         self._sep: str = sep
         self._user_name: str = user_name
         self._assistant_name: str = assistant_name
+        self._stop = stop
 
-    def _to_prompt(
-        self,
-        prompt: str,
-        system_prompt: str,
-        chat_history: List[ChatCompletionMessage],
-    ):
-        ret = system_prompt
-        for message in chat_history:
-            role = message["role"]
-            content = message["content"]
-            ret += f"{self._sep}{role}: {content}"
-        ret += f"{self._sep}{self._user_name}: {prompt}"
-        ret += f"{self._sep}{self._assistant_name}:"
-        return ret
-
-    @staticmethod
-    def _convert_chat_completion_chunks_to_chat(
-        chunks: Iterator[CompletionChunk],
-    ) -> Iterator[ChatCompletionChunk]:
-        for i, chunk in enumerate(chunks):
-            if i == 0:
-                yield {
-                    "id": "chat" + chunk["id"],
-                    "model": chunk["model"],
-                    "created": chunk["created"],
-                    "object": "chat.completion.chunk",
-                    "choices": [
-                        {
-                            "index": 0,
-                            "delta": {
-                                "role": "assistant",
-                            },
-                            "finish_reason": None,
-                        }
-                    ],
-                }
-            yield {
-                "id": "chat" + chunk["id"],
-                "model": chunk["model"],
-                "created": chunk["created"],
-                "object": "chat.completion.chunk",
-                "choices": [
-                    {
-                        "index": 0,
-                        "delta": {
-                            "content": chunk["choices"][0]["text"],
-                        },
-                        "finish_reason": chunk["choices"][0]["finish_reason"],
-                    }
-                ],
-            }
-
-    @staticmethod
-    def _convert_text_completion_to_chat(completion: Completion) -> ChatCompletion:
-        return {
-            "id": "chat" + completion["id"],
-            "object": "chat.completion",
-            "created": completion["created"],
-            "model": completion["model"],
-            "choices": [
-                {
-                    "index": 0,
-                    "message": {
-                        "role": "assistant",
-                        "content": completion["choices"][0]["text"],
-                    },
-                    "finish_reason": completion["choices"][0]["finish_reason"],
-                }
-            ],
-            "usage": completion["usage"],
-        }
+    def _sanitize_generate_config(
+        self, generate_config: Optional[LlamaCppGenerateConfig]
+    ) -> LlamaCppGenerateConfig:
+        generate_config = super()._sanitize_generate_config(generate_config)
+        if self._stop:
+            generate_config["stop"] = self._stop
+        return generate_config
 
     def chat(
         self,
         prompt: str,
         system_prompt: Optional[str] = None,
         chat_history: Optional[List[ChatCompletionMessage]] = None,
         generate_config: Optional[LlamaCppGenerateConfig] = None,
```

### Comparing `xinference-0.0.4/xinference/model/llm/orca.py` & `xinference-0.0.5/xinference/model/llm/orca.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/model/llm/vicuna.py` & `xinference-0.0.5/xinference/model/llm/vicuna.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/model/llm/wizardlm.py` & `xinference-0.0.5/xinference/model/llm/wizardlm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference/types.py` & `xinference-0.0.5/xinference/types.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.4/xinference.egg-info/PKG-INFO` & `xinference-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,19 @@
-Metadata-Version: 2.1
-Name: xinference
-Version: 0.0.4
-Summary: Model Serving Made Easy
-Home-page: https://github.com/xorbitsai/inference
-Author: Qin Xuye
-Author-email: qinxuye@xprobe.io
-Maintainer: Qin Xuye
-Maintainer-email: qinxuye@xprobe.io
-License: Apache License 2.0
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
+
+English | [中文介绍](README_zh_CN.md)
 </div>
 <br />
 
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
@@ -73,15 +51,15 @@
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
 ```bash
 $ pip install "xinference[all]"
 ```
-"xinference[all]" installs all the necessary packages for serving models. If you want to achieve acceleration on 
+`xinference[all]` installs all the necessary packages for serving models. If you want to achieve acceleration on 
 different hardware, refer to the installation documentation of the corresponding package.
 - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
 - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
 
 
 ### Deployment
 You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
@@ -179,28 +157,31 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
-| Name                 | Type             | Language | Format | Size (in billions) | Quantization                           |
-| -------------------- |------------------|----------|--------|--------------------|----------------------------------------|
-| baichuan             | Foundation Model | en, zh   | ggmlv3 | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| chatglm              | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-| chatglm2             | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-| wizardlm-v1.0        | SFT Model        | en       | ggmlv3 | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| vicuna-v1.3          | SFT Model        | en       | ggmlv3 | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
-| orca                 | SFT Model        | en       | ggmlv3 | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| Name          | Type             | Language | Format  | Size (in billions) | Quantization                            |
+|---------------|------------------|----------|---------|--------------------|-----------------------------------------|
+| llama-2       | Foundation Model | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| baichuan      | Foundation Model | en, zh   | ggmlv3  | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| chatglm       | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
+| chatglm2      | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
+| wizardlm-v1.0 | SFT Model        | en       | ggmlv3  | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| wizardlm-v1.1 | SFT Model        | en       | ggmlv3  | 13                 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| vicuna-v1.3   | SFT Model        | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
-- SFT models provide both `generate` and `chat`.
+- RLHF and SFT models provide both `generate` and `chat`.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
 With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
```

#### html2text {}

```diff
@@ -1,31 +1,20 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.4 Summary: Model Serving
-Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
-Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
-qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Software Development :: Libraries Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all License-
-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
   xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
   t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
  (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
-                    badge)](https://twitter.com/xorbitsio)
+        badge)](https://twitter.com/xorbitsio) English | [ä¸­æä»ç»]
+                               (README_zh_CN.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
 full potential of cutting-edge AI models. ![demo](assets/demo.gif)
@@ -44,15 +33,15 @@
 WebUI for seamless management and monitoring. ð **Distributed Deployment**:
 Excel in distributed deployment scenarios, allowing the seamless distribution
 of model inference across multiple devices or machines. ð **Built-in
 Integration with Third-Party Libraries**: Xorbits Inference seamlessly
 integrates with popular third-party libraries like LangChain and LlamaIndex.
 (Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
 It is highly recommended to create a new virtual environment to avoid
-conflicts. ```bash $ pip install "xinference[all]" ``` "xinference[all]"
+conflicts. ```bash $ pip install "xinference[all]" ``` `xinference[all]`
 installs all the necessary packages for serving models. If you want to achieve
 acceleration on different hardware, refer to the installation documentation of
 the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
 llama-cpp-python#installation-from-pypi-recommended) is required to run
 `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
 (https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
 `chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
@@ -95,25 +84,29 @@
 known to science may be larger still. Some scientists believe that the largest
 animals may not have a clear \"size\" in the same way that humans do, as their
 size can vary depending on the environment and the stage of their life." },
 "finish_reason": "None" } ], "usage": { "prompt_tokens": -1,
 "completion_tokens": -1, "total_tokens": -1 } } ``` See [examples](examples)
 for more examples. ## Builtin models To view the builtin models, run the
 following command: ```bash $ xinference list --all ``` | Name | Type | Language
-| Format | Size (in billions) | Quantization | | -------------------- |--------
-----------|----------|--------|--------------------|---------------------------
--------------| | baichuan | Foundation Model | en, zh | ggmlv3 | 7 | 'q2_K',
-'q3_K_L', ... , 'q6_K', 'q8_0' | | chatglm | SFT Model | en, zh | ggmlv3 | 6 |
-'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | chatglm2 | SFT Model | en, zh |
-ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT
-Model | en | ggmlv3 | 7, 13, 33 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
-vicuna-v1.3 | SFT Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K',
-'q8_0' | | orca | SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0',
-'q5_1', 'q8_0' | **NOTE**: - Xinference will download models automatically for
-you, and by default the models will be saved under `${USER}/.xinference/cache`.
-- Foundation models only provide interface `generate`. - SFT models provide
-both `generate` and `chat`. ## Roadmap Xinference is currently under active
-development. Here's a roadmap outlining our planned developments for the next
-few weeks: ### PyTorch Support With PyTorch integration, users will be able to
-seamlessly utilize PyTorch models from Hugging Face within Xinference. ###
-Langchain & LlamaIndex integration With Xinference, it will be much easier for
-users to use these libraries and build applications with LLMs.
+| Format | Size (in billions) | Quantization | |---------------|---------------
+---|----------|---------|--------------------|---------------------------------
+--------| | llama-2 | Foundation Model | en | ggmlv3 | 7, 13 | 'q2_K',
+'q3_K_L', ... , 'q6_K', 'q8_0' | | baichuan | Foundation Model | en, zh |
+ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | llama-2-chat | RLHF
+Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
+chatglm | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1',
+'q8_0' | | chatglm2 | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0',
+'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT Model | en | ggmlv3 | 7, 13, 33 |
+'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
+ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
+Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
+SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+**NOTE**: - Xinference will download models automatically for you, and by
+default the models will be saved under `${USER}/.xinference/cache`. -
+Foundation models only provide interface `generate`. - RLHF and SFT models
+provide both `generate` and `chat`. ## Roadmap Xinference is currently under
+active development. Here's a roadmap outlining our planned developments for the
+next few weeks: ### PyTorch Support With PyTorch integration, users will be
+able to seamlessly utilize PyTorch models from Hugging Face within Xinference.
+### Langchain & LlamaIndex integration With Xinference, it will be much easier
+for users to use these libraries and build applications with LLMs.
```

### Comparing `xinference-0.0.4/xinference.egg-info/SOURCES.txt` & `xinference-0.0.5/xinference.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -35,10 +35,17 @@
 xinference/locale/__init__.py
 xinference/locale/utils.py
 xinference/locale/zh_CN.json
 xinference/model/__init__.py
 xinference/model/llm/__init__.py
 xinference/model/llm/chatglm.py
 xinference/model/llm/core.py
+xinference/model/llm/llama2.py
 xinference/model/llm/orca.py
+xinference/model/llm/utils.py
 xinference/model/llm/vicuna.py
-xinference/model/llm/wizardlm.py
+xinference/model/llm/wizardlm.py
+xinference/model/llm/pytorch/__init__.py
+xinference/model/llm/pytorch/baichuan.py
+xinference/model/llm/pytorch/core.py
+xinference/model/llm/pytorch/utils.py
+xinference/model/llm/pytorch/vicuna.py
```

