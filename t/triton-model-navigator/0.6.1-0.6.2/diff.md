# Comparing `tmp/triton_model_navigator-0.6.1-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,147 +1,147 @@
-Zip file size: 254320 bytes, number of entries: 145
--rw-r--r--  2.0 unx      881 b- defN 23-Jul-07 09:14 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Jul-07 10:38 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3915 b- defN 23-Jul-07 09:14 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     1716 b- defN 23-Jul-07 09:14 model_navigator/api/__init__.py
--rw-rw-rw-  2.0 unx    24220 b- defN 23-Jul-07 10:38 model_navigator/api/config.py
--rw-rw-rw-  2.0 unx     6263 b- defN 23-Jul-07 10:38 model_navigator/api/jax.py
--rw-rw-rw-  2.0 unx     5268 b- defN 23-Jul-07 10:38 model_navigator/api/onnx.py
--rw-rw-rw-  2.0 unx    16279 b- defN 23-Jul-07 10:38 model_navigator/api/package.py
--rw-r--r--  2.0 unx     4795 b- defN 23-Jul-07 09:14 model_navigator/api/python.py
--rw-rw-rw-  2.0 unx     7751 b- defN 23-Jul-07 10:38 model_navigator/api/pytriton.py
--rw-rw-rw-  2.0 unx     6350 b- defN 23-Jul-07 10:38 model_navigator/api/tensorflow.py
--rw-rw-rw-  2.0 unx     6158 b- defN 23-Jul-07 10:38 model_navigator/api/torch.py
--rw-r--r--  2.0 unx     1553 b- defN 23-Jul-07 09:14 model_navigator/api/triton.py
--rw-r--r--  2.0 unx     1811 b- defN 23-Jul-07 09:14 model_navigator/api/utilities.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/__init__.py
--rw-rw-rw-  2.0 unx     5542 b- defN 23-Jul-07 10:38 model_navigator/commands/base.py
--rw-r--r--  2.0 unx     9486 b- defN 23-Jul-07 09:14 model_navigator/commands/execution_context.py
--rw-r--r--  2.0 unx    12793 b- defN 23-Jul-07 09:14 model_navigator/commands/infer_metadata.py
--rw-r--r--  2.0 unx     3325 b- defN 23-Jul-07 09:14 model_navigator/commands/load.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/__init__.py
--rw-rw-rw-  2.0 unx     9868 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/base.py
--rw-rw-rw-  2.0 unx     7633 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/tf.py
--rw-rw-rw-  2.0 unx    10029 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/torch.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/__init__.py
--rw-r--r--  2.0 unx     3418 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/ts2onnx.py
--rw-r--r--  2.0 unx     4992 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-r--r--  2.0 unx      680 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/onnx/__init__.py
--rw-r--r--  2.0 unx     1727 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    10733 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-r--r--  2.0 unx     2235 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/copy/__init__.py
--rw-r--r--  2.0 unx     1798 b- defN 23-Jul-07 09:14 model_navigator/commands/copy/onnx.py
--rw-r--r--  2.0 unx      678 b- defN 23-Jul-07 09:14 model_navigator/commands/correctness/__init__.py
--rw-rw-rw-  2.0 unx     5674 b- defN 23-Jul-07 10:38 model_navigator/commands/correctness/correctness.py
--rw-r--r--  2.0 unx     4733 b- defN 23-Jul-07 09:14 model_navigator/commands/correctness/correctness_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/data_dump/__init__.py
--rw-r--r--  2.0 unx    10740 b- defN 23-Jul-07 09:14 model_navigator/commands/data_dump/samples.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/export/__init__.py
--rw-r--r--  2.0 unx     3611 b- defN 23-Jul-07 09:14 model_navigator/commands/export/jax.py
--rw-r--r--  2.0 unx     5598 b- defN 23-Jul-07 09:14 model_navigator/commands/export/tf.py
--rw-r--r--  2.0 unx     9156 b- defN 23-Jul-07 09:14 model_navigator/commands/export/torch.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/__init__.py
--rw-r--r--  2.0 unx     3945 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-r--r--  2.0 unx     3122 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/torch2onnx.py
--rw-r--r--  2.0 unx     2728 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-r--r--  2.0 unx      715 b- defN 23-Jul-07 09:14 model_navigator/commands/find_max_batch_size/__init__.py
--rw-r--r--  2.0 unx     7156 b- defN 23-Jul-07 09:14 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-r--r--  2.0 unx     3075 b- defN 23-Jul-07 09:14 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/__init__.py
--rw-r--r--  2.0 unx     5260 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/performance.py
--rw-r--r--  2.0 unx     6964 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/profile.py
--rw-r--r--  2.0 unx     3104 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/profile_script.py
--rw-r--r--  2.0 unx     7269 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/profiler.py
--rw-rw-rw-  2.0 unx     5476 b- defN 23-Jul-07 10:38 model_navigator/commands/performance/results.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/verification/__init__.py
--rw-r--r--  2.0 unx     4657 b- defN 23-Jul-07 09:14 model_navigator/commands/verification/verify.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/configuration/__init__.py
--rw-rw-rw-  2.0 unx     2002 b- defN 23-Jul-07 10:38 model_navigator/configuration/common_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/configuration/model/__init__.py
--rw-rw-rw-  2.0 unx    15653 b- defN 23-Jul-07 10:38 model_navigator/configuration/model/model_config.py
--rw-rw-rw-  2.0 unx    13677 b- defN 23-Jul-07 10:38 model_navigator/configuration/model/model_config_builder.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/core/__init__.py
--rw-rw-rw-  2.0 unx     1389 b- defN 23-Jul-07 10:38 model_navigator/core/constants.py
--rw-r--r--  2.0 unx     5299 b- defN 23-Jul-07 09:14 model_navigator/core/logger.py
--rw-r--r--  2.0 unx     9941 b- defN 23-Jul-07 09:14 model_navigator/core/tensor.py
--rw-r--r--  2.0 unx     2147 b- defN 23-Jul-07 09:14 model_navigator/core/workspace.py
--rw-r--r--  2.0 unx     2817 b- defN 23-Jul-07 09:14 model_navigator/frameworks/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-Jul-07 09:14 model_navigator/frameworks/jax/__init__.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-07 09:14 model_navigator/frameworks/jax/model.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/frameworks/onnx/__init__.py
--rw-r--r--  2.0 unx     1085 b- defN 23-Jul-07 09:14 model_navigator/frameworks/onnx/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/frameworks/tensorrt/__init__.py
--rw-r--r--  2.0 unx    27191 b- defN 23-Jul-07 09:14 model_navigator/frameworks/tensorrt/cuda.py
--rw-rw-rw-  2.0 unx    10627 b- defN 23-Jul-07 10:38 model_navigator/frameworks/tensorrt/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/frameworks/torch/__init__.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Jul-07 09:14 model_navigator/frameworks/torch/utils.py
--rw-r--r--  2.0 unx      622 b- defN 23-Jul-07 09:14 model_navigator/package/__init__.py
--rw-r--r--  2.0 unx    12176 b- defN 23-Jul-07 09:14 model_navigator/package/builder.py
--rw-r--r--  2.0 unx     4651 b- defN 23-Jul-07 09:14 model_navigator/package/loader.py
--rw-rw-rw-  2.0 unx    11860 b- defN 23-Jul-07 10:38 model_navigator/package/package.py
--rw-rw-rw-  2.0 unx     2819 b- defN 23-Jul-07 10:38 model_navigator/package/profiling_results.py
--rw-rw-rw-  2.0 unx    21135 b- defN 23-Jul-07 10:38 model_navigator/package/status.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/pipelines/__init__.py
--rw-r--r--  2.0 unx     5232 b- defN 23-Jul-07 09:14 model_navigator/pipelines/pipeline.py
--rw-rw-rw-  2.0 unx    14762 b- defN 23-Jul-07 10:38 model_navigator/pipelines/pipeline_context.py
--rw-r--r--  2.0 unx     3832 b- defN 23-Jul-07 09:14 model_navigator/pipelines/pipeline_manager.py
--rw-rw-rw-  2.0 unx     9693 b- defN 23-Jul-07 10:38 model_navigator/pipelines/validation.py
--rw-rw-rw-  2.0 unx     1883 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/__init__.py
--rw-r--r--  2.0 unx     2106 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/correctness.py
--rw-rw-rw-  2.0 unx     5682 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-r--r--  2.0 unx     1660 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/jax.py
--rw-rw-rw-  2.0 unx     2509 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/onnx.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/performance.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/preprocessing.py
--rw-r--r--  2.0 unx     2504 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/profiling.py
--rw-rw-rw-  2.0 unx     2921 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/tensorflow.py
--rw-rw-rw-  2.0 unx     3326 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/torch.py
--rw-r--r--  2.0 unx     2112 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/verify.py
--rw-r--r--  2.0 unx      622 b- defN 23-Jul-07 09:14 model_navigator/pipelines/wrappers/__init__.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Jul-07 09:14 model_navigator/pipelines/wrappers/optimize.py
--rw-r--r--  2.0 unx     4881 b- defN 23-Jul-07 09:14 model_navigator/pipelines/wrappers/profile.py
--rw-r--r--  2.0 unx     1584 b- defN 23-Jul-07 09:14 model_navigator/runners/__init__.py
--rw-r--r--  2.0 unx    13796 b- defN 23-Jul-07 09:14 model_navigator/runners/base.py
--rw-r--r--  2.0 unx     2620 b- defN 23-Jul-07 09:14 model_navigator/runners/jax.py
--rw-r--r--  2.0 unx     9999 b- defN 23-Jul-07 09:14 model_navigator/runners/onnx.py
--rw-r--r--  2.0 unx     2267 b- defN 23-Jul-07 09:14 model_navigator/runners/python.py
--rw-r--r--  2.0 unx     2290 b- defN 23-Jul-07 09:14 model_navigator/runners/registry.py
--rw-r--r--  2.0 unx     7976 b- defN 23-Jul-07 09:14 model_navigator/runners/tensorflow.py
--rw-r--r--  2.0 unx    26748 b- defN 23-Jul-07 09:14 model_navigator/runners/tensorrt.py
--rw-r--r--  2.0 unx    10041 b- defN 23-Jul-07 09:14 model_navigator/runners/torch.py
--rw-r--r--  2.0 unx     3559 b- defN 23-Jul-07 09:14 model_navigator/runners/utils.py
--rw-r--r--  2.0 unx      937 b- defN 23-Jul-07 09:14 model_navigator/runtime_analyzer/__init__.py
--rw-r--r--  2.0 unx    11714 b- defN 23-Jul-07 09:14 model_navigator/runtime_analyzer/analyzer.py
--rw-r--r--  2.0 unx     2304 b- defN 23-Jul-07 09:14 model_navigator/runtime_analyzer/strategy.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/triton/__init__.py
--rw-rw-rw-  2.0 unx     3180 b- defN 23-Jul-07 10:38 model_navigator/triton/model_config.py
--rw-r--r--  2.0 unx     5218 b- defN 23-Jul-07 09:14 model_navigator/triton/model_config_builder.py
--rw-r--r--  2.0 unx    23090 b- defN 23-Jul-07 09:14 model_navigator/triton/model_config_generator.py
--rw-r--r--  2.0 unx    15243 b- defN 23-Jul-07 09:14 model_navigator/triton/model_repository.py
--rw-r--r--  2.0 unx     2081 b- defN 23-Jul-07 09:14 model_navigator/triton/utils.py
--rw-r--r--  2.0 unx      944 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/__init__.py
--rw-rw-rw-  2.0 unx     2872 b- defN 23-Jul-07 10:38 model_navigator/triton/specialized_configs/base_model_config.py
--rw-r--r--  2.0 unx    22326 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/common.py
--rw-r--r--  2.0 unx     2229 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/internal.py
--rw-r--r--  2.0 unx     2685 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/python_model_config.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-r--r--  2.0 unx     3162 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/utils/__init__.py
--rw-rw-rw-  2.0 unx    14509 b- defN 23-Jul-07 10:38 model_navigator/utils/common.py
--rw-r--r--  2.0 unx     8132 b- defN 23-Jul-07 09:14 model_navigator/utils/dataloader.py
--rw-r--r--  2.0 unx     3902 b- defN 23-Jul-07 09:14 model_navigator/utils/devices.py
--rw-r--r--  2.0 unx     1308 b- defN 23-Jul-07 09:14 model_navigator/utils/enums.py
--rw-r--r--  2.0 unx     6163 b- defN 23-Jul-07 09:14 model_navigator/utils/environment.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Jul-07 09:14 model_navigator/utils/format_helpers.py
--rw-r--r--  2.0 unx     2330 b- defN 23-Jul-07 09:14 model_navigator/utils/module.py
--rw-r--r--  2.0 unx    10140 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    10798 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    14493 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/RECORD
-145 files, 768716 bytes uncompressed, 230700 bytes compressed:  70.0%
+Zip file size: 254449 bytes, number of entries: 145
+-rw-r--r--  2.0 unx      881 b- defN 23-Jul-18 03:12 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Jul-19 07:20 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3915 b- defN 23-Jul-18 03:12 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     1716 b- defN 23-Jul-18 03:12 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    24220 b- defN 23-Jul-19 07:20 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6263 b- defN 23-Jul-19 07:20 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5268 b- defN 23-Jul-19 07:20 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    16279 b- defN 23-Jul-19 07:20 model_navigator/api/package.py
+-rw-r--r--  2.0 unx     4795 b- defN 23-Jul-18 03:12 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7751 b- defN 23-Jul-19 07:20 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6350 b- defN 23-Jul-19 07:20 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6158 b- defN 23-Jul-19 07:20 model_navigator/api/torch.py
+-rw-rw-rw-  2.0 unx     1585 b- defN 23-Jul-19 07:20 model_navigator/api/triton.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-Jul-18 03:12 model_navigator/api/utilities.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     5542 b- defN 23-Jul-19 07:20 model_navigator/commands/base.py
+-rw-r--r--  2.0 unx     9486 b- defN 23-Jul-18 03:12 model_navigator/commands/execution_context.py
+-rw-r--r--  2.0 unx    12793 b- defN 23-Jul-18 03:12 model_navigator/commands/infer_metadata.py
+-rw-r--r--  2.0 unx     3325 b- defN 23-Jul-18 03:12 model_navigator/commands/load.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     9876 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7642 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx    10251 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/torch.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/converters/__init__.py
+-rw-r--r--  2.0 unx     3418 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-rw-rw-  2.0 unx     4992 b- defN 23-Jul-18 14:03 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-r--r--  2.0 unx      680 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/onnx/__init__.py
+-rw-r--r--  2.0 unx     1727 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    11390 b- defN 23-Jul-19 07:20 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-r--r--  2.0 unx     2235 b- defN 23-Jul-18 03:12 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/copy/__init__.py
+-rw-r--r--  2.0 unx     1798 b- defN 23-Jul-18 03:12 model_navigator/commands/copy/onnx.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Jul-18 03:12 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5674 b- defN 23-Jul-19 07:20 model_navigator/commands/correctness/correctness.py
+-rw-r--r--  2.0 unx     4733 b- defN 23-Jul-18 03:12 model_navigator/commands/correctness/correctness_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/data_dump/__init__.py
+-rw-r--r--  2.0 unx    10740 b- defN 23-Jul-18 03:12 model_navigator/commands/data_dump/samples.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/export/__init__.py
+-rw-r--r--  2.0 unx     3611 b- defN 23-Jul-18 03:12 model_navigator/commands/export/jax.py
+-rw-r--r--  2.0 unx     5598 b- defN 23-Jul-18 03:12 model_navigator/commands/export/tf.py
+-rw-r--r--  2.0 unx     9156 b- defN 23-Jul-18 03:12 model_navigator/commands/export/torch.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/__init__.py
+-rw-r--r--  2.0 unx     3945 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-r--r--  2.0 unx     3122 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-Jul-18 03:12 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jul-18 03:12 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-r--r--  2.0 unx     7156 b- defN 23-Jul-18 03:12 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-r--r--  2.0 unx     3075 b- defN 23-Jul-18 03:12 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/__init__.py
+-rw-r--r--  2.0 unx     5260 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/performance.py
+-rw-r--r--  2.0 unx     6964 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/profile.py
+-rw-r--r--  2.0 unx     3104 b- defN 23-Jul-18 03:12 model_navigator/commands/performance/profile_script.py
+-rw-rw-rw-  2.0 unx     7269 b- defN 23-Jul-18 15:55 model_navigator/commands/performance/profiler.py
+-rw-rw-rw-  2.0 unx     5476 b- defN 23-Jul-19 07:20 model_navigator/commands/performance/results.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/commands/verification/__init__.py
+-rw-r--r--  2.0 unx     4657 b- defN 23-Jul-18 03:12 model_navigator/commands/verification/verify.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2002 b- defN 23-Jul-19 07:20 model_navigator/configuration/common_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    15653 b- defN 23-Jul-19 07:20 model_navigator/configuration/model/model_config.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 23-Jul-19 07:20 model_navigator/configuration/model/model_config_builder.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1389 b- defN 23-Jul-19 07:20 model_navigator/core/constants.py
+-rw-r--r--  2.0 unx     5299 b- defN 23-Jul-18 03:12 model_navigator/core/logger.py
+-rw-r--r--  2.0 unx     9941 b- defN 23-Jul-18 03:12 model_navigator/core/tensor.py
+-rw-r--r--  2.0 unx     2147 b- defN 23-Jul-18 03:12 model_navigator/core/workspace.py
+-rw-r--r--  2.0 unx     2817 b- defN 23-Jul-18 03:12 model_navigator/frameworks/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jul-18 03:12 model_navigator/frameworks/jax/__init__.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-18 03:12 model_navigator/frameworks/jax/model.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/frameworks/onnx/__init__.py
+-rw-r--r--  2.0 unx     1085 b- defN 23-Jul-18 03:12 model_navigator/frameworks/onnx/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/frameworks/tensorrt/__init__.py
+-rw-r--r--  2.0 unx    27191 b- defN 23-Jul-18 03:12 model_navigator/frameworks/tensorrt/cuda.py
+-rw-rw-rw-  2.0 unx    10627 b- defN 23-Jul-19 07:20 model_navigator/frameworks/tensorrt/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/frameworks/torch/__init__.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jul-18 03:12 model_navigator/frameworks/torch/utils.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-18 03:12 model_navigator/package/__init__.py
+-rw-r--r--  2.0 unx    12176 b- defN 23-Jul-18 03:12 model_navigator/package/builder.py
+-rw-r--r--  2.0 unx     4651 b- defN 23-Jul-18 03:12 model_navigator/package/loader.py
+-rw-r--r--  2.0 unx    11860 b- defN 23-Jul-18 03:12 model_navigator/package/package.py
+-rw-rw-rw-  2.0 unx     2819 b- defN 23-Jul-19 07:20 model_navigator/package/profiling_results.py
+-rw-rw-rw-  2.0 unx    21135 b- defN 23-Jul-19 07:20 model_navigator/package/status.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/pipelines/__init__.py
+-rw-r--r--  2.0 unx     5232 b- defN 23-Jul-18 03:12 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx    14762 b- defN 23-Jul-19 07:20 model_navigator/pipelines/pipeline_context.py
+-rw-r--r--  2.0 unx     3832 b- defN 23-Jul-18 03:12 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9693 b- defN 23-Jul-19 07:20 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1883 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/__init__.py
+-rw-r--r--  2.0 unx     2106 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     5682 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2509 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/onnx.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/performance.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/preprocessing.py
+-rw-r--r--  2.0 unx     2504 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2921 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3326 b- defN 23-Jul-19 07:20 model_navigator/pipelines/builders/torch.py
+-rw-r--r--  2.0 unx     2112 b- defN 23-Jul-18 03:12 model_navigator/pipelines/builders/verify.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-18 03:12 model_navigator/pipelines/wrappers/__init__.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Jul-18 03:12 model_navigator/pipelines/wrappers/optimize.py
+-rw-rw-rw-  2.0 unx     4881 b- defN 23-Jul-18 15:55 model_navigator/pipelines/wrappers/profile.py
+-rw-r--r--  2.0 unx     1584 b- defN 23-Jul-18 03:12 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    13796 b- defN 23-Jul-18 15:55 model_navigator/runners/base.py
+-rw-r--r--  2.0 unx     2620 b- defN 23-Jul-18 03:12 model_navigator/runners/jax.py
+-rw-r--r--  2.0 unx     9999 b- defN 23-Jul-18 03:12 model_navigator/runners/onnx.py
+-rw-r--r--  2.0 unx     2267 b- defN 23-Jul-18 03:12 model_navigator/runners/python.py
+-rw-r--r--  2.0 unx     2290 b- defN 23-Jul-18 03:12 model_navigator/runners/registry.py
+-rw-r--r--  2.0 unx     7976 b- defN 23-Jul-18 03:12 model_navigator/runners/tensorflow.py
+-rw-r--r--  2.0 unx    26748 b- defN 23-Jul-18 03:12 model_navigator/runners/tensorrt.py
+-rw-r--r--  2.0 unx    10041 b- defN 23-Jul-18 03:12 model_navigator/runners/torch.py
+-rw-r--r--  2.0 unx     3559 b- defN 23-Jul-18 03:12 model_navigator/runners/utils.py
+-rw-r--r--  2.0 unx      937 b- defN 23-Jul-18 03:12 model_navigator/runtime_analyzer/__init__.py
+-rw-r--r--  2.0 unx    11714 b- defN 23-Jul-18 03:12 model_navigator/runtime_analyzer/analyzer.py
+-rw-r--r--  2.0 unx     2304 b- defN 23-Jul-18 03:12 model_navigator/runtime_analyzer/strategy.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/triton/__init__.py
+-rw-rw-rw-  2.0 unx     3180 b- defN 23-Jul-19 07:20 model_navigator/triton/model_config.py
+-rw-r--r--  2.0 unx     5218 b- defN 23-Jul-18 03:12 model_navigator/triton/model_config_builder.py
+-rw-rw-rw-  2.0 unx    23090 b- defN 23-Jul-19 07:20 model_navigator/triton/model_config_generator.py
+-rw-rw-rw-  2.0 unx    15243 b- defN 23-Jul-19 07:20 model_navigator/triton/model_repository.py
+-rw-rw-rw-  2.0 unx     2081 b- defN 23-Jul-19 07:20 model_navigator/triton/utils.py
+-rw-rw-rw-  2.0 unx      997 b- defN 23-Jul-18 15:55 model_navigator/triton/specialized_configs/__init__.py
+-rw-rw-rw-  2.0 unx     2872 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-rw-rw-  2.0 unx    22326 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/common.py
+-rw-r--r--  2.0 unx     2229 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/internal.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-rw-rw-  2.0 unx     3162 b- defN 23-Jul-19 07:20 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Jul-18 03:12 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-18 03:12 model_navigator/utils/__init__.py
+-rw-r--r--  2.0 unx    14509 b- defN 23-Jul-18 03:12 model_navigator/utils/common.py
+-rw-r--r--  2.0 unx     8132 b- defN 23-Jul-18 03:12 model_navigator/utils/dataloader.py
+-rw-r--r--  2.0 unx     3902 b- defN 23-Jul-18 03:12 model_navigator/utils/devices.py
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jul-18 03:12 model_navigator/utils/enums.py
+-rw-r--r--  2.0 unx     6163 b- defN 23-Jul-18 03:12 model_navigator/utils/environment.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jul-18 03:12 model_navigator/utils/format_helpers.py
+-rw-r--r--  2.0 unx     2330 b- defN 23-Jul-18 03:12 model_navigator/utils/module.py
+-rw-r--r--  2.0 unx    10140 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10798 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    14493 b- defN 23-Jul-19 07:24 triton_model_navigator-0.6.2.dist-info/RECORD
+145 files, 769697 bytes uncompressed, 230829 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -414,23 +414,23 @@
 
 Filename: model_navigator/utils/format_helpers.py
 Comment: 
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
-Filename: triton_model_navigator-0.6.1.dist-info/LICENSE
+Filename: triton_model_navigator-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.6.1.dist-info/METADATA
+Filename: triton_model_navigator-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.6.1.dist-info/WHEEL
+Filename: triton_model_navigator-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.6.1.dist-info/top_level.txt
+Filename: triton_model_navigator-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.6.1.dist-info/RECORD
+Filename: triton_model_navigator-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.6.1"
+__version__ = "0.6.2"
```

## model_navigator/api/triton.py

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Public API definition for Triton related functionality."""
 from model_navigator.triton import model_repository  # noqa: F401
 from model_navigator.triton.specialized_configs import (  # noqa: F401
     AutoMixedPrecisionAccelerator,
+    BaseSpecializedModelConfig,
     DeviceKind,
     DynamicBatcher,
     GPUIOAccelerator,
     InputTensorFormat,
     InputTensorSpec,
     InstanceGroup,
     ONNXModelConfig,
```

## model_navigator/commands/convert/base.py

```diff
@@ -56,29 +56,29 @@
         run_search = cls._run_search(
             custom_trt_profile_available=custom_trt_profile_available,
             batch_dim=batch_dim,
             dataloader_batch_size=dataloader_max_batch_size,
             device_max_batch_size=device_max_batch_size,
         )
         if run_search:
-            max_conversion_batch_size = (
+            conversion_max_batch_size = (
                 cls._execute_conversion_with_max_batch_size_search(  # TODO what is the best value?
                     convert_func=convert_func,
                     get_args=get_args,
                     device_max_batch_size=device_max_batch_size,
                     dataloader_max_batch_size=dataloader_max_batch_size,
                 )
             )
-            LOGGER.info(f"Converted with maximal batch size: {max_conversion_batch_size}.")
+            LOGGER.info(f"Converted with maximal batch size: {conversion_max_batch_size}.")
         else:
             LOGGER.info("Search for maximal batch size disable. Execute single conversion.")
-            max_conversion_batch_size = dataloader_max_batch_size
+            conversion_max_batch_size = dataloader_max_batch_size
             convert_func(get_args())
 
-        return max_conversion_batch_size
+        return conversion_max_batch_size
 
     @classmethod
     def _execute_conversion_with_max_batch_size_search(
         cls,
         convert_func: Callable,
         get_args: Callable,
         device_max_batch_size: int,
@@ -101,23 +101,23 @@
         Raises:
             A conversion exception when command and fallback failed.
         """
         LOGGER.info("Search for maximal batch size enabled. Execute conversion with adaptive batch size adjustment.")
         try:
             max_batch_size = cls._get_conversion_max_batch_sizes(device_max_batch_size, dataloader_max_batch_size)
             convert_func(get_args(max_batch_size=max_batch_size))
-            max_conversion_batch_size = max_batch_size
-            LOGGER.info(f"Successful conversion for max batch size: {max_conversion_batch_size}.")
+            conversion_max_batch_size = max_batch_size
+            LOGGER.info(f"Successful conversion for max batch size: {conversion_max_batch_size}.")
         except Exception as e:
             LOGGER.debug(f"Conversion failed with error: {str(e)}.Trying fallback with smaller batch sizes.")
-            max_conversion_batch_size = cls._fallback_conversion(
+            conversion_max_batch_size = cls._fallback_conversion(
                 convert_func, get_args, device_max_batch_size, dataloader_max_batch_size
             )
 
-        return max_conversion_batch_size
+        return conversion_max_batch_size
 
     @classmethod
     def _fallback_conversion(
         cls,
         convert_func: Callable,
         get_args: Callable,
         device_max_batch_size: int,
@@ -141,31 +141,31 @@
 
         Returns:
             New max batch size for which conversion succeeded
 
         Raises:
             A conversion exception when command failed.
         """
-        max_conversion_batch_size = None
+        conversion_max_batch_size = None
         fallback_batch_sizes = cls._get_conversion_fallback_batch_sizes(
             device_max_batch_size,
             dataloader_max_batch_size,
         )
-        while max_conversion_batch_size is None:
+        while conversion_max_batch_size is None:
             max_batch_size = next(fallback_batch_sizes)
             try:
                 convert_func(get_args(max_batch_size=max_batch_size))
-                max_conversion_batch_size = max_batch_size
-                LOGGER.info(f"Successfully converted with max batch size: {max_conversion_batch_size}.")
+                conversion_max_batch_size = max_batch_size
+                LOGGER.info(f"Successfully converted with max batch size: {conversion_max_batch_size}.")
             except Exception as e:
                 LOGGER.debug(f"Conversion failed with error: {str(e)}")
                 if max_batch_size == dataloader_max_batch_size:
                     raise e
 
-        return max_conversion_batch_size
+        return conversion_max_batch_size
 
     @staticmethod
     def _get_conversion_max_batch_sizes(device_max_batch_size: Optional[int], dataloader_max_batch_size: int) -> int:
         """Select the batch size for first conversion attempt."""
         if device_max_batch_size:
             return device_max_batch_size
         else:
@@ -221,15 +221,15 @@
                 f"    device_max_batch_size: {device_max_batch_size}\n"
             )
             return False
 
         return True
 
     @classmethod
-    def _get_trt_profile(
+    def _get_initial_trt_profile(
         cls,
         dataloader_trt_profile: TensorRTProfile,
         custom_trt_profile: Optional[TensorRTProfile],
     ):
         """Obtain the TensorRT profiles from dataloader or custom values provided by user."""
         if not custom_trt_profile:
             LOGGER.info("Using dataloader profile for TRT conversion")
```

## model_navigator/commands/convert/tf.py

```diff
@@ -132,15 +132,15 @@
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported SavedModel model not found at {exported_model_path}. Skipping conversion")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         custom_trt_profile = trt_profile
-        trt_profile = self._get_trt_profile(
+        trt_profile = self._get_initial_trt_profile(
             dataloader_trt_profile=dataloader_trt_profile, custom_trt_profile=custom_trt_profile
         )
 
         if batch_dim is not None:
             max_batch_size = list(trt_profile.values())[0].max[batch_dim]
         else:
             max_batch_size = None
@@ -166,17 +166,18 @@
         with ExecutionContext(
             workspace=workspace,
             script_path=converted_model_path.parent / "reproduce_conversion.py",
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
             verbose=verbose,
         ) as context:
 
-            max_conversion_batch_size = self._execute_conversion(
+            conversion_max_batch_size = self._execute_conversion(
                 convert_func=lambda args: context.execute_external_runtime_script(sm2tftrt.__file__, args),
                 get_args=get_args,
                 batch_dim=batch_dim,
                 device_max_batch_size=device_max_batch_size,
                 dataloader_max_batch_size=dataloader_max_batch_size,
                 custom_trt_profile_available=bool(custom_trt_profile),
             )
+
         LOGGER.info("Converted SavedModel to Tensorflow-TensorRT.")
-        return CommandOutput(status=CommandStatus.OK, output={"max_conversion_batch_size": max_conversion_batch_size})
+        return CommandOutput(status=CommandStatus.OK, output={"conversion_max_batch_size": conversion_max_batch_size})
```

## model_navigator/commands/convert/torch.py

```diff
@@ -154,15 +154,15 @@
         converted_model_path = workspace.path / path
 
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported TorchScript model not found at {exported_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         custom_trt_profile = trt_profile
-        trt_profile = self._get_trt_profile(
+        trt_profile = self._get_initial_trt_profile(
             dataloader_trt_profile=dataloader_trt_profile, custom_trt_profile=custom_trt_profile
         )
 
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         input_dtypes_str = [tensorrt_utils.cast_type(input_spec.dtype).name for input_spec in input_metadata.values()]
 
@@ -186,24 +186,30 @@
         with ExecutionContext(
             workspace=workspace,
             script_path=converted_model_path.parent / "reproduce_conversion.py",
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
             verbose=verbose,
         ) as context:
 
-            max_conversion_batch_size = self._execute_conversion(
+            conversion_max_batch_size = self._execute_conversion(
                 convert_func=lambda args: context.execute_external_runtime_script(ts2torchtrt.__file__, args),
                 get_args=get_args,
                 batch_dim=batch_dim,
                 device_max_batch_size=device_max_batch_size,
                 dataloader_max_batch_size=dataloader_max_batch_size,
                 custom_trt_profile_available=bool(custom_trt_profile),
             )
+        shapes = self._get_shape_args(
+            trt_profile=trt_profile, batch_dim=batch_dim, max_batch_size=conversion_max_batch_size
+        )
         LOGGER.info("Converted TorchScript to Torch-TensorRT.")
-        return CommandOutput(status=CommandStatus.OK, output={"max_conversion_batch_size": max_conversion_batch_size})
+        return CommandOutput(
+            status=CommandStatus.OK,
+            output={"conversion_max_batch_size": conversion_max_batch_size, "conversion_profiles": shapes},
+        )
 
     @staticmethod
     def _get_shape_args(
         trt_profile: TensorRTProfile,
         batch_dim: Optional[int] = None,
         max_batch_size: Optional[int] = None,
     ):
```

## model_navigator/commands/convert/onnx/onnx2trt.py

```diff
@@ -93,15 +93,15 @@
 
         if not input_model_path.exists():
             LOGGER.warning(f"Exported ONNX model not found at {input_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         custom_trt_profile = trt_profile
-        trt_profile = self._get_trt_profile(
+        trt_profile = self._get_initial_trt_profile(
             dataloader_trt_profile=dataloader_trt_profile, custom_trt_profile=custom_trt_profile
         )
 
         onnx_input_metadata = self._get_onnx_input_metadata(
             input_model_path=input_model_path,
             input_metadata=input_metadata,
             output_metadata=output_metadata,
@@ -164,42 +164,65 @@
                 "input_metadata": input_metadata.to_json(),
                 "output_metadata": output_metadata.to_json(),
             }
 
             load_args = parse_kwargs_to_cmd(kwargs)
             from . import trt_load_script
 
-            max_conversion_batch_size = self._execute_conversion(
+            conversion_max_batch_size = self._execute_conversion(
                 convert_func=lambda args: context.execute_cmd(
                     args + ["&&", sys.executable, trt_load_script.__file__] + load_args
                 ),
                 get_args=get_args,
                 batch_dim=batch_dim,
                 device_max_batch_size=device_max_batch_size,
                 dataloader_max_batch_size=dataloader_max_batch_size,
                 custom_trt_profile_available=bool(custom_trt_profile),
             )
 
+        shapes = self._get_adapted_trt_profile(
+            trt_profile=trt_profile,
+            batch_dim=batch_dim,
+            max_batch_size=conversion_max_batch_size,
+        )
+
         LOGGER.info("Converted ONNX to TensorRT.")
-        return CommandOutput(status=CommandStatus.OK, output={"max_conversion_batch_size": max_conversion_batch_size})
+        return CommandOutput(
+            status=CommandStatus.OK,
+            output={"conversion_max_batch_size": conversion_max_batch_size, "conversion_profiles": shapes},
+        )
 
     @staticmethod
-    def _get_shape_args(
-        onnx_input_metadata: TensorMetadata,
+    def _get_adapted_trt_profile(
         trt_profile: TensorRTProfile,
         batch_dim: Optional[int] = None,
         max_batch_size: Optional[int] = None,
     ):
         if batch_dim is not None and max_batch_size is not None and max_batch_size > 0:
             trt_profile = tensorrt_utils.get_trt_profile_with_new_max_batch_size(
                 trt_profile=trt_profile,
                 max_batch_size=max_batch_size,
                 batch_dim=batch_dim,
             )
 
+        return trt_profile
+
+    @staticmethod
+    def _get_shape_args(
+        onnx_input_metadata: TensorMetadata,
+        trt_profile: TensorRTProfile,
+        batch_dim: Optional[int] = None,
+        max_batch_size: Optional[int] = None,
+    ):
+        trt_profile = ConvertONNX2TRT._get_adapted_trt_profile(
+            trt_profile=trt_profile,
+            batch_dim=batch_dim,
+            max_batch_size=max_batch_size,
+        )
+
         shape_args = []
         for attr in ("min", "opt", "max"):
             arg = f"--trt-{attr}-shapes"
             shapes = []
             for input_name in trt_profile:
                 if input_name not in onnx_input_metadata:
                     continue
```

## model_navigator/triton/specialized_configs/__init__.py

```diff
@@ -8,13 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D104
+from .base_model_config import *  # noqa: F401, F403
 from .common import *  # noqa: F401, F403
 from .onnx_model_config import *  # noqa: F401, F403
 from .python_model_config import *  # noqa: F401, F403
 from .pytorch_model_config import *  # noqa: F401, F403
 from .tensorflow_model_config import *  # noqa: F401, F403
 from .tensorrt_model_config import *  # noqa: F401, F403
```

## Comparing `triton_model_navigator-0.6.1.dist-info/LICENSE` & `triton_model_navigator-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.6.1.dist-info/METADATA` & `triton_model_navigator-0.6.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.6.1
+Version: 0.6.2
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.6.1.dist-info/RECORD` & `triton_model_navigator-0.6.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=ECVKemedbrrIEIqnW9Awybdq6tFv_UIZ-6WA1YCq-v8,649
+model_navigator/__version__.py,sha256=7vvkQh0eqmNgtq6_vPlJXbvzyGqtMkGz68y6ijnvTtw,649
 model_navigator/exceptions.py,sha256=AnYKlbe6WHk4_3lEhksgONKjtcNK7_g0-qs8mIHARuA,3915
 model_navigator/api/__init__.py,sha256=Jt9Du5gr7UP0ljMEur81SAqLg99DokO0vyw1qaonOqY,1716
 model_navigator/api/config.py,sha256=buMLeLqvirV4efpIAxgDBFo0gSoHGNttOns4dHkU_V4,24220
 model_navigator/api/jax.py,sha256=QwOjMl89TPZpj4lOOMLrGOnNrWMoVMCFhgTgk1mmCLA,6263
 model_navigator/api/onnx.py,sha256=CwX50QTt6seCbCDAOvgPLbOQjw29sL-bVWvMViFlU18,5268
 model_navigator/api/package.py,sha256=BqPo9VD_alP4aMbvvQCdqGEZZ3YrQ1PNMcDH-B-uBC8,16279
 model_navigator/api/python.py,sha256=n3Pdc_2TK9Q1yYui4R2rLh8ImC3ezhHnh-n0K1Hcom0,4795
 model_navigator/api/pytriton.py,sha256=qTMb83nJvOHCGMXVRwYMlGRKI8kW-Eqwt_K9lJJwTR4,7751
 model_navigator/api/tensorflow.py,sha256=cjo_-HGh8ZOh0kCs-4dJOkBvJTyOE4wtTp3J5kNlCiI,6350
 model_navigator/api/torch.py,sha256=y6hLMmkkl3OJICEOTZDL6yQ7b-ijiiOEWEe6joXIReM,6158
-model_navigator/api/triton.py,sha256=hdrU_WJn5DFzhJ5slcdJqzRcC7n69vhmP0RKa1B3QYQ,1553
+model_navigator/api/triton.py,sha256=5F5QKDLaZpTWCtHwSd7yR9m63lbg5PedXvCrpzZicJk,1585
 model_navigator/api/utilities.py,sha256=iDAsvY2lFZ1ri54OSmThTVokJ31vCnHoylBHiKkYUNg,1811
 model_navigator/commands/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/base.py,sha256=apYokswe-yQ8DvRKcGp6jQR6KNFGAtpLMIG5pIkugw8,5542
 model_navigator/commands/execution_context.py,sha256=v7cecavg6Xn0QD-3b_3qb9IaIzcKY8htnSZZtDw-fzM,9486
 model_navigator/commands/infer_metadata.py,sha256=xWwubLpHI_Y46XrH0yXWvo1inSkDuIXXakpnA1rlI6Q,12793
 model_navigator/commands/load.py,sha256=NhcPPfkWqnRJJt18qCaNw54mffqs84Aotei8Vt72qv4,3325
 model_navigator/commands/convert/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/convert/base.py,sha256=A_1BeYl2eEz7mAIJyt0j4KV_4p6T8-tEGaM_oO5jf8o,9868
-model_navigator/commands/convert/tf.py,sha256=d3whrl14w0i9wmertOc96XpZlaApsQInBs2ovpbTCOw,7633
-model_navigator/commands/convert/torch.py,sha256=acOP_Xm0PeNsPWo24IES5MM5R6AD2hmPJxZOTR9O-tk,10029
+model_navigator/commands/convert/base.py,sha256=o06Ny57FdTqQgoiS5iC0dBpfq0JwCydtLrDDxVH4peM,9876
+model_navigator/commands/convert/tf.py,sha256=A1d3PBUcetrjwjW1GGPSewRXNfPY_vu6m9IykOx5Fbo,7642
+model_navigator/commands/convert/torch.py,sha256=SCtxyf6KoIOExl_iaaBQJ2YHKjy-_2baMe-Y_pe5POc,10251
 model_navigator/commands/convert/converters/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/converters/sm2tftrt.py,sha256=AcNyKV60yCUrzJ5B501H5SHKjtkr7kaNXNIewnOFJzk,3418
 model_navigator/commands/convert/converters/ts2onnx.py,sha256=ezjlPeHHbhx2LB4HDoLkVlmaZa1dreVMQMk2PL5UMos,3105
 model_navigator/commands/convert/converters/ts2torchtrt.py,sha256=a_mpR0j4y5ClaY6Ik_oIKEAlh45zD-ycCLHigsy1C7M,4992
 model_navigator/commands/convert/onnx/__init__.py,sha256=LwvvDj4oH7rwmUJXVEyRxIOWZnUxix6n_DmkAJzEJBY,680
 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py,sha256=KQR-qrVWVVBGVr5pqcKink2dcDNCk1Lszvl8x6TwqjU,1727
-model_navigator/commands/convert/onnx/onnx2trt.py,sha256=hOwaQ5oIIuVyaniXOusRtBUk5VLeOVrKWs2xcwaBMFg,10733
+model_navigator/commands/convert/onnx/onnx2trt.py,sha256=HUfib42F3vP9pzzlolLHVyQoCuBfmqskuvW3DgLLOuE,11390
 model_navigator/commands/convert/onnx/trt_load_script.py,sha256=D2fTNNIBELAsBSmy3ij9oxMyRDxi0RNFV29zAlPYFz8,2235
 model_navigator/commands/copy/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/copy/onnx.py,sha256=iQvV13MLoE9XjPKv--gSBTnDrjO-WYeSHOQI3ITRSp4,1798
 model_navigator/commands/correctness/__init__.py,sha256=Xm-ikcHX6zpdmukjkSgL4JnPt2FIImoxXUPsL-334FM,678
 model_navigator/commands/correctness/correctness.py,sha256=qM4FhOAnLzazob4PyZLdcZkWMG62PLG54k4QHyvJW8Y,5674
 model_navigator/commands/correctness/correctness_script.py,sha256=Ejdk8rM7_wPxP5gwIkryOVghKMzCUrqF9L2J8V9kKF0,4733
 model_navigator/commands/data_dump/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
@@ -117,15 +117,15 @@
 model_navigator/runtime_analyzer/strategy.py,sha256=L6dqnf1OS0s5mrBvxTTFgNPghKbuEFC2X_2tMm3_Hs4,2304
 model_navigator/triton/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/triton/model_config.py,sha256=Efcx0_48bmkmBwJgqm6Ejsuwh0ZPnYmyR1o6bz4Y5to,3180
 model_navigator/triton/model_config_builder.py,sha256=4uh5xArtOMnyzIKO2Duliz9SRltrP5El2xPqzE1At_0,5218
 model_navigator/triton/model_config_generator.py,sha256=i45y9ezQJ9xcQmNcGHW_5r0TZ7-Ikxvmzb9pgfBlZaY,23090
 model_navigator/triton/model_repository.py,sha256=w8LtO3UoYB4gDstfye5x-oUuPOnYmX18pLAU_SNr3VQ,15243
 model_navigator/triton/utils.py,sha256=uJeGyzMSvxZj2hyUAC3bTk0cuMcKTYeCKAi7zerP3hA,2081
-model_navigator/triton/specialized_configs/__init__.py,sha256=lcQy-49A74vMSidK-avYy6xdX4p3OG3ygzSw6y9-OQw,944
+model_navigator/triton/specialized_configs/__init__.py,sha256=9xcAy4dDPv29vS9Z7SliDEuaEmEeXtJYpxhL6S0zepo,997
 model_navigator/triton/specialized_configs/base_model_config.py,sha256=UOeuce-xT9lC3Zv3H3BbdSem7cTNyn7boKybxChzRgs,2872
 model_navigator/triton/specialized_configs/common.py,sha256=l6FPhZTU1WQHDVXG8HxEXx2c8s87EWgYUvtQrxqUH1k,22326
 model_navigator/triton/specialized_configs/internal.py,sha256=R42XlgUEOC5B-WotI_dAQs8sQyHJOnVyTvVk3CaZ6kM,2229
 model_navigator/triton/specialized_configs/onnx_model_config.py,sha256=oN76Ux7JI4eqlarlEVSSiIbbajAqdrF3bW0n6WQBPPw,2685
 model_navigator/triton/specialized_configs/python_model_config.py,sha256=NGijgogtoJnbBLL1hQqhw-n4rBo_OgFsCdn9ezw24VI,1785
 model_navigator/triton/specialized_configs/pytorch_model_config.py,sha256=GxJnFB4UpnUwB75t09d5XZ2iqeMZM1SmTbGe2aqmph8,2239
 model_navigator/triton/specialized_configs/tensorflow_model_config.py,sha256=C_qMi-5TAWTSL_wBDIoJju3gHRHX10RBbHvBE9of780,3162
@@ -134,12 +134,12 @@
 model_navigator/utils/common.py,sha256=zDD3FCSPJsig7GK2EcqzKX-q2umzO34xg4a8tL7iuxw,14509
 model_navigator/utils/dataloader.py,sha256=r549fsb5tq7ZQpnKFw4Zk9Mgc8WKzwP4wZHlpWXNj1g,8132
 model_navigator/utils/devices.py,sha256=pGjRBByJqFjG6dyJ0H2E6GJA7hIgF6rgeINLNdS27kU,3902
 model_navigator/utils/enums.py,sha256=T-G5VV5CqimxpctOqPaCvVoAwx-pp10Eeo0rKlWoVGU,1308
 model_navigator/utils/environment.py,sha256=MnpdF5eCx2DJpHtaq8fUSky0hdT03qTJrGnJDhCnFhM,6163
 model_navigator/utils/format_helpers.py,sha256=3UGJhNTFZiMorbMQrciDzJgfFW2nvLMroNmeqC8FlGs,4096
 model_navigator/utils/module.py,sha256=BX9Da3b-tOHvOFb4Ffts0Qc1i9hbgwreGbScqq_DINY,2330
-triton_model_navigator-0.6.1.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.6.1.dist-info/METADATA,sha256=67GVztavILQkw37c074Z6seXgk-NoebcEg0vA8e9y10,10798
-triton_model_navigator-0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.6.1.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.6.1.dist-info/RECORD,,
+triton_model_navigator-0.6.2.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.6.2.dist-info/METADATA,sha256=axM9Gs2j56BXrAXmn2YdshVD0bkM_rq5Q3EFskp4xLU,10798
+triton_model_navigator-0.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.6.2.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.6.2.dist-info/RECORD,,
```

