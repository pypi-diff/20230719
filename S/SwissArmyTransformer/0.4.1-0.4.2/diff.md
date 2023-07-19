# Comparing `tmp/SwissArmyTransformer-0.4.1.tar.gz` & `tmp/SwissArmyTransformer-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwissArmyTransformer-0.4.1.tar", last modified: Thu Jul 13 14:26:33 2023, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-q0ozjl1_/SwissArmyTransformer-0.4.2.tar", last modified: Wed Jul 19 11:34:58 2023, max compression
```

## Comparing `SwissArmyTransformer-0.4.1.tar` & `SwissArmyTransformer-0.4.2.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.417250 SwissArmyTransformer-0.4.1/
--rw-rw-r--   0 dm        (2000) dm        (2000)    11338 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/LICENSE
--rw-rw-r--   0 dm        (2000) dm        (2000)      191 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/MANIFEST.in
--rw-rw-r--   0 dm        (2000) dm        (2000)     9893 2023-07-13 14:26:33.416622 SwissArmyTransformer-0.4.1/PKG-INFO
--rw-rw-r--   0 dm        (2000) dm        (2000)     9521 2023-07-13 14:24:51.000000 SwissArmyTransformer-0.4.1/README.md
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.305028 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 dm        (2000) dm        (2000)     9893 2023-07-13 14:26:33.303612 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (2000) dm        (2000)     4934 2023-07-13 14:26:33.303909 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (2000) dm        (2000)        1 2023-07-13 14:26:33.304350 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (2000) dm        (2000)       90 2023-07-13 14:26:33.304731 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 dm        (2000) dm        (2000)        4 2023-07-13 14:26:33.305118 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 dm        (2000) dm        (2000)       89 2023-06-28 10:49:48.000000 SwissArmyTransformer-0.4.1/requirements.txt
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.306929 SwissArmyTransformer-0.4.1/sat/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      433 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    25746 2023-07-13 03:48:02.000000 SwissArmyTransformer-0.4.1/sat/arguments.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.310757 SwissArmyTransformer-0.4.1/sat/data_utils/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      288 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    15633 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/data_utils/configure_data.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     2676 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/datasets.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1894 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     7028 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/samplers.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     7129 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/webds.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.313895 SwissArmyTransformer-0.4.1/sat/generation/
--rwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     9777 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3218 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1709 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/magnify.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.316453 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      161 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     4300 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     7659 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     2270 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3201 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/utils.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     5187 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/helpers.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.319249 SwissArmyTransformer-0.4.1/sat/model/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      214 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/__init__.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.319954 SwissArmyTransformer-0.4.1/sat/model/attention/
--rw-rw-r--   0 dm        (2000) dm        (2000)      110 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/attention/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3654 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/attention/memory_efficient_attention.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    16317 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/model/base_model.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1731 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     5479 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.323231 SwissArmyTransformer-0.4.1/sat/model/finetune/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      187 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     2659 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/adapter.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     2019 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/ffadd.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3879 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/lora.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    12022 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/lora2.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1110 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1611 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)      391 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/mixins.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.323867 SwissArmyTransformer-0.4.1/sat/model/normalization/
--rw-rw-r--   0 dm        (2000) dm        (2000)       24 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/normalization/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      610 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/normalization/rms.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.339156 SwissArmyTransformer-0.4.1/sat/model/official/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      676 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/official/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     1923 2023-06-28 11:04:30.000000 SwissArmyTransformer-0.4.1/sat/model/official/bert_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    10409 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/cait_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     7173 2023-07-13 14:01:04.000000 SwissArmyTransformer-0.4.1/sat/model/official/chatglm2_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    11797 2023-07-13 14:01:05.000000 SwissArmyTransformer-0.4.1/sat/model/official/chatglm_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     7294 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/clip_model.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     9612 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     1310 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/distill_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3942 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/dpr_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     7369 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/eva2_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    13903 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3751 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/glm_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3488 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/gpt2_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     4648 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/gptneo_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     5239 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/model/official/llama_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     8336 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/mae_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      262 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/roberta_model.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    14715 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/t5_model.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     6254 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/vit_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     2969 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/yolos_model.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.342443 SwissArmyTransformer-0.4.1/sat/model/position_embedding/
--rw-rw-r--   0 dm        (2000) dm        (2000)      296 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     5388 2023-07-13 07:20:14.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     2713 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings_original.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     4078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     5021 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     1199 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/model/registry.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    29395 2023-07-13 12:51:21.000000 SwissArmyTransformer-0.4.1/sat/model/transformer.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.347753 SwissArmyTransformer-0.4.1/sat/mpu/
--rwxrwxr-x   0 dm        (2000) dm        (2000)     2263 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     4716 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     4018 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/mpu/data.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     6435 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/initialize.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    22165 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/layers.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     4136 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/mpu/mappings.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3898 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/operation.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3924 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/mpu/utils.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.350118 SwissArmyTransformer-0.4.1/sat/ops/
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1233 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/__init__.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.299962 SwissArmyTransformer-0.4.1/sat/ops/csrc/
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.351559 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/
--rw-rw-r--   0 dm        (2000) dm        (2000)      947 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
--rw-rw-r--   0 dm        (2000) dm        (2000)     5595 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_apply.cuh
--rw-rw-r--   0 dm        (2000) dm        (2000)     7076 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.352778 SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/
--rw-rw-r--   0 dm        (2000) dm        (2000)      336 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/compat.h
--rw-rw-r--   0 dm        (2000) dm        (2000)     6388 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/type_shim.h
--rw-rw-r--   0 dm        (2000) dm        (2000)    10712 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/fused_ema_adam.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1159 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/layernorm.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     2067 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/local_attention_function.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      578 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/memory_efficient_attention.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.354889 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/
--rw-rw-r--   0 dm        (2000) dm        (2000)     1982 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    28554 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/builder.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      957 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/fused_ema_adam.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      389 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/scaled_mask_softmax.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.355494 SwissArmyTransformer-0.4.1/sat/quantization/
--rw-rw-r--   0 dm        (2000) dm        (2000)       29 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/quantization/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    18674 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/quantization/kernels.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.357362 SwissArmyTransformer-0.4.1/sat/resources/
--rwxrwxr-x   0 dm        (2000) dm        (2000)       33 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/resources/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     6815 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/resources/download.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3531 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/resources/urls.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.358024 SwissArmyTransformer-0.4.1/sat/tokenization/
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3810 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/__init__.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.361007 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      303 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     5092 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1767 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     7095 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.364101 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 dm        (2000) dm        (2000)      167 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     7691 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    30392 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    12917 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     2453 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.301044 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.369743 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 dm        (2000) dm        (2000)  1021864 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 dm        (2000) dm        (2000)   723078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.393180 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 dm        (2000) dm        (2000)   231508 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 dm        (2000) dm        (2000)   231508 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 dm        (2000) dm        (2000)   456318 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 dm        (2000) dm        (2000)  1042301 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 dm        (2000) dm        (2000)   456318 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 dm        (2000) dm        (2000)   898823 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.401770 SwissArmyTransformer-0.4.1/sat/tokenization/glm/
--rwxrwxr-x   0 dm        (2000) dm        (2000)       87 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3272 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    23223 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    13844 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 dm        (2000) dm        (2000)    14571 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3271 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.404224 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 dm        (2000) dm        (2000)       40 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     9661 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     2295 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.408078 SwissArmyTransformer-0.4.1/sat/training/
--rwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/training/__init__.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    24074 2023-07-12 13:12:07.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_training.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)      392 2023-07-12 13:17:48.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 dm        (2000) dm        (2000)      999 2023-07-12 13:17:55.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 dm        (2000) dm        (2000)     1151 2023-07-12 13:18:02.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 dm        (2000) dm        (2000)     3475 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/training/learning_rates.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)    11576 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/training/model_io.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     4488 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/training/utils.py
--rwxrwxr-x   0 dm        (2000) dm        (2000)     9663 2023-07-13 12:52:36.000000 SwissArmyTransformer-0.4.1/sat/transformer_defaults.py
--rw-rw-r--   0 dm        (2000) dm        (2000)       38 2023-07-13 14:26:33.417402 SwissArmyTransformer-0.4.1/setup.cfg
--rw-rw-r--   0 dm        (2000) dm        (2000)      880 2023-07-13 14:21:56.000000 SwissArmyTransformer-0.4.1/setup.py
-drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.415271 SwissArmyTransformer-0.4.1/tests/
--rw-rw-r--   0 dm        (2000) dm        (2000)     2000 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_base_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     1530 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_inference.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      290 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_list_info.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     3104 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_mea.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      913 2023-06-28 16:44:01.000000 SwissArmyTransformer-0.4.1/tests/test_model_parallel.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     2134 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_nested_model.py
--rw-rw-r--   0 dm        (2000) dm        (2000)      611 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_speed.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     4078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_train.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     4078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_train_dp.py
--rw-rw-r--   0 dm        (2000) dm        (2000)     4336 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_train_nested.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.768708 SwissArmyTransformer-0.4.2/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.4.2/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      191 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9893 2023-07-19 11:34:58.768708 SwissArmyTransformer-0.4.2/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9521 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.712709 SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9893 2023-07-19 11:34:58.000000 SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4934 2023-07-19 11:34:58.000000 SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-07-19 11:34:58.000000 SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       90 2023-07-19 11:34:58.000000 SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-07-19 11:34:58.000000 SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       89 2023-06-28 07:19:19.000000 SwissArmyTransformer-0.4.2/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.712709 SwissArmyTransformer-0.4.2/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    25746 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.712709 SwissArmyTransformer-0.4.2/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15633 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2676 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.4.2/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/data_utils/samplers.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7129 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/data_utils/webds.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.716709 SwissArmyTransformer-0.4.2/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9777 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.716709 SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4300 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7659 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.4.2/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.4.2/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.716709 SwissArmyTransformer-0.4.2/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/model/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.716709 SwissArmyTransformer-0.4.2/sat/model/attention/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      110 2023-06-06 14:36:22.000000 SwissArmyTransformer-0.4.2/sat/model/attention/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3654 2023-06-07 06:54:10.000000 SwissArmyTransformer-0.4.2/sat/model/attention/memory_efficient_attention.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    16317 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1731 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.716709 SwissArmyTransformer-0.4.2/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/lora.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12022 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/lora2.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1611 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      391 2023-06-06 14:36:32.000000 SwissArmyTransformer-0.4.2/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.720708 SwissArmyTransformer-0.4.2/sat/model/normalization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       24 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/model/normalization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      610 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/model/normalization/rms.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.724708 SwissArmyTransformer-0.4.2/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      676 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1923 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7173 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/official/chatglm2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11846 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.4.2/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13903 2023-06-06 13:57:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.2/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      978 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5113 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/official/llama_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.4.2/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.724708 SwissArmyTransformer-0.4.2/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5388 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2713 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/model/position_embedding/rotary_embeddings_original.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.4.2/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1199 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    29395 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.724708 SwissArmyTransformer-0.4.2/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2263 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6435 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    22165 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/mpu/mappings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3898 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/mpu/operation.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3924 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.724708 SwissArmyTransformer-0.4.2/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/ops/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.712709 SwissArmyTransformer-0.4.2/sat/ops/csrc/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      947 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5595 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/multi_tensor_apply.cuh
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7076 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/ops/csrc/includes/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      336 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/csrc/includes/compat.h
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     6388 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/csrc/includes/type_shim.h
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10712 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/fused_ema_adam.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/ops/local_attention_function.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      578 2023-06-07 05:52:48.000000 SwissArmyTransformer-0.4.2/sat/ops/memory_efficient_attention.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/ops/ops_builder/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1982 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/ops_builder/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    28554 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/ops_builder/builder.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      957 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.2/sat/ops/ops_builder/fused_ema_adam.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-06-05 05:26:26.000000 SwissArmyTransformer-0.4.2/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/quantization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.2/sat/quantization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.2/sat/quantization/kernels.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6815 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3531 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.4.2/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.728708 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.732709 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.712709 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.736708 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.756708 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.760708 SwissArmyTransformer-0.4.2/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.764708 SwissArmyTransformer-0.4.2/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.764708 SwissArmyTransformer-0.4.2/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.2/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24074 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      392 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      999 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1151 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.4.2/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11576 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.4.2/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9665 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.2/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-07-19 11:34:58.768708 SwissArmyTransformer-0.4.2/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-07-19 11:34:39.000000 SwissArmyTransformer-0.4.2/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-19 11:34:58.768708 SwissArmyTransformer-0.4.2/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.2/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.2/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3104 2023-06-07 06:54:04.000000 SwissArmyTransformer-0.4.2/tests/test_mea.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      913 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.2/tests/test_model_parallel.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.2/tests/test_nested_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.4.2/tests/test_speed.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.2/tests/test_train.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.4.2/tests/test_train_dp.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.2/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.4.1/LICENSE` & `SwissArmyTransformer-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/PKG-INFO` & `SwissArmyTransformer-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.4.1
+Version: 0.4.2
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.4.1/README.md` & `SwissArmyTransformer-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.4.1
+Version: 0.4.2
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.4.2/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/arguments.py` & `SwissArmyTransformer-0.4.2/sat/arguments.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.4.2/sat/data_utils/configure_data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.4.2/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.4.2/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.4.2/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/data_utils/webds.py` & `SwissArmyTransformer-0.4.2/sat/data_utils/webds.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.4.2/sat/generation/autoregressive_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.4.2/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/magnify.py` & `SwissArmyTransformer-0.4.2/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/base_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.4.2/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/generation/utils.py` & `SwissArmyTransformer-0.4.2/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/helpers.py` & `SwissArmyTransformer-0.4.2/sat/helpers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/attention/memory_efficient_attention.py` & `SwissArmyTransformer-0.4.2/sat/model/attention/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/base_model.py` & `SwissArmyTransformer-0.4.2/sat/model/base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.4.2/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.4.2/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.4.2/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.4.2/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.4.2/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/finetune/lora2.py` & `SwissArmyTransformer-0.4.2/sat/model/finetune/lora2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.4.2/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.4.2/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/normalization/rms.py` & `SwissArmyTransformer-0.4.2/sat/model/normalization/rms.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/__init__.py` & `SwissArmyTransformer-0.4.2/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/chatglm2_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/chatglm2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/chatglm_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
             output = hidden_states + mlp_output
 
         return output
     
 class ChatGLMModel(BaseModel):
     def __init__(self, args, transformer=None, **kwargs):
         super(ChatGLMModel, self).__init__(args, transformer=transformer, activation_func=gelu, **kwargs)
+        del self.transformer.position_embeddings
         self.add_mixin("chatglm-final", ChatGLMFinalMixin(args.vocab_size, args.hidden_size))
         self.add_mixin("chatglm-attn", ChatGLMAttnMixin(args.hidden_size, args.num_attention_heads))
         self.add_mixin("chatglm-layer", ChatGLMLayerMixin(args.num_layers))
         self.bos_token_id = args.bos_token_id
         self.mask_token_id = args.mask_token_id
         self.gmask_token_id = args.gmask_token_id
         self.pad_token_id = args.pad_token_id
```

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/glm130B_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/llama_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/llama_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from sat.model import BaseMixin, BaseModel
 import torch
 import torch.nn as nn
 
-from sat.model.official.gpt2_model import GPT2AttnMixin
-from sat.transformer_defaults import standard_attention
+from sat.transformer_defaults import attention_fn_default
 from sat.mpu.utils import split_tensor_along_last_dim
 from sat.model.position_embedding.rotary_embeddings import RotaryEmbedding, rotate_half
 import torch.nn.functional as F
 from sat.mpu import ColumnParallelLinear
 
 def apply_rotary_pos_emb_index_bhs(q, k, cos, sin, position_id):
     # batch_size, num_head, seq_len, hidden_size
@@ -25,15 +24,15 @@
             precision=torch.half,
             learnable=False,
         )
 
     def attention_forward(self, hidden_states, mask, **kw_args):
         origin = self
         self = self.transformer.layers[kw_args['layer_id']].attention
-        attention_fn = standard_attention
+        attention_fn = attention_fn_default
         if 'attention_fn' in self.hooks:
             attention_fn = self.hooks['attention_fn']
 
         mixed_raw_layer = self.query_key_value(hidden_states)
         (mixed_query_layer,
             mixed_key_layer,
             mixed_value_layer) = split_tensor_along_last_dim(mixed_raw_layer, 3)
@@ -104,15 +103,14 @@
 class LLaMAModel(BaseModel):
     def __init__(self, args, transformer=None, parallel_output=True, layernorm=RMSNorm, activation_func=nn.functional.silu, **kwargs):
         super().__init__(args, transformer=transformer, parallel_output=parallel_output, layernorm=layernorm, activation_func=activation_func, **kwargs)
         del self.transformer.position_embeddings
         self.add_mixin("rotary", RotaryMixin(args.hidden_size, args.num_attention_heads))
         self.add_mixin("lm", LMMixin(args.vocab_size, args.hidden_size))
         self.add_mixin("mlp", LLaMAMlpMixin(args.num_layers, args.hidden_size, args.inner_hidden_size))
-        self.add_mixin("causal", GPT2AttnMixin(args.max_sequence_length))
     
     def position_embedding_forward(self, *args, **kwargs):
         return None
     
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('LLaMA', 'LLaMA Configurations')
```

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/vit_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.4.2/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.4.2/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings_original.py` & `SwissArmyTransformer-0.4.2/sat/model/position_embedding/rotary_embeddings_original.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.4.2/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.4.2/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/registry.py` & `SwissArmyTransformer-0.4.2/sat/model/registry.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/model/transformer.py` & `SwissArmyTransformer-0.4.2/sat/model/transformer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/__init__.py` & `SwissArmyTransformer-0.4.2/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.4.2/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/data.py` & `SwissArmyTransformer-0.4.2/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/initialize.py` & `SwissArmyTransformer-0.4.2/sat/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/layers.py` & `SwissArmyTransformer-0.4.2/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/mappings.py` & `SwissArmyTransformer-0.4.2/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/operation.py` & `SwissArmyTransformer-0.4.2/sat/mpu/operation.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/mpu/utils.py` & `SwissArmyTransformer-0.4.2/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/__init__.py` & `SwissArmyTransformer-0.4.2/sat/ops/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 # here put the import lib
 import os
 import sys
 import math
 import random
 
-from .layernorm import LayerNorm
-from .fused_ema_adam import FusedEmaAdam
 # dynamic import according to name with importlib
 from importlib import import_module
 
 avaliable_ops = {
     'LayerNorm': 'sat.ops.layernorm',
     'f_similar': 'sat.ops.local_attention_function',
     'f_weighting': 'sat.ops.local_attention_function',
```

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp` & `SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_apply.cuh` & `SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_ema_adam.cu` & `SwissArmyTransformer-0.4.2/sat/ops/csrc/adam/multi_tensor_ema_adam.cu`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/type_shim.h` & `SwissArmyTransformer-0.4.2/sat/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/fused_ema_adam.py` & `SwissArmyTransformer-0.4.2/sat/ops/fused_ema_adam.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/layernorm.py` & `SwissArmyTransformer-0.4.2/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.4.2/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/memory_efficient_attention.py` & `SwissArmyTransformer-0.4.2/sat/ops/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/ops_builder/__init__.py` & `SwissArmyTransformer-0.4.2/sat/ops/ops_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/ops_builder/builder.py` & `SwissArmyTransformer-0.4.2/sat/ops/ops_builder/builder.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/ops/ops_builder/fused_ema_adam.py` & `SwissArmyTransformer-0.4.2/sat/ops/ops_builder/fused_ema_adam.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/quantization/kernels.py` & `SwissArmyTransformer-0.4.2/sat/quantization/kernels.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/resources/download.py` & `SwissArmyTransformer-0.4.2/sat/resources/download.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/resources/urls.py` & `SwissArmyTransformer-0.4.2/sat/resources/urls.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.4.2/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.4.2/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.4.2/sat/training/deepspeed_training.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.4.2/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.4.2/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/training/learning_rates.py` & `SwissArmyTransformer-0.4.2/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/training/model_io.py` & `SwissArmyTransformer-0.4.2/sat/training/model_io.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/training/utils.py` & `SwissArmyTransformer-0.4.2/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/sat/transformer_defaults.py` & `SwissArmyTransformer-0.4.2/sat/transformer_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     if self.training:
         output = self.output_dropout(output)
     return output
 
 def cross_attention_forward_default(self, hidden_states, cross_attention_mask, encoder_outputs, **kw_args):
     self = self.transformer.layers[kw_args['layer_id']].cross_attention
-    attention_fn = standard_attention
+    attention_fn = attention_fn_default
     if 'attention_fn' in self.hooks:
         attention_fn = self.hooks['attention_fn']
 
     mixed_query_layer = self.query(hidden_states)
     mixed_x_layer = self.key_value(encoder_outputs)
     (mixed_key_layer, mixed_value_layer) = split_tensor_along_last_dim(mixed_x_layer, 2)
```

### Comparing `SwissArmyTransformer-0.4.1/setup.py` & `SwissArmyTransformer-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.4.1',
+    version='0.4.2',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.4.1/tests/test_base_model.py` & `SwissArmyTransformer-0.4.2/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_inference.py` & `SwissArmyTransformer-0.4.2/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_mea.py` & `SwissArmyTransformer-0.4.2/tests/test_mea.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_model_parallel.py` & `SwissArmyTransformer-0.4.2/tests/test_model_parallel.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_nested_model.py` & `SwissArmyTransformer-0.4.2/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_speed.py` & `SwissArmyTransformer-0.4.2/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_train.py` & `SwissArmyTransformer-0.4.2/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_train_dp.py` & `SwissArmyTransformer-0.4.2/tests/test_train_dp.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.1/tests/test_train_nested.py` & `SwissArmyTransformer-0.4.2/tests/test_train_nested.py`

 * *Files identical despite different names*

