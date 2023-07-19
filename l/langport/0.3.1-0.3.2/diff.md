# Comparing `tmp/langport-0.3.1.tar.gz` & `tmp/langport-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.3.1.tar", last modified: Fri Jul 14 07:43:15 2023, max compression
+gzip compressed data, was "langport-0.3.2.tar", last modified: Wed Jul 19 09:19:59 2023, max compression
```

## Comparing `langport-0.3.1.tar` & `langport-0.3.2.tar`

### file list

```diff
@@ -1,145 +1,157 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.1/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5865 2023-07-14 07:43:15.120559 langport-0.3.1/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5365 2023-07-14 07:42:48.000000 langport-0.3.1/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.1/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.3.1/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.1/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.1/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.1/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.3.1/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.1/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.1/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6133 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/settings/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/mpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      286 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/settings/ningyu.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/settings/wizardlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.1/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.1/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/baichuan.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/codegen.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      840 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/ningyu.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/starcoder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/text2vec.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/wizardlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7287 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-07-13 17:09:49.000000 langport-0.3.1/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5276 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/generation/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    20845 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/generation/optimum.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2341 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7679 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1567 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/optimum.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-30 05:32:15.000000 langport-0.3.1/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-30 07:22:43.000000 langport-0.3.1/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.1/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.1/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/monkey_patch_non_inplace.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.1/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.1/langport/protocol/huggingface_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4665 2023-07-14 07:42:48.000000 langport-0.3.1/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.1/langport/protocol/tabby_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2948 2023-07-14 07:42:48.000000 langport-0.3.1/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.3.1/langport/routers/gateway/common.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16721 2023-07-14 07:42:48.000000 langport-0.3.1/langport/routers/gateway/openai_compatible.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.1/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3580 2023-07-14 07:42:48.000000 langport-0.3.1/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.1/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/cluster_monitor.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/cluster_monitor_app.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/graphite_feeder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/huggingface_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-25 16:41:24.000000 langport-0.3.1/langport/service/gateway/openai_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/tabby_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2614 2023-07-14 07:42:48.000000 langport-0.3.1/langport/service/server/generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3034 2023-07-14 07:42:48.000000 langport-0.3.1/langport/service/server/ggml_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2582 2023-07-14 07:42:48.000000 langport-0.3.1/langport/service/server/optimum_generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-07-14 07:42:48.000000 langport-0.3.1/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.3.1/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.1/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.1/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.3.1/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-07-14 07:42:48.000000 langport-0.3.1/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.3.1/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3175 2023-07-14 07:42:48.000000 langport-0.3.1/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5865 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4553 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-07-14 07:42:48.000000 langport-0.3.1/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-07-14 07:43:15.120559 langport-0.3.1/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.2/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5999 2023-07-19 09:19:59.248772 langport-0.3.2/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5499 2023-07-19 09:19:34.000000 langport-0.3.2/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.2/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.3.2/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.2/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.2/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.2/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.3.2/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.2/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.2/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     8139 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-07-14 07:42:48.000000 langport-0.3.2/langport/data/conversation/settings/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      274 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/settings/firefly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      354 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/settings/internlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/settings/llama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      286 2023-07-14 07:42:48.000000 langport-0.3.2/langport/data/conversation/settings/ningyu.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-07-14 07:42:48.000000 langport-0.3.2/langport/data/conversation/settings/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.2/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.2/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/baichuan.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/changgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      761 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/firefly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/internlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1528 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/llama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/longchat.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      840 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/ningyu.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/robin.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      635 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/snoozy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      651 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/tigerbot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    14471 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1756 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5837 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5276 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/executor/generation/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    20892 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/executor/generation/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2358 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     8620 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1584 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-30 05:32:15.000000 langport-0.3.2/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1461 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.2/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.2/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/monkey_patch_non_inplace.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2973 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/svd.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.2/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.2/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4665 2023-07-14 07:42:48.000000 langport-0.3.2/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.2/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2948 2023-07-14 07:42:48.000000 langport-0.3.2/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.3.2/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16352 2023-07-19 09:19:34.000000 langport-0.3.2/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.2/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3580 2023-07-14 07:42:48.000000 langport-0.3.2/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.2/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-25 16:41:24.000000 langport-0.3.2/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2220 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2766 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3184 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/ggml_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2731 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/optimum_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-07-14 07:42:48.000000 langport-0.3.2/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.3.2/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.2/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.2/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.3.2/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-07-19 09:19:34.000000 langport-0.3.2/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.3.2/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3175 2023-07-14 07:42:48.000000 langport-0.3.2/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5999 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4994 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-07-19 09:19:34.000000 langport-0.3.2/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-07-19 09:19:59.248772 langport-0.3.2/setup.cfg
```

### Comparing `langport-0.3.1/LICENSE` & `langport-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/PKG-INFO` & `langport-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.3.1
+Version: 0.3.2
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -42,39 +42,28 @@
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
 - Tabby-compatible RESTful APIs.
 
 ## Support Model Architectures
-* LLaMa
-* GLM
-* Bloom
-* OPT
-* GPT2
-* GPT Neo
-* GPT Big Code
+* LLaMa, LLaMa2, GLM, Bloom, OPT, GPT2, GPT Neo, GPT Big Code and so on.
 
 ## Tested Models
-* LLaMa
-* Vicuna
-* ChatGLM
-* ChatGLM2
-* Falcon
-* Starcoder
-* WizardLM
-* OpenBuddy
+* NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon, Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV, StableLM and so on.
+
 
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/07/16] Support int4 quantization.
 - [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.3.1 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.3.2 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
 Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -14,48 +14,50 @@
 training and evaluation make it complicated. The core features include: -
 Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
 serving system for state-of-the-art models. - Streaming generation support with
 various decoding strategies. - Batch inference for higher throughput. - Support
 for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
 RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
 RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
-LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
-LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
-## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
-V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
-server, and the following figure shows the Queries Per Second (QPS) and Tokens
-Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/07/13]
-Support generation logprobs parameter. - [2023/06/18] Add ggml (llama.cpp
-gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add LLama.cpp worker
-support. - [2023/06/01] Add HuggingFace Bert embedding worker support. - [2023/
-06/01] Add HuggingFace text generation API support. - [2023/06/01] Add tabby
-API support. - [2023/05/23] Add chat throughput test script. - [2023/05/22] New
-distributed architecture. - [2023/05/14] Batch inference supported. - [2023/05/
-10] Langport project started. ## Install ### Method 1: With pip ```bash pip
-install langport ``` or: ```bash pip install git+https://github.com/vtuber-
-plan/langport.git ``` If you need ggml generation worker, use this command:
-```bash pip install langport[ggml] ``` If you wanna use GPU: ```bash
-CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1. Clone
-this repository ```bash git clone https://github.com/vtuber-plan/langport.git
-cd langport ``` 2. Install the Package ```bash pip install --upgrade pip pip
-install -e . ``` ## Start the server It is simple to start a single node chat
-API service: ``` bash python -m langport.service.server.generation_worker --
-port 21001 --model-path  python -m langport.service.gateway.openai_api ``` If
-you need the embeddings API or other features, you can deploy a distributed
-inference cluster: ``` bash python -m langport.service.server.dummy_worker --
-port 21001 python -m langport.service.server.generation_worker --model-path  --
-neighbors http://localhost:21001 python -
-m langport.service.server.embedding_worker --model-path  --neighbors http://
-localhost:21001 python -m langport.service.gateway.openai_api --controller-
-address http://localhost:21001 ``` In practice, the gateway can connect to any
-node to distribute inference tasks: ``` bash python -
-m langport.service.server.dummy_worker --port 21001 python -
-m langport.service.server.generation_worker --port 21002 --model-path  --
-neighbors http://localhost:21001 python -
+LLaMa, LLaMa2, GLM, Bloom, OPT, GPT2, GPT Neo, GPT Big Code and so on. ##
+Tested Models * NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon,
+Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV,
+StableLM and so on. ## Benchmark We use single RTX3090 to run a finetuned 7B
+LLaMA model (OpenBuddy V0.9) under the bf16 setting. We create 32 threads to
+submit chat tasks to the server, and the following figure shows the Queries Per
+Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with
+different max model concurrency settings. ![benchmark_chat](assets/
+benchmark_chat.jpg) ## News - [2023/07/16] Support int4 quantization. - [2023/
+07/13] Support generation logprobs parameter. - [2023/06/18] Add ggml
+(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
+LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
+support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
+06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
+[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
+supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
+With pip ```bash pip install langport ``` or: ```bash pip install git+https://
+github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
+this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
+```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
+Clone this repository ```bash git clone https://github.com/vtuber-plan/
+langport.git cd langport ``` 2. Install the Package ```bash pip install --
+upgrade pip pip install -e . ``` ## Start the server It is simple to start a
+single node chat API service: ``` bash python -
+m langport.service.server.generation_worker --port 21001 --model-path  python -
+m langport.service.gateway.openai_api ``` If you need the embeddings API or
+other features, you can deploy a distributed inference cluster: ``` bash python
+-m langport.service.server.dummy_worker --port 21001 python -
+m langport.service.server.generation_worker --model-path  --neighbors http://
+localhost:21001 python -m langport.service.server.embedding_worker --model-path
+--neighbors http://localhost:21001 python -
+m langport.service.gateway.openai_api --controller-address http://localhost:
+21001 ``` In practice, the gateway can connect to any node to distribute
+inference tasks: ``` bash python -m langport.service.server.dummy_worker --port
+21001 python -m langport.service.server.generation_worker --port 21002 --model-
+path  --neighbors http://localhost:21001 python -
 m langport.service.server.generation_worker --port 21003 --model-path  --
 neighbors http://localhost:21001 http://localhost:21002 python -
 m langport.service.server.generation_worker --port 21004 --model-path  --
 neighbors http://localhost:21001 http://localhost:21003 python -
 m langport.service.server.generation_worker --port 21005 --model-path  --
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
```

### Comparing `langport-0.3.1/README.md` & `langport-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,39 +27,28 @@
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
 - Tabby-compatible RESTful APIs.
 
 ## Support Model Architectures
-* LLaMa
-* GLM
-* Bloom
-* OPT
-* GPT2
-* GPT Neo
-* GPT Big Code
+* LLaMa, LLaMa2, GLM, Bloom, OPT, GPT2, GPT Neo, GPT Big Code and so on.
 
 ## Tested Models
-* LLaMa
-* Vicuna
-* ChatGLM
-* ChatGLM2
-* Falcon
-* Starcoder
-* WizardLM
-* OpenBuddy
+* NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon, Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV, StableLM and so on.
+
 
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/07/16] Support int4 quantization.
 - [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
```

#### html2text {}

```diff
@@ -7,48 +7,50 @@
 training and evaluation make it complicated. The core features include: -
 Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
 serving system for state-of-the-art models. - Streaming generation support with
 various decoding strategies. - Batch inference for higher throughput. - Support
 for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
 RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
 RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
-LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
-LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
-## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
-V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
-server, and the following figure shows the Queries Per Second (QPS) and Tokens
-Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/07/13]
-Support generation logprobs parameter. - [2023/06/18] Add ggml (llama.cpp
-gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add LLama.cpp worker
-support. - [2023/06/01] Add HuggingFace Bert embedding worker support. - [2023/
-06/01] Add HuggingFace text generation API support. - [2023/06/01] Add tabby
-API support. - [2023/05/23] Add chat throughput test script. - [2023/05/22] New
-distributed architecture. - [2023/05/14] Batch inference supported. - [2023/05/
-10] Langport project started. ## Install ### Method 1: With pip ```bash pip
-install langport ``` or: ```bash pip install git+https://github.com/vtuber-
-plan/langport.git ``` If you need ggml generation worker, use this command:
-```bash pip install langport[ggml] ``` If you wanna use GPU: ```bash
-CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1. Clone
-this repository ```bash git clone https://github.com/vtuber-plan/langport.git
-cd langport ``` 2. Install the Package ```bash pip install --upgrade pip pip
-install -e . ``` ## Start the server It is simple to start a single node chat
-API service: ``` bash python -m langport.service.server.generation_worker --
-port 21001 --model-path  python -m langport.service.gateway.openai_api ``` If
-you need the embeddings API or other features, you can deploy a distributed
-inference cluster: ``` bash python -m langport.service.server.dummy_worker --
-port 21001 python -m langport.service.server.generation_worker --model-path  --
-neighbors http://localhost:21001 python -
-m langport.service.server.embedding_worker --model-path  --neighbors http://
-localhost:21001 python -m langport.service.gateway.openai_api --controller-
-address http://localhost:21001 ``` In practice, the gateway can connect to any
-node to distribute inference tasks: ``` bash python -
-m langport.service.server.dummy_worker --port 21001 python -
-m langport.service.server.generation_worker --port 21002 --model-path  --
-neighbors http://localhost:21001 python -
+LLaMa, LLaMa2, GLM, Bloom, OPT, GPT2, GPT Neo, GPT Big Code and so on. ##
+Tested Models * NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon,
+Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV,
+StableLM and so on. ## Benchmark We use single RTX3090 to run a finetuned 7B
+LLaMA model (OpenBuddy V0.9) under the bf16 setting. We create 32 threads to
+submit chat tasks to the server, and the following figure shows the Queries Per
+Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with
+different max model concurrency settings. ![benchmark_chat](assets/
+benchmark_chat.jpg) ## News - [2023/07/16] Support int4 quantization. - [2023/
+07/13] Support generation logprobs parameter. - [2023/06/18] Add ggml
+(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
+LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
+support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
+06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
+[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
+supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
+With pip ```bash pip install langport ``` or: ```bash pip install git+https://
+github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
+this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
+```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
+Clone this repository ```bash git clone https://github.com/vtuber-plan/
+langport.git cd langport ``` 2. Install the Package ```bash pip install --
+upgrade pip pip install -e . ``` ## Start the server It is simple to start a
+single node chat API service: ``` bash python -
+m langport.service.server.generation_worker --port 21001 --model-path  python -
+m langport.service.gateway.openai_api ``` If you need the embeddings API or
+other features, you can deploy a distributed inference cluster: ``` bash python
+-m langport.service.server.dummy_worker --port 21001 python -
+m langport.service.server.generation_worker --model-path  --neighbors http://
+localhost:21001 python -m langport.service.server.embedding_worker --model-path
+--neighbors http://localhost:21001 python -
+m langport.service.gateway.openai_api --controller-address http://localhost:
+21001 ``` In practice, the gateway can connect to any node to distribute
+inference tasks: ``` bash python -m langport.service.server.dummy_worker --port
+21001 python -m langport.service.server.generation_worker --port 21002 --model-
+path  --neighbors http://localhost:21001 python -
 m langport.service.server.generation_worker --port 21003 --model-path  --
 neighbors http://localhost:21001 http://localhost:21002 python -
 m langport.service.server.generation_worker --port 21004 --model-path  --
 neighbors http://localhost:21001 http://localhost:21003 python -
 m langport.service.server.generation_worker --port 21005 --model-path  --
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
```

### Comparing `langport-0.3.1/langport/constants.py` & `langport-0.3.2/langport/constants.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/core/base_node.py` & `langport-0.3.2/langport/core/base_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/core/cluster_node.py` & `langport-0.3.2/langport/core/cluster_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/core/cluster_worker.py` & `langport-0.3.2/langport/core/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/data/conversation/conversation_settings.py` & `langport-0.3.2/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/baichuan.py` & `langport-0.3.2/langport/model/adapters/baichuan.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/baize.py` & `langport-0.3.2/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/bard.py` & `langport-0.3.2/langport/model/adapters/bard.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/billa.py` & `langport-0.3.2/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/chatglm.py` & `langport-0.3.2/langport/model/adapters/chatglm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/chatgpt.py` & `langport-0.3.2/langport/model/adapters/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/claude.py` & `langport-0.3.2/langport/model/adapters/claude.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/dolly_v2.py` & `langport-0.3.2/langport/model/adapters/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/falcon.py` & `langport-0.3.2/langport/model/adapters/falcon.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/koala.py` & `langport-0.3.2/langport/model/adapters/koala.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 class KoalaAdapter(BaseAdapter):
     """The model adapter for koala"""
 
     def match(self, model_path: str):
         return "koala" in model_path
 
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("dolly_v2")
+        settings = get_conv_settings("koala_v1")
         return ConversationHistory(
             system="BEGINNING OF CONVERSATION:",
-            messages=(),
+            messages=[],
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.3.1/langport/model/adapters/ningyu.py` & `langport-0.3.2/langport/model/adapters/ningyu.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/oasst_pythia.py` & `langport-0.3.2/langport/model/adapters/oasst_pythia.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/openbuddy.py` & `langport-0.3.2/langport/model/adapters/openbuddy.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/phoenix.py` & `langport-0.3.2/langport/model/adapters/phoenix.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/rwkv.py` & `langport-0.3.2/langport/model/adapters/rwkv.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/stable_lm.py` & `langport-0.3.2/langport/model/adapters/stable_lm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/vicuna.py` & `langport-0.3.2/langport/model/adapters/vicuna.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/adapters/wizardlm.py` & `langport-0.3.2/langport/model/adapters/wizardlm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/executor/base.py` & `langport-0.3.2/langport/model/executor/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
-        load_8bit: bool = False,
+        quantization: Optional[str] = None,
         cpu_offloading: bool = False,
     ) -> None:
         super(LocalModelExecutor, self).__init__(
             model_name=model_name,
         )
 
         self.model_path = model_path
         self.device = device
         self.num_gpus = num_gpus
         self.max_gpu_memory = max_gpu_memory
-        self.load_8bit = load_8bit
+        self.quantization = quantization
         self.cpu_offloading = cpu_offloading
         
     @property
     def context_length(self) -> int:
         return 2048
 
     def tokenize(self, text: str) -> List[int]:
```

### Comparing `langport-0.3.1/langport/model/executor/embedding/__init__.py` & `langport-0.3.2/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/executor/embedding/huggingface.py` & `langport-0.3.2/langport/model/executor/embedding/huggingface.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,33 @@
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
-        load_8bit: bool,
+        quantization: Optional[str],
         cpu_offloading: bool,
         deepspeed: bool = False,
         trust_remote_code: bool = False,
     ) -> None:
         super(HuggingfaceEmbeddingExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device=device,
             num_gpus=num_gpus,
             max_gpu_memory=max_gpu_memory,
-            load_8bit=load_8bit,
+            quantization=quantization,
             cpu_offloading=cpu_offloading
         )
         self.adapter = None
         self.model = None
         self.tokenizer = None
         self.adapter, self.model, self.tokenizer = self.load_model(
-            model_path, device, num_gpus, max_gpu_memory, load_8bit, cpu_offloading, deepspeed, trust_remote_code
+            model_path, device, num_gpus, max_gpu_memory, quantization, cpu_offloading, deepspeed, trust_remote_code
         )
 
         if hasattr(self.model.config, "max_sequence_length"):
             self._context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self._context_len = self.model.config.max_position_embeddings
         else:
```

### Comparing `langport-0.3.1/langport/model/executor/generation/__init__.py` & `langport-0.3.2/langport/model/executor/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/executor/generation/chatgpt.py` & `langport-0.3.2/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/executor/generation/ggml.py` & `langport-0.3.2/langport/model/executor/generation/ggml.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/executor/generation/huggingface.py` & `langport-0.3.2/langport/model/executor/generation/huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             if (self.done[i] or generated_len % self.stream_interval != 0) and self.done[i]==self.task_batch.is_stop(i):
                 continue
             task = self.task_batch.tasks[i]
 
             token_ids = self.task_batch.get_generated_ids(i)
 
             # text = self.tokenizer.decode(token_ids, skip_special_tokens=True)
-            tokens = self.tokenizer.convert_ids_to_tokens(token_ids)
+            tokens = self.tokenizer.convert_ids_to_tokens(token_ids, skip_special_tokens=True)
             text = self.tokenizer.convert_tokens_to_string(tokens)
 
             # get offset mapping from token to text
             text_offset = []
             for token_i in range(0, len(tokens)):
                 if token_i == 0:
                     text_offset.append(-1)
@@ -473,33 +473,33 @@
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
-        load_8bit: bool,
+        quantization: Optional[str],
         cpu_offloading: bool,
         deepspeed: bool = False,
         trust_remote_code: bool = False
     ) -> None:
         super(HuggingfaceGenerationExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device=device,
             num_gpus=num_gpus,
             max_gpu_memory=max_gpu_memory,
-            load_8bit=load_8bit,
+            quantization=quantization,
             cpu_offloading=cpu_offloading
         )
         self.adapter = None
         self.model = None
         self.tokenizer = None
         self.adapter, self.model, self.tokenizer = self.load_model(
-            model_path, device, num_gpus, max_gpu_memory, load_8bit, cpu_offloading, deepspeed, trust_remote_code
+            model_path, device, num_gpus, max_gpu_memory, quantization, cpu_offloading, deepspeed, trust_remote_code
         )
 
         # self.model = torch.compile(self.model)
 
         if hasattr(self.model.config, "max_sequence_length"):
             self._context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
```

### Comparing `langport-0.3.1/langport/model/executor/generation/optimum.py` & `langport-0.3.2/langport/model/executor/generation/optimum.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/executor/ggml.py` & `langport-0.3.2/langport/model/executor/ggml.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,24 +26,24 @@
         num_gpus: int,
         max_gpu_memory: Optional[str],
         lib: Optional[str] = None,
         gpu_layers: int = 0,
         model_type: str = 'llama',
         chunk_size: int = 1024,
         threads: int = -1,
-        load_8bit: bool = False,
+        quantization: Optional[str] = None,
         cpu_offloading: bool = False,
     ) -> None:
         super(GgmlExecutor, self).__init__(
             model_name = model_name,
             model_path = model_path,
             device = device,
             num_gpus = num_gpus,
             max_gpu_memory = max_gpu_memory,
-            load_8bit = load_8bit,
+            quantization = quantization,
             cpu_offloading = cpu_offloading,
         )
         self.gpu_layers = gpu_layers
         # ctransformers has a bug
         self.lib = lib
         self.model_type = model_type
         self.chunk_size = chunk_size
```

### Comparing `langport-0.3.1/langport/model/executor/huggingface.py` & `langport-0.3.2/langport/model/executor/huggingface.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 import math
 from typing import Optional
 import warnings
 import psutil
 
 import torch
-from langport.model.compression import load_compress_model
+from langport.model.compression import load_compress_model, default_compression_config, bit4_compression_config
+from langport.model.svd import load_svd_model
 from langport.model.executor.base import BaseModelExecutor
 from langport.model.model_adapter import get_model_adapter, raise_warning_for_incompatible_cpu_offloading_configuration
 from langport.model.monkey_patch_non_inplace import replace_llama_attn_with_non_inplace_operations
 from langport.utils import get_gpu_memory
 
 
 
@@ -39,25 +40,25 @@
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
-        load_8bit: bool,
+        quantization: Optional[str],
         cpu_offloading: bool,
         deepspeed: bool = False,
     ) -> None:
         super(HuggingfaceExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device=device,
             num_gpus=num_gpus,
             max_gpu_memory=max_gpu_memory,
-            load_8bit=load_8bit,
+            quantization=quantization,
             cpu_offloading=cpu_offloading
         )
     
       
     def _load_hf_model(self, adapter, model_path: str, from_pretrained_kwargs: dict):
         if isinstance(adapter, DollyV2Adapter):
             tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
@@ -98,26 +99,26 @@
 
     def load_model(
         self,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str] = None,
-        load_8bit: bool = False,
+        quantization: Optional[str] = None,
         cpu_offloading: bool = False,
         deepspeed: bool = False,
         trust_remote_code: bool = False,
         debug: bool = False,
     ):
         """Load a model from Hugging Face."""
         adapter = get_model_adapter(model_path)
 
         # Handle device mapping
         cpu_offloading = raise_warning_for_incompatible_cpu_offloading_configuration(
-            device, load_8bit, cpu_offloading
+            device, quantization!=None, cpu_offloading
         )
         if device == "cpu":
             kwargs = {"torch_dtype": torch.float32}
         elif device == "cuda":
             kwargs = {"torch_dtype": torch.float16}
             if num_gpus != 1:
                 kwargs["device_map"] = "auto"
@@ -148,37 +149,47 @@
             if "max_memory" in kwargs:
                 kwargs["max_memory"]["cpu"] = (
                     str(math.floor(psutil.virtual_memory().available / 2**20)) + "Mib"
                 )
             kwargs["quantization_config"] = BitsAndBytesConfig(
                 load_in_8bit_fp32_cpu_offload=cpu_offloading
             )
-            kwargs["load_in_8bit"] = load_8bit
+            kwargs["load_in_8bit"] = quantization!=None
             # Load model
             model, tokenizer = self._load_hf_model(adapter, model_path, kwargs)
-        elif load_8bit:
+        elif quantization is not None:
             if num_gpus != 1:
                 warnings.warn(
-                    "8-bit quantization is not supported for multi-gpu inference."
+                    "n-bit quantization is not supported for multi-gpu inference."
                 )
             else:
-                model, tokenizer = load_compress_model(
-                    model_path=model_path, device=device, torch_dtype=kwargs["torch_dtype"]
-                )
+                if "8" in quantization:
+                    model, tokenizer = load_compress_model(
+                        model_path=model_path, device=device, torch_dtype=kwargs["torch_dtype"], compression_config=default_compression_config, trust_remote_code=trust_remote_code
+                    )
+                elif "4" in quantization:
+                    model, tokenizer = load_compress_model(
+                        model_path=model_path, device=device, torch_dtype=kwargs["torch_dtype"], compression_config=bit4_compression_config, trust_remote_code=trust_remote_code
+                    )
+                else:
+                    model, tokenizer = load_compress_model(
+                        model_path=model_path, device=device, torch_dtype=kwargs["torch_dtype"], compression_config=default_compression_config, trust_remote_code=trust_remote_code
+                    )
                 # return adapter, model, tokenizer
         else:
             # Load model
             model, tokenizer = self._load_hf_model(adapter, model_path, kwargs)
 
         if deepspeed:
             from transformers.deepspeed import HfDeepSpeedConfig
             import deepspeed
 
             dtype = torch.float16
-            if load_8bit:
+            # FIXME: deepspeed quantization
+            if quantization is not None:
                 dtype = torch.int8
             config = {
                 # "mp_size": 1,        # Number of GPU
                 "dtype": dtype, # dtype of the weights (fp16)
                 "replace_method": "auto", # Lets DS autmatically identify the layer to replace
                 "replace_with_kernel_inject": True, # replace the model with the kernel injector
                 "enable_cuda_graph": True,
```

### Comparing `langport-0.3.1/langport/model/executor/optimum.py` & `langport-0.3.2/langport/model/executor/optimum.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
-        load_8bit: bool = False,
+        quantization: Optional[str] = None,
         cpu_offloading: bool = False,
     ) -> None:
         super(OptimumExecutor, self).__init__(
             model_name = model_name,
             model_path = model_path,
             device = device,
             num_gpus = num_gpus,
             max_gpu_memory = max_gpu_memory,
-            load_8bit = load_8bit,
+            quantization = quantization,
             cpu_offloading = cpu_offloading,
         )
 
     def load_model(self, model_path: str, from_pretrained_kwargs: dict):
         adapter = get_model_adapter(model_path)
         
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
```

### Comparing `langport-0.3.1/langport/model/model_adapter.py` & `langport-0.3.2/langport/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/model_args.py` & `langport-0.3.2/langport/model/model_args.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,20 @@
         type=str,
         help="The maximum memory per gpu. Use a string like '13Gib'",
     )
     parser.add_argument(
         "--load-8bit", action="store_true", help="Use 8-bit quantization"
     )
     parser.add_argument(
+        "--load-4bit", action="store_true", help="Use 4-bit quantization"
+    )
+    parser.add_argument(
+        "--svd", action="store_true", help="Use SVD"
+    )
+    parser.add_argument(
         "--cpu-offloading",
         action="store_true",
         help="Only when using 8-bit quantization: Offload excess weights to the CPU that don't fit on the GPU",
     )
     parser.add_argument(
         "--deepspeed", action="store_true", help="Use deepspeed"
     )
```

### Comparing `langport-0.3.1/langport/model/models/rwkv_model.py` & `langport-0.3.2/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/model/monkey_patch_non_inplace.py` & `langport-0.3.2/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/protocol/huggingface_api_protocol.py` & `langport-0.3.2/langport/protocol/huggingface_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/protocol/openai_api_protocol.py` & `langport-0.3.2/langport/protocol/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/protocol/tabby_api_protocol.py` & `langport-0.3.2/langport/protocol/tabby_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/protocol/worker_protocol.py` & `langport-0.3.2/langport/protocol/worker_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/routers/gateway/common.py` & `langport-0.3.2/langport/routers/gateway/common.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/routers/gateway/openai_compatible.py` & `langport-0.3.2/langport/routers/gateway/openai_compatible.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,20 @@
 import asyncio
 
-import argparse
 import asyncio
 import json
-import logging
 
-import os
-import random
-import traceback
 from typing import Generator, Optional, Union, Dict, List, Any
 
-import fastapi
-from fastapi.middleware.cors import CORSMiddleware
-from fastapi.responses import StreamingResponse, JSONResponse
-from starlette.middleware.base import BaseHTTPMiddleware, DispatchFunction
+from fastapi.responses import StreamingResponse
 import httpx
-import numpy as np
 import shortuuid
-from starlette.types import ASGIApp
-from tenacity import retry, stop_after_attempt
-import uvicorn
-from pydantic import BaseSettings
 
 from langport.constants import WORKER_API_TIMEOUT, ErrorCode
 from langport.model.model_adapter import get_conversation_template
-from fastapi.exceptions import RequestValidationError
 from langport.protocol.openai_api_protocol import (
     ChatCompletionRequest,
     ChatCompletionResponse,
     ChatCompletionResponseStreamChoice,
     ChatCompletionStreamResponse,
     ChatMessage,
     ChatCompletionResponseChoice,
@@ -38,26 +24,23 @@
     CompletionResponseChoice,
     DeltaMessage,
     CompletionResponseStreamChoice,
     CompletionStreamResponse,
     EmbeddingsData,
     EmbeddingsRequest,
     EmbeddingsResponse,
-    ErrorResponse,
     ModelCard,
     ModelList,
     ModelPermission,
     UsageInfo,
 )
 from langport.protocol.worker_protocol import (
     BaseWorkerResult,
     EmbeddingWorkerResult,
     GenerationWorkerResult,
-    WorkerAddressRequest,
-    WorkerAddressResponse,
 )
 from langport.core.dispatch import DispatchMethod
 from langport.routers.gateway.common import LANGPORT_HEADER, AppSettings, _get_worker_address, _list_models, check_model, check_requests, create_error_response
 
 
 def get_gen_params(
     model_name: str,
@@ -100,22 +83,25 @@
         "prompt": prompt,
         "temperature": temperature,
         "top_p": top_p,
         "max_tokens": max_tokens,
         "echo": echo,
         "stream": stream,
         "logprobs": logprobs,
+        "stop_token_ids": conv.settings.stop_token_ids,
     }
 
     if stop is None:
         gen_params.update(
-            {"stop": conv.settings.stop_str, "stop_token_ids": conv.settings.stop_token_ids}
+            {"stop": conv.settings.stop_str}
         )
+    elif isinstance(stop, str):
+        gen_params.update({"stop": [stop, conv.settings.stop_str]})
     else:
-        gen_params.update({"stop": stop})
+        gen_params.update({"stop": stop + [conv.settings.stop_str]})
 
     return gen_params
 
 async def api_models(app_settings: AppSettings):
     async with httpx.AsyncClient() as client:
         models = await _list_models(app_settings, None, client)
     models.sort()
```

### Comparing `langport-0.3.1/langport/routers/server/core_node.py` & `langport-0.3.2/langport/routers/server/core_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/routers/server/embedding_node.py` & `langport-0.3.2/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/routers/server/generation_node.py` & `langport-0.3.2/langport/routers/server/generation_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/cluster_monitor.py` & `langport-0.3.2/langport/service/gateway/cluster_monitor.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/cluster_monitor_app.py` & `langport-0.3.2/langport/service/gateway/cluster_monitor_app.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/fauxpilot_api.py` & `langport-0.3.2/langport/service/gateway/fauxpilot_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/graphite_feeder.py` & `langport-0.3.2/langport/service/gateway/graphite_feeder.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/huggingface_api.py` & `langport-0.3.2/langport/service/gateway/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/openai_api.py` & `langport-0.3.2/langport/service/gateway/openai_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/gateway/tabby_api.py` & `langport-0.3.2/langport/service/gateway/tabby_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/server/chatgpt_generation_worker.py` & `langport-0.3.2/langport/service/server/chatgpt_generation_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     parser.add_argument("--model-name", default="gpt-3.5-turbo", type=str, help="Optional display name")
     parser.add_argument("--limit-model-concurrency", type=int, default=8)
     parser.add_argument("--batch", type=int, default=4)
     parser.add_argument("--stream-interval", type=int, default=2)
     args = parser.parse_args()
 
     node_id = str(uuid.uuid4())
-    logger = build_logger("generation_worker", f"generation_worker_{node_id}.log")
+    logger = build_logger("langport.service.chatgpt_generation_worker", f"chatgpt_generation_worker_{node_id}.log")
     logger.info(f"args: {args}")
 
     if args.port is None:
         args.port = random.randint(21001, 29001)
 
     if args.worker_address is None:
         args.worker_address = f"http://{args.host}:{args.port}"
```

### Comparing `langport-0.3.1/langport/service/server/dummy_worker.py` & `langport-0.3.2/langport/service/server/dummy_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/server/embedding_worker.py` & `langport-0.3.2/langport/service/server/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/service/server/generation_worker.py` & `langport-0.3.2/langport/service/server/generation_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,22 +41,29 @@
 
     if args.worker_address is None:
         args.worker_address = f"http://{args.host}:{args.port}"
     
     if args.model_name is None:
         args.model_name = os.path.basename(os.path.normpath(args.model_path))
     
+    if args.load_8bit:
+        quantization = "8bit"
+    elif args.load_4bit:
+        quantization = "4bit"
+    else:
+        quantization = None
+    
     from langport.model.executor.generation.huggingface import HuggingfaceGenerationExecutor
     executor = HuggingfaceGenerationExecutor(
         model_name=args.model_name,
         model_path=args.model_path,
         device=args.device,
         num_gpus=args.num_gpus,
         max_gpu_memory=args.max_gpu_memory,
-        load_8bit=args.load_8bit,
+        quantization=quantization,
         cpu_offloading=args.cpu_offloading,
         deepspeed=args.deepspeed,
         trust_remote_code=args.trust_remote_code
     )
     
     app.node = GenerationModelWorker(
         node_addr=args.worker_address,
```

### Comparing `langport-0.3.1/langport/service/server/ggml_generation_worker.py` & `langport-0.3.2/langport/service/server/ggml_generation_worker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
 import random
 import uuid
+import warnings
 import uvicorn
 
 from langport.workers.generation_worker import GenerationModelWorker
 from langport.model.model_args import add_model_args
 from langport.utils import build_logger
 from langport.routers.server.generation_node import app
 
@@ -37,14 +38,17 @@
 
     if args.gpus:
         if len(args.gpus.split(",")) < args.num_gpus:
             raise ValueError(
                 f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!"
             )
         os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
+    
+    if args.load_8bit or args.load_4bit:
+        warnings.warn("The ggml backend does not yet support quantization parameters.")
 
     if args.port is None:
         args.port = random.randint(21001, 29001)
 
     if args.worker_address is None:
         args.worker_address = f"http://{args.host}:{args.port}"
```

### Comparing `langport-0.3.1/langport/service/server/optimum_generation_worker.py` & `langport-0.3.2/langport/service/server/optimum_generation_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
 import random
 import uuid
+import warnings
 import uvicorn
 
 from langport.workers.generation_worker import GenerationModelWorker
 from langport.model.model_args import add_model_args
 from langport.utils import build_logger
 from langport.routers.server.generation_node import app
 
@@ -33,14 +34,17 @@
     if args.gpus:
         if len(args.gpus.split(",")) < args.num_gpus:
             raise ValueError(
                 f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!"
             )
         os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
 
+    if args.load_8bit or args.load_4bit:
+        warnings.warn("The optimum backend does not yet support quantization parameters.")
+
     if args.port is None:
         args.port = random.randint(21001, 29001)
 
     if args.worker_address is None:
         args.worker_address = f"http://{args.host}:{args.port}"
     
     if args.model_name is None:
```

### Comparing `langport-0.3.1/langport/utils/__init__.py` & `langport-0.3.2/langport/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/utils/evaluation.py` & `langport-0.3.2/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/utils/http_pool.py` & `langport-0.3.2/langport/utils/http_pool.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/utils/interval_timer.py` & `langport-0.3.2/langport/utils/interval_timer.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/workers/embedding_worker.py` & `langport-0.3.2/langport/workers/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport/workers/generation_worker.py` & `langport-0.3.2/langport/workers/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.1/langport.egg-info/PKG-INFO` & `langport-0.3.2/langport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.3.1
+Version: 0.3.2
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -42,39 +42,28 @@
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
 - Tabby-compatible RESTful APIs.
 
 ## Support Model Architectures
-* LLaMa
-* GLM
-* Bloom
-* OPT
-* GPT2
-* GPT Neo
-* GPT Big Code
+* LLaMa, LLaMa2, GLM, Bloom, OPT, GPT2, GPT Neo, GPT Big Code and so on.
 
 ## Tested Models
-* LLaMa
-* Vicuna
-* ChatGLM
-* ChatGLM2
-* Falcon
-* Starcoder
-* WizardLM
-* OpenBuddy
+* NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon, Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV, StableLM and so on.
+
 
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/07/16] Support int4 quantization.
 - [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.3.1 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.3.2 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
 Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -14,48 +14,50 @@
 training and evaluation make it complicated. The core features include: -
 Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
 serving system for state-of-the-art models. - Streaming generation support with
 various decoding strategies. - Batch inference for higher throughput. - Support
 for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
 RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
 RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
-LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
-LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
-## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
-V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
-server, and the following figure shows the Queries Per Second (QPS) and Tokens
-Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/07/13]
-Support generation logprobs parameter. - [2023/06/18] Add ggml (llama.cpp
-gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add LLama.cpp worker
-support. - [2023/06/01] Add HuggingFace Bert embedding worker support. - [2023/
-06/01] Add HuggingFace text generation API support. - [2023/06/01] Add tabby
-API support. - [2023/05/23] Add chat throughput test script. - [2023/05/22] New
-distributed architecture. - [2023/05/14] Batch inference supported. - [2023/05/
-10] Langport project started. ## Install ### Method 1: With pip ```bash pip
-install langport ``` or: ```bash pip install git+https://github.com/vtuber-
-plan/langport.git ``` If you need ggml generation worker, use this command:
-```bash pip install langport[ggml] ``` If you wanna use GPU: ```bash
-CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1. Clone
-this repository ```bash git clone https://github.com/vtuber-plan/langport.git
-cd langport ``` 2. Install the Package ```bash pip install --upgrade pip pip
-install -e . ``` ## Start the server It is simple to start a single node chat
-API service: ``` bash python -m langport.service.server.generation_worker --
-port 21001 --model-path  python -m langport.service.gateway.openai_api ``` If
-you need the embeddings API or other features, you can deploy a distributed
-inference cluster: ``` bash python -m langport.service.server.dummy_worker --
-port 21001 python -m langport.service.server.generation_worker --model-path  --
-neighbors http://localhost:21001 python -
-m langport.service.server.embedding_worker --model-path  --neighbors http://
-localhost:21001 python -m langport.service.gateway.openai_api --controller-
-address http://localhost:21001 ``` In practice, the gateway can connect to any
-node to distribute inference tasks: ``` bash python -
-m langport.service.server.dummy_worker --port 21001 python -
-m langport.service.server.generation_worker --port 21002 --model-path  --
-neighbors http://localhost:21001 python -
+LLaMa, LLaMa2, GLM, Bloom, OPT, GPT2, GPT Neo, GPT Big Code and so on. ##
+Tested Models * NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon,
+Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV,
+StableLM and so on. ## Benchmark We use single RTX3090 to run a finetuned 7B
+LLaMA model (OpenBuddy V0.9) under the bf16 setting. We create 32 threads to
+submit chat tasks to the server, and the following figure shows the Queries Per
+Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with
+different max model concurrency settings. ![benchmark_chat](assets/
+benchmark_chat.jpg) ## News - [2023/07/16] Support int4 quantization. - [2023/
+07/13] Support generation logprobs parameter. - [2023/06/18] Add ggml
+(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
+LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
+support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
+06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
+[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
+supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
+With pip ```bash pip install langport ``` or: ```bash pip install git+https://
+github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
+this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
+```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
+Clone this repository ```bash git clone https://github.com/vtuber-plan/
+langport.git cd langport ``` 2. Install the Package ```bash pip install --
+upgrade pip pip install -e . ``` ## Start the server It is simple to start a
+single node chat API service: ``` bash python -
+m langport.service.server.generation_worker --port 21001 --model-path  python -
+m langport.service.gateway.openai_api ``` If you need the embeddings API or
+other features, you can deploy a distributed inference cluster: ``` bash python
+-m langport.service.server.dummy_worker --port 21001 python -
+m langport.service.server.generation_worker --model-path  --neighbors http://
+localhost:21001 python -m langport.service.server.embedding_worker --model-path
+--neighbors http://localhost:21001 python -
+m langport.service.gateway.openai_api --controller-address http://localhost:
+21001 ``` In practice, the gateway can connect to any node to distribute
+inference tasks: ``` bash python -m langport.service.server.dummy_worker --port
+21001 python -m langport.service.server.generation_worker --port 21002 --model-
+path  --neighbors http://localhost:21001 python -
 m langport.service.server.generation_worker --port 21003 --model-path  --
 neighbors http://localhost:21001 http://localhost:21002 python -
 m langport.service.server.generation_worker --port 21004 --model-path  --
 neighbors http://localhost:21001 http://localhost:21003 python -
 m langport.service.server.generation_worker --port 21005 --model-path  --
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
```

### Comparing `langport-0.3.1/langport.egg-info/SOURCES.txt` & `langport-0.3.2/langport.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 langport/data/conversation/settings/bard.py
 langport/data/conversation/settings/billa.py
 langport/data/conversation/settings/chatglm.py
 langport/data/conversation/settings/chatgpt.py
 langport/data/conversation/settings/claude.py
 langport/data/conversation/settings/dolly.py
 langport/data/conversation/settings/falcon.py
+langport/data/conversation/settings/firefly.py
 langport/data/conversation/settings/h2ogpt.py
+langport/data/conversation/settings/internlm.py
 langport/data/conversation/settings/koala.py
+langport/data/conversation/settings/llama.py
 langport/data/conversation/settings/mpt.py
 langport/data/conversation/settings/ningyu.py
 langport/data/conversation/settings/oasst_pythia.py
 langport/data/conversation/settings/one_shot.py
 langport/data/conversation/settings/openbuddy.py
 langport/data/conversation/settings/phoenix.py
 langport/data/conversation/settings/redpajama.py
@@ -41,35 +44,44 @@
 langport/data/conversation/settings/wizardlm.py
 langport/data/conversation/settings/zero_shot.py
 langport/model/__init__.py
 langport/model/compression.py
 langport/model/model_adapter.py
 langport/model/model_args.py
 langport/model/monkey_patch_non_inplace.py
+langport/model/svd.py
 langport/model/adapters/__init__.py
 langport/model/adapters/baichuan.py
 langport/model/adapters/baize.py
 langport/model/adapters/bard.py
 langport/model/adapters/billa.py
+langport/model/adapters/changgpt.py
 langport/model/adapters/chatglm.py
 langport/model/adapters/chatgpt.py
 langport/model/adapters/claude.py
 langport/model/adapters/codegen.py
 langport/model/adapters/dolly_v2.py
 langport/model/adapters/falcon.py
+langport/model/adapters/firefly.py
+langport/model/adapters/internlm.py
 langport/model/adapters/koala.py
+langport/model/adapters/llama.py
+langport/model/adapters/longchat.py
 langport/model/adapters/ningyu.py
 langport/model/adapters/oasst_pythia.py
 langport/model/adapters/openbuddy.py
 langport/model/adapters/phoenix.py
+langport/model/adapters/robin.py
 langport/model/adapters/rwkv.py
+langport/model/adapters/snoozy.py
 langport/model/adapters/stable_lm.py
 langport/model/adapters/starcoder.py
 langport/model/adapters/t5.py
 langport/model/adapters/text2vec.py
+langport/model/adapters/tigerbot.py
 langport/model/adapters/vicuna.py
 langport/model/adapters/wizardlm.py
 langport/model/executor/__init__.py
 langport/model/executor/base.py
 langport/model/executor/ggml.py
 langport/model/executor/huggingface.py
 langport/model/executor/optimum.py
```

### Comparing `langport-0.3.1/pyproject.toml` & `langport-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.3.1"
+version = "0.3.2"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

