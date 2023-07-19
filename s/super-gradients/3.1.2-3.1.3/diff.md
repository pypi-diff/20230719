# Comparing `tmp/super_gradients-3.1.2-py3-none-any.whl.zip` & `tmp/super_gradients-3.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,569 +1,577 @@
-Zip file size: 983193 bytes, number of entries: 567
--rw-r--r--  2.0 unx      916 b- defN 23-Jun-07 12:02 super_gradients/__init__.py
--rw-r--r--  2.0 unx     1657 b- defN 23-Jun-07 12:02 super_gradients/evaluate_checkpoint.py
--rw-r--r--  2.0 unx     1807 b- defN 23-Jun-07 12:02 super_gradients/evaluate_from_recipe.py
--rw-r--r--  2.0 unx      639 b- defN 23-Jun-07 12:02 super_gradients/qat_from_recipe.py
--rwxr-xr-x  2.0 unx       28 b- defN 23-Jun-07 12:03 super_gradients/requirements.pro.txt
--rwxr-xr-x  2.0 unx      729 b- defN 23-Jun-07 12:03 super_gradients/requirements.txt
--rw-r--r--  2.0 unx      537 b- defN 23-Jun-07 12:02 super_gradients/resume_experiment.py
--rw-r--r--  2.0 unx      693 b- defN 23-Jun-07 12:02 super_gradients/train_from_kd_recipe.py
--rw-r--r--  2.0 unx      650 b- defN 23-Jun-07 12:02 super_gradients/train_from_recipe.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Jun-07 12:02 super_gradients/common/__init__.py
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-07 12:02 super_gradients/common/object_names.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/abstractions/__init__.py
--rw-r--r--  2.0 unx      879 b- defN 23-Jun-07 12:02 super_gradients/common/abstractions/abstract_logger.py
--rw-r--r--  2.0 unx     3129 b- defN 23-Jun-07 12:02 super_gradients/common/abstractions/mute_processes.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/auto_logging/__init__.py
--rw-r--r--  2.0 unx     4846 b- defN 23-Jun-07 12:02 super_gradients/common/auto_logging/auto_logger.py
--rw-r--r--  2.0 unx     6625 b- defN 23-Jun-07 12:02 super_gradients/common/auto_logging/console_logging.py
--rw-r--r--  2.0 unx      142 b- defN 23-Jun-07 12:02 super_gradients/common/aws_connection/__init__.py
--rw-r--r--  2.0 unx     4182 b- defN 23-Jun-07 12:02 super_gradients/common/aws_connection/aws_connector.py
--rw-r--r--  2.0 unx     7198 b- defN 23-Jun-07 12:02 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
--rw-r--r--  2.0 unx      119 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/crash_handler.py
--rw-r--r--  2.0 unx    11775 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/crash_tips.py
--rw-r--r--  2.0 unx      886 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/crash_tips_setup.py
--rw-r--r--  2.0 unx     1740 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/exception.py
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/exception_monitoring_setup.py
--rw-r--r--  2.0 unx      789 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/utils.py
--rw-r--r--  2.0 unx      140 b- defN 23-Jun-07 12:02 super_gradients/common/data_connection/__init__.py
--rw-r--r--  2.0 unx    17959 b- defN 23-Jun-07 12:02 super_gradients/common/data_connection/s3_connector.py
--rw-r--r--  2.0 unx      325 b- defN 23-Jun-07 12:02 super_gradients/common/data_interface/__init__.py
--rw-r--r--  2.0 unx     9699 b- defN 23-Jun-07 12:02 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
--rw-r--r--  2.0 unx     2050 b- defN 23-Jun-07 12:02 super_gradients/common/data_interface/dataset_data_interface.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/__init__.py
--rw-r--r--  2.0 unx      597 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/__init__.py
--rw-r--r--  2.0 unx      309 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/deep_learning_task.py
--rw-r--r--  2.0 unx      108 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/downsample_mode.py
--rw-r--r--  2.0 unx      317 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/evaluation_type.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/multi_gpu_mode.py
--rw-r--r--  2.0 unx     1200 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/strict_load.py
--rw-r--r--  2.0 unx      202 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/upsample_mode.py
--rw-r--r--  2.0 unx      257 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/code_save_decorator.py
--rw-r--r--  2.0 unx     3663 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/deci_logger.py
--rw-r--r--  2.0 unx     2921 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/explicit_params_validator.py
--rw-r--r--  2.0 unx     1315 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/factory_decorator.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/singleton.py
--rw-r--r--  2.0 unx      202 b- defN 23-Jun-07 12:02 super_gradients/common/environment/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Jun-07 12:02 super_gradients/common/environment/argparse_utils.py
--rw-r--r--  2.0 unx     9170 b- defN 23-Jun-07 12:02 super_gradients/common/environment/cfg_utils.py
--rw-r--r--  2.0 unx     4383 b- defN 23-Jun-07 12:02 super_gradients/common/environment/checkpoints_dir_utils.py
--rw-r--r--  2.0 unx     2682 b- defN 23-Jun-07 12:02 super_gradients/common/environment/ddp_utils.py
--rw-r--r--  2.0 unx      752 b- defN 23-Jun-07 12:02 super_gradients/common/environment/device_utils.py
--rw-r--r--  2.0 unx      927 b- defN 23-Jun-07 12:02 super_gradients/common/environment/env_variables.py
--rw-r--r--  2.0 unx     4047 b- defN 23-Jun-07 12:02 super_gradients/common/environment/omegaconf_utils.py
--rw-r--r--  2.0 unx      459 b- defN 23-Jun-07 12:02 super_gradients/common/environment/path_utils.py
--rw-r--r--  2.0 unx      112 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/__init__.py
--rw-r--r--  2.0 unx      153 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/cpu.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/data_models.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/disk.py
--rw-r--r--  2.0 unx     5427 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/monitoring.py
--rw-r--r--  2.0 unx      948 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/network.py
--rw-r--r--  2.0 unx      629 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/utils.py
--rw-r--r--  2.0 unx      145 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/virtual_memory.py
--rw-r--r--  2.0 unx      681 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/gpu/__init__.py
--rw-r--r--  2.0 unx     2270 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/gpu/gpu.py
--rw-r--r--  2.0 unx   121647 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/gpu/pynvml.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/exceptions/__init__.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jun-07 12:02 super_gradients/common/exceptions/factory_exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/factories/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-Jun-07 12:02 super_gradients/common/factories/activations_type_factory.py
--rw-r--r--  2.0 unx     2881 b- defN 23-Jun-07 12:02 super_gradients/common/factories/base_factory.py
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-07 12:02 super_gradients/common/factories/bbox_format_factory.py
--rw-r--r--  2.0 unx      232 b- defN 23-Jun-07 12:02 super_gradients/common/factories/callbacks_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-Jun-07 12:02 super_gradients/common/factories/collate_functions_factory.py
--rw-r--r--  2.0 unx      292 b- defN 23-Jun-07 12:02 super_gradients/common/factories/context_modules_factory.py
--rw-r--r--  2.0 unx      321 b- defN 23-Jun-07 12:02 super_gradients/common/factories/data_formats_factory.py
--rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/common/factories/datasets_factory.py
--rw-r--r--  2.0 unx     1014 b- defN 23-Jun-07 12:02 super_gradients/common/factories/detection_modules_factory.py
--rw-r--r--  2.0 unx      572 b- defN 23-Jun-07 12:02 super_gradients/common/factories/list_factory.py
--rw-r--r--  2.0 unx      223 b- defN 23-Jun-07 12:02 super_gradients/common/factories/losses_factory.py
--rw-r--r--  2.0 unx      226 b- defN 23-Jun-07 12:02 super_gradients/common/factories/metrics_factory.py
--rw-r--r--  2.0 unx      467 b- defN 23-Jun-07 12:02 super_gradients/common/factories/optimizers_type_factory.py
--rw-r--r--  2.0 unx      271 b- defN 23-Jun-07 12:02 super_gradients/common/factories/pre_launch_callbacks_factory.py
--rw-r--r--  2.0 unx      623 b- defN 23-Jun-07 12:02 super_gradients/common/factories/processing_factory.py
--rw-r--r--  2.0 unx      229 b- defN 23-Jun-07 12:02 super_gradients/common/factories/samplers_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-Jun-07 12:02 super_gradients/common/factories/target_generator_factory.py
--rw-r--r--  2.0 unx     1873 b- defN 23-Jun-07 12:02 super_gradients/common/factories/transforms_factory.py
--rw-r--r--  2.0 unx     2377 b- defN 23-Jun-07 12:02 super_gradients/common/factories/type_factory.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/__init__.py
--rw-r--r--  2.0 unx    12245 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/deci_client.py
--rw-r--r--  2.0 unx      143 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/wandb/__init__.py
--rw-r--r--  2.0 unx     2329 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/wandb/log_predictions.py
--rw-r--r--  2.0 unx      271 b- defN 23-Jun-07 12:02 super_gradients/common/registry/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Jun-07 12:02 super_gradients/common/registry/albumentation.py
--rw-r--r--  2.0 unx     6006 b- defN 23-Jun-07 12:02 super_gradients/common/registry/registry.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/registry/registry_utils.py
--rw-r--r--  2.0 unx      508 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/__init__.py
--rw-r--r--  2.0 unx     7460 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/abstract_sg_logger.py
--rw-r--r--  2.0 unx    15095 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/base_sg_logger.py
--rw-r--r--  2.0 unx    10055 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/clearml_sg_logger.py
--rw-r--r--  2.0 unx    10103 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/dagshub_sg_logger.py
--rw-r--r--  2.0 unx     6618 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
--rw-r--r--  2.0 unx    15000 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/wandb_sg_logger.py
--rw-r--r--  2.0 unx    85509 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_Walkthrough.ipynb
--rw-r--r--  2.0 unx    69618 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_quickstart_classification.ipynb
--rw-r--r--  2.0 unx    54966 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
--rw-r--r--  2.0 unx    65090 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/cifar10_training_torch_objects/__init__.py
--rw-r--r--  2.0 unx     2526 b- defN 23-Jun-07 12:02 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/convert_recipe_example/__init__.py
--rw-r--r--  2.0 unx      870 b- defN 23-Jun-07 12:02 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/ddrnet_imagenet/__init__.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Jun-07 12:02 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/deci_lab_export_example/__init__.py
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-07 12:02 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/early_stop/__init__.py
--rw-r--r--  2.0 unx     1596 b- defN 23-Jun-07 12:02 super_gradients/examples/early_stop/early_stop_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_checkpoint_example/__init__.py
--rw-r--r--  2.0 unx      289 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/loggers_examples/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-Jun-07 12:02 super_gradients/examples/loggers_examples/clearml_logger_example.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Jun-07 12:02 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/qat_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      277 b- defN 23-Jun-07 12:02 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/non_default_calibrators_example.py
--rw-r--r--  2.0 unx     2310 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/ptq_e2e_example.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
--rw-r--r--  2.0 unx     4732 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/resnet_qat_example.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/skipping_quantization_example.py
--rw-r--r--  2.0 unx      832 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/vanilla_quantize_all_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/regseg_transfer_learning_example/__init__.py
--rw-r--r--  2.0 unx     2379 b- defN 23-Jun-07 12:02 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/resume_experiment_example/__init__.py
--rw-r--r--  2.0 unx      283 b- defN 23-Jun-07 12:02 super_gradients/examples/resume_experiment_example/resume_experiment.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_kd_recipe_example/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      283 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
--rw-r--r--  2.0 unx     1643 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_user_objects/train.py
--rw-r--r--  2.0 unx     2548 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
--rw-r--r--  2.0 unx      174 b- defN 23-Jun-07 12:02 super_gradients/module_interfaces/__init__.py
--rw-r--r--  2.0 unx     2043 b- defN 23-Jun-07 12:02 super_gradients/module_interfaces/module_interfaces.py
--rw-r--r--  2.0 unx     3366 b- defN 23-Jun-07 12:02 super_gradients/modules/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/modules/all_detection_modules.py
--rw-r--r--  2.0 unx      617 b- defN 23-Jun-07 12:02 super_gradients/modules/anti_alias.py
--rw-r--r--  2.0 unx      776 b- defN 23-Jun-07 12:02 super_gradients/modules/base_modules.py
--rw-r--r--  2.0 unx     3054 b- defN 23-Jun-07 12:02 super_gradients/modules/conv_bn_act_block.py
--rw-r--r--  2.0 unx     1976 b- defN 23-Jun-07 12:02 super_gradients/modules/conv_bn_relu_block.py
--rw-r--r--  2.0 unx    14805 b- defN 23-Jun-07 12:02 super_gradients/modules/detection_modules.py
--rw-r--r--  2.0 unx     2143 b- defN 23-Jun-07 12:02 super_gradients/modules/head_replacement_utils.py
--rw-r--r--  2.0 unx     4362 b- defN 23-Jun-07 12:02 super_gradients/modules/multi_output_modules.py
--rw-r--r--  2.0 unx      860 b- defN 23-Jun-07 12:02 super_gradients/modules/pixel_shuffle.py
--rw-r--r--  2.0 unx     3927 b- defN 23-Jun-07 12:02 super_gradients/modules/pose_estimation_modules.py
--rw-r--r--  2.0 unx    12250 b- defN 23-Jun-07 12:02 super_gradients/modules/qarepvgg_block.py
--rw-r--r--  2.0 unx     8699 b- defN 23-Jun-07 12:02 super_gradients/modules/repvgg_block.py
--rw-r--r--  2.0 unx     2138 b- defN 23-Jun-07 12:02 super_gradients/modules/sampling.py
--rw-r--r--  2.0 unx     1459 b- defN 23-Jun-07 12:02 super_gradients/modules/se_blocks.py
--rw-r--r--  2.0 unx     1403 b- defN 23-Jun-07 12:02 super_gradients/modules/skip_connections.py
--rw-r--r--  2.0 unx     2968 b- defN 23-Jun-07 12:02 super_gradients/modules/utils.py
--rw-r--r--  2.0 unx      716 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/quantized_skip_connections.py
--rw-r--r--  2.0 unx     4604 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/quantized_stdc_blocks.py
--rw-r--r--  2.0 unx     1281 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/resnet_bottleneck.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/recipes/__init__.py
--rw-r--r--  2.0 unx     1136 b- defN 23-Jun-07 12:02 super_gradients/recipes/cifar10_resnet.yaml
--rw-r--r--  2.0 unx     2727 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_al_ddrnet.yaml
--rw-r--r--  2.0 unx     3502 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_ddrnet.yaml
--rw-r--r--  2.0 unx     3754 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_kd_base.yaml
--rw-r--r--  2.0 unx     3354 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_pplite_seg50.yaml
--rw-r--r--  2.0 unx     3253 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_pplite_seg75.yaml
--rw-r--r--  2.0 unx     2498 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_regseg48.yaml
--rw-r--r--  2.0 unx     4020 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_segformer.yaml
--rw-r--r--  2.0 unx      618 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_stdc_base.yaml
--rw-r--r--  2.0 unx     2862 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_stdc_seg50.yaml
--rw-r--r--  2.0 unx     3055 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_stdc_seg75.yaml
--rw-r--r--  2.0 unx     1620 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_pose_dekr_rescoring.yaml
--rw-r--r--  2.0 unx     2992 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
--rw-r--r--  2.0 unx     1996 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_l.yaml
--rw-r--r--  2.0 unx     1996 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_m.yaml
--rw-r--r--  2.0 unx     1882 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_s.yaml
--rw-r--r--  2.0 unx     1975 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_x.yaml
--rw-r--r--  2.0 unx     1889 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
--rw-r--r--  2.0 unx     1385 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_yolo_nas_s.yaml
--rw-r--r--  2.0 unx     2583 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_yolox.yaml
--rw-r--r--  2.0 unx     1376 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
--rw-r--r--  2.0 unx     1145 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_efficientnet.yaml
--rw-r--r--  2.0 unx     1129 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv2.yaml
--rw-r--r--  2.0 unx      507 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
--rw-r--r--  2.0 unx      719 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
--rw-r--r--  2.0 unx      719 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
--rw-r--r--  2.0 unx     1997 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_regnetY.yaml
--rw-r--r--  2.0 unx     1246 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_repvgg.yaml
--rw-r--r--  2.0 unx     1169 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_resnet50.yaml
--rw-r--r--  2.0 unx     2722 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_resnet50_kd.yaml
--rw-r--r--  2.0 unx     1136 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_vit_base.yaml
--rw-r--r--  2.0 unx     1010 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_vit_large.yaml
--rw-r--r--  2.0 unx     2007 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_ppyoloe.yaml
--rw-r--r--  2.0 unx     2347 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolo_nas_m.yaml
--rw-r--r--  2.0 unx     2347 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolo_nas_s.yaml
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
--rw-r--r--  2.0 unx     1915 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolox.yaml
--rw-r--r--  2.0 unx     1344 b- defN 23-Jun-07 12:02 super_gradients/recipes/script_generate_rescoring_data_dekr_coco2017.yaml
--rw-r--r--  2.0 unx     1246 b- defN 23-Jun-07 12:02 super_gradients/recipes/supervisely_unet.yaml
--rw-r--r--  2.0 unx     1672 b- defN 23-Jun-07 12:02 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
--rw-r--r--  2.0 unx     2133 b- defN 23-Jun-07 12:02 super_gradients/recipes/user_recipe_mnist_example.yaml
--rw-r--r--  2.0 unx     2000 b- defN 23-Jun-07 12:02 super_gradients/recipes/variable_setup.yaml
--rw-r--r--  2.0 unx     2222 b- defN 23-Jun-07 12:02 super_gradients/recipes/anchors/ssd_anchors.yaml
--rw-r--r--  2.0 unx      563 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
--rw-r--r--  2.0 unx      104 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
--rw-r--r--  2.0 unx      194 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
--rw-r--r--  2.0 unx      409 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
--rw-r--r--  2.0 unx      356 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
--rw-r--r--  2.0 unx      324 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml
--rw-r--r--  2.0 unx     1113 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
--rw-r--r--  2.0 unx      985 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
--rw-r--r--  2.0 unx     1112 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
--rw-r--r--  2.0 unx      196 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
--rw-r--r--  2.0 unx      352 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
--rw-r--r--  2.0 unx       98 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
--rw-r--r--  2.0 unx       89 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
--rw-r--r--  2.0 unx       88 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
--rw-r--r--  2.0 unx       32 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
--rw-r--r--  2.0 unx      655 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
--rw-r--r--  2.0 unx      605 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
--rw-r--r--  2.0 unx     1369 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/unet_arch_params.yaml
--rw-r--r--  2.0 unx     3031 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
--rw-r--r--  2.0 unx       63 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
--rw-r--r--  2.0 unx     2393 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_arch_params.yaml
--rw-r--r--  2.0 unx     2353 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
--rw-r--r--  2.0 unx     2362 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
--rw-r--r--  2.0 unx     2357 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
--rw-r--r--  2.0 unx      235 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
--rw-r--r--  2.0 unx      229 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
--rw-r--r--  2.0 unx      228 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
--rw-r--r--  2.0 unx      622 b- defN 23-Jun-07 12:02 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
--rw-r--r--  2.0 unx       72 b- defN 23-Jun-07 12:02 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/recipes/conversion_params/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 23-Jun-07 12:02 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
--rw-r--r--  2.0 unx     2040 b- defN 23-Jun-07 12:02 super_gradients/recipes/conversion_params/default_conversion_params.yaml
--rw-r--r--  2.0 unx      869 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
--rw-r--r--  2.0 unx     1530 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
--rw-r--r--  2.0 unx     1056 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
--rw-r--r--  2.0 unx     1328 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_al_dataset_params.yaml
--rw-r--r--  2.0 unx      615 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
--rw-r--r--  2.0 unx      525 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
--rw-r--r--  2.0 unx      706 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx      644 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
--rw-r--r--  2.0 unx      721 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
--rw-r--r--  2.0 unx      709 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
--rw-r--r--  2.0 unx      708 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx     3946 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     4202 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
--rw-r--r--  2.0 unx     3590 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
--rw-r--r--  2.0 unx     5568 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
--rw-r--r--  2.0 unx     3684 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
--rw-r--r--  2.0 unx     2700 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
--rw-r--r--  2.0 unx      405 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
--rw-r--r--  2.0 unx      842 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml
--rw-r--r--  2.0 unx     1466 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx      931 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx      732 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
--rw-r--r--  2.0 unx      142 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
--rw-r--r--  2.0 unx      734 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
--rw-r--r--  2.0 unx     1059 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
--rw-r--r--  2.0 unx     1093 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
--rw-r--r--  2.0 unx      845 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
--rw-r--r--  2.0 unx     1762 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
--rw-r--r--  2.0 unx      149 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     1571 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     1414 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     4112 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
--rw-r--r--  2.0 unx      961 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
--rw-r--r--  2.0 unx      559 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx     1155 b- defN 23-Jun-07 12:02 super_gradients/recipes/quantization_params/default_quantization_params.yaml
--rw-r--r--  2.0 unx      591 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
--rw-r--r--  2.0 unx      700 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
--rw-r--r--  2.0 unx     2063 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
--rw-r--r--  2.0 unx     1302 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
--rw-r--r--  2.0 unx      771 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_rescoring_train_params.yaml
--rw-r--r--  2.0 unx      723 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
--rw-r--r--  2.0 unx     1121 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
--rw-r--r--  2.0 unx      956 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
--rw-r--r--  2.0 unx      461 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
--rw-r--r--  2.0 unx     6081 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/default_train_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
--rw-r--r--  2.0 unx      742 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
--rw-r--r--  2.0 unx      549 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
--rw-r--r--  2.0 unx      795 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
--rw-r--r--  2.0 unx      476 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
--rw-r--r--  2.0 unx      484 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
--rw-r--r--  2.0 unx      522 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
--rw-r--r--  2.0 unx      602 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
--rw-r--r--  2.0 unx      519 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
--rw-r--r--  2.0 unx      107 b- defN 23-Jun-07 12:02 super_gradients/sanity_check/__init__.py
--rw-r--r--  2.0 unx     5267 b- defN 23-Jun-07 12:02 super_gradients/sanity_check/env_sanity_check.py
--rw-r--r--  2.0 unx      775 b- defN 23-Jun-07 12:02 super_gradients/training/__init__.py
--rw-r--r--  2.0 unx     4715 b- defN 23-Jun-07 12:02 super_gradients/training/params.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Jun-07 12:02 super_gradients/training/pretrained_models.py
--rw-r--r--  2.0 unx     3344 b- defN 23-Jun-07 12:02 super_gradients/training/dataloaders/__init__.py
--rw-r--r--  2.0 unx    36154 b- defN 23-Jun-07 12:02 super_gradients/training/dataloaders/dataloaders.py
--rw-r--r--  2.0 unx     1867 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/__init__.py
--rw-r--r--  2.0 unx    14162 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/auto_augment.py
--rw-r--r--  2.0 unx     3705 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_augmentation.py
--rw-r--r--  2.0 unx     3484 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/datasets_conf.py
--rw-r--r--  2.0 unx    29577 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/datasets_utils.py
--rw-r--r--  2.0 unx    14663 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/mixup.py
--rw-r--r--  2.0 unx    11746 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/sg_dataset.py
--rw-r--r--  2.0 unx      252 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/classification_datasets/__init__.py
--rw-r--r--  2.0 unx     3096 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/classification_datasets/cifar.py
--rw-r--r--  2.0 unx     1706 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
--rw-r--r--  2.0 unx      862 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/default_formats.py
--rw-r--r--  2.0 unx     3071 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/format_converter.py
--rw-r--r--  2.0 unx     7928 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/formats.py
--rw-r--r--  2.0 unx     1044 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
--rw-r--r--  2.0 unx     2674 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
--rw-r--r--  2.0 unx     5131 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
--rw-r--r--  2.0 unx     2089 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
--rw-r--r--  2.0 unx     2043 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
--rw-r--r--  2.0 unx     5043 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
--rw-r--r--  2.0 unx     2948 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
--rw-r--r--  2.0 unx      575 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
--rw-r--r--  2.0 unx     1792 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
--rw-r--r--  2.0 unx     8373 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
--rw-r--r--  2.0 unx      683 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/__init__.py
--rw-r--r--  2.0 unx     2505 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/coco_detection.py
--rw-r--r--  2.0 unx     9258 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
--rw-r--r--  2.0 unx    26566 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/detection_dataset.py
--rw-r--r--  2.0 unx    11353 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
--rw-r--r--  2.0 unx    11120 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
--rw-r--r--  2.0 unx      328 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
--rw-r--r--  2.0 unx    18882 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
--rw-r--r--  2.0 unx     3503 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
--rw-r--r--  2.0 unx     1997 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
--rw-r--r--  2.0 unx      502 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
--rw-r--r--  2.0 unx     4910 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
--rw-r--r--  2.0 unx     9088 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
--rw-r--r--  2.0 unx     5929 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
--rw-r--r--  2.0 unx     3736 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/rescoring_dataset.py
--rw-r--r--  2.0 unx    10281 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
--rw-r--r--  2.0 unx      385 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/samplers/__init__.py
--rw-r--r--  2.0 unx      738 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/samplers/infinite_sampler.py
--rw-r--r--  2.0 unx     4809 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
--rw-r--r--  2.0 unx     1093 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/__init__.py
--rw-r--r--  2.0 unx     8304 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
--rw-r--r--  2.0 unx     7757 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
--rw-r--r--  2.0 unx     5518 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
--rw-r--r--  2.0 unx    11146 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
--rw-r--r--  2.0 unx     8572 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
--rw-r--r--  2.0 unx     3062 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/__init__.py
--rw-r--r--  2.0 unx     1761 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/dataset_exceptions.py
--rw-r--r--  2.0 unx     2826 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/kd_trainer_exceptions.py
--rw-r--r--  2.0 unx      946 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/loss_exceptions.py
--rw-r--r--  2.0 unx     1268 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/sg_trainer_exceptions.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jun-07 12:02 super_gradients/training/kd_trainer/__init__.py
--rw-r--r--  2.0 unx    16582 b- defN 23-Jun-07 12:02 super_gradients/training/kd_trainer/kd_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/legacy/__init__.py
--rw-r--r--  2.0 unx     4198 b- defN 23-Jun-07 12:02 super_gradients/training/legacy/utils.py
--rw-r--r--  2.0 unx     1570 b- defN 23-Jun-07 12:02 super_gradients/training/losses/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/losses/all_losses.py
--rw-r--r--  2.0 unx     1219 b- defN 23-Jun-07 12:02 super_gradients/training/losses/bce_dice_loss.py
--rw-r--r--  2.0 unx      419 b- defN 23-Jun-07 12:02 super_gradients/training/losses/bce_loss.py
--rw-r--r--  2.0 unx     2374 b- defN 23-Jun-07 12:02 super_gradients/training/losses/cwd_loss.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ddrnet_loss.py
--rw-r--r--  2.0 unx     4038 b- defN 23-Jun-07 12:02 super_gradients/training/losses/dekr_loss.py
--rw-r--r--  2.0 unx     5618 b- defN 23-Jun-07 12:02 super_gradients/training/losses/dice_ce_edge_loss.py
--rw-r--r--  2.0 unx     5208 b- defN 23-Jun-07 12:02 super_gradients/training/losses/dice_loss.py
--rw-r--r--  2.0 unx     1214 b- defN 23-Jun-07 12:02 super_gradients/training/losses/focal_loss.py
--rw-r--r--  2.0 unx     5051 b- defN 23-Jun-07 12:02 super_gradients/training/losses/iou_loss.py
--rw-r--r--  2.0 unx     2176 b- defN 23-Jun-07 12:02 super_gradients/training/losses/kd_losses.py
--rw-r--r--  2.0 unx     4177 b- defN 23-Jun-07 12:02 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
--rw-r--r--  2.0 unx      550 b- defN 23-Jun-07 12:02 super_gradients/training/losses/loss_utils.py
--rw-r--r--  2.0 unx     4004 b- defN 23-Jun-07 12:02 super_gradients/training/losses/mask_loss.py
--rw-r--r--  2.0 unx     4129 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ohem_ce_loss.py
--rw-r--r--  2.0 unx    41319 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ppyolo_loss.py
--rw-r--r--  2.0 unx     1010 b- defN 23-Jun-07 12:02 super_gradients/training/losses/r_squared_loss.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jun-07 12:02 super_gradients/training/losses/rescoring_loss.py
--rw-r--r--  2.0 unx     3453 b- defN 23-Jun-07 12:02 super_gradients/training/losses/seg_kd_loss.py
--rw-r--r--  2.0 unx     1650 b- defN 23-Jun-07 12:02 super_gradients/training/losses/shelfnet_ohem_loss.py
--rw-r--r--  2.0 unx     1949 b- defN 23-Jun-07 12:02 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
--rw-r--r--  2.0 unx     8794 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ssd_loss.py
--rw-r--r--  2.0 unx     9721 b- defN 23-Jun-07 12:02 super_gradients/training/losses/stdc_loss.py
--rw-r--r--  2.0 unx     5771 b- defN 23-Jun-07 12:02 super_gradients/training/losses/structure_loss.py
--rw-r--r--  2.0 unx    50149 b- defN 23-Jun-07 12:02 super_gradients/training/losses/yolox_loss.py
--rw-r--r--  2.0 unx     1052 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/all_metrics.py
--rw-r--r--  2.0 unx     3262 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/classification_metrics.py
--rw-r--r--  2.0 unx    10741 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/detection_metrics.py
--rw-r--r--  2.0 unx     3973 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/metric_utils.py
--rw-r--r--  2.0 unx    15404 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/pose_estimation_metrics.py
--rw-r--r--  2.0 unx    11536 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/pose_estimation_utils.py
--rw-r--r--  2.0 unx    11935 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/segmentation_metrics.py
--rw-r--r--  2.0 unx    11245 b- defN 23-Jun-07 12:02 super_gradients/training/models/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Jun-07 12:02 super_gradients/training/models/arch_params_factory.py
--rw-r--r--  2.0 unx    12587 b- defN 23-Jun-07 12:02 super_gradients/training/models/conversion.py
--rw-r--r--  2.0 unx    11887 b- defN 23-Jun-07 12:02 super_gradients/training/models/model_factory.py
--rw-r--r--  2.0 unx    10997 b- defN 23-Jun-07 12:02 super_gradients/training/models/prediction_results.py
--rw-r--r--  2.0 unx     2054 b- defN 23-Jun-07 12:02 super_gradients/training/models/predictions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/results.py
--rw-r--r--  2.0 unx     2998 b- defN 23-Jun-07 12:02 super_gradients/training/models/sg_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/__init__.py
--rw-r--r--  2.0 unx    20025 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/beit.py
--rw-r--r--  2.0 unx     7472 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/densenet.py
--rw-r--r--  2.0 unx     3707 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/dpn.py
--rw-r--r--  2.0 unx    36745 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/efficientnet.py
--rw-r--r--  2.0 unx     8862 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/googlenet.py
--rw-r--r--  2.0 unx      798 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/lenet.py
--rw-r--r--  2.0 unx     2407 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/mobilenet.py
--rw-r--r--  2.0 unx     9472 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/mobilenetv2.py
--rw-r--r--  2.0 unx     8696 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/mobilenetv3.py
--rw-r--r--  2.0 unx     4339 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/pnasnet.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/preact_resnet.py
--rw-r--r--  2.0 unx    13599 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/regnet.py
--rw-r--r--  2.0 unx     7924 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/repvgg.py
--rw-r--r--  2.0 unx    15067 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/resnet.py
--rw-r--r--  2.0 unx     6294 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/resnext.py
--rw-r--r--  2.0 unx     4134 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/senet.py
--rw-r--r--  2.0 unx     3660 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/shufflenet.py
--rw-r--r--  2.0 unx     9768 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/shufflenetv2.py
--rw-r--r--  2.0 unx     1538 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/vgg.py
--rw-r--r--  2.0 unx     9210 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/vit.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/__init__.py
--rw-r--r--  2.0 unx     9130 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/csp_darknet53.py
--rw-r--r--  2.0 unx     9814 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/csp_resnet.py
--rw-r--r--  2.0 unx     9986 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/customizable_detector.py
--rw-r--r--  2.0 unx     4746 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/darknet53.py
--rw-r--r--  2.0 unx     2315 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/ssd.py
--rw-r--r--  2.0 unx    30262 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_base.py
--rw-r--r--  2.0 unx     2459 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolox.py
--rw-r--r--  2.0 unx      251 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
--rw-r--r--  2.0 unx     7000 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
--rw-r--r--  2.0 unx     3487 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
--rw-r--r--  2.0 unx     9023 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
--rw-r--r--  2.0 unx    12397 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
--rw-r--r--  2.0 unx      756 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/__init__.py
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
--rw-r--r--  2.0 unx     2646 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/panneck.py
--rw-r--r--  2.0 unx     4166 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
--rw-r--r--  2.0 unx    13329 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/kd_modules/__init__.py
--rw-r--r--  2.0 unx     3553 b- defN 23-Jun-07 12:02 super_gradients/training/models/kd_modules/kd_module.py
--rw-r--r--  2.0 unx      179 b- defN 23-Jun-07 12:02 super_gradients/training/models/pose_estimation_models/__init__.py
--rw-r--r--  2.0 unx    23096 b- defN 23-Jun-07 12:02 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
--rw-r--r--  2.0 unx     4298 b- defN 23-Jun-07 12:02 super_gradients/training/models/pose_estimation_models/rescoring_net.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/__init__.py
--rw-r--r--  2.0 unx      964 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/common.py
--rw-r--r--  2.0 unx     5139 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/context_modules.py
--rw-r--r--  2.0 unx    28514 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/ddrnet.py
--rw-r--r--  2.0 unx     2439 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
--rw-r--r--  2.0 unx    21760 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/laddernet.py
--rw-r--r--  2.0 unx    15648 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/ppliteseg.py
--rw-r--r--  2.0 unx    14424 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/regseg.py
--rw-r--r--  2.0 unx    20334 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/segformer.py
--rw-r--r--  2.0 unx     2256 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/segmentation_module.py
--rw-r--r--  2.0 unx    24851 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/shelfnet.py
--rw-r--r--  2.0 unx    29091 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/stdc.py
--rw-r--r--  2.0 unx      260 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/__init__.py
--rw-r--r--  2.0 unx    12324 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/unet.py
--rw-r--r--  2.0 unx    10718 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
--rw-r--r--  2.0 unx    13292 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
--rw-r--r--  2.0 unx      119 b- defN 23-Jun-07 12:02 super_gradients/training/models/user_models/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/pipelines/__init__.py
--rw-r--r--  2.0 unx    15639 b- defN 23-Jun-07 12:02 super_gradients/training/pipelines/pipelines.py
--rw-r--r--  2.0 unx      445 b- defN 23-Jun-07 12:02 super_gradients/training/pre_launch_callbacks/__init__.py
--rw-r--r--  2.0 unx    21020 b- defN 23-Jun-07 12:02 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
--rw-r--r--  2.0 unx      517 b- defN 23-Jun-07 12:02 super_gradients/training/processing/__init__.py
--rw-r--r--  2.0 unx    13177 b- defN 23-Jun-07 12:02 super_gradients/training/processing/processing.py
--rw-r--r--  2.0 unx       98 b- defN 23-Jun-07 12:02 super_gradients/training/qat_trainer/__init__.py
--rw-r--r--  2.0 unx      608 b- defN 23-Jun-07 12:02 super_gradients/training/qat_trainer/qat_trainer.py
--rw-r--r--  2.0 unx      184 b- defN 23-Jun-07 12:02 super_gradients/training/sg_trainer/__init__.py
--rw-r--r--  2.0 unx   116430 b- defN 23-Jun-07 12:02 super_gradients/training/sg_trainer/sg_trainer.py
--rw-r--r--  2.0 unx     1685 b- defN 23-Jun-07 12:02 super_gradients/training/training_hyperparams/__init__.py
--rw-r--r--  2.0 unx     3774 b- defN 23-Jun-07 12:02 super_gradients/training/training_hyperparams/training_hyperparams.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/all_transforms.py
--rw-r--r--  2.0 unx    16193 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/keypoint_transforms.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/pipeline_adaptors.py
--rw-r--r--  2.0 unx    55587 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/transforms.py
--rw-r--r--  2.0 unx     6048 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/utils.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jun-07 12:02 super_gradients/training/utils/__init__.py
--rw-r--r--  2.0 unx     1673 b- defN 23-Jun-07 12:02 super_gradients/training/utils/activations_utils.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Jun-07 12:02 super_gradients/training/utils/bbox_utils.py
--rw-r--r--  2.0 unx    15712 b- defN 23-Jun-07 12:02 super_gradients/training/utils/checkpoint_utils.py
--rw-r--r--  2.0 unx     9794 b- defN 23-Jun-07 12:02 super_gradients/training/utils/config_utils.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Jun-07 12:02 super_gradients/training/utils/deprecated_utils.py
--rw-r--r--  2.0 unx    53289 b- defN 23-Jun-07 12:02 super_gradients/training/utils/detection_utils.py
--rw-r--r--  2.0 unx    16195 b- defN 23-Jun-07 12:02 super_gradients/training/utils/distributed_training_utils.py
--rw-r--r--  2.0 unx     6352 b- defN 23-Jun-07 12:02 super_gradients/training/utils/early_stopping.py
--rw-r--r--  2.0 unx     9322 b- defN 23-Jun-07 12:02 super_gradients/training/utils/ema.py
--rw-r--r--  2.0 unx     2610 b- defN 23-Jun-07 12:02 super_gradients/training/utils/ema_decay_schedules.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Jun-07 12:02 super_gradients/training/utils/export_utils.py
--rw-r--r--  2.0 unx     7508 b- defN 23-Jun-07 12:02 super_gradients/training/utils/get_model_stats.py
--rw-r--r--  2.0 unx      771 b- defN 23-Jun-07 12:02 super_gradients/training/utils/kd_trainer_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/load_image.py
--rw-r--r--  2.0 unx     5827 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizer_utils.py
--rw-r--r--  2.0 unx      839 b- defN 23-Jun-07 12:02 super_gradients/training/utils/regularization_utils.py
--rw-r--r--  2.0 unx    10388 b- defN 23-Jun-07 12:02 super_gradients/training/utils/segmentation_utils.py
--rw-r--r--  2.0 unx    19625 b- defN 23-Jun-07 12:02 super_gradients/training/utils/sg_trainer_utils.py
--rw-r--r--  2.0 unx     6272 b- defN 23-Jun-07 12:02 super_gradients/training/utils/ssd_utils.py
--rw-r--r--  2.0 unx    20438 b- defN 23-Jun-07 12:02 super_gradients/training/utils/utils.py
--rw-r--r--  2.0 unx      303 b- defN 23-Jun-07 12:02 super_gradients/training/utils/version_utils.py
--rw-r--r--  2.0 unx     5687 b- defN 23-Jun-07 12:02 super_gradients/training/utils/weight_averaging_utils.py
--rw-r--r--  2.0 unx     2030 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/all_callbacks.py
--rw-r--r--  2.0 unx    20126 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/base_callbacks.py
--rw-r--r--  2.0 unx    33409 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/callbacks.py
--rw-r--r--  2.0 unx     1169 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/__init__.py
--rw-r--r--  2.0 unx     5880 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/image.py
--rw-r--r--  2.0 unx     4046 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/stream.py
--rw-r--r--  2.0 unx     6926 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/video.py
--rw-r--r--  2.0 unx      396 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/__init__.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/all_optimizers.py
--rw-r--r--  2.0 unx     9760 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/lamb.py
--rw-r--r--  2.0 unx     3008 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/lion.py
--rw-r--r--  2.0 unx     6834 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/rmsprop_tf.py
--rw-r--r--  2.0 unx      324 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/__init__.py
--rw-r--r--  2.0 unx    11309 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
--rw-r--r--  2.0 unx     7140 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
--rw-r--r--  2.0 unx      920 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/rescoring_callback.py
--rw-r--r--  2.0 unx      387 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/__init__.py
--rw-r--r--  2.0 unx     6271 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/calibrator.py
--rw-r--r--  2.0 unx     8417 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/core.py
--rw-r--r--  2.0 unx     2504 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/export.py
--rw-r--r--  2.0 unx    17062 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/selective_quantization_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/visualization/__init__.py
--rw-r--r--  2.0 unx     1698 b- defN 23-Jun-07 12:02 super_gradients/training/utils/visualization/detection.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-07 12:02 super_gradients/training/utils/visualization/utils.py
--rw-r--r--  2.0 unx     2218 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md
--rw-r--r--  2.0 unx    11341 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    35552 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    65481 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/RECORD
-567 files, 2880515 bytes uncompressed, 873153 bytes compressed:  69.7%
+Zip file size: 1018089 bytes, number of entries: 575
+-rw-r--r--  2.0 unx      916 b- defN 23-Jul-19 09:35 super_gradients/__init__.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-Jul-19 09:35 super_gradients/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Jul-19 09:35 super_gradients/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx      639 b- defN 23-Jul-19 09:35 super_gradients/qat_from_recipe.py
+-rwxr-xr-x  2.0 unx       28 b- defN 23-Jul-19 09:35 super_gradients/requirements.pro.txt
+-rwxr-xr-x  2.0 unx      729 b- defN 23-Jul-19 09:35 super_gradients/requirements.txt
+-rw-r--r--  2.0 unx      537 b- defN 23-Jul-19 09:35 super_gradients/resume_experiment.py
+-rw-r--r--  2.0 unx      693 b- defN 23-Jul-19 09:35 super_gradients/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Jul-19 09:35 super_gradients/train_from_recipe.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Jul-19 09:35 super_gradients/common/__init__.py
+-rw-r--r--  2.0 unx    15892 b- defN 23-Jul-19 09:35 super_gradients/common/object_names.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/abstractions/__init__.py
+-rw-r--r--  2.0 unx      879 b- defN 23-Jul-19 09:35 super_gradients/common/abstractions/abstract_logger.py
+-rw-r--r--  2.0 unx     3147 b- defN 23-Jul-19 09:35 super_gradients/common/abstractions/mute_processes.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/auto_logging/__init__.py
+-rw-r--r--  2.0 unx     4846 b- defN 23-Jul-19 09:35 super_gradients/common/auto_logging/auto_logger.py
+-rw-r--r--  2.0 unx     6625 b- defN 23-Jul-19 09:35 super_gradients/common/auto_logging/console_logging.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-19 09:35 super_gradients/common/aws_connection/__init__.py
+-rw-r--r--  2.0 unx     4182 b- defN 23-Jul-19 09:35 super_gradients/common/aws_connection/aws_connector.py
+-rw-r--r--  2.0 unx     7198 b- defN 23-Jul-19 09:35 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/crash_handler.py
+-rw-r--r--  2.0 unx    11775 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/crash_tips.py
+-rw-r--r--  2.0 unx      886 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/crash_tips_setup.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/exception.py
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/exception_monitoring_setup.py
+-rw-r--r--  2.0 unx      789 b- defN 23-Jul-19 09:35 super_gradients/common/crash_handler/utils.py
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-19 09:35 super_gradients/common/data_connection/__init__.py
+-rw-r--r--  2.0 unx    17959 b- defN 23-Jul-19 09:35 super_gradients/common/data_connection/s3_connector.py
+-rw-r--r--  2.0 unx      325 b- defN 23-Jul-19 09:35 super_gradients/common/data_interface/__init__.py
+-rw-r--r--  2.0 unx     9699 b- defN 23-Jul-19 09:35 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-Jul-19 09:35 super_gradients/common/data_interface/dataset_data_interface.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/__init__.py
+-rw-r--r--  2.0 unx      597 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/__init__.py
+-rw-r--r--  2.0 unx      309 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/deep_learning_task.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/downsample_mode.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/evaluation_type.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/multi_gpu_mode.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/strict_load.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Jul-19 09:35 super_gradients/common/data_types/enum/upsample_mode.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Jul-19 09:35 super_gradients/common/decorators/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-Jul-19 09:35 super_gradients/common/decorators/code_save_decorator.py
+-rw-r--r--  2.0 unx     3663 b- defN 23-Jul-19 09:35 super_gradients/common/decorators/deci_logger.py
+-rw-r--r--  2.0 unx     2921 b- defN 23-Jul-19 09:35 super_gradients/common/decorators/explicit_params_validator.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-Jul-19 09:35 super_gradients/common/decorators/factory_decorator.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jul-19 09:35 super_gradients/common/decorators/singleton.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Jul-19 09:35 super_gradients/common/environment/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Jul-19 09:35 super_gradients/common/environment/argparse_utils.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-Jul-19 09:35 super_gradients/common/environment/cfg_utils.py
+-rw-r--r--  2.0 unx     4398 b- defN 23-Jul-19 09:35 super_gradients/common/environment/checkpoints_dir_utils.py
+-rw-r--r--  2.0 unx     2682 b- defN 23-Jul-19 09:35 super_gradients/common/environment/ddp_utils.py
+-rw-r--r--  2.0 unx      752 b- defN 23-Jul-19 09:35 super_gradients/common/environment/device_utils.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Jul-19 09:35 super_gradients/common/environment/env_variables.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-Jul-19 09:35 super_gradients/common/environment/omegaconf_utils.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Jul-19 09:35 super_gradients/common/environment/path_utils.py
+-rw-r--r--  2.0 unx      112 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/__init__.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/cpu.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/data_models.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/disk.py
+-rw-r--r--  2.0 unx     5427 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/monitoring.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/network.py
+-rw-r--r--  2.0 unx      629 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/utils.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/virtual_memory.py
+-rw-r--r--  2.0 unx      681 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/gpu/__init__.py
+-rw-r--r--  2.0 unx     2270 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/gpu/gpu.py
+-rw-r--r--  2.0 unx   121647 b- defN 23-Jul-19 09:35 super_gradients/common/environment/monitoring/gpu/pynvml.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/exceptions/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-Jul-19 09:35 super_gradients/common/exceptions/dataset_exceptions.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jul-19 09:35 super_gradients/common/exceptions/factory_exceptions.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-Jul-19 09:35 super_gradients/common/exceptions/kd_trainer_exceptions.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Jul-19 09:35 super_gradients/common/exceptions/loss_exceptions.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jul-19 09:35 super_gradients/common/exceptions/sg_trainer_exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/factories/__init__.py
+-rw-r--r--  2.0 unx     1715 b- defN 23-Jul-19 09:35 super_gradients/common/factories/activations_type_factory.py
+-rw-r--r--  2.0 unx     2881 b- defN 23-Jul-19 09:35 super_gradients/common/factories/base_factory.py
+-rw-r--r--  2.0 unx      258 b- defN 23-Jul-19 09:35 super_gradients/common/factories/bbox_format_factory.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-19 09:35 super_gradients/common/factories/callbacks_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-19 09:35 super_gradients/common/factories/collate_functions_factory.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-19 09:35 super_gradients/common/factories/context_modules_factory.py
+-rw-r--r--  2.0 unx      321 b- defN 23-Jul-19 09:35 super_gradients/common/factories/data_formats_factory.py
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-19 09:35 super_gradients/common/factories/datasets_factory.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-Jul-19 09:35 super_gradients/common/factories/detection_modules_factory.py
+-rw-r--r--  2.0 unx      572 b- defN 23-Jul-19 09:35 super_gradients/common/factories/list_factory.py
+-rw-r--r--  2.0 unx      223 b- defN 23-Jul-19 09:35 super_gradients/common/factories/losses_factory.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jul-19 09:35 super_gradients/common/factories/metrics_factory.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Jul-19 09:35 super_gradients/common/factories/optimizers_type_factory.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Jul-19 09:35 super_gradients/common/factories/pre_launch_callbacks_factory.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Jul-19 09:35 super_gradients/common/factories/processing_factory.py
+-rw-r--r--  2.0 unx      229 b- defN 23-Jul-19 09:35 super_gradients/common/factories/samplers_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-19 09:35 super_gradients/common/factories/target_generator_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/factories/torch_schedulers_factory.py
+-rw-r--r--  2.0 unx     1873 b- defN 23-Jul-19 09:35 super_gradients/common/factories/transforms_factory.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-Jul-19 09:35 super_gradients/common/factories/type_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/plugins/__init__.py
+-rw-r--r--  2.0 unx    12245 b- defN 23-Jul-19 09:35 super_gradients/common/plugins/deci_client.py
+-rw-r--r--  2.0 unx      143 b- defN 23-Jul-19 09:35 super_gradients/common/plugins/wandb/__init__.py
+-rw-r--r--  2.0 unx     2317 b- defN 23-Jul-19 09:35 super_gradients/common/plugins/wandb/log_predictions.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Jul-19 09:35 super_gradients/common/registry/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Jul-19 09:35 super_gradients/common/registry/albumentation.py
+-rw-r--r--  2.0 unx     6634 b- defN 23-Jul-19 09:35 super_gradients/common/registry/registry.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/common/registry/registry_utils.py
+-rw-r--r--  2.0 unx      662 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/__init__.py
+-rw-r--r--  2.0 unx     7544 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/abstract_sg_logger.py
+-rw-r--r--  2.0 unx    15274 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/base_sg_logger.py
+-rw-r--r--  2.0 unx    10234 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/clearml_sg_logger.py
+-rw-r--r--  2.0 unx    10277 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/dagshub_sg_logger.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/time_units.py
+-rw-r--r--  2.0 unx    15242 b- defN 23-Jul-19 09:35 super_gradients/common/sg_loggers/wandb_sg_logger.py
+-rw-r--r--  2.0 unx    85509 b- defN 23-Jul-19 09:35 super_gradients/examples/SG_Walkthrough.ipynb
+-rw-r--r--  2.0 unx    69618 b- defN 23-Jul-19 09:35 super_gradients/examples/SG_quickstart_classification.ipynb
+-rw-r--r--  2.0 unx    54966 b- defN 23-Jul-19 09:35 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
+-rw-r--r--  2.0 unx    65090 b- defN 23-Jul-19 09:35 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/cifar10_training_torch_objects/__init__.py
+-rw-r--r--  2.0 unx     2526 b- defN 23-Jul-19 09:35 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/convert_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      870 b- defN 23-Jul-19 09:35 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/ddrnet_imagenet/__init__.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jul-19 09:35 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/deci_lab_export_example/__init__.py
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-19 09:35 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/early_stop/__init__.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-Jul-19 09:35 super_gradients/examples/early_stop/early_stop_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/evaluate_checkpoint_example/__init__.py
+-rw-r--r--  2.0 unx      289 b- defN 23-Jul-19 09:35 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/evaluate_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-19 09:35 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/loggers_examples/__init__.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-Jul-19 09:35 super_gradients/examples/loggers_examples/clearml_logger_example.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jul-19 09:35 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/qat_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      277 b- defN 23-Jul-19 09:35 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/non_default_calibrators_example.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/ptq_e2e_example.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
+-rw-r--r--  2.0 unx     4732 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/resnet_qat_example.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/skipping_quantization_example.py
+-rw-r--r--  2.0 unx      832 b- defN 23-Jul-19 09:35 super_gradients/examples/quantization/vanilla_quantize_all_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/regseg_transfer_learning_example/__init__.py
+-rw-r--r--  2.0 unx     2379 b- defN 23-Jul-19 09:35 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/resume_experiment_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-Jul-19 09:35 super_gradients/examples/resume_experiment_example/resume_experiment.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_kd_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
+-rw-r--r--  2.0 unx     1643 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_with_user_objects/train.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jul-19 09:35 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-19 09:35 super_gradients/module_interfaces/__init__.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Jul-19 09:35 super_gradients/module_interfaces/module_interfaces.py
+-rw-r--r--  2.0 unx     3366 b- defN 23-Jul-19 09:35 super_gradients/modules/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/modules/all_detection_modules.py
+-rw-r--r--  2.0 unx      617 b- defN 23-Jul-19 09:35 super_gradients/modules/anti_alias.py
+-rw-r--r--  2.0 unx      776 b- defN 23-Jul-19 09:35 super_gradients/modules/base_modules.py
+-rw-r--r--  2.0 unx     3054 b- defN 23-Jul-19 09:35 super_gradients/modules/conv_bn_act_block.py
+-rw-r--r--  2.0 unx     1976 b- defN 23-Jul-19 09:35 super_gradients/modules/conv_bn_relu_block.py
+-rw-r--r--  2.0 unx    14805 b- defN 23-Jul-19 09:35 super_gradients/modules/detection_modules.py
+-rw-r--r--  2.0 unx     2143 b- defN 23-Jul-19 09:35 super_gradients/modules/head_replacement_utils.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-Jul-19 09:35 super_gradients/modules/multi_output_modules.py
+-rw-r--r--  2.0 unx      860 b- defN 23-Jul-19 09:35 super_gradients/modules/pixel_shuffle.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-Jul-19 09:35 super_gradients/modules/pose_estimation_modules.py
+-rw-r--r--  2.0 unx    12250 b- defN 23-Jul-19 09:35 super_gradients/modules/qarepvgg_block.py
+-rw-r--r--  2.0 unx     8699 b- defN 23-Jul-19 09:35 super_gradients/modules/repvgg_block.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-Jul-19 09:35 super_gradients/modules/sampling.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-Jul-19 09:35 super_gradients/modules/se_blocks.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-Jul-19 09:35 super_gradients/modules/skip_connections.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-Jul-19 09:35 super_gradients/modules/utils.py
+-rw-r--r--  2.0 unx      716 b- defN 23-Jul-19 09:35 super_gradients/modules/quantization/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-Jul-19 09:35 super_gradients/modules/quantization/quantized_skip_connections.py
+-rw-r--r--  2.0 unx     4604 b- defN 23-Jul-19 09:35 super_gradients/modules/quantization/quantized_stdc_blocks.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-Jul-19 09:35 super_gradients/modules/quantization/resnet_bottleneck.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/recipes/__init__.py
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jul-19 09:35 super_gradients/recipes/cifar10_resnet.yaml
+-rw-r--r--  2.0 unx     2727 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_al_ddrnet.yaml
+-rw-r--r--  2.0 unx     3502 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_ddrnet.yaml
+-rw-r--r--  2.0 unx     3754 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_kd_base.yaml
+-rw-r--r--  2.0 unx     3354 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_pplite_seg50.yaml
+-rw-r--r--  2.0 unx     3253 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_pplite_seg75.yaml
+-rw-r--r--  2.0 unx     2498 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_regseg48.yaml
+-rw-r--r--  2.0 unx     4020 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_segformer.yaml
+-rw-r--r--  2.0 unx      618 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_stdc_base.yaml
+-rw-r--r--  2.0 unx     2862 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_stdc_seg50.yaml
+-rw-r--r--  2.0 unx     3055 b- defN 23-Jul-19 09:35 super_gradients/recipes/cityscapes_stdc_seg75.yaml
+-rw-r--r--  2.0 unx     1620 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_pose_dekr_rescoring.yaml
+-rw-r--r--  2.0 unx     2992 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_ppyoloe_l.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_ppyoloe_m.yaml
+-rw-r--r--  2.0 unx     1882 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_ppyoloe_s.yaml
+-rw-r--r--  2.0 unx     1975 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_ppyoloe_x.yaml
+-rw-r--r--  2.0 unx     1889 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx     2583 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco2017_yolox.yaml
+-rw-r--r--  2.0 unx     1376 b- defN 23-Jul-19 09:35 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
+-rw-r--r--  2.0 unx     1145 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_efficientnet.yaml
+-rw-r--r--  2.0 unx     1129 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_mobilenetv2.yaml
+-rw-r--r--  2.0 unx      507 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
+-rw-r--r--  2.0 unx     1997 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_regnetY.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_repvgg.yaml
+-rw-r--r--  2.0 unx     1169 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_resnet50.yaml
+-rw-r--r--  2.0 unx     2722 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_resnet50_kd.yaml
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_vit_base.yaml
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jul-19 09:35 super_gradients/recipes/imagenet_vit_large.yaml
+-rw-r--r--  2.0 unx     2007 b- defN 23-Jul-19 09:35 super_gradients/recipes/roboflow_ppyoloe.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-Jul-19 09:35 super_gradients/recipes/roboflow_yolo_nas_m.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-Jul-19 09:35 super_gradients/recipes/roboflow_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-19 09:35 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
+-rw-r--r--  2.0 unx     1917 b- defN 23-Jul-19 09:35 super_gradients/recipes/roboflow_yolox.yaml
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jul-19 09:35 super_gradients/recipes/script_generate_rescoring_data_dekr_coco2017.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-Jul-19 09:35 super_gradients/recipes/supervisely_unet.yaml
+-rw-r--r--  2.0 unx     1672 b- defN 23-Jul-19 09:35 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
+-rw-r--r--  2.0 unx     2133 b- defN 23-Jul-19 09:35 super_gradients/recipes/user_recipe_mnist_example.yaml
+-rw-r--r--  2.0 unx     2000 b- defN 23-Jul-19 09:35 super_gradients/recipes/variable_setup.yaml
+-rw-r--r--  2.0 unx     2222 b- defN 23-Jul-19 09:35 super_gradients/recipes/anchors/ssd_anchors.yaml
+-rw-r--r--  2.0 unx      563 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
+-rw-r--r--  2.0 unx      104 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
+-rw-r--r--  2.0 unx      194 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
+-rw-r--r--  2.0 unx      409 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
+-rw-r--r--  2.0 unx      356 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
+-rw-r--r--  2.0 unx      323 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml
+-rw-r--r--  2.0 unx     1113 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
+-rw-r--r--  2.0 unx      985 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
+-rw-r--r--  2.0 unx      196 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
+-rw-r--r--  2.0 unx      352 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
+-rw-r--r--  2.0 unx       98 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
+-rw-r--r--  2.0 unx       89 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
+-rw-r--r--  2.0 unx       88 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
+-rw-r--r--  2.0 unx       32 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
+-rw-r--r--  2.0 unx      655 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
+-rw-r--r--  2.0 unx      605 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
+-rw-r--r--  2.0 unx     1369 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/unet_arch_params.yaml
+-rw-r--r--  2.0 unx     3031 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
+-rw-r--r--  2.0 unx     2393 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolo_arch_params.yaml
+-rw-r--r--  2.0 unx     2353 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
+-rw-r--r--  2.0 unx     2362 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
+-rw-r--r--  2.0 unx     2357 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
+-rw-r--r--  2.0 unx      235 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
+-rw-r--r--  2.0 unx      229 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-19 09:35 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-19 09:35 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-19 09:35 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/recipes/conversion_params/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Jul-19 09:35 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
+-rw-r--r--  2.0 unx     2040 b- defN 23-Jul-19 09:35 super_gradients/recipes/conversion_params/default_conversion_params.yaml
+-rw-r--r--  2.0 unx      869 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_al_dataset_params.yaml
+-rw-r--r--  2.0 unx      615 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
+-rw-r--r--  2.0 unx      525 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      706 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx      644 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
+-rw-r--r--  2.0 unx      721 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
+-rw-r--r--  2.0 unx      709 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
+-rw-r--r--  2.0 unx      708 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx     3899 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     4152 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
+-rw-r--r--  2.0 unx     3517 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
+-rw-r--r--  2.0 unx     5521 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     3610 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
+-rw-r--r--  2.0 unx     4073 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
+-rw-r--r--  2.0 unx      405 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
+-rw-r--r--  2.0 unx      841 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx      931 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx      732 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
+-rw-r--r--  2.0 unx      734 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
+-rw-r--r--  2.0 unx      845 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     1762 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     1523 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     1414 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     4016 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx      961 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
+-rw-r--r--  2.0 unx      559 b- defN 23-Jul-19 09:35 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx     1155 b- defN 23-Jul-19 09:35 super_gradients/recipes/quantization_params/default_quantization_params.yaml
+-rw-r--r--  2.0 unx      591 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
+-rw-r--r--  2.0 unx      700 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
+-rw-r--r--  2.0 unx     2063 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
+-rw-r--r--  2.0 unx      771 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco2017_rescoring_train_params.yaml
+-rw-r--r--  2.0 unx      723 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
+-rw-r--r--  2.0 unx     1121 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
+-rw-r--r--  2.0 unx      957 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
+-rw-r--r--  2.0 unx      461 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
+-rw-r--r--  2.0 unx     7133 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/default_train_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
+-rw-r--r--  2.0 unx      742 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
+-rw-r--r--  2.0 unx      795 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
+-rw-r--r--  2.0 unx      476 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
+-rw-r--r--  2.0 unx      484 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
+-rw-r--r--  2.0 unx      522 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
+-rw-r--r--  2.0 unx      602 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-19 09:35 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-19 09:35 super_gradients/sanity_check/__init__.py
+-rw-r--r--  2.0 unx     5267 b- defN 23-Jul-19 09:35 super_gradients/sanity_check/env_sanity_check.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/scripts/__init__.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-Jul-19 09:35 super_gradients/scripts/find_detection_score_threshold.py
+-rw-r--r--  2.0 unx      775 b- defN 23-Jul-19 09:35 super_gradients/training/__init__.py
+-rw-r--r--  2.0 unx     5513 b- defN 23-Jul-19 09:35 super_gradients/training/params.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Jul-19 09:35 super_gradients/training/pretrained_models.py
+-rw-r--r--  2.0 unx     3344 b- defN 23-Jul-19 09:35 super_gradients/training/dataloaders/__init__.py
+-rw-r--r--  2.0 unx    36154 b- defN 23-Jul-19 09:35 super_gradients/training/dataloaders/dataloaders.py
+-rw-r--r--  2.0 unx     1867 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/__init__.py
+-rw-r--r--  2.0 unx    14162 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/auto_augment.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_augmentation.py
+-rw-r--r--  2.0 unx    32184 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/datasets_conf.py
+-rw-r--r--  2.0 unx    29577 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/datasets_utils.py
+-rw-r--r--  2.0 unx    14661 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/mixup.py
+-rw-r--r--  2.0 unx    11723 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/sg_dataset.py
+-rw-r--r--  2.0 unx      252 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/classification_datasets/__init__.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/classification_datasets/cifar.py
+-rw-r--r--  2.0 unx     1706 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
+-rw-r--r--  2.0 unx      862 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/__init__.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/default_formats.py
+-rw-r--r--  2.0 unx     3071 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/format_converter.py
+-rw-r--r--  2.0 unx     7928 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/formats.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
+-rw-r--r--  2.0 unx     2674 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
+-rw-r--r--  2.0 unx     5131 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
+-rw-r--r--  2.0 unx     2089 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
+-rw-r--r--  2.0 unx     2948 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
+-rw-r--r--  2.0 unx      575 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
+-rw-r--r--  2.0 unx      683 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/__init__.py
+-rw-r--r--  2.0 unx     2505 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/coco_detection.py
+-rw-r--r--  2.0 unx     9258 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
+-rw-r--r--  2.0 unx    26564 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/detection_dataset.py
+-rw-r--r--  2.0 unx    11353 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
+-rw-r--r--  2.0 unx    11117 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
+-rw-r--r--  2.0 unx    18882 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
+-rw-r--r--  2.0 unx     3503 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
+-rw-r--r--  2.0 unx      502 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
+-rw-r--r--  2.0 unx     6314 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
+-rw-r--r--  2.0 unx    10545 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
+-rw-r--r--  2.0 unx     5929 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
+-rw-r--r--  2.0 unx     3736 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/pose_estimation_datasets/rescoring_dataset.py
+-rw-r--r--  2.0 unx    10281 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/samplers/__init__.py
+-rw-r--r--  2.0 unx      738 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/samplers/infinite_sampler.py
+-rw-r--r--  2.0 unx     4809 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/__init__.py
+-rw-r--r--  2.0 unx     8304 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
+-rw-r--r--  2.0 unx     7757 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
+-rw-r--r--  2.0 unx    11146 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
+-rw-r--r--  2.0 unx     8572 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-Jul-19 09:35 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-19 09:35 super_gradients/training/kd_trainer/__init__.py
+-rw-r--r--  2.0 unx    16599 b- defN 23-Jul-19 09:35 super_gradients/training/kd_trainer/kd_trainer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/legacy/__init__.py
+-rw-r--r--  2.0 unx     4198 b- defN 23-Jul-19 09:35 super_gradients/training/legacy/utils.py
+-rw-r--r--  2.0 unx     1570 b- defN 23-Jul-19 09:35 super_gradients/training/losses/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/losses/all_losses.py
+-rw-r--r--  2.0 unx     1219 b- defN 23-Jul-19 09:35 super_gradients/training/losses/bce_dice_loss.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Jul-19 09:35 super_gradients/training/losses/bce_loss.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-Jul-19 09:35 super_gradients/training/losses/cwd_loss.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-Jul-19 09:35 super_gradients/training/losses/ddrnet_loss.py
+-rw-r--r--  2.0 unx     4038 b- defN 23-Jul-19 09:35 super_gradients/training/losses/dekr_loss.py
+-rw-r--r--  2.0 unx     5618 b- defN 23-Jul-19 09:35 super_gradients/training/losses/dice_ce_edge_loss.py
+-rw-r--r--  2.0 unx     5208 b- defN 23-Jul-19 09:35 super_gradients/training/losses/dice_loss.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-Jul-19 09:35 super_gradients/training/losses/focal_loss.py
+-rw-r--r--  2.0 unx     5051 b- defN 23-Jul-19 09:35 super_gradients/training/losses/iou_loss.py
+-rw-r--r--  2.0 unx     2176 b- defN 23-Jul-19 09:35 super_gradients/training/losses/kd_losses.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-Jul-19 09:35 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
+-rw-r--r--  2.0 unx      550 b- defN 23-Jul-19 09:35 super_gradients/training/losses/loss_utils.py
+-rw-r--r--  2.0 unx     4004 b- defN 23-Jul-19 09:35 super_gradients/training/losses/mask_loss.py
+-rw-r--r--  2.0 unx     4127 b- defN 23-Jul-19 09:35 super_gradients/training/losses/ohem_ce_loss.py
+-rw-r--r--  2.0 unx    41319 b- defN 23-Jul-19 09:35 super_gradients/training/losses/ppyolo_loss.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jul-19 09:35 super_gradients/training/losses/r_squared_loss.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jul-19 09:35 super_gradients/training/losses/rescoring_loss.py
+-rw-r--r--  2.0 unx     3453 b- defN 23-Jul-19 09:35 super_gradients/training/losses/seg_kd_loss.py
+-rw-r--r--  2.0 unx     1650 b- defN 23-Jul-19 09:35 super_gradients/training/losses/shelfnet_ohem_loss.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jul-19 09:35 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
+-rw-r--r--  2.0 unx     8794 b- defN 23-Jul-19 09:35 super_gradients/training/losses/ssd_loss.py
+-rw-r--r--  2.0 unx     9721 b- defN 23-Jul-19 09:35 super_gradients/training/losses/stdc_loss.py
+-rw-r--r--  2.0 unx     5771 b- defN 23-Jul-19 09:35 super_gradients/training/losses/structure_loss.py
+-rw-r--r--  2.0 unx    50149 b- defN 23-Jul-19 09:35 super_gradients/training/losses/yolox_loss.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/all_metrics.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/classification_metrics.py
+-rw-r--r--  2.0 unx    16709 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/detection_metrics.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/metric_utils.py
+-rw-r--r--  2.0 unx    15813 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/pose_estimation_metrics.py
+-rw-r--r--  2.0 unx    11536 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/pose_estimation_utils.py
+-rw-r--r--  2.0 unx    19665 b- defN 23-Jul-19 09:35 super_gradients/training/metrics/segmentation_metrics.py
+-rw-r--r--  2.0 unx    11309 b- defN 23-Jul-19 09:35 super_gradients/training/models/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Jul-19 09:35 super_gradients/training/models/arch_params_factory.py
+-rw-r--r--  2.0 unx    12587 b- defN 23-Jul-19 09:35 super_gradients/training/models/conversion.py
+-rw-r--r--  2.0 unx    12758 b- defN 23-Jul-19 09:35 super_gradients/training/models/model_factory.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-19 09:35 super_gradients/training/models/predictions.py
+-rw-r--r--  2.0 unx     2998 b- defN 23-Jul-19 09:35 super_gradients/training/models/sg_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/__init__.py
+-rw-r--r--  2.0 unx     3080 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/base_classifer.py
+-rw-r--r--  2.0 unx    20025 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/beit.py
+-rw-r--r--  2.0 unx     7472 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/densenet.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/dpn.py
+-rw-r--r--  2.0 unx    36745 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/efficientnet.py
+-rw-r--r--  2.0 unx     8862 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/googlenet.py
+-rw-r--r--  2.0 unx      798 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/lenet.py
+-rw-r--r--  2.0 unx     2407 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/mobilenet.py
+-rw-r--r--  2.0 unx     9472 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/mobilenetv2.py
+-rw-r--r--  2.0 unx     8696 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/mobilenetv3.py
+-rw-r--r--  2.0 unx     4339 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/pnasnet.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/preact_resnet.py
+-rw-r--r--  2.0 unx    13603 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/regnet.py
+-rw-r--r--  2.0 unx     7924 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/repvgg.py
+-rw-r--r--  2.0 unx    15077 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/resnet.py
+-rw-r--r--  2.0 unx     6294 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/resnext.py
+-rw-r--r--  2.0 unx     4134 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/senet.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/shufflenet.py
+-rw-r--r--  2.0 unx     9768 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/shufflenetv2.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/vgg.py
+-rw-r--r--  2.0 unx     9210 b- defN 23-Jul-19 09:35 super_gradients/training/models/classification_models/vit.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/__init__.py
+-rw-r--r--  2.0 unx     9130 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/csp_darknet53.py
+-rw-r--r--  2.0 unx     9821 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/csp_resnet.py
+-rw-r--r--  2.0 unx    10173 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/customizable_detector.py
+-rw-r--r--  2.0 unx     4746 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/darknet53.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/ssd.py
+-rw-r--r--  2.0 unx    32774 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolo_base.py
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolox.py
+-rw-r--r--  2.0 unx      251 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
+-rw-r--r--  2.0 unx     7000 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
+-rw-r--r--  2.0 unx     3889 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
+-rw-r--r--  2.0 unx     9210 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
+-rw-r--r--  2.0 unx    12404 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
+-rw-r--r--  2.0 unx      756 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolo_nas/__init__.py
+-rw-r--r--  2.0 unx    12692 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolo_nas/panneck.py
+-rw-r--r--  2.0 unx     4166 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
+-rw-r--r--  2.0 unx    15510 b- defN 23-Jul-19 09:35 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/models/kd_modules/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Jul-19 09:35 super_gradients/training/models/kd_modules/kd_module.py
+-rw-r--r--  2.0 unx      179 b- defN 23-Jul-19 09:35 super_gradients/training/models/pose_estimation_models/__init__.py
+-rw-r--r--  2.0 unx    29151 b- defN 23-Jul-19 09:35 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
+-rw-r--r--  2.0 unx     4286 b- defN 23-Jul-19 09:35 super_gradients/training/models/pose_estimation_models/rescoring_net.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/__init__.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/common.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/context_modules.py
+-rw-r--r--  2.0 unx    28514 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/ddrnet.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
+-rw-r--r--  2.0 unx    21760 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/laddernet.py
+-rw-r--r--  2.0 unx    15648 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/ppliteseg.py
+-rw-r--r--  2.0 unx    14424 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/regseg.py
+-rw-r--r--  2.0 unx    20334 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/segformer.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/segmentation_module.py
+-rw-r--r--  2.0 unx    24851 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/shelfnet.py
+-rw-r--r--  2.0 unx    29091 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/stdc.py
+-rw-r--r--  2.0 unx      260 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/unet/__init__.py
+-rw-r--r--  2.0 unx    12324 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/unet/unet.py
+-rw-r--r--  2.0 unx    10718 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
+-rw-r--r--  2.0 unx    13292 b- defN 23-Jul-19 09:35 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Jul-19 09:35 super_gradients/training/models/user_models/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/pipelines/__init__.py
+-rw-r--r--  2.0 unx    23544 b- defN 23-Jul-19 09:35 super_gradients/training/pipelines/pipelines.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jul-19 09:35 super_gradients/training/pre_launch_callbacks/__init__.py
+-rw-r--r--  2.0 unx    21083 b- defN 23-Jul-19 09:35 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-19 09:35 super_gradients/training/processing/__init__.py
+-rw-r--r--  2.0 unx    20260 b- defN 23-Jul-19 09:35 super_gradients/training/processing/processing.py
+-rw-r--r--  2.0 unx       98 b- defN 23-Jul-19 09:35 super_gradients/training/qat_trainer/__init__.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Jul-19 09:35 super_gradients/training/qat_trainer/qat_trainer.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Jul-19 09:35 super_gradients/training/sg_trainer/__init__.py
+-rw-r--r--  2.0 unx   123049 b- defN 23-Jul-19 09:35 super_gradients/training/sg_trainer/sg_trainer.py
+-rw-r--r--  2.0 unx     1685 b- defN 23-Jul-19 09:35 super_gradients/training/training_hyperparams/__init__.py
+-rw-r--r--  2.0 unx     3774 b- defN 23-Jul-19 09:35 super_gradients/training/training_hyperparams/training_hyperparams.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jul-19 09:35 super_gradients/training/transforms/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/transforms/all_transforms.py
+-rw-r--r--  2.0 unx    20123 b- defN 23-Jul-19 09:35 super_gradients/training/transforms/keypoint_transforms.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jul-19 09:35 super_gradients/training/transforms/pipeline_adaptors.py
+-rw-r--r--  2.0 unx    57393 b- defN 23-Jul-19 09:35 super_gradients/training/transforms/transforms.py
+-rw-r--r--  2.0 unx     7307 b- defN 23-Jul-19 09:35 super_gradients/training/transforms/utils.py
+-rw-r--r--  2.0 unx     1141 b- defN 23-Jul-19 09:35 super_gradients/training/utils/__init__.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-Jul-19 09:35 super_gradients/training/utils/activations_utils.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Jul-19 09:35 super_gradients/training/utils/bbox_utils.py
+-rw-r--r--  2.0 unx    16205 b- defN 23-Jul-19 09:35 super_gradients/training/utils/checkpoint_utils.py
+-rw-r--r--  2.0 unx     9794 b- defN 23-Jul-19 09:35 super_gradients/training/utils/config_utils.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jul-19 09:35 super_gradients/training/utils/deprecated_utils.py
+-rw-r--r--  2.0 unx    60150 b- defN 23-Jul-19 09:35 super_gradients/training/utils/detection_utils.py
+-rw-r--r--  2.0 unx    16195 b- defN 23-Jul-19 09:35 super_gradients/training/utils/distributed_training_utils.py
+-rw-r--r--  2.0 unx     6352 b- defN 23-Jul-19 09:35 super_gradients/training/utils/early_stopping.py
+-rw-r--r--  2.0 unx     9304 b- defN 23-Jul-19 09:35 super_gradients/training/utils/ema.py
+-rw-r--r--  2.0 unx     2610 b- defN 23-Jul-19 09:35 super_gradients/training/utils/ema_decay_schedules.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jul-19 09:35 super_gradients/training/utils/export_utils.py
+-rw-r--r--  2.0 unx     7508 b- defN 23-Jul-19 09:35 super_gradients/training/utils/get_model_stats.py
+-rw-r--r--  2.0 unx      771 b- defN 23-Jul-19 09:35 super_gradients/training/utils/kd_trainer_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/utils/load_image.py
+-rw-r--r--  2.0 unx     6120 b- defN 23-Jul-19 09:35 super_gradients/training/utils/optimizer_utils.py
+-rw-r--r--  2.0 unx     1833 b- defN 23-Jul-19 09:35 super_gradients/training/utils/regularization_utils.py
+-rw-r--r--  2.0 unx    10388 b- defN 23-Jul-19 09:35 super_gradients/training/utils/segmentation_utils.py
+-rw-r--r--  2.0 unx    19713 b- defN 23-Jul-19 09:35 super_gradients/training/utils/sg_trainer_utils.py
+-rw-r--r--  2.0 unx     6423 b- defN 23-Jul-19 09:35 super_gradients/training/utils/ssd_utils.py
+-rw-r--r--  2.0 unx    21363 b- defN 23-Jul-19 09:35 super_gradients/training/utils/utils.py
+-rw-r--r--  2.0 unx      303 b- defN 23-Jul-19 09:35 super_gradients/training/utils/version_utils.py
+-rw-r--r--  2.0 unx     5628 b- defN 23-Jul-19 09:35 super_gradients/training/utils/weight_averaging_utils.py
+-rw-r--r--  2.0 unx     2024 b- defN 23-Jul-19 09:35 super_gradients/training/utils/callbacks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/utils/callbacks/all_callbacks.py
+-rw-r--r--  2.0 unx    20007 b- defN 23-Jul-19 09:35 super_gradients/training/utils/callbacks/base_callbacks.py
+-rw-r--r--  2.0 unx    42787 b- defN 23-Jul-19 09:35 super_gradients/training/utils/callbacks/callbacks.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-Jul-19 09:35 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/utils/media/__init__.py
+-rw-r--r--  2.0 unx     5894 b- defN 23-Jul-19 09:35 super_gradients/training/utils/media/image.py
+-rw-r--r--  2.0 unx     4046 b- defN 23-Jul-19 09:35 super_gradients/training/utils/media/stream.py
+-rw-r--r--  2.0 unx     6926 b- defN 23-Jul-19 09:35 super_gradients/training/utils/media/video.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Jul-19 09:35 super_gradients/training/utils/optimizers/__init__.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jul-19 09:35 super_gradients/training/utils/optimizers/all_optimizers.py
+-rw-r--r--  2.0 unx     9760 b- defN 23-Jul-19 09:35 super_gradients/training/utils/optimizers/lamb.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-Jul-19 09:35 super_gradients/training/utils/optimizers/lion.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-Jul-19 09:35 super_gradients/training/utils/optimizers/rmsprop_tf.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Jul-19 09:35 super_gradients/training/utils/pose_estimation/__init__.py
+-rw-r--r--  2.0 unx    13624 b- defN 23-Jul-19 09:35 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
+-rw-r--r--  2.0 unx     7140 b- defN 23-Jul-19 09:35 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
+-rw-r--r--  2.0 unx      920 b- defN 23-Jul-19 09:35 super_gradients/training/utils/pose_estimation/rescoring_callback.py
+-rw-r--r--  2.0 unx     1012 b- defN 23-Jul-19 09:35 super_gradients/training/utils/predict/__init__.py
+-rw-r--r--  2.0 unx    14550 b- defN 23-Jul-19 09:35 super_gradients/training/utils/predict/prediction_pose_estimation_results.py
+-rw-r--r--  2.0 unx    13944 b- defN 23-Jul-19 09:35 super_gradients/training/utils/predict/prediction_results.py
+-rw-r--r--  2.0 unx     5263 b- defN 23-Jul-19 09:35 super_gradients/training/utils/predict/predictions.py
+-rw-r--r--  2.0 unx      387 b- defN 23-Jul-19 09:35 super_gradients/training/utils/quantization/__init__.py
+-rw-r--r--  2.0 unx     6271 b- defN 23-Jul-19 09:35 super_gradients/training/utils/quantization/calibrator.py
+-rw-r--r--  2.0 unx     8417 b- defN 23-Jul-19 09:35 super_gradients/training/utils/quantization/core.py
+-rw-r--r--  2.0 unx     2504 b- defN 23-Jul-19 09:35 super_gradients/training/utils/quantization/export.py
+-rw-r--r--  2.0 unx    17062 b- defN 23-Jul-19 09:35 super_gradients/training/utils/quantization/selective_quantization_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 09:35 super_gradients/training/utils/visualization/__init__.py
+-rw-r--r--  2.0 unx     1647 b- defN 23-Jul-19 09:35 super_gradients/training/utils/visualization/classification.py
+-rw-r--r--  2.0 unx     1698 b- defN 23-Jul-19 09:35 super_gradients/training/utils/visualization/detection.py
+-rw-r--r--  2.0 unx     2684 b- defN 23-Jul-19 09:35 super_gradients/training/utils/visualization/pose_estimation.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jul-19 09:35 super_gradients/training/utils/visualization/utils.py
+-rw-r--r--  2.0 unx     2218 b- defN 23-Jul-19 09:35 super_gradients-3.1.3.dist-info/LICENSE.YOLONAS.md
+-rw-r--r--  2.0 unx    11341 b- defN 23-Jul-19 09:35 super_gradients-3.1.3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    35723 b- defN 23-Jul-19 09:35 super_gradients-3.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 09:35 super_gradients-3.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-19 09:35 super_gradients-3.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    66425 b- defN 23-Jul-19 09:35 super_gradients-3.1.3.dist-info/RECORD
+575 files, 3027988 bytes uncompressed, 906473 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -195,17 +195,29 @@
 
 Filename: super_gradients/common/environment/monitoring/gpu/pynvml.py
 Comment: 
 
 Filename: super_gradients/common/exceptions/__init__.py
 Comment: 
 
+Filename: super_gradients/common/exceptions/dataset_exceptions.py
+Comment: 
+
 Filename: super_gradients/common/exceptions/factory_exceptions.py
 Comment: 
 
+Filename: super_gradients/common/exceptions/kd_trainer_exceptions.py
+Comment: 
+
+Filename: super_gradients/common/exceptions/loss_exceptions.py
+Comment: 
+
+Filename: super_gradients/common/exceptions/sg_trainer_exceptions.py
+Comment: 
+
 Filename: super_gradients/common/factories/__init__.py
 Comment: 
 
 Filename: super_gradients/common/factories/activations_type_factory.py
 Comment: 
 
 Filename: super_gradients/common/factories/base_factory.py
@@ -252,14 +264,17 @@
 
 Filename: super_gradients/common/factories/samplers_factory.py
 Comment: 
 
 Filename: super_gradients/common/factories/target_generator_factory.py
 Comment: 
 
+Filename: super_gradients/common/factories/torch_schedulers_factory.py
+Comment: 
+
 Filename: super_gradients/common/factories/transforms_factory.py
 Comment: 
 
 Filename: super_gradients/common/factories/type_factory.py
 Comment: 
 
 Filename: super_gradients/common/plugins/__init__.py
@@ -300,14 +315,17 @@
 
 Filename: super_gradients/common/sg_loggers/dagshub_sg_logger.py
 Comment: 
 
 Filename: super_gradients/common/sg_loggers/deci_platform_sg_logger.py
 Comment: 
 
+Filename: super_gradients/common/sg_loggers/time_units.py
+Comment: 
+
 Filename: super_gradients/common/sg_loggers/wandb_sg_logger.py
 Comment: 
 
 Filename: super_gradients/examples/SG_Walkthrough.ipynb
 Comment: 
 
 Filename: super_gradients/examples/SG_quickstart_classification.ipynb
@@ -972,14 +990,20 @@
 
 Filename: super_gradients/sanity_check/__init__.py
 Comment: 
 
 Filename: super_gradients/sanity_check/env_sanity_check.py
 Comment: 
 
+Filename: super_gradients/scripts/__init__.py
+Comment: 
+
+Filename: super_gradients/scripts/find_detection_score_threshold.py
+Comment: 
+
 Filename: super_gradients/training/__init__.py
 Comment: 
 
 Filename: super_gradients/training/params.py
 Comment: 
 
 Filename: super_gradients/training/pretrained_models.py
@@ -1140,29 +1164,14 @@
 
 Filename: super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
 Comment: 
 
 Filename: super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
 Comment: 
 
-Filename: super_gradients/training/exceptions/__init__.py
-Comment: 
-
-Filename: super_gradients/training/exceptions/dataset_exceptions.py
-Comment: 
-
-Filename: super_gradients/training/exceptions/kd_trainer_exceptions.py
-Comment: 
-
-Filename: super_gradients/training/exceptions/loss_exceptions.py
-Comment: 
-
-Filename: super_gradients/training/exceptions/sg_trainer_exceptions.py
-Comment: 
-
 Filename: super_gradients/training/kd_trainer/__init__.py
 Comment: 
 
 Filename: super_gradients/training/kd_trainer/kd_trainer.py
 Comment: 
 
 Filename: super_gradients/training/legacy/__init__.py
@@ -1281,29 +1290,26 @@
 
 Filename: super_gradients/training/models/conversion.py
 Comment: 
 
 Filename: super_gradients/training/models/model_factory.py
 Comment: 
 
-Filename: super_gradients/training/models/prediction_results.py
-Comment: 
-
 Filename: super_gradients/training/models/predictions.py
 Comment: 
 
-Filename: super_gradients/training/models/results.py
-Comment: 
-
 Filename: super_gradients/training/models/sg_module.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/__init__.py
 Comment: 
 
+Filename: super_gradients/training/models/classification_models/base_classifer.py
+Comment: 
+
 Filename: super_gradients/training/models/classification_models/beit.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/densenet.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/dpn.py
@@ -1653,14 +1659,26 @@
 
 Filename: super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
 Comment: 
 
 Filename: super_gradients/training/utils/pose_estimation/rescoring_callback.py
 Comment: 
 
+Filename: super_gradients/training/utils/predict/__init__.py
+Comment: 
+
+Filename: super_gradients/training/utils/predict/prediction_pose_estimation_results.py
+Comment: 
+
+Filename: super_gradients/training/utils/predict/prediction_results.py
+Comment: 
+
+Filename: super_gradients/training/utils/predict/predictions.py
+Comment: 
+
 Filename: super_gradients/training/utils/quantization/__init__.py
 Comment: 
 
 Filename: super_gradients/training/utils/quantization/calibrator.py
 Comment: 
 
 Filename: super_gradients/training/utils/quantization/core.py
@@ -1671,32 +1689,38 @@
 
 Filename: super_gradients/training/utils/quantization/selective_quantization_utils.py
 Comment: 
 
 Filename: super_gradients/training/utils/visualization/__init__.py
 Comment: 
 
+Filename: super_gradients/training/utils/visualization/classification.py
+Comment: 
+
 Filename: super_gradients/training/utils/visualization/detection.py
 Comment: 
 
+Filename: super_gradients/training/utils/visualization/pose_estimation.py
+Comment: 
+
 Filename: super_gradients/training/utils/visualization/utils.py
 Comment: 
 
-Filename: super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md
+Filename: super_gradients-3.1.3.dist-info/LICENSE.YOLONAS.md
 Comment: 
 
-Filename: super_gradients-3.1.2.dist-info/LICENSE.md
+Filename: super_gradients-3.1.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: super_gradients-3.1.2.dist-info/METADATA
+Filename: super_gradients-3.1.3.dist-info/METADATA
 Comment: 
 
-Filename: super_gradients-3.1.2.dist-info/WHEEL
+Filename: super_gradients-3.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: super_gradients-3.1.2.dist-info/top_level.txt
+Filename: super_gradients-3.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: super_gradients-3.1.2.dist-info/RECORD
+Filename: super_gradients-3.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## super_gradients/__init__.py

```diff
@@ -19,10 +19,10 @@
     "is_distributed",
     "env_sanity_check",
     "setup_device",
     "QATRecipeModificationCallback",
     "AutoTrainBatchSizeSelectionCallback",
 ]
 
-__version__ = "3.1.2"
+__version__ = "3.1.3"
 
 env_sanity_check()
```

## super_gradients/common/object_names.py

```diff
@@ -53,14 +53,15 @@
     DetectionMosaic = "DetectionMosaic"
     DetectionRandomAffine = "DetectionRandomAffine"
     DetectionMixup = "DetectionMixup"
     DetectionHSV = "DetectionHSV"
     DetectionRGB2BGR = "DetectionRGB2BGR"
     DetectionRandomRotate90 = "DetectionRandomRotate90"
     DetectionHorizontalFlip = "DetectionHorizontalFlip"
+    DetectionVerticalFlip = "DetectionVerticalFlip"
     DetectionRescale = "DetectionRescale"
     DetectionPadToSize = "DetectionPadToSize"
     DetectionImagePermute = "DetectionImagePermute"
     DetectionPaddedRescale = "DetectionPaddedRescale"
     DetectionTargetsFormatTransform = "DetectionTargetsFormatTransform"
     DetectionNormalize = "DetectionNormalize"
     #
@@ -106,14 +107,15 @@
     RandomAdjustSharpness = "RandomAdjustSharpness"
     RandomAutocontrast = "RandomAutocontrast"
     RandomEqualize = "RandomEqualize"
 
     # Keypoints
     KeypointsRandomAffineTransform = "KeypointsRandomAffineTransform"
     KeypointsImageNormalize = "KeypointsImageNormalize"
+    KeypointsImageStandardize = "KeypointsImageStandardize"
     KeypointsImageToTensor = "KeypointsImageToTensor"
     KeypointTransform = "KeypointTransform"
     KeypointsPadIfNeeded = "KeypointsPadIfNeeded"
     KeypointsLongestMaxSize = "KeypointsLongestMaxSize"
     KeypointsRandomVerticalFlip = "KeypointsRandomVerticalFlip"
     KeypointsRandomHorizontalFlip = "KeypointsRandomHorizontalFlip"
 
@@ -141,14 +143,15 @@
     EARLY_STOP = "EarlyStop"
     DETECTION_MULTISCALE_PREPREDICTION = "DetectionMultiscalePrePredictionCallback"
     YOLOX_TRAINING_STAGE_SWITCH = "YoloXTrainingStageSwitchCallback"
     PPYOLOE_TRAINING_STAGE_SWITCH = "PPYoloETrainingStageSwitchCallback"
     DETECTION_VISUALIZATION_CALLBACK = "DetectionVisualizationCallback"
     DEKR_VISUALIZATION = "DEKRVisualizationCallback"
     ROBOFLOW_RESULT_CALLBACK = "RoboflowResultCallback"
+    TIMER = "TimerCallback"
 
 
 class LRSchedulers:
     """Static class to hold all the supported LR Scheduler names"""
 
     STEP = "step"
     POLY = "poly"
@@ -409,12 +412,16 @@
 
 
 class Processings:
     StandardizeImage = "StandardizeImage"
     DetectionCenterPadding = "DetectionCenterPadding"
     DetectionLongestMaxSizeRescale = "DetectionLongestMaxSizeRescale"
     DetectionBottomRightPadding = "DetectionBottomRightPadding"
-    ImagePermute = "ImagePermute"
     DetectionRescale = "DetectionRescale"
+    KeypointsLongestMaxSizeRescale = "KeypointsLongestMaxSizeRescale"
+    KeypointsBottomRightPadding = "KeypointsBottomRightPadding"
+    ImagePermute = "ImagePermute"
     ReverseImageChannels = "ReverseImageChannels"
     NormalizeImage = "NormalizeImage"
     ComposeProcessing = "ComposeProcessing"
+    CenterCrop = "CenterCrop"
+    Resize = "Resize"
```

## super_gradients/common/abstractions/mute_processes.py

```diff
@@ -23,15 +23,15 @@
     import warnings
 
     warnings.filterwarnings("ignore")
 
     # Ignore prints
     import sys
 
-    sys.stdout = open(os.devnull, "w")
+    sys.stdout = open(os.devnull, "w", encoding="utf-8")
 
     # Only show ERRORS
     process_loggers = [logging.getLogger(name) for name in logging.root.manager.loggerDict]
     for logger in process_loggers:
         logger.setLevel(logging.ERROR)
```

## super_gradients/common/environment/checkpoints_dir_utils.py

```diff
@@ -33,15 +33,15 @@
     """Get the checkpoints' directory that is at the root of the users project. Create it if it doesn't exist. Return None if root not found."""
     project_root_path = _get_project_root_path()
     if project_root_path is None:
         return None
 
     checkpoints_path = os.path.join(project_root_path, "checkpoints")
     if not os.path.exists(checkpoints_path):
-        os.makedirs(checkpoints_path)
+        os.makedirs(checkpoints_path, exist_ok=True)
         logger.info(f'A checkpoints directory was just created at "{checkpoints_path}". To work with another directory, please set "ckpt_root_dir"')
     return checkpoints_path
 
 
 def get_checkpoints_dir_path(experiment_name: str, ckpt_root_dir: str = None) -> str:
     """Get the directory that includes all the checkpoints (and logs) of an experiment.
```

## super_gradients/common/plugins/wandb/log_predictions.py

```diff
@@ -1,13 +1,13 @@
 try:
     import wandb
 except (ModuleNotFoundError, ImportError, NameError):
     pass  # no action or logging - this is normal in most cases
 
-from super_gradients.training.models.prediction_results import ImageDetectionPrediction, ImagesDetectionPrediction
+from super_gradients.training.utils.predict import ImageDetectionPrediction, ImagesDetectionPrediction
 
 
 def _visualize_image_detection_prediction_on_wandb(prediction: ImageDetectionPrediction, show_confidence: bool):
     boxes = []
     image = prediction.image.copy()
     height, width, _ = image.shape
     class_id_to_labels = {int(_id): str(_class_name) for _id, _class_name in enumerate(prediction.class_names)}
```

## super_gradients/common/registry/registry.py

```diff
@@ -140,11 +140,25 @@
 
 OPTIMIZERS = {
     Optimizers.SGD: optim.SGD,
     Optimizers.ADAM: optim.Adam,
     Optimizers.ADAMW: optim.AdamW,
     Optimizers.RMS_PROP: optim.RMSprop,
 }
+
+TORCH_LR_SCHEDULERS = {
+    "StepLR": torch.optim.lr_scheduler.StepLR,
+    "LambdaLR": torch.optim.lr_scheduler.LambdaLR,
+    "MultiStepLR": torch.optim.lr_scheduler.MultiStepLR,
+    "ConstantLR": torch.optim.lr_scheduler.ConstantLR,
+    "CosineAnnealingLR": torch.optim.lr_scheduler.CosineAnnealingLR,
+    "CosineAnnealingWarmRestarts": torch.optim.lr_scheduler.CosineAnnealingWarmRestarts,
+    "CyclicLR": torch.optim.lr_scheduler.CyclicLR,
+    "ExponentialLR": torch.optim.lr_scheduler.ExponentialLR,
+    "ReduceLROnPlateau": torch.optim.lr_scheduler.ReduceLROnPlateau,
+    "LinearLR": torch.optim.lr_scheduler.LinearLR,
+}
+
 register_optimizer = create_register_decorator(registry=OPTIMIZERS)
 
 PROCESSINGS = {}
 register_processing = create_register_decorator(registry=PROCESSINGS)
```

## super_gradients/common/sg_loggers/__init__.py

```diff
@@ -1,7 +1,8 @@
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.sg_loggers.clearml_sg_logger import ClearMLSGLogger
 from super_gradients.common.sg_loggers.deci_platform_sg_logger import DeciPlatformSGLogger
 from super_gradients.common.sg_loggers.wandb_sg_logger import WandBSGLogger
 from super_gradients.common.sg_loggers.dagshub_sg_logger import DagsHubSGLogger
+from super_gradients.common.sg_loggers.time_units import TimeUnit, EpochNumber, GlobalBatchStepNumber
 
-__all__ = ["BaseSGLogger", "ClearMLSGLogger", "DeciPlatformSGLogger", "WandBSGLogger", "DagsHubSGLogger"]
+__all__ = ["BaseSGLogger", "ClearMLSGLogger", "DeciPlatformSGLogger", "WandBSGLogger", "DagsHubSGLogger", "TimeUnit", "EpochNumber", "GlobalBatchStepNumber"]
```

## super_gradients/common/sg_loggers/abstract_sg_logger.py

```diff
@@ -1,14 +1,16 @@
 from abc import abstractmethod, ABC
 from typing import Union, Any
 
 import numpy as np
 from PIL import Image
 import torch
 
+from super_gradients.common.sg_loggers.time_units import TimeUnit
+
 
 class AbstractSGLogger(ABC):
     """
     A SGLogger handles all outputs of the training process.
     Every generated file, log, metrics value, image or other artifacts produced by the trainer will be processed and saved.
 
     Inheriting SGLogger can be used in order to integrate experiment management framework, special storage setting, a specific logging library etc.
@@ -36,15 +38,15 @@
 
         :param tag: Data identifier
         :param config: a dictionary of the experiment config
         """
         raise NotImplementedError
 
     @abstractmethod
-    def add_scalar(self, tag: str, scalar_value: float, global_step: int = None):
+    def add_scalar(self, tag: str, scalar_value: float, global_step: Union[int, TimeUnit] = None):
         """
         Add scalar data to SGLogger.
         Typically, this function will add scalar to tensorboard or other experiment management framework.
 
         :param tag: Data identifier
         :param scalar_value: Value to save
         :param global_step: Global step value to record
```

## super_gradients/common/sg_loggers/base_sg_logger.py

```diff
@@ -6,25 +6,26 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import psutil
 import torch
 from PIL import Image
 
-from super_gradients.common.registry.registry import register_sg_logger
-from super_gradients.common.data_interface.adnn_model_repository_data_interface import ADNNModelRepositoryDataInterfaces
 from super_gradients.common.abstractions.abstract_logger import get_logger
+from super_gradients.common.auto_logging.auto_logger import AutoLoggerConfig
+from super_gradients.common.auto_logging.console_logging import ConsoleSink
+from super_gradients.common.data_interface.adnn_model_repository_data_interface import ADNNModelRepositoryDataInterfaces
 from super_gradients.common.decorators.code_save_decorator import saved_codes
 from super_gradients.common.environment.ddp_utils import multi_process_safe
+from super_gradients.common.environment.monitoring import SystemMonitor
+from super_gradients.common.registry.registry import register_sg_logger
 from super_gradients.common.sg_loggers.abstract_sg_logger import AbstractSGLogger
+from super_gradients.common.sg_loggers.time_units import TimeUnit
 from super_gradients.training.params import TrainingParams
 from super_gradients.training.utils import sg_trainer_utils, get_param
-from super_gradients.common.environment.monitoring import SystemMonitor
-from super_gradients.common.auto_logging.auto_logger import AutoLoggerConfig
-from super_gradients.common.auto_logging.console_logging import ConsoleSink
 
 logger = get_logger(__name__)
 
 EXPERIMENT_LOGS_PREFIX = "experiment_logs"
 LOGGER_LOGS_PREFIX = "logs"
 CONSOLE_LOGS_PREFIX = "console"
 
@@ -151,15 +152,17 @@
         log_lines.append(json.dumps(config, indent=4, default=str))
         log_lines.append("------- config parameters end --------")
 
         self.tensorboard_writer.add_text(tag, json.dumps(config, indent=4, default=str).replace(" ", "&nbsp;").replace("\n", "  \n  "))
         self._write_to_log_file(log_lines)
 
     @multi_process_safe
-    def add_scalar(self, tag: str, scalar_value: float, global_step: int = None):
+    def add_scalar(self, tag: str, scalar_value: float, global_step: Union[int, TimeUnit] = None):
+        if isinstance(global_step, TimeUnit):
+            global_step = global_step.get_value()
         self.tensorboard_writer.add_scalar(tag=tag.lower().replace(" ", "_"), scalar_value=scalar_value, global_step=global_step)
 
     @multi_process_safe
     def add_scalars(self, tag_scalar_dict: dict, global_step: int = None):
         """
         add multiple scalars.
         Unlike Tensorboard implementation, this does not add all scalars with a main tag (all scalars to the same chart).
```

## super_gradients/common/sg_loggers/clearml_sg_logger.py

```diff
@@ -8,14 +8,15 @@
 import torch
 
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.registry.registry import register_sg_logger
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.environment.ddp_utils import multi_process_safe
+from super_gradients.common.sg_loggers.time_units import TimeUnit
 
 logger = get_logger(__name__)
 
 try:
     from clearml import Task
 
     _imported_clear_ml_failure = None
@@ -110,16 +111,18 @@
         super(ClearMLSGLogger, self).add_config(tag=tag, config=config)
         self.task.connect(config)
 
     def __add_scalar(self, tag: str, scalar_value: float, global_step: int):
         self.clearml_logger.report_scalar(title=tag, series=tag, value=scalar_value, iteration=global_step)
 
     @multi_process_safe
-    def add_scalar(self, tag: str, scalar_value: float, global_step: int = 0):
+    def add_scalar(self, tag: str, scalar_value: float, global_step: Union[int, TimeUnit] = 0):
         super(ClearMLSGLogger, self).add_scalar(tag=tag, scalar_value=scalar_value, global_step=global_step)
+        if isinstance(global_step, TimeUnit):
+            global_step = global_step.get_value()
         self.__add_scalar(tag=tag, scalar_value=scalar_value, global_step=global_step)
 
     @multi_process_safe
     def add_scalars(self, tag_scalar_dict: dict, global_step: int = 0):
         super(ClearMLSGLogger, self).add_scalars(tag_scalar_dict=tag_scalar_dict, global_step=global_step)
         for tag, scalar_value in tag_scalar_dict.items():
             self.__add_scalar(tag=tag, scalar_value=scalar_value, global_step=global_step)
```

## super_gradients/common/sg_loggers/dagshub_sg_logger.py

```diff
@@ -5,14 +5,15 @@
 import torch
 
 from super_gradients.common.registry.registry import register_sg_logger
 from super_gradients.common.abstractions.abstract_logger import get_logger
 
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.environment.ddp_utils import multi_process_safe
+from super_gradients.common.sg_loggers.time_units import TimeUnit
 
 logger = get_logger(__name__)
 
 try:
     import dagshub
     from dagshub.upload import Repo
 
@@ -173,16 +174,18 @@
             for k, v in config[pk].items():
                 try:
                     mlflow.log_params({k: v})
                 except Exception:
                     logger.warning(f"Skip to log {k}: {v}")
 
     @multi_process_safe
-    def add_scalar(self, tag: str, scalar_value: float, global_step: int = 0):
+    def add_scalar(self, tag: str, scalar_value: float, global_step: [int, TimeUnit] = 0):
         super(DagsHubSGLogger, self).add_scalar(tag=tag, scalar_value=scalar_value, global_step=global_step)
+        if isinstance(global_step, TimeUnit):
+            global_step = global_step.get_value()
         mlflow.log_metric(key=tag, value=scalar_value, step=global_step)
 
     @multi_process_safe
     def add_scalars(self, tag_scalar_dict: dict, global_step: int = 0):
         super(DagsHubSGLogger, self).add_scalars(tag_scalar_dict=tag_scalar_dict, global_step=global_step)
         mlflow.log_metrics(metrics=tag_scalar_dict, step=global_step)
```

## super_gradients/common/sg_loggers/wandb_sg_logger.py

```diff
@@ -1,22 +1,21 @@
 import os
-
 from typing import Union, Optional, Any
 
-import numpy as np
-from PIL import Image
 import matplotlib.pyplot as plt
+import numpy as np
 import torch
+from PIL import Image
 
-from super_gradients.common.registry.registry import register_sg_logger
-from super_gradients.common.environment.env_variables import env_variables
 from super_gradients.common.abstractions.abstract_logger import get_logger
-
-from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.environment.ddp_utils import multi_process_safe
+from super_gradients.common.environment.env_variables import env_variables
+from super_gradients.common.registry.registry import register_sg_logger
+from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
+from super_gradients.common.sg_loggers.time_units import TimeUnit
 
 logger = get_logger(__name__)
 
 try:
     import wandb
 except (ModuleNotFoundError, ImportError, NameError):
     pass  # no action or logging - this is normal in most cases
@@ -165,17 +164,20 @@
 
     @multi_process_safe
     def add_config(self, tag: str, config: dict):
         super(WandBSGLogger, self).add_config(tag=tag, config=config)
         wandb.config.update(config, allow_val_change=self.resumed)
 
     @multi_process_safe
-    def add_scalar(self, tag: str, scalar_value: float, global_step: int = 0):
+    def add_scalar(self, tag: str, scalar_value: float, global_step: Union[int, TimeUnit] = 0):
         super(WandBSGLogger, self).add_scalar(tag=tag, scalar_value=scalar_value, global_step=global_step)
-        wandb.log(data={tag: scalar_value}, step=global_step)
+        if isinstance(global_step, TimeUnit):
+            wandb.log(data={tag: scalar_value, global_step.get_name(): global_step.get_value()})
+        else:
+            wandb.log(data={tag: scalar_value}, step=global_step)
 
     @multi_process_safe
     def add_scalars(self, tag_scalar_dict: dict, global_step: int = 0):
         super(WandBSGLogger, self).add_scalars(tag_scalar_dict=tag_scalar_dict, global_step=global_step)
         wandb.log(data=tag_scalar_dict, step=global_step)
 
     @multi_process_safe
```

## super_gradients/recipes/roboflow_yolox.yaml

```diff
@@ -41,23 +41,23 @@
   resume: ${resume}
   criterion_params:
     num_classes: ${num_classes}
   train_metrics_list:
     - DetectionMetrics:
         normalize_targets: True
         post_prediction_callback:
-          _target_: super_gradients.training.models.detection_models.yolo_base.YoloPostPredictionCallback
+          _target_: super_gradients.training.models.detection_models.yolo_base.YoloXPostPredictionCallback
           iou: 0.65
           conf: 0.01
         num_cls: 80
   valid_metrics_list:
     - DetectionMetrics:
         normalize_targets: True
         post_prediction_callback:
-          _target_: super_gradients.training.models.detection_models.yolo_base.YoloPostPredictionCallback
+          _target_: super_gradients.training.models.detection_models.yolo_base.YoloXPostPredictionCallback
           iou: 0.65
           conf: 0.01
         num_cls: 80
 
 
 multi_gpu: DDP
 num_gpus: 3
```

## super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml

```diff
@@ -1,11 +1,11 @@
 num_classes: 17
 hidden_channels: 256
 num_layers: 2
-joint_links:
+edge_links:
   - [ 0, 1 ]
   - [ 0, 2 ]
   - [ 1, 2 ]
   - [ 1, 3 ]
   - [ 2, 4 ]
   - [ 3, 5 ]
   - [ 4, 6 ]
```

## super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml

```diff
@@ -29,15 +29,14 @@
         hgain: 5                        # HSV transform hue gain (randomly sampled from [-hgain, hgain])
         sgain: 30                       # HSV transform saturation gain (randomly sampled from [-sgain, sgain])
         vgain: 30                       # HSV transform value gain (randomly sampled from [-vgain, vgain])
     - DetectionHorizontalFlip:
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 120
     - DetectionTargetsFormatTransform:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
         output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
@@ -61,15 +60,14 @@
   input_dim: [640, 640]
   cache_dir:
   cache: False
   transforms:
   - DetectionPaddedRescale:
       input_dim: ${dataset_params.val_dataset_params.input_dim}
   - DetectionTargetsFormatTransform:
-      max_targets: 50
       input_dim: ${dataset_params.val_dataset_params.input_dim}
       output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
```

## super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml

```diff
@@ -32,15 +32,14 @@
         mixup_scale: [ 0.5, 1.5 ]         # random rescale range for the additional sample in mixup
         prob: 0.5                       # probability to apply per-sample mixup
         flip_prob: 0.5                  # probability to apply horizontal flip
     - DetectionNormalize:
         mean: [ 123.675, 116.28, 103.53 ]
         std: [ 58.395,  57.12,  57.375 ]
     - DetectionTargetsFormatTransform:
-        max_targets: 256
         output_format: LABEL_CXCYWH
 
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
 
@@ -74,15 +73,14 @@
   transforms:
     - DetectionRescale:
         output_shape: [640, 640]
     - DetectionNormalize:
         mean: [ 123.675, 116.28, 103.53 ]
         std: [ 58.395,  57.12,  57.375 ]
     - DetectionTargetsFormatTransform:
-        max_targets: 256
         output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
 
 val_dataloader_params:
```

## super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml

```diff
@@ -24,18 +24,16 @@
         hgain: 5                        # HSV transform hue gain (randomly sampled from [-hgain, hgain])
         sgain: 30                       # HSV transform saturation gain (randomly sampled from [-sgain, sgain])
         vgain: 30                       # HSV transform value gain (randomly sampled from [-vgain, vgain])
     - DetectionHorizontalFlip:
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 120
     - DetectionTargetsFormatTransform:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 50
         output_format: LABEL_NORMALIZED_CXCYWH
 
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
 
@@ -59,15 +57,14 @@
   cache_dir:
   cache: False
   transforms:
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.val_dataset_params.input_dim}
     - DetectionTargetsFormatTransform:
         input_dim: ${dataset_params.val_dataset_params.input_dim}
-        max_targets: 50
         output_format: LABEL_NORMALIZED_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
 
 val_dataloader_params:
```

## super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml

```diff
@@ -37,15 +37,14 @@
         hgain: 5                        # HSV transform hue gain (randomly sampled from [-hgain, hgain])
         sgain: 30                       # HSV transform saturation gain (randomly sampled from [-sgain, sgain])
         vgain: 30                       # HSV transform value gain (randomly sampled from [-vgain, vgain])
     - DetectionHorizontalFlip:
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 120
     - DetectionTargetsFormatTransform:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
         output_format: LABEL_CXCYWH
   class_inclusion_list:
   max_num_samples:
 
 train_dataloader_params:
@@ -71,15 +70,14 @@
   input_dim: [640, 640]
   cache_dir:
   cache: False
   transforms:
   - DetectionPaddedRescale:
       input_dim: ${dataset_params.val_dataset_params.input_dim}
   - DetectionTargetsFormatTransform:
-      max_targets: 50
       input_dim: ${dataset_params.val_dataset_params.input_dim}
       output_format: LABEL_CXCYWH
   class_inclusion_list:
   max_num_samples:
 
 val_dataloader_params:
   batch_size: 25
```

## super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml

```diff
@@ -28,20 +28,18 @@
     - DetectionMixup:
         input_dim:
         mixup_scale: [ 0.5, 1.5 ]         # random rescale range for the additional sample in mixup
         prob: 0.5                       # probability to apply per-sample mixup
         flip_prob: 0.5                  # probability to apply horizontal flip
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 120
         pad_value: 114
     - DetectionStandardize:
         max_value: 255.
     - DetectionTargetsFormatTransform:
-        max_targets: 256
         output_format: LABEL_CXCYWH
 
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
 
@@ -67,15 +65,14 @@
     - DetectionPadToSize:
         output_size: [640, 640]
         pad_value: 114
     - DetectionStandardize:
         max_value: 255.
     - DetectionImagePermute
     - DetectionTargetsFormatTransform:
-        max_targets: 50
         input_dim: [640, 640]
         output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
```

## super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml

```diff
@@ -1,16 +1,15 @@
 num_joints: 17
 
 # OKs sigma values take from https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocotools/cocoeval.py#L523
 oks_sigmas: [0.026, 0.025, 0.025, 0.035, 0.035, 0.079, 0.079, 0.072, 0.072, 0.062, 0.062, 1.007, 1.007, 0.087, 0.087, 0.089, 0.089]
 
-flip_indexes_heatmap: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15, 17]
-flip_indexes_offset: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15,]
+flip_indexes: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15,]
 
-joint_links:
+edge_links:
   - [0, 1]
   - [0, 2]
   - [1, 2]
   - [1, 3]
   - [2, 4]
   - [3, 5]
   - [4, 6]
@@ -23,79 +22,133 @@
   - [8, 10]
   - [11, 12]
   - [11, 13]
   - [12, 14]
   - [13, 15]
   - [14, 16]
 
+edge_colors:
+ - [214, 39, 40]  # Nose -> LeftEye
+ - [148, 103, 189]  # Nose -> RightEye
+ - [44, 160, 44]  # LeftEye -> RightEye
+ - [140, 86, 75]  # LeftEye -> LeftEar
+ - [227, 119, 194]  # RightEye -> RightEar
+ - [127, 127, 127]  # LeftEar -> LeftShoulder
+ - [188, 189, 34]  # RightEar -> RightShoulder
+ - [127, 127, 127]  # Shoulders
+ - [188, 189, 34]  # LeftShoulder -> LeftElbow
+ - [140, 86, 75]  # LeftTorso
+ - [23, 190, 207]  # RightShoulder -> RightElbow
+ - [227, 119, 194]  # RightTorso
+ - [31, 119, 180]  # LeftElbow -> LeftArm
+ - [255, 127, 14]  # RightElbow -> RightArm
+ - [148, 103, 189]  # Waist
+ - [255, 127, 14]  # Left Hip -> Left Knee
+ - [214, 39, 40]  # Right Hip -> Right Knee
+ - [31, 119, 180]  # Left Knee -> Left Ankle
+ - [44, 160, 44]  # Right Knee -> Right Ankle
+
+
+keypoint_colors:
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+  - [31, 119, 180]
+  - [148, 103, 189]
+
 
 train_dataset_params:
   data_dir: /data/coco # root path to coco data
   images_dir: images/train2017
   json_file: annotations/person_keypoints_train2017.json
 
   include_empty_samples: False
   min_instance_area: 64
 
+  edge_links: ${dataset_params.edge_links}
+  edge_colors: ${dataset_params.edge_colors}
+  keypoint_colors: ${dataset_params.keypoint_colors}
+
   transforms:
     - KeypointsLongestMaxSize:
         max_height: 640
         max_width: 640
 
     - KeypointsPadIfNeeded:
         min_height: 640
         min_width: 640
-        image_pad_value: [ 127, 127, 127 ]
+        image_pad_value: 127
         mask_pad_value: 1
 
     - KeypointsRandomHorizontalFlip:
         # Note these indexes are COCO-specific. If you're using a different dataset, you'll need to change these accordingly.
-        flip_index: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15 ]
+        flip_index: ${dataset_params.flip_indexes}
         prob: 0.5
 
     - KeypointsRandomAffineTransform:
         max_rotation: 30
         min_scale: 0.5
         max_scale: 2
         max_translate: 0.2
-        image_pad_value: [ 127, 127, 127 ]
+        image_pad_value: 127
         mask_pad_value: 1
         prob: 0.75
 
-    - KeypointsImageToTensor
+    - KeypointsImageStandardize:
+        max_value: 255
 
     - KeypointsImageNormalize:
         mean: [ 0.485, 0.456, 0.406 ]
         std: [ 0.229, 0.224, 0.225 ]
 
+    - KeypointsImageToTensor
 
 val_dataset_params:
   data_dir: /data/coco/
 
   images_dir: images/val2017
   json_file: annotations/person_keypoints_val2017.json
   include_empty_samples: True
   min_instance_area: 128
+
+  edge_links: ${dataset_params.edge_links}
+  edge_colors: ${dataset_params.edge_colors}
+  keypoint_colors: ${dataset_params.keypoint_colors}
+
   transforms:
     - KeypointsLongestMaxSize:
         max_height: 640
         max_width: 640
 
     - KeypointsPadIfNeeded:
         min_height: 640
         min_width: 640
-        image_pad_value: [ 127, 127, 127 ]
+        image_pad_value: 127
         mask_pad_value: 1
 
-    - KeypointsImageToTensor
+    - KeypointsImageStandardize:
+        max_value: 255
 
     - KeypointsImageNormalize:
-        mean: [0.485, 0.456, 0.406]
-        std: [0.229, 0.224, 0.225]
+        mean: [ 0.485, 0.456, 0.406 ]
+        std: [ 0.229, 0.224, 0.225 ]
 
+    - KeypointsImageToTensor
 
 train_dataloader_params:
   shuffle: True
   batch_size: 8
   num_workers: 8
   drop_last: True
   collate_fn:
```

## super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml

```diff
@@ -1,13 +1,13 @@
 num_joints: 17
 
 # OKs sigma values take from https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocotools/cocoeval.py#L523
 oks_sigmas: [0.026, 0.025, 0.025, 0.035, 0.035, 0.079, 0.079, 0.072, 0.072, 0.062, 0.062, 1.007, 1.007, 0.087, 0.087, 0.089, 0.089]
 
-joint_links:
+edge_links:
   - [0, 1]
   - [0, 2]
   - [1, 2]
   - [1, 3]
   - [2, 4]
   - [3, 5]
   - [4, 6]
```

## super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml

```diff
@@ -3,15 +3,14 @@
   input_dim: [320, 320]
   cache: False
   cache_dir:
   transforms:
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
     - DetectionTargetsFormatTransform:
-        max_targets: 50
         input_dim: ${dataset_params.train_dataset_params.input_dim}
         output_format: LABEL_CXCYWH
   class_inclusion_list:
   max_num_samples:
   download: True
 
 val_dataset_params:
@@ -19,15 +18,14 @@
   input_dim: [320, 320]
   cache: False
   cache_dir:
   transforms:
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
     - DetectionTargetsFormatTransform:
-        max_targets: 50
         input_dim: ${dataset_params.train_dataset_params.input_dim}
         output_format: LABEL_CXCYWH
   images_sub_directory: images/test2007/
   class_inclusion_list:
   max_num_samples:
   download: True
```

## super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml

```diff
@@ -35,19 +35,17 @@
         hgain: 5                        # HSV transform hue gain (randomly sampled from [-hgain, hgain])
         sgain: 30                       # HSV transform saturation gain (randomly sampled from [-sgain, sgain])
         vgain: 30                       # HSV transform value gain (randomly sampled from [-vgain, vgain])
     - DetectionHorizontalFlip:
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionPaddedRescale:
         input_dim: ${dataset_params.train_dataset_params.input_dim}
-        max_targets: 300
     - DetectionStandardize:
         max_value: 255.
     - DetectionTargetsFormatTransform:
-        max_targets: 300
         input_dim: ${dataset_params.train_dataset_params.input_dim}
         output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: False
   verbose: 0
@@ -72,20 +70,18 @@
   input_dim: [640, 640]
   cache_dir:
   cache: False
   ignore_empty_annotations: False
   transforms:
   - DetectionPaddedRescale:
       input_dim: ${dataset_params.val_dataset_params.input_dim}
-      max_targets: 300
       pad_value: 114
   - DetectionStandardize:
       max_value: 255.
   - DetectionTargetsFormatTransform:
-      max_targets: 300
       input_dim: ${dataset_params.val_dataset_params.input_dim}
       output_format: LABEL_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
   with_crowd: True
   verbose: 0
```

## super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml

```diff
@@ -29,15 +29,15 @@
 ema: True
 mixed_precision: True
 
 valid_metrics_list:
   - DetectionMetrics:
       normalize_targets: True
       post_prediction_callback:
-        _target_: super_gradients.training.models.detection_models.yolo_base.YoloPostPredictionCallback
+        _target_: super_gradients.training.models.detection_models.yolo_base.YoloXPostPredictionCallback
         iou: 0.65
         conf: 0.01
       num_cls: 80
 
 pre_prediction_callback:
 
 phase_callbacks:
```

## super_gradients/recipes/training_hyperparams/default_train_params.yaml

```diff
@@ -6,15 +6,19 @@
 #        prior to loading weights, then training is resumed from that checkpoint. The source is unique to
 #        every logger, and currently supported for WandB loggers only.
 #
 #        IMPORTANT: Only works for experiments that were ran with sg_logger_params.save_checkpoints_remote=True.
 #        IMPORTANT: For WandB loggers, one must also pass the run id through the wandb_id arg in sg_logger_params.
 
 ckpt_name: ckpt_latest.pth  # The checkpoint (.pth file) filename in CKPT_ROOT_DIR/EXPERIMENT_NAME/ to use when resume=True and resume_path=None
-lr_mode: # Learning rate scheduling policy, one of ['step','poly','cosine','function']
+
+lr_mode: # Union[str, Mapping]
+         # when str: Learning rate scheduling policy, one of ['step','poly','cosine','function']
+         # when Mapping: refers to a torch.optim.lr_scheduler._LRScheduler, following the below API: lr_mode = {LR_SCHEDULER_CLASS_NAME: {**LR_SCHEDULER_KWARGS, "phase": XXX, "metric_name": XXX)
+
 lr_schedule_function: # Learning rate scheduling function to be used when `lr_mode` is 'function'.
 lr_warmup_epochs: 0 # number of epochs for learning rate warm up - see https://arxiv.org/pdf/1706.02677.pdf (Section 2.2).
 lr_warmup_steps: 0  # number of warmup steps (Used when warmup_mode=linear_batch_step)
 lr_cooldown_epochs: 0 # epochs to cooldown LR (i.e the last epoch from scheduling view point=max_epochs-cooldown)
 warmup_initial_lr: # Initial lr for linear_epoch_step/linear_batch_step. When none is given, initial_lr/(warmup_epochs+1) will be used.
 step_lr_update_freq: # (float) update frequency in epoch units for computing lr_updates when lr_mode=`step`.
 cosine_final_lr_ratio: 0.01 # final learning rate ratio (only relevant when `lr_mode`='cosine')
@@ -74,15 +78,16 @@
 
 dataset_statistics: False  # add a dataset statistical analysis and sample images to tensorboard
 
 
 batch_accumulate: 1  # number of batches to accumulate before every backward pass
 
 
-run_validation_freq: 1 # The frequency in which validation is performed during training
+run_validation_freq: 1 # The frequency in which validation is performed during training.
+run_test_freq: 1 # The frequency in which test is performed during training.
 
 
 save_model: True # Whether to save the model checkpoints
 
 
 seed: 42 # seed for reproducibility
 
@@ -109,8 +114,22 @@
   launch_tensorboard: False
   tensorboard_port:
   save_checkpoints_remote: False  # upload checkpoint files to s3
   save_tensorboard_remote: False  # upload tensorboard files to s3
   save_logs_remote: False  # upload log files to s3
   monitor_system: True  # Monitor and write to tensorboard the system statistics, such as CPU usage, GPU, ...
 
+torch_compile: False        # Enable or disable use of torch.compile to optimize the model (Requires Pytorch 2.0)
+torch_compile_loss: False   # Enable or disable use of torch.compile to optimize the loss  (Requires Pytorch 2.0)
+
+# torch.compile options from https://pytorch.org/docs/stable/generated/torch.compile.html
+torch_compile_options:
+  mode: reduce-overhead # default / reduce-overhead / max-autotune
+  fullgraph: False      # Whether it is ok to break model into several subgraphs
+  dynamic: False        # Use dynamic shape tracing
+  backend: inductor     # backend to be used
+  options:              # A dictionary of options to pass to the backend.
+  disable: False        # Turn torch.compile() into a no-op for testing
+
+
+
 _convert_: all
```

## super_gradients/training/params.py

```diff
@@ -12,14 +12,15 @@
     "criterion_params": {},
     "ema": False,
     "batch_accumulate": 1,  # number of batches to accumulate before every backward pass
     "ema_params": {},
     "zero_weight_decay_on_bias_and_bn": False,
     "load_opt_params": True,
     "run_validation_freq": 1,
+    "run_test_freq": 1,
     "save_model": True,
     "metric_to_watch": "Accuracy",
     "launch_tensorboard": False,
     "tb_files_user_prompt": False,  # Asks User for Tensorboard Deletion Prompt
     "silent_mode": False,  # Silents the Print outs
     "mixed_precision": False,
     "tensorboard_port": None,
@@ -60,19 +61,29 @@
     "resume_strict_load": False,
     "sync_bn": False,
     "kill_ddp_pgroup_on_end": True,  # Whether to kill the DDP process group in the end of training.
     "max_train_batches": None,  # For debug- when not None- will break out of inner train loop
     # (i.e iterating over train_loader) when reaching this number of batches.
     "max_valid_batches": None,  # For debug- when not None- will break out of inner valid loop
     # (i.e iterating over valid_loader) when reaching this number of batches.
-    "resume_from_remote_sg_logger": False  # When true, ckpt_name (checkpoint filename to resume, ckpt_latest.pth by
+    "resume_from_remote_sg_logger": False,  # When true, ckpt_name (checkpoint filename to resume, ckpt_latest.pth by
     # default) will be downloaded into the experiment checkpoints directory prior to loading weights, then resumed
     # from that checkpoint. The source is unique to every logger, and currently supported for WandB loggers only.
     # Note that for this to work, the experiment must be ran with sg_logger_params.save_checkpoints_remote=True. For
     # WandB loggers, one must also pass the run id through the wandb_id arg in sg_logger_params.
+    "torch_compile": False,  # Enable or disable use of torch.compile to optimize the model
+    "torch_compile_loss": False,  # Enable or disable use of torch.compile to optimize the loss
+    "torch_compile_options": {
+        "mode": "reduce-overhead",  # Can be either “default”, “reduce-overhead” or “max-autotune”
+        "fullgraph": False,  # Whether it is ok to break model into several subgraphs
+        "dynamic": False,  # Use dynamic shape tracing
+        "backend": "inductor",  # backend to be used
+        "options": None,  # A dictionary of options to pass to the backend.
+        "disable": False,  # Turn torch.compile() into a no-op for testing
+    },  # torch.compile options from https://pytorch.org/docs/stable/generated/torch.compile.html
 }
 
 DEFAULT_OPTIMIZER_PARAMS_SGD = {"weight_decay": 1e-4, "momentum": 0.9}
 
 DEFAULT_OPTIMIZER_PARAMS_ADAM = {"weight_decay": 1e-4}
 
 DEFAULT_OPTIMIZER_PARAMS_RMSPROP = {"weight_decay": 1e-4, "momentum": 0.9}
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## super_gradients/training/datasets/datasets_conf.py

```diff
@@ -195,7 +195,1011 @@
     "person",
     "pottedplant",
     "sheep",
     "sofa",
     "train",
     "tvmonitor",
 ]
+
+
+IMAGENET_CLASSES = [
+    "tench, Tinca tinca",
+    "goldfish, Carassius auratus",
+    "great white shark, white shark, man-eater, man-eating shark, Carcharodon carcharias",
+    "tiger shark, Galeocerdo cuvieri",
+    "hammerhead, hammerhead shark",
+    "electric ray, crampfish, numbfish, torpedo",
+    "stingray",
+    "cock",
+    "hen",
+    "ostrich, Struthio camelus",
+    "brambling, Fringilla montifringilla",
+    "goldfinch, Carduelis carduelis",
+    "house finch, linnet, Carpodacus mexicanus",
+    "junco, snowbird",
+    "indigo bunting, indigo finch, indigo bird, Passerina cyanea",
+    "robin, American robin, Turdus migratorius",
+    "bulbul",
+    "jay",
+    "magpie",
+    "chickadee",
+    "water ouzel, dipper",
+    "kite",
+    "bald eagle, American eagle, Haliaeetus leucocephalus",
+    "vulture",
+    "great grey owl, great gray owl, Strix nebulosa",
+    "European fire salamander, Salamandra salamandra",
+    "common newt, Triturus vulgaris",
+    "eft",
+    "spotted salamander, Ambystoma maculatum",
+    "axolotl, mud puppy, Ambystoma mexicanum",
+    "bullfrog, Rana catesbeiana",
+    "tree frog, tree-frog",
+    "tailed frog, bell toad, ribbed toad, tailed toad, Ascaphus trui",
+    "loggerhead, loggerhead turtle, Caretta caretta",
+    "leatherback turtle, leatherback, leathery turtle, Dermochelys coriacea",
+    "mud turtle",
+    "terrapin",
+    "box turtle, box tortoise",
+    "banded gecko",
+    "common iguana, iguana, Iguana iguana",
+    "American chameleon, anole, Anolis carolinensis",
+    "whiptail, whiptail lizard",
+    "agama",
+    "frilled lizard, Chlamydosaurus kingi",
+    "alligator lizard",
+    "Gila monster, Heloderma suspectum",
+    "green lizard, Lacerta viridis",
+    "African chameleon, Chamaeleo chamaeleon",
+    "Komodo dragon, Komodo lizard, dragon lizard, giant lizard, Varanus komodoensis",
+    "African crocodile, Nile crocodile, Crocodylus niloticus",
+    "American alligator, Alligator mississipiensis",
+    "triceratops",
+    "thunder snake, worm snake, Carphophis amoenus",
+    "ringneck snake, ring-necked snake, ring snake",
+    "hognose snake, puff adder, sand viper",
+    "green snake, grass snake",
+    "king snake, kingsnake",
+    "garter snake, grass snake",
+    "water snake",
+    "vine snake",
+    "night snake, Hypsiglena torquata",
+    "boa constrictor, Constrictor constrictor",
+    "rock python, rock snake, Python sebae",
+    "Indian cobra, Naja naja",
+    "green mamba",
+    "sea snake",
+    "horned viper, cerastes, sand viper, horned asp, Cerastes cornutus",
+    "diamondback, diamondback rattlesnake, Crotalus adamanteus",
+    "sidewinder, horned rattlesnake, Crotalus cerastes",
+    "trilobite",
+    "harvestman, daddy longlegs, Phalangium opilio",
+    "scorpion",
+    "black and gold garden spider, Argiope aurantia",
+    "barn spider, Araneus cavaticus",
+    "garden spider, Aranea diademata",
+    "black widow, Latrodectus mactans",
+    "tarantula",
+    "wolf spider, hunting spider",
+    "tick",
+    "centipede",
+    "black grouse",
+    "ptarmigan",
+    "ruffed grouse, partridge, Bonasa umbellus",
+    "prairie chicken, prairie grouse, prairie fowl",
+    "peacock",
+    "quail",
+    "partridge",
+    "African grey, African gray, Psittacus erithacus",
+    "macaw",
+    "sulphur-crested cockatoo, Kakatoe galerita, Cacatua galerita",
+    "lorikeet",
+    "coucal",
+    "bee eater",
+    "hornbill",
+    "hummingbird",
+    "jacamar",
+    "toucan",
+    "drake",
+    "red-breasted merganser, Mergus serrator",
+    "goose",
+    "black swan, Cygnus atratus",
+    "tusker",
+    "echidna, spiny anteater, anteater",
+    "platypus, duckbill, duckbilled platypus, duck-billed platypus, Ornithorhynchus anatinus",
+    "wallaby, brush kangaroo",
+    "koala, koala bear, kangaroo bear, native bear, Phascolarctos cinereus",
+    "wombat",
+    "jellyfish",
+    "sea anemone, anemone",
+    "brain coral",
+    "flatworm, platyhelminth",
+    "nematode, nematode worm, roundworm",
+    "conch",
+    "snail",
+    "slug",
+    "sea slug, nudibranch",
+    "chiton, coat-of-mail shell, sea cradle, polyplacophore",
+    "chambered nautilus, pearly nautilus, nautilus",
+    "Dungeness crab, Cancer magister",
+    "rock crab, Cancer irroratus",
+    "fiddler crab",
+    "king crab, Alaska crab, Alaskan king crab, Alaska king crab, Paralithodes camtschatica",
+    "American lobster, Northern lobster, Maine lobster, Homarus americanus",
+    "spiny lobster, langouste, rock lobster, crawfish, crayfish, sea crawfish",
+    "crayfish, crawfish, crawdad, crawdaddy",
+    "hermit crab",
+    "isopod",
+    "white stork, Ciconia ciconia",
+    "black stork, Ciconia nigra",
+    "spoonbill",
+    "flamingo",
+    "little blue heron, Egretta caerulea",
+    "American egret, great white heron, Egretta albus",
+    "bittern",
+    "crane",
+    "limpkin, Aramus pictus",
+    "European gallinule, Porphyrio porphyrio",
+    "American coot, marsh hen, mud hen, water hen, Fulica americana",
+    "bustard",
+    "ruddy turnstone, Arenaria interpres",
+    "red-backed sandpiper, dunlin, Erolia alpina",
+    "redshank, Tringa totanus",
+    "dowitcher",
+    "oystercatcher, oyster catcher",
+    "pelican",
+    "king penguin, Aptenodytes patagonica",
+    "albatross, mollymawk",
+    "grey whale, gray whale, devilfish, Eschrichtius gibbosus, Eschrichtius robustus",
+    "killer whale, killer, orca, grampus, sea wolf, Orcinus orca",
+    "dugong, Dugong dugon",
+    "sea lion",
+    "Chihuahua",
+    "Japanese spaniel",
+    "Maltese dog, Maltese terrier, Maltese",
+    "Pekinese, Pekingese, Peke",
+    "Shih-Tzu",
+    "Blenheim spaniel",
+    "papillon",
+    "toy terrier",
+    "Rhodesian ridgeback",
+    "Afghan hound, Afghan",
+    "basset, basset hound",
+    "beagle",
+    "bloodhound, sleuthhound",
+    "bluetick",
+    "black-and-tan coonhound",
+    "Walker hound, Walker foxhound",
+    "English foxhound",
+    "redbone",
+    "borzoi, Russian wolfhound",
+    "Irish wolfhound",
+    "Italian greyhound",
+    "whippet",
+    "Ibizan hound, Ibizan Podenco",
+    "Norwegian elkhound, elkhound",
+    "otterhound, otter hound",
+    "Saluki, gazelle hound",
+    "Scottish deerhound, deerhound",
+    "Weimaraner",
+    "Staffordshire bullterrier, Staffordshire bull terrier",
+    "American Staffordshire terrier, Staffordshire terrier, American pit bull terrier, pit bull terrier",
+    "Bedlington terrier",
+    "Border terrier",
+    "Kerry blue terrier",
+    "Irish terrier",
+    "Norfolk terrier",
+    "Norwich terrier",
+    "Yorkshire terrier",
+    "wire-haired fox terrier",
+    "Lakeland terrier",
+    "Sealyham terrier, Sealyham",
+    "Airedale, Airedale terrier",
+    "cairn, cairn terrier",
+    "Australian terrier",
+    "Dandie Dinmont, Dandie Dinmont terrier",
+    "Boston bull, Boston terrier",
+    "miniature schnauzer",
+    "giant schnauzer",
+    "standard schnauzer",
+    "Scotch terrier, Scottish terrier, Scottie",
+    "Tibetan terrier, chrysanthemum dog",
+    "silky terrier, Sydney silky",
+    "soft-coated wheaten terrier",
+    "West Highland white terrier",
+    "Lhasa, Lhasa apso",
+    "flat-coated retriever",
+    "curly-coated retriever",
+    "golden retriever",
+    "Labrador retriever",
+    "Chesapeake Bay retriever",
+    "German short-haired pointer",
+    "vizsla, Hungarian pointer",
+    "English setter",
+    "Irish setter, red setter",
+    "Gordon setter",
+    "Brittany spaniel",
+    "clumber, clumber spaniel",
+    "English springer, English springer spaniel",
+    "Welsh springer spaniel",
+    "cocker spaniel, English cocker spaniel, cocker",
+    "Sussex spaniel",
+    "Irish water spaniel",
+    "kuvasz",
+    "schipperke",
+    "groenendael",
+    "malinois",
+    "briard",
+    "kelpie",
+    "komondor",
+    "Old English sheepdog, bobtail",
+    "Shetland sheepdog, Shetland sheep dog, Shetland",
+    "collie",
+    "Border collie",
+    "Bouvier des Flandres, Bouviers des Flandres",
+    "Rottweiler",
+    "German shepherd, German shepherd dog, German police dog, alsatian",
+    "Doberman, Doberman pinscher",
+    "miniature pinscher",
+    "Greater Swiss Mountain dog",
+    "Bernese mountain dog",
+    "Appenzeller",
+    "EntleBucher",
+    "boxer",
+    "bull mastiff",
+    "Tibetan mastiff",
+    "French bulldog",
+    "Great Dane",
+    "Saint Bernard, St Bernard",
+    "Eskimo dog, husky",
+    "malamute, malemute, Alaskan malamute",
+    "Siberian husky",
+    "dalmatian, coach dog, carriage dog",
+    "affenpinscher, monkey pinscher, monkey dog",
+    "basenji",
+    "pug, pug-dog",
+    "Leonberg",
+    "Newfoundland, Newfoundland dog",
+    "Great Pyrenees",
+    "Samoyed, Samoyede",
+    "Pomeranian",
+    "chow, chow chow",
+    "keeshond",
+    "Brabancon griffon",
+    "Pembroke, Pembroke Welsh corgi",
+    "Cardigan, Cardigan Welsh corgi",
+    "toy poodle",
+    "miniature poodle",
+    "standard poodle",
+    "Mexican hairless",
+    "timber wolf, grey wolf, gray wolf, Canis lupus",
+    "white wolf, Arctic wolf, Canis lupus tundrarum",
+    "red wolf, maned wolf, Canis rufus, Canis niger",
+    "coyote, prairie wolf, brush wolf, Canis latrans",
+    "dingo, warrigal, warragal, Canis dingo",
+    "dhole, Cuon alpinus",
+    "African hunting dog, hyena dog, Cape hunting dog, Lycaon pictus",
+    "hyena, hyaena",
+    "red fox, Vulpes vulpes",
+    "kit fox, Vulpes macrotis",
+    "Arctic fox, white fox, Alopex lagopus",
+    "grey fox, gray fox, Urocyon cinereoargenteus",
+    "tabby, tabby cat",
+    "tiger cat",
+    "Persian cat",
+    "Siamese cat, Siamese",
+    "Egyptian cat",
+    "cougar, puma, catamount, mountain lion, painter, panther, Felis concolor",
+    "lynx, catamount",
+    "leopard, Panthera pardus",
+    "snow leopard, ounce, Panthera uncia",
+    "jaguar, panther, Panthera onca, Felis onca",
+    "lion, king of beasts, Panthera leo",
+    "tiger, Panthera tigris",
+    "cheetah, chetah, Acinonyx jubatus",
+    "brown bear, bruin, Ursus arctos",
+    "American black bear, black bear, Ursus americanus, Euarctos americanus",
+    "ice bear, polar bear, Ursus Maritimus, Thalarctos maritimus",
+    "sloth bear, Melursus ursinus, Ursus ursinus",
+    "mongoose",
+    "meerkat, mierkat",
+    "tiger beetle",
+    "ladybug, ladybeetle, lady beetle, ladybird, ladybird beetle",
+    "ground beetle, carabid beetle",
+    "long-horned beetle, longicorn, longicorn beetle",
+    "leaf beetle, chrysomelid",
+    "dung beetle",
+    "rhinoceros beetle",
+    "weevil",
+    "fly",
+    "bee",
+    "ant, emmet, pismire",
+    "grasshopper, hopper",
+    "cricket",
+    "walking stick, walkingstick, stick insect",
+    "cockroach, roach",
+    "mantis, mantid",
+    "cicada, cicala",
+    "leafhopper",
+    "lacewing, lacewing fly",
+    "dragonfly, darning needle, devil's darning needle, sewing needle, snake feeder, snake doctor, mosquito hawk, skeeter hawk",
+    "damselfly",
+    "admiral",
+    "ringlet, ringlet butterfly",
+    "monarch, monarch butterfly, milkweed butterfly, Danaus plexippus",
+    "cabbage butterfly",
+    "sulphur butterfly, sulfur butterfly",
+    "lycaenid, lycaenid butterfly",
+    "starfish, sea star",
+    "sea urchin",
+    "sea cucumber, holothurian",
+    "wood rabbit, cottontail, cottontail rabbit",
+    "hare",
+    "Angora, Angora rabbit",
+    "hamster",
+    "porcupine, hedgehog",
+    "fox squirrel, eastern fox squirrel, Sciurus niger",
+    "marmot",
+    "beaver",
+    "guinea pig, Cavia cobaya",
+    "sorrel",
+    "zebra",
+    "hog, pig, grunter, squealer, Sus scrofa",
+    "wild boar, boar, Sus scrofa",
+    "warthog",
+    "hippopotamus, hippo, river horse, Hippopotamus amphibius",
+    "ox",
+    "water buffalo, water ox, Asiatic buffalo, Bubalus bubalis",
+    "bison",
+    "ram, tup",
+    "bighorn, bighorn sheep, cimarron, Rocky Mountain bighorn, Rocky Mountain sheep, Ovis canadensis",
+    "ibex, Capra ibex",
+    "hartebeest",
+    "impala, Aepyceros melampus",
+    "gazelle",
+    "Arabian camel, dromedary, Camelus dromedarius",
+    "llama",
+    "weasel",
+    "mink",
+    "polecat, fitch, foulmart, foumart, Mustela putorius",
+    "black-footed ferret, ferret, Mustela nigripes",
+    "otter",
+    "skunk, polecat, wood pussy",
+    "badger",
+    "armadillo",
+    "three-toed sloth, ai, Bradypus tridactylus",
+    "orangutan, orang, orangutang, Pongo pygmaeus",
+    "gorilla, Gorilla gorilla",
+    "chimpanzee, chimp, Pan troglodytes",
+    "gibbon, Hylobates lar",
+    "siamang, Hylobates syndactylus, Symphalangus syndactylus",
+    "guenon, guenon monkey",
+    "patas, hussar monkey, Erythrocebus patas",
+    "baboon",
+    "macaque",
+    "langur",
+    "colobus, colobus monkey",
+    "proboscis monkey, Nasalis larvatus",
+    "marmoset",
+    "capuchin, ringtail, Cebus capucinus",
+    "howler monkey, howler",
+    "titi, titi monkey",
+    "spider monkey, Ateles geoffroyi",
+    "squirrel monkey, Saimiri sciureus",
+    "Madagascar cat, ring-tailed lemur, Lemur catta",
+    "indri, indris, Indri indri, Indri brevicaudatus",
+    "Indian elephant, Elephas maximus",
+    "African elephant, Loxodonta africana",
+    "lesser panda, red panda, panda, bear cat, cat bear, Ailurus fulgens",
+    "giant panda, panda, panda bear, coon bear, Ailuropoda melanoleuca",
+    "barracouta, snoek",
+    "eel",
+    "coho, cohoe, coho salmon, blue jack, silver salmon, Oncorhynchus kisutch",
+    "rock beauty, Holocanthus tricolor",
+    "anemone fish",
+    "sturgeon",
+    "gar, garfish, garpike, billfish, Lepisosteus osseus",
+    "lionfish",
+    "puffer, pufferfish, blowfish, globefish",
+    "abacus",
+    "abaya",
+    "academic gown, academic robe, judge's robe",
+    "accordion, piano accordion, squeeze box",
+    "acoustic guitar",
+    "aircraft carrier, carrier, flattop, attack aircraft carrier",
+    "airliner",
+    "airship, dirigible",
+    "altar",
+    "ambulance",
+    "amphibian, amphibious vehicle",
+    "analog clock",
+    "apiary, bee house",
+    "apron",
+    "ashcan, trash can, garbage can, wastebin, ash bin, ash-bin, ashbin, dustbin, trash barrel, trash bin",
+    "assault rifle, assault gun",
+    "backpack, back pack, knapsack, packsack, rucksack, haversack",
+    "bakery, bakeshop, bakehouse",
+    "balance beam, beam",
+    "balloon",
+    "ballpoint, ballpoint pen, ballpen, Biro",
+    "Band Aid",
+    "banjo",
+    "bannister, banister, balustrade, balusters, handrail",
+    "barbell",
+    "barber chair",
+    "barbershop",
+    "barn",
+    "barometer",
+    "barrel, cask",
+    "barrow, garden cart, lawn cart, wheelbarrow",
+    "baseball",
+    "basketball",
+    "bassinet",
+    "bassoon",
+    "bathing cap, swimming cap",
+    "bath towel",
+    "bathtub, bathing tub, bath, tub",
+    "beach wagon, station wagon, wagon, estate car, beach waggon, station waggon, waggon",
+    "beacon, lighthouse, beacon light, pharos",
+    "beaker",
+    "bearskin, busby, shako",
+    "beer bottle",
+    "beer glass",
+    "bell cote, bell cot",
+    "bib",
+    "bicycle-built-for-two, tandem bicycle, tandem",
+    "bikini, two-piece",
+    "binder, ring-binder",
+    "binoculars, field glasses, opera glasses",
+    "birdhouse",
+    "boathouse",
+    "bobsled, bobsleigh, bob",
+    "bolo tie, bolo, bola tie, bola",
+    "bonnet, poke bonnet",
+    "bookcase",
+    "bookshop, bookstore, bookstall",
+    "bottlecap",
+    "bow",
+    "bow tie, bow-tie, bowtie",
+    "brass, memorial tablet, plaque",
+    "brassiere, bra, bandeau",
+    "breakwater, groin, groyne, mole, bulwark, seawall, jetty",
+    "breastplate, aegis, egis",
+    "broom",
+    "bucket, pail",
+    "buckle",
+    "bulletproof vest",
+    "bullet train, bullet",
+    "butcher shop, meat market",
+    "cab, hack, taxi, taxicab",
+    "caldron, cauldron",
+    "candle, taper, wax light",
+    "cannon",
+    "canoe",
+    "can opener, tin opener",
+    "cardigan",
+    "car mirror",
+    "carousel, carrousel, merry-go-round, roundabout, whirligig",
+    "carpenter's kit, tool kit",
+    "carton",
+    "car wheel",
+    "cash machine, cash dispenser, automated teller machine, automatic teller machine, automated teller, automatic teller, ATM",
+    "cassette",
+    "cassette player",
+    "castle",
+    "catamaran",
+    "CD player",
+    "cello, violoncello",
+    "cellular telephone, cellular phone, cellphone, cell, mobile phone",
+    "chain",
+    "chainlink fence",
+    "chain mail, ring mail, mail, chain armor, chain armour, ring armor, ring armour",
+    "chain saw, chainsaw",
+    "chest",
+    "chiffonier, commode",
+    "chime, bell, gong",
+    "china cabinet, china closet",
+    "Christmas stocking",
+    "church, church building",
+    "cinema, movie theater, movie theatre, movie house, picture palace",
+    "cleaver, meat cleaver, chopper",
+    "cliff dwelling",
+    "cloak",
+    "clog, geta, patten, sabot",
+    "cocktail shaker",
+    "coffee mug",
+    "coffeepot",
+    "coil, spiral, volute, whorl, helix",
+    "combination lock",
+    "computer keyboard, keypad",
+    "confectionery, confectionary, candy store",
+    "container ship, containership, container vessel",
+    "convertible",
+    "corkscrew, bottle screw",
+    "cornet, horn, trumpet, trump",
+    "cowboy boot",
+    "cowboy hat, ten-gallon hat",
+    "cradle",
+    "crane",
+    "crash helmet",
+    "crate",
+    "crib, cot",
+    "Crock Pot",
+    "croquet ball",
+    "crutch",
+    "cuirass",
+    "dam, dike, dyke",
+    "desk",
+    "desktop computer",
+    "dial telephone, dial phone",
+    "diaper, nappy, napkin",
+    "digital clock",
+    "digital watch",
+    "dining table, board",
+    "dishrag, dishcloth",
+    "dishwasher, dish washer, dishwashing machine",
+    "disk brake, disc brake",
+    "dock, dockage, docking facility",
+    "dogsled, dog sled, dog sleigh",
+    "dome",
+    "doormat, welcome mat",
+    "drilling platform, offshore rig",
+    "drum, membranophone, tympan",
+    "drumstick",
+    "dumbbell",
+    "Dutch oven",
+    "electric fan, blower",
+    "electric guitar",
+    "electric locomotive",
+    "entertainment center",
+    "envelope",
+    "espresso maker",
+    "face powder",
+    "feather boa, boa",
+    "file, file cabinet, filing cabinet",
+    "fireboat",
+    "fire engine, fire truck",
+    "fire screen, fireguard",
+    "flagpole, flagstaff",
+    "flute, transverse flute",
+    "folding chair",
+    "football helmet",
+    "forklift",
+    "fountain",
+    "fountain pen",
+    "four-poster",
+    "freight car",
+    "French horn, horn",
+    "frying pan, frypan, skillet",
+    "fur coat",
+    "garbage truck, dustcart",
+    "gasmask, respirator, gas helmet",
+    "gas pump, gasoline pump, petrol pump, island dispenser",
+    "goblet",
+    "go-kart",
+    "golf ball",
+    "golfcart, golf cart",
+    "gondola",
+    "gong, tam-tam",
+    "gown",
+    "grand piano, grand",
+    "greenhouse, nursery, glasshouse",
+    "grille, radiator grille",
+    "grocery store, grocery, food market, market",
+    "guillotine",
+    "hair slide",
+    "hair spray",
+    "half track",
+    "hammer",
+    "hamper",
+    "hand blower, blow dryer, blow drier, hair dryer, hair drier",
+    "hand-held computer, hand-held microcomputer",
+    "handkerchief, hankie, hanky, hankey",
+    "hard disc, hard disk, fixed disk",
+    "harmonica, mouth organ, harp, mouth harp",
+    "harp",
+    "harvester, reaper",
+    "hatchet",
+    "holster",
+    "home theater, home theatre",
+    "honeycomb",
+    "hook, claw",
+    "hoopskirt, crinoline",
+    "horizontal bar, high bar",
+    "horse cart, horse-cart",
+    "hourglass",
+    "iPod",
+    "iron, smoothing iron",
+    "jack-o'-lantern",
+    "jean, blue jean, denim",
+    "jeep, landrover",
+    "jersey, T-shirt, tee shirt",
+    "jigsaw puzzle",
+    "jinrikisha, ricksha, rickshaw",
+    "joystick",
+    "kimono",
+    "knee pad",
+    "knot",
+    "lab coat, laboratory coat",
+    "ladle",
+    "lampshade, lamp shade",
+    "laptop, laptop computer",
+    "lawn mower, mower",
+    "lens cap, lens cover",
+    "letter opener, paper knife, paperknife",
+    "library",
+    "lifeboat",
+    "lighter, light, igniter, ignitor",
+    "limousine, limo",
+    "liner, ocean liner",
+    "lipstick, lip rouge",
+    "Loafer",
+    "lotion",
+    "loudspeaker, speaker, speaker unit, loudspeaker system, speaker system",
+    "loupe, jeweler's loupe",
+    "lumbermill, sawmill",
+    "magnetic compass",
+    "mailbag, postbag",
+    "mailbox, letter box",
+    "maillot",
+    "maillot, tank suit",
+    "manhole cover",
+    "maraca",
+    "marimba, xylophone",
+    "mask",
+    "matchstick",
+    "maypole",
+    "maze, labyrinth",
+    "measuring cup",
+    "medicine chest, medicine cabinet",
+    "megalith, megalithic structure",
+    "microphone, mike",
+    "microwave, microwave oven",
+    "military uniform",
+    "milk can",
+    "minibus",
+    "miniskirt, mini",
+    "minivan",
+    "missile",
+    "mitten",
+    "mixing bowl",
+    "mobile home, manufactured home",
+    "Model T",
+    "modem",
+    "monastery",
+    "monitor",
+    "moped",
+    "mortar",
+    "mortarboard",
+    "mosque",
+    "mosquito net",
+    "motor scooter, scooter",
+    "mountain bike, all-terrain bike, off-roader",
+    "mountain tent",
+    "mouse, computer mouse",
+    "mousetrap",
+    "moving van",
+    "muzzle",
+    "nail",
+    "neck brace",
+    "necklace",
+    "nipple",
+    "notebook, notebook computer",
+    "obelisk",
+    "oboe, hautboy, hautbois",
+    "ocarina, sweet potato",
+    "odometer, hodometer, mileometer, milometer",
+    "oil filter",
+    "organ, pipe organ",
+    "oscilloscope, scope, cathode-ray oscilloscope, CRO",
+    "overskirt",
+    "oxcart",
+    "oxygen mask",
+    "packet",
+    "paddle, boat paddle",
+    "paddlewheel, paddle wheel",
+    "padlock",
+    "paintbrush",
+    "pajama, pyjama, pj's, jammies",
+    "palace",
+    "panpipe, pandean pipe, syrinx",
+    "paper towel",
+    "parachute, chute",
+    "parallel bars, bars",
+    "park bench",
+    "parking meter",
+    "passenger car, coach, carriage",
+    "patio, terrace",
+    "pay-phone, pay-station",
+    "pedestal, plinth, footstall",
+    "pencil box, pencil case",
+    "pencil sharpener",
+    "perfume, essence",
+    "Petri dish",
+    "photocopier",
+    "pick, plectrum, plectron",
+    "pickelhaube",
+    "picket fence, paling",
+    "pickup, pickup truck",
+    "pier",
+    "piggy bank, penny bank",
+    "pill bottle",
+    "pillow",
+    "ping-pong ball",
+    "pinwheel",
+    "pirate, pirate ship",
+    "pitcher, ewer",
+    "plane, carpenter's plane, woodworking plane",
+    "planetarium",
+    "plastic bag",
+    "plate rack",
+    "plow, plough",
+    "plunger, plumber's helper",
+    "Polaroid camera, Polaroid Land camera",
+    "pole",
+    "police van, police wagon, paddy wagon, patrol wagon, wagon, black Maria",
+    "poncho",
+    "pool table, billiard table, snooker table",
+    "pop bottle, soda bottle",
+    "pot, flowerpot",
+    "potter's wheel",
+    "power drill",
+    "prayer rug, prayer mat",
+    "printer",
+    "prison, prison house",
+    "projectile, missile",
+    "projector",
+    "puck, hockey puck",
+    "punching bag, punch bag, punching ball, punchball",
+    "purse",
+    "quill, quill pen",
+    "quilt, comforter, comfort, puff",
+    "racer, race car, racing car",
+    "racket, racquet",
+    "radiator",
+    "radio, wireless",
+    "radio telescope, radio reflector",
+    "rain barrel",
+    "recreational vehicle, RV, R.V.",
+    "reel",
+    "reflex camera",
+    "refrigerator, icebox",
+    "remote control, remote",
+    "restaurant, eating house, eating place, eatery",
+    "revolver, six-gun, six-shooter",
+    "rifle",
+    "rocking chair, rocker",
+    "rotisserie",
+    "rubber eraser, rubber, pencil eraser",
+    "rugby ball",
+    "rule, ruler",
+    "running shoe",
+    "safe",
+    "safety pin",
+    "saltshaker, salt shaker",
+    "sandal",
+    "sarong",
+    "sax, saxophone",
+    "scabbard",
+    "scale, weighing machine",
+    "school bus",
+    "schooner",
+    "scoreboard",
+    "screen, CRT screen",
+    "screw",
+    "screwdriver",
+    "seat belt, seatbelt",
+    "sewing machine",
+    "shield, buckler",
+    "shoe shop, shoe-shop, shoe store",
+    "shoji",
+    "shopping basket",
+    "shopping cart",
+    "shovel",
+    "shower cap",
+    "shower curtain",
+    "ski",
+    "ski mask",
+    "sleeping bag",
+    "slide rule, slipstick",
+    "sliding door",
+    "slot, one-armed bandit",
+    "snorkel",
+    "snowmobile",
+    "snowplow, snowplough",
+    "soap dispenser",
+    "soccer ball",
+    "sock",
+    "solar dish, solar collector, solar furnace",
+    "sombrero",
+    "soup bowl",
+    "space bar",
+    "space heater",
+    "space shuttle",
+    "spatula",
+    "speedboat",
+    "spider web, spider's web",
+    "spindle",
+    "sports car, sport car",
+    "spotlight, spot",
+    "stage",
+    "steam locomotive",
+    "steel arch bridge",
+    "steel drum",
+    "stethoscope",
+    "stole",
+    "stone wall",
+    "stopwatch, stop watch",
+    "stove",
+    "strainer",
+    "streetcar, tram, tramcar, trolley, trolley car",
+    "stretcher",
+    "studio couch, day bed",
+    "stupa, tope",
+    "submarine, pigboat, sub, U-boat",
+    "suit, suit of clothes",
+    "sundial",
+    "sunglass",
+    "sunglasses, dark glasses, shades",
+    "sunscreen, sunblock, sun blocker",
+    "suspension bridge",
+    "swab, swob, mop",
+    "sweatshirt",
+    "swimming trunks, bathing trunks",
+    "swing",
+    "switch, electric switch, electrical switch",
+    "syringe",
+    "table lamp",
+    "tank, army tank, armored combat vehicle, armoured combat vehicle",
+    "tape player",
+    "teapot",
+    "teddy, teddy bear",
+    "television, television system",
+    "tennis ball",
+    "thatch, thatched roof",
+    "theater curtain, theatre curtain",
+    "thimble",
+    "thresher, thrasher, threshing machine",
+    "throne",
+    "tile roof",
+    "toaster",
+    "tobacco shop, tobacconist shop, tobacconist",
+    "toilet seat",
+    "torch",
+    "totem pole",
+    "tow truck, tow car, wrecker",
+    "toyshop",
+    "tractor",
+    "trailer truck, tractor trailer, trucking rig, rig, articulated lorry, semi",
+    "tray",
+    "trench coat",
+    "tricycle, trike, velocipede",
+    "trimaran",
+    "tripod",
+    "triumphal arch",
+    "trolleybus, trolley coach, trackless trolley",
+    "trombone",
+    "tub, vat",
+    "turnstile",
+    "typewriter keyboard",
+    "umbrella",
+    "unicycle, monocycle",
+    "upright, upright piano",
+    "vacuum, vacuum cleaner",
+    "vase",
+    "vault",
+    "velvet",
+    "vending machine",
+    "vestment",
+    "viaduct",
+    "violin, fiddle",
+    "volleyball",
+    "waffle iron",
+    "wall clock",
+    "wallet, billfold, notecase, pocketbook",
+    "wardrobe, closet, press",
+    "warplane, military plane",
+    "washbasin, handbasin, washbowl, lavabo, wash-hand basin",
+    "washer, automatic washer, washing machine",
+    "water bottle",
+    "water jug",
+    "water tower",
+    "whiskey jug",
+    "whistle",
+    "wig",
+    "window screen",
+    "window shade",
+    "Windsor tie",
+    "wine bottle",
+    "wing",
+    "wok",
+    "wooden spoon",
+    "wool, woolen, woollen",
+    "worm fence, snake fence, snake-rail fence, Virginia fence",
+    "wreck",
+    "yawl",
+    "yurt",
+    "web site, website, internet site, site",
+    "comic book",
+    "crossword puzzle, crossword",
+    "street sign",
+    "traffic light, traffic signal, stoplight",
+    "book jacket, dust cover, dust jacket, dust wrapper",
+    "menu",
+    "plate",
+    "guacamole",
+    "consomme",
+    "hot pot, hotpot",
+    "trifle",
+    "ice cream, icecream",
+    "ice lolly, lolly, lollipop, popsicle",
+    "French loaf",
+    "bagel, beigel",
+    "pretzel",
+    "cheeseburger",
+    "hotdog, hot dog, red hot",
+    "mashed potato",
+    "head cabbage",
+    "broccoli",
+    "cauliflower",
+    "zucchini, courgette",
+    "spaghetti squash",
+    "acorn squash",
+    "butternut squash",
+    "cucumber, cuke",
+    "artichoke, globe artichoke",
+    "bell pepper",
+    "cardoon",
+    "mushroom",
+    "Granny Smith",
+    "strawberry",
+    "orange",
+    "lemon",
+    "fig",
+    "pineapple, ananas",
+    "banana",
+    "jackfruit, jak, jack",
+    "custard apple",
+    "pomegranate",
+    "hay",
+    "carbonara",
+    "chocolate sauce, chocolate syrup",
+    "dough",
+    "meat loaf, meatloaf",
+    "pizza, pizza pie",
+    "potpie",
+    "burrito",
+    "red wine",
+    "espresso",
+    "cup",
+    "eggnog",
+    "alp",
+    "bubble",
+    "cliff, drop, drop-off",
+    "coral reef",
+    "geyser",
+    "lakeside, lakeshore",
+    "promontory, headland, head, foreland",
+    "sandbar, sand bar",
+    "seashore, coast, seacoast, sea-coast",
+    "valley, vale",
+    "volcano",
+    "ballplayer, baseball player",
+    "groom, bridegroom",
+    "scuba diver",
+    "rapeseed",
+    "daisy",
+    "yellow lady's slipper, yellow lady-slipper, Cypripedium calceolus, Cypripedium parviflorum",
+    "corn",
+    "acorn",
+    "hip, rose hip, rosehip",
+    "buckeye, horse chestnut, conker",
+    "coral fungus",
+    "agaric",
+    "gyromitra",
+    "stinkhorn, carrion fungus",
+    "earthstar",
+    "hen-of-the-woods, hen of the woods, Polyporus frondosus, Grifola frondosa",
+    "bolete",
+    "ear, spike, capitulum",
+    "toilet tissue, toilet paper, bathroom tissue",
+]
```

## super_gradients/training/datasets/mixup.py

```diff
@@ -12,15 +12,15 @@
 """
 from typing import List, Union
 
 import numpy as np
 import torch
 
 from super_gradients.common.registry.registry import register_collate_function
-from super_gradients.training.exceptions.dataset_exceptions import IllegalDatasetParameterException
+from super_gradients.common.exceptions.dataset_exceptions import IllegalDatasetParameterException
 
 
 def one_hot(x, num_classes, on_value=1.0, off_value=0.0, device="cuda"):
     x = x.long().view(-1, 1)
     return torch.full((x.size()[0], num_classes), off_value, device=device).scatter_(1, x, on_value)
```

## super_gradients/training/datasets/sg_dataset.py

```diff
@@ -3,15 +3,15 @@
 import os
 import os.path
 from typing import Callable, Tuple, Any
 
 from torchvision.datasets import VisionDataset
 from torchvision.datasets.folder import default_loader
 
-IMG_EXTENSIONS = (".jpg", ".jpeg", ".png", ".ppm", ".bmp", ".pgm", ".tif", ".tiff", ".webp")
+from super_gradients.training.utils.media.image import IMG_EXTENSIONS
 
 
 class BaseSgVisionDataset(VisionDataset):
     """
     BaseSgVisionDataset
     """
```

## super_gradients/training/datasets/detection_datasets/coco_format_detection.py

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 from pycocotools.coco import COCO
 from typing import List, Optional
 
 from contextlib import redirect_stdout
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.datasets.detection_datasets.detection_dataset import DetectionDataset
-from super_gradients.training.exceptions.dataset_exceptions import DatasetValidationException, ParameterMismatchException
+from super_gradients.common.exceptions.dataset_exceptions import DatasetValidationException, ParameterMismatchException
 from super_gradients.training.datasets.data_formats.default_formats import XYXY_LABEL
 
 logger = get_logger(__name__)
 
 
 class COCOFormatDetectionDataset(DetectionDataset):
     """Base dataset to load ANY dataset that is with a similar structure to the COCO dataset.
@@ -139,15 +139,15 @@
         for ix, annotation in enumerate(non_crowd_annotations):
             cls = self.class_ids.index(annotation["category_id"])
             target[ix, 0:4] = annotation["clean_bbox"]
             target[ix, 4] = cls
             if self.tight_box_rotation:
                 seg_points = [j for i in annotation.get("segmentation", []) for j in i]
                 if seg_points:
-                    seg_points_c = np.array(seg_points).reshape((-1, 2)).astype(np.int)
+                    seg_points_c = np.array(seg_points).reshape((-1, 2)).astype(np.int32)
                     seg_points_convex = cv2.convexHull(seg_points_c).ravel()
                 else:
                     seg_points_convex = []
                 target_segmentation[ix, : len(seg_points_convex)] = seg_points_convex
 
         crowd_annotations = [annotation for annotation in cleaned_annotations if annotation["iscrowd"] == 1]
```

## super_gradients/training/datasets/detection_datasets/detection_dataset.py

```diff
@@ -15,15 +15,15 @@
 
 from super_gradients.common.object_names import Datasets, Processings
 from super_gradients.common.registry.registry import register_dataset
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.training.utils.detection_utils import get_cls_posx_in_target
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.transforms.transforms import DetectionTransform, DetectionTargetsFormatTransform, DetectionTargetsFormat
-from super_gradients.training.exceptions.dataset_exceptions import EmptyDatasetException, DatasetValidationException
+from super_gradients.common.exceptions.dataset_exceptions import EmptyDatasetException, DatasetValidationException
 from super_gradients.common.factories.list_factory import ListFactory
 from super_gradients.common.factories.transforms_factory import TransformsFactory
 from super_gradients.training.datasets.data_formats.default_formats import XYXY_LABEL
 from super_gradients.training.datasets.data_formats.formats import ConcatenatedTensorFormat
 from super_gradients.training.utils.utils import ensure_is_tuple_of_two
 
 logger = get_logger(__name__)
```

## super_gradients/training/datasets/detection_datasets/yolo_format_detection.py

```diff
@@ -224,15 +224,15 @@
         """
         with open(label_file_path, "r") as f:
             lines = f.readlines()
 
         labels_yolo_format, invalid_labels = [], []
         for line in filter(lambda x: x != "\n", lines):
             try:
-                label_id, cx, cw, w, h = line.split(" ")
+                label_id, cx, cw, w, h = line.split()
                 labels_yolo_format.append([int(label_id), float(cx), float(cw), float(w), float(h)])
             except Exception as e:
                 if ignore_invalid_labels:
                     invalid_labels.append(line)
                     if show_warnings:
                         logger.warning(f"Line `{line}` of file {label_file_path} will be ignored because not in LABEL_NORMALIZED_CXCYWH format: {e}")
                 else:
```

## super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py

```diff
@@ -1,18 +1,20 @@
 import abc
-from typing import Tuple, List, Mapping, Any, Dict
+from typing import Tuple, List, Mapping, Any, Dict, Union
 
 import numpy as np
 import torch
 from torch.utils.data.dataloader import default_collate, Dataset
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
+from super_gradients.common.object_names import Processings
 from super_gradients.common.registry.registry import register_collate_function
 from super_gradients.training.datasets.pose_estimation_datasets.target_generators import KeypointsTargetsGenerator
 from super_gradients.training.transforms.keypoint_transforms import KeypointsCompose, KeypointTransform
+from super_gradients.training.utils.visualization.utils import generate_color_mapping
 
 logger = get_logger(__name__)
 
 
 class BaseKeypointsDataset(Dataset):
     """
     Base class for pose estimation datasets.
@@ -20,26 +22,38 @@
     """
 
     def __init__(
         self,
         target_generator: KeypointsTargetsGenerator,
         transforms: List[KeypointTransform],
         min_instance_area: float,
+        num_joints: int,
+        edge_links: Union[List[Tuple[int, int]], np.ndarray],
+        edge_colors: Union[List[Tuple[int, int, int]], np.ndarray, None],
+        keypoint_colors: Union[List[Tuple[int, int, int]], np.ndarray, None],
     ):
         """
 
         :param target_generator: Target generator that will be used to generate the targets for the model.
             See DEKRTargetsGenerator for an example.
         :param transforms: Transforms to be applied to the image & keypoints
         :param min_instance_area: Minimum area of an instance to be included in the dataset
+        :param num_joints: Number of joints to be predicted
+        :param edge_links: Edge links between joints
+        :param edge_colors: Color of the edge links. If None, the color will be generated randomly.
+        :param keypoint_colors: Color of the keypoints. If None, the color will be generated randomly.
         """
         super().__init__()
         self.target_generator = target_generator
         self.transforms = KeypointsCompose(transforms)
         self.min_instance_area = min_instance_area
+        self.num_joints = num_joints
+        self.edge_links = edge_links
+        self.edge_colors = edge_colors or generate_color_mapping(len(edge_links))
+        self.keypoint_colors = keypoint_colors or generate_color_mapping(num_joints)
 
     @abc.abstractmethod
     def __len__(self) -> int:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def load_sample(self, index) -> Tuple[np.ndarray, np.ndarray, np.ndarray, Dict[str, Any]]:
@@ -91,14 +105,29 @@
 
         # Remove instances with too small area
         areas = self.compute_area(joints)
         joints = joints[areas > self.min_instance_area]
 
         return joints
 
+    def get_dataset_preprocessing_params(self):
+        """
+
+        :return:
+        """
+        pipeline = self.transforms.get_equivalent_preprocessing()
+        params = dict(
+            conf=0.25,
+            image_processor={Processings.ComposeProcessing: {"processings": pipeline}},
+            edge_links=self.edge_links,
+            edge_colors=self.edge_colors,
+            keypoint_colors=self.keypoint_colors,
+        )
+        return params
+
 
 @register_collate_function()
 class KeypointsCollate:
     """
     Collate image & targets, return extras as is.
     """
```

## super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py

```diff
@@ -1,18 +1,18 @@
 import os
-from typing import Tuple, List, Mapping, Any
+from typing import Tuple, List, Mapping, Any, Union
 
 import cv2
 import numpy as np
 import pycocotools
 from pycocotools.coco import COCO
 from torch import Tensor
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
-from super_gradients.common.object_names import Datasets
+from super_gradients.common.object_names import Datasets, Processings
 from super_gradients.common.registry.registry import register_dataset
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.target_generator_factory import TargetGeneratorsFactory
 from super_gradients.common.factories.transforms_factory import TransformsFactory
 from super_gradients.training.datasets.pose_estimation_datasets.base_keypoints import BaseKeypointsDataset
 from super_gradients.training.transforms.keypoint_transforms import KeypointTransform
 
@@ -33,40 +33,55 @@
         data_dir: str,
         images_dir: str,
         json_file: str,
         include_empty_samples: bool,
         target_generator,
         transforms: List[KeypointTransform],
         min_instance_area: float,
+        edge_links: Union[List[Tuple[int, int]], np.ndarray],
+        edge_colors: Union[List[Tuple[int, int, int]], np.ndarray, None],
+        keypoint_colors: Union[List[Tuple[int, int, int]], np.ndarray, None],
     ):
         """
 
         :param data_dir: Root directory of the COCO dataset
         :param images_dir: path suffix to the images directory inside the dataset_root
         :param json_file: path suffix to the json file inside the dataset_root
         :param include_empty_samples: if True, images without any annotations will be included in the dataset.
             Otherwise, they will be filtered out.
         :param target_generator: Target generator that will be used to generate the targets for the model.
             See DEKRTargetsGenerator for an example.
         :param transforms: Transforms to be applied to the image & keypoints
         :param min_instance_area: Minimum area of an instance to be included in the dataset
+        :param edge_links: Edge links between joints
+        :param edge_colors: Color of the edge links. If None, the color will be generated randomly.
+        :param keypoint_colors: Color of the keypoints. If None, the color will be generated randomly.
         """
-        super().__init__(transforms=transforms, target_generator=target_generator, min_instance_area=min_instance_area)
-        self.root = data_dir
-        self.images_dir = os.path.join(data_dir, images_dir)
-        self.json_file = os.path.join(data_dir, json_file)
 
-        coco = COCO(self.json_file)
+        json_file = os.path.join(data_dir, json_file)
+        coco = COCO(json_file)
         if len(coco.dataset["categories"]) != 1:
             raise ValueError("Dataset must contain exactly one category")
+        joints = coco.dataset["categories"][0]["keypoints"]
+        num_joints = len(joints)
 
+        super().__init__(
+            transforms=transforms,
+            target_generator=target_generator,
+            min_instance_area=min_instance_area,
+            num_joints=num_joints,
+            edge_links=edge_links,
+            edge_colors=edge_colors,
+            keypoint_colors=keypoint_colors,
+        )
+        self.root = data_dir
+        self.images_dir = os.path.join(data_dir, images_dir)
         self.coco = coco
         self.ids = list(self.coco.imgs.keys())
-        self.joints = coco.dataset["categories"][0]["keypoints"]
-        self.num_joints = len(self.joints)
+        self.joints = joints
 
         if not include_empty_samples:
             subset = [img_id for img_id in self.ids if len(self.coco.getAnnIds(imgIds=img_id, iscrowd=None)) > 0]
             self.ids = subset
 
     def __len__(self):
         return len(self.ids)
@@ -186,7 +201,25 @@
                     if mask.shape != m.shape:
                         logger.warning(f"Mask shape {mask.shape} does not match image shape {m.shape} for image {img_info['file_name']}")
                         continue
 
                     m += mask
 
         return (m < 0.5).astype(np.float32)
+
+    def get_dataset_preprocessing_params(self):
+        """
+
+        :return:
+        """
+        # Since we are using cv2.imread to read images, our model in fact is trained on BGR images.
+        # In our pipelines the convention that input images are RGB, so we need to reverse the channels to get BGR
+        # to match with the expected input of the model.
+        pipeline = [Processings.ReverseImageChannels] + self.transforms.get_equivalent_preprocessing()
+        params = dict(
+            conf=0.25,
+            image_processor={Processings.ComposeProcessing: {"processings": pipeline}},
+            edge_links=self.edge_links,
+            edge_colors=self.edge_colors,
+            keypoint_colors=self.keypoint_colors,
+        )
+        return params
```

## super_gradients/training/kd_trainer/kd_trainer.py

```diff
@@ -5,15 +5,15 @@
 from omegaconf import DictConfig, OmegaConf
 from torch.utils.data import DataLoader
 
 from super_gradients.common import MultiGPUMode, StrictLoad
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training import utils as core_utils, models
 from super_gradients.training.dataloaders import dataloaders
-from super_gradients.training.exceptions.kd_trainer_exceptions import (
+from super_gradients.common.exceptions.kd_trainer_exceptions import (
     ArchitectureKwargsException,
     UnsupportedKDArchitectureException,
     InconsistentParamsException,
     UnsupportedKDModelArgException,
     TeacherKnowledgeException,
     UndefinedNumClassesException,
 )
@@ -23,14 +23,15 @@
 from super_gradients.training.pretrained_models import PRETRAINED_NUM_CLASSES
 from super_gradients.training.sg_trainer import Trainer
 from super_gradients.training.utils import get_param, HpmStruct
 from super_gradients.training.utils.callbacks import KDModelMetricsUpdateCallback
 from super_gradients.training.utils.checkpoint_utils import read_ckpt_state_dict, load_checkpoint_to_model
 from super_gradients.training.utils.distributed_training_utils import setup_device
 from super_gradients.training.utils.ema import KDModelEMA
+from super_gradients.training.utils.utils import unwrap_model
 
 logger = get_logger(__name__)
 
 
 class KDTrainer(Trainer):
     def __init__(self, experiment_name: str, device: str = None, multi_gpu: Union[MultiGPUMode, str] = None, ckpt_root_dir: str = None):
         super().__init__(experiment_name=experiment_name, device=device, multi_gpu=multi_gpu, ckpt_root_dir=ckpt_root_dir)
@@ -207,15 +208,15 @@
 
     def _load_checkpoint_to_model(self):
         """
         Initializes teacher weights with teacher_checkpoint_path if needed, then handles checkpoint loading for
          the entire KD network following the same logic as in Trainer.
         """
         teacher_checkpoint_path = get_param(self.checkpoint_params, "teacher_checkpoint_path")
-        teacher_net = self.net.module.teacher
+        teacher_net = unwrap_model(self.net).teacher
 
         if teacher_checkpoint_path is not None:
 
             #  WARN THAT TEACHER_CKPT WILL OVERRIDE TEACHER'S PRETRAINED WEIGHTS
             teacher_pretrained_weights = get_param(self.checkpoint_params, "teacher_pretrained_weights")
             if teacher_pretrained_weights:
                 logger.warning(teacher_checkpoint_path + " checkpoint is " "overriding " + teacher_pretrained_weights + " for teacher model")
@@ -267,20 +268,20 @@
         return KDModelEMA.from_params(self.net, **ema_params)
 
     def _save_best_checkpoint(self, epoch, state):
         """
         Overrides parent best_ckpt saving to modify the state dict so that we only save the student.
         """
         if self.ema:
-            best_net = core_utils.WrappedModel(self.ema_model.ema.module.student)
+            best_net = self.ema_model.ema.student
             state.pop("ema_net")
         else:
-            best_net = core_utils.WrappedModel(self.net.module.student)
+            best_net = self.net.student
 
-        state["net"] = best_net.state_dict()
+        state["net"] = unwrap_model(best_net).state_dict()
         self.sg_logger.add_checkpoint(tag=self.ckpt_best_name, state_dict=state, global_step=epoch)
 
     def train(
         self,
         model: KDModule = None,
         training_params: Dict = None,
         student: SgModule = None,
```

## super_gradients/training/losses/ohem_ce_loss.py

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import nn
 from torch.nn.modules.loss import _Loss
-from super_gradients.training.exceptions.loss_exceptions import IllegalRangeForLossAttributeException, RequiredLossComponentReductionException
+from super_gradients.common.exceptions.loss_exceptions import IllegalRangeForLossAttributeException, RequiredLossComponentReductionException
 
 
 class OhemLoss(_Loss):
     """
     OhemLoss - Online Hard Example Mining Cross Entropy Loss
     """
```

## super_gradients/training/metrics/detection_metrics.py

```diff
@@ -1,8 +1,11 @@
-from typing import Dict, Optional, Union
+import collections
+from typing import Dict, Optional, Union, Tuple, List
+
+import numpy as np
 import torch
 from torchmetrics import Metric
 
 import super_gradients
 from super_gradients.common.object_names import Metrics
 from super_gradients.common.registry.registry import register_metric
 from super_gradients.training.utils import tensor_container_to_device
@@ -20,51 +23,102 @@
 
     Metric class for computing F1, Precision, Recall and Mean Average Precision.
 
     :param num_cls:                         Number of classes.
     :param post_prediction_callback:        DetectionPostPredictionCallback to be applied on net's output prior to the metric computation (NMS).
     :param normalize_targets:               Whether to normalize bbox coordinates by image size.
     :param iou_thres:                       IoU threshold to compute the mAP.
+                                            Could be either instance of IouThreshold, a tuple (lower bound, upper_bound) or single scalar.
     :param recall_thres:                    Recall threshold to compute the mAP.
     :param score_thres:                     Score threshold to compute Recall, Precision and F1.
     :param top_k_predictions:               Number of predictions per class used to compute metrics, ordered by confidence score
     :param dist_sync_on_step:               Synchronize metric state across processes at each ``forward()`` before returning the value at the step.
     :param accumulate_on_cpu:               Run on CPU regardless of device used in other parts.
                                             This is to avoid "CUDA out of memory" that might happen on GPU.
+    :param calc_best_score_thresholds       Whether to calculate the best score threshold overall and per class
+                                            If True, the compute() function will return a metrics dictionary that not
+                                            only includes the average metrics calculated across all classes,
+                                            but also the optimal score threshold overall and for each individual class.
+    :param include_classwise_ap:            Whether to include the class-wise average precision in the returned metrics dictionary.
+                                            If enabled, output metrics dictionary will look similar to this:
+                                            {
+                                                'Precision0.5:0.95': 0.5,
+                                                'Recall0.5:0.95': 0.5,
+                                                'F10.5:0.95': 0.5,
+                                                'mAP0.5:0.95': 0.5,
+                                                'AP0.5:0.95_person': 0.5,
+                                                'AP0.5:0.95_car': 0.5,
+                                                'AP0.5:0.95_bicycle': 0.5,
+                                                'AP0.5:0.95_motorcycle': 0.5,
+                                                ...
+                                            }
+                                            Class names are either provided via the class_names parameter or are generated automatically.
+    :param class_names:                     Array of class names. When include_classwise_ap=True, will use these names to make
+                                            per-class APs keys in the output metrics dictionary.
+                                            If None, will use dummy names `class_{idx}` instead.
     """
 
     def __init__(
         self,
         num_cls: int,
         post_prediction_callback: DetectionPostPredictionCallback,
         normalize_targets: bool = False,
-        iou_thres: Union[IouThreshold, float] = IouThreshold.MAP_05_TO_095,
+        iou_thres: Union[IouThreshold, Tuple[float, float], float] = IouThreshold.MAP_05_TO_095,
         recall_thres: torch.Tensor = None,
         score_thres: float = 0.1,
         top_k_predictions: int = 100,
         dist_sync_on_step: bool = False,
         accumulate_on_cpu: bool = True,
+        calc_best_score_thresholds: bool = False,
+        include_classwise_ap: bool = False,
+        class_names: List[str] = None,
     ):
+        if class_names is None and include_classwise_ap:
+            logger.warning(
+                "Parameter 'include_classwise_ap' is set to True, but no class names are provided. "
+                "We will generate dummy class names, but we recommend to provide class names explicitly to"
+                "have meaningful names in reported metrics."
+            )
+            class_names = ["class_" + str(i) for i in range(num_cls)]
+
+        if class_names is not None and len(class_names) != num_cls:
+            raise ValueError(f"Number of class names ({len(class_names)}) does not match number of classes ({num_cls})")
+
         super().__init__(dist_sync_on_step=dist_sync_on_step)
         self.num_cls = num_cls
         self.iou_thres = iou_thres
 
         if isinstance(iou_thres, IouThreshold):
             self.iou_thresholds = iou_thres.to_tensor()
+        if isinstance(iou_thres, tuple):
+            low, high = iou_thres
+            self.iou_thresholds = IouThreshold.from_bounds(low, high)
         else:
             self.iou_thresholds = torch.tensor([iou_thres])
 
         self.map_str = "mAP" + self._get_range_str()
-        self.greater_component_is_better = {
-            f"Precision{self._get_range_str()}": True,
-            f"Recall{self._get_range_str()}": True,
-            f"mAP{self._get_range_str()}": True,
-            f"F1{self._get_range_str()}": True,
-        }
+        self.include_classwise_ap = include_classwise_ap
+
+        greater_component_is_better = [
+            (f"Precision{self._get_range_str()}", True),
+            (f"Recall{self._get_range_str()}", True),
+            (f"mAP{self._get_range_str()}", True),
+            (f"F1{self._get_range_str()}", True),
+        ]
+
+        if self.include_classwise_ap:
+            self.per_class_ap_names = [f"AP{self._get_range_str()}_{class_name}" for class_name in class_names]
+            greater_component_is_better += [(key, True) for key in self.per_class_ap_names]
+
+        self.greater_component_is_better = collections.OrderedDict(greater_component_is_better)
         self.component_names = list(self.greater_component_is_better.keys())
+        self.calc_best_score_thresholds = calc_best_score_thresholds
+        if self.calc_best_score_thresholds:
+            self.component_names.append("Best_score_threshold")
+            self.component_names += [f"Best_score_threshold_cls_{i}" for i in range(self.num_cls)]
         self.components = len(self.component_names)
 
         self.post_prediction_callback = post_prediction_callback
         self.is_distributed = super_gradients.is_distributed()
         self.denormalize_targets = not normalize_targets
         self.world_size = None
         self.rank = None
@@ -111,42 +165,58 @@
         accumulated_matching_info = getattr(self, f"matching_info{self._get_range_str()}")
         setattr(self, f"matching_info{self._get_range_str()}", accumulated_matching_info + new_matching_info)
 
     def compute(self) -> Dict[str, Union[float, torch.Tensor]]:
         """Compute the metrics for all the accumulated results.
         :return: Metrics of interest
         """
-        mean_ap, mean_precision, mean_recall, mean_f1 = -1.0, -1.0, -1.0, -1.0
+        mean_ap, mean_precision, mean_recall, mean_f1, best_score_threshold, best_score_threshold_per_cls = -1.0, -1.0, -1.0, -1.0, -1.0, None
         accumulated_matching_info = getattr(self, f"matching_info{self._get_range_str()}")
+        mean_ap_per_class = np.zeros(self.num_cls)
 
         if len(accumulated_matching_info):
             matching_info_tensors = [torch.cat(x, 0) for x in list(zip(*accumulated_matching_info))]
 
             # shape (n_class, nb_iou_thresh)
-            ap, precision, recall, f1, unique_classes = compute_detection_metrics(
+            ap, precision, recall, f1, unique_classes, best_score_threshold, best_score_threshold_per_cls = compute_detection_metrics(
                 *matching_info_tensors,
                 recall_thresholds=self.recall_thresholds,
                 score_threshold=self.score_threshold,
                 device="cpu" if self.accumulate_on_cpu else self.device,
+                calc_best_score_thresholds=self.calc_best_score_thresholds,
             )
 
             # Precision, recall and f1 are computed for IoU threshold range, averaged over classes
             # results before version 3.0.4 (Dec 11 2022) were computed only for smallest value (i.e IoU 0.5 if metric is @0.5:0.95)
             mean_precision, mean_recall, mean_f1 = precision.mean(), recall.mean(), f1.mean()
 
             # MaP is averaged over IoU thresholds and over classes
             mean_ap = ap.mean()
 
-        return {
+            # Fill array of per-class AP scores with values for classes that were present in the dataset
+            ap_per_class = ap.mean(1)
+            for i, class_index in enumerate(unique_classes):
+                mean_ap_per_class[class_index] = float(ap_per_class[i])
+
+        output_dict = {
             f"Precision{self._get_range_str()}": mean_precision,
             f"Recall{self._get_range_str()}": mean_recall,
             f"mAP{self._get_range_str()}": mean_ap,
             f"F1{self._get_range_str()}": mean_f1,
         }
 
+        if self.include_classwise_ap:
+            for i, ap_i in enumerate(mean_ap_per_class):
+                output_dict[self.per_class_ap_names[i]] = float(ap_i)
+
+        if self.calc_best_score_thresholds:
+            output_dict["Best_score_threshold"] = best_score_threshold
+            output_dict.update(best_score_threshold_per_cls)
+        return output_dict
+
     def _sync_dist(self, dist_sync_fn=None, process_group=None):
         """
         When in distributed mode, stats are aggregated after each forward pass to the metric state. Since these have all
         different sizes we override the synchronization function since it works only for tensors (and use
         all_gather_object)
         :param dist_sync_fn:
         :return:
@@ -180,26 +250,32 @@
         post_prediction_callback: DetectionPostPredictionCallback = None,
         normalize_targets: bool = False,
         recall_thres: torch.Tensor = None,
         score_thres: float = 0.1,
         top_k_predictions: int = 100,
         dist_sync_on_step: bool = False,
         accumulate_on_cpu: bool = True,
+        calc_best_score_thresholds: bool = False,
+        include_classwise_ap: bool = False,
+        class_names: List[str] = None,
     ):
 
         super().__init__(
-            num_cls,
-            post_prediction_callback,
-            normalize_targets,
-            IouThreshold.MAP_05,
-            recall_thres,
-            score_thres,
-            top_k_predictions,
-            dist_sync_on_step,
-            accumulate_on_cpu,
+            num_cls=num_cls,
+            post_prediction_callback=post_prediction_callback,
+            normalize_targets=normalize_targets,
+            iou_thres=IouThreshold.MAP_05,
+            recall_thres=recall_thres,
+            score_thres=score_thres,
+            top_k_predictions=top_k_predictions,
+            dist_sync_on_step=dist_sync_on_step,
+            accumulate_on_cpu=accumulate_on_cpu,
+            calc_best_score_thresholds=calc_best_score_thresholds,
+            include_classwise_ap=include_classwise_ap,
+            class_names=class_names,
         )
 
 
 @register_metric(Metrics.DETECTION_METRICS_075)
 class DetectionMetrics_075(DetectionMetrics):
     def __init__(
         self,
@@ -207,18 +283,32 @@
         post_prediction_callback: DetectionPostPredictionCallback = None,
         normalize_targets: bool = False,
         recall_thres: torch.Tensor = None,
         score_thres: float = 0.1,
         top_k_predictions: int = 100,
         dist_sync_on_step: bool = False,
         accumulate_on_cpu: bool = True,
+        calc_best_score_thresholds: bool = False,
+        include_classwise_ap: bool = False,
+        class_names: List[str] = None,
     ):
 
         super().__init__(
-            num_cls, post_prediction_callback, normalize_targets, 0.75, recall_thres, score_thres, top_k_predictions, dist_sync_on_step, accumulate_on_cpu
+            num_cls=num_cls,
+            post_prediction_callback=post_prediction_callback,
+            normalize_targets=normalize_targets,
+            iou_thres=0.75,
+            recall_thres=recall_thres,
+            score_thres=score_thres,
+            top_k_predictions=top_k_predictions,
+            dist_sync_on_step=dist_sync_on_step,
+            accumulate_on_cpu=accumulate_on_cpu,
+            calc_best_score_thresholds=calc_best_score_thresholds,
+            include_classwise_ap=include_classwise_ap,
+            class_names=class_names,
         )
 
 
 @register_metric(Metrics.DETECTION_METRICS_050_095)
 class DetectionMetrics_050_095(DetectionMetrics):
     def __init__(
         self,
@@ -226,20 +316,26 @@
         post_prediction_callback: DetectionPostPredictionCallback = None,
         normalize_targets: bool = False,
         recall_thres: torch.Tensor = None,
         score_thres: float = 0.1,
         top_k_predictions: int = 100,
         dist_sync_on_step: bool = False,
         accumulate_on_cpu: bool = True,
+        calc_best_score_thresholds: bool = False,
+        include_classwise_ap: bool = False,
+        class_names: List[str] = None,
     ):
 
         super().__init__(
-            num_cls,
-            post_prediction_callback,
-            normalize_targets,
-            IouThreshold.MAP_05_TO_095,
-            recall_thres,
-            score_thres,
-            top_k_predictions,
-            dist_sync_on_step,
-            accumulate_on_cpu,
+            num_cls=num_cls,
+            post_prediction_callback=post_prediction_callback,
+            normalize_targets=normalize_targets,
+            iou_thres=IouThreshold.MAP_05_TO_095,
+            recall_thres=recall_thres,
+            score_thres=score_thres,
+            top_k_predictions=top_k_predictions,
+            dist_sync_on_step=dist_sync_on_step,
+            accumulate_on_cpu=accumulate_on_cpu,
+            calc_best_score_thresholds=calc_best_score_thresholds,
+            include_classwise_ap=include_classwise_ap,
+            class_names=class_names,
         )
```

## super_gradients/training/metrics/pose_estimation_metrics.py

```diff
@@ -99,15 +99,22 @@
             self.stats_names += [f"AR_{t:.2f}" for t in self.iou_thresholds_to_report]
         else:
             self.iou_thresholds_to_report = None
 
         self.greater_component_is_better = dict((k, True) for k in self.stats_names)
 
         if oks_sigmas is None:
-            oks_sigmas = np.array([0.26, 0.25, 0.25, 0.35, 0.35, 0.79, 0.79, 0.72, 0.72, 0.62, 0.62, 1.07, 1.07, 0.87, 0.87, 0.89, 0.89]) / 10.0
+            if num_joints == 17:
+                oks_sigmas = np.array([0.26, 0.25, 0.25, 0.35, 0.35, 0.79, 0.79, 0.72, 0.72, 0.62, 0.62, 1.07, 1.07, 0.87, 0.87, 0.89, 0.89]) / 10.0
+            else:
+                oks_sigmas = np.array([0.1] * num_joints)
+                logger.warning(
+                    f"Using default OKS sigmas of `0.1` for a custom dataset with {num_joints} joints. "
+                    f"To silence this warning, you may want to specify OKS sigmas explicitly as it has direct impact on the AP score."
+                )
 
         if len(oks_sigmas) != num_joints:
             raise ValueError(f"Length of oks_sigmas ({len(oks_sigmas)}) should be equal to num_joints {num_joints}")
 
         self.oks_sigmas = torch.tensor(oks_sigmas).float()
 
         self.component_names = list(self.greater_component_is_better.keys())
@@ -274,15 +281,15 @@
         predictions = self.predictions  # All gathered by this time
         if len(predictions) > 0:
             preds_matched = torch.cat([x[0].cpu() for x in predictions], dim=0)
             preds_to_ignore = torch.cat([x[1].cpu() for x in predictions], dim=0)
             preds_scores = torch.cat([x[2].cpu() for x in predictions], dim=0)
             n_targets = sum([x[3] for x in predictions])
 
-            cls_precision, _, cls_recall = compute_detection_metrics_per_cls(
+            cls_precision, _, cls_recall, _, _ = compute_detection_metrics_per_cls(
                 preds_matched=preds_matched,
                 preds_to_ignore=preds_to_ignore,
                 preds_scores=preds_scores,
                 n_targets=n_targets,
                 recall_thresholds=self.recall_thresholds.cpu(),
                 score_threshold=0,
                 device="cpu",
```

## super_gradients/training/metrics/segmentation_metrics.py

```diff
@@ -1,12 +1,14 @@
+import typing
+
 import numpy as np
 import torch
 import torchmetrics
 from torchmetrics import Metric
-from typing import Optional, Tuple
+from typing import Optional, Tuple, List, Union
 from torchmetrics.utilities.distributed import reduce
 from abc import ABC, abstractmethod
 
 
 from super_gradients.common.object_names import Metrics
 from super_gradients.common.registry.registry import register_metric
 
@@ -118,14 +120,43 @@
     # Compute area union:
     area_pred, _ = np.histogram(im_pred, bins=num_class - 1, range=(1, num_class - 1))
     area_lab, _ = np.histogram(im_lab, bins=num_class - 1, range=(1, num_class - 1))
     area_union = area_pred + area_lab - area_inter
     return area_inter, area_union
 
 
+def _map_ignored_inds(target: torch.Tensor, ignore_index_list: List[int], unfiltered_num_classes: int) -> torch.Tensor:
+    """
+    Creaetes a copy of target, mapping indices in range(unfiltered_num_classes) to range(unfiltered_num_classes-len(
+    ignore_index_list)+1). Indices in ignore_index_list are being mapped to 0, which can later on be used as
+     "ignore_index".
+
+     Example:
+        >>>_map_ignored_inds(torch.tensor([0,1,2,3,4,5,6]), ignore_index_list=[3,5,1], unfiltered_num_classes=7)
+        >>> tensor([1, 0, 2, 0, 3, 0, 4])
+
+
+
+    :param target: torch.Tensor, tensor to perform the mapping on.
+    :param ignore_index_list: List[int], list of indices to map to 0 in the output tensor.
+    :param unfiltered_num_classes: int, Total number of possible class indices in target.
+
+    :return: mapped tensor as described above.
+    """
+    target_copy = torch.zeros_like(target)
+    all_unfiltered_classes = list(range(unfiltered_num_classes))
+    filtered_classes = [i for i in all_unfiltered_classes if i not in ignore_index_list]
+    for mapped_idx in range(len(filtered_classes)):
+        cls_to_map = filtered_classes[mapped_idx]
+        map_val = mapped_idx + 1
+        target_copy[target == cls_to_map] = map_val
+
+    return target_copy
+
+
 class AbstractMetricsArgsPrepFn(ABC):
     """
     Abstract preprocess metrics arguments class.
     """
 
     @abstractmethod
     def __call__(self, preds, target: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
@@ -160,83 +191,200 @@
 
         target = target.long()
         return preds, target
 
 
 @register_metric(Metrics.PIXEL_ACCURACY)
 class PixelAccuracy(Metric):
-    def __init__(self, ignore_label=-100, dist_sync_on_step=False, metrics_args_prep_fn: Optional[AbstractMetricsArgsPrepFn] = None):
+    """
+    Pixel Accuracy
+
+    Args:
+        ignore_label: Optional[Union[int, List[int]]], specifying a target class(es) to ignore.
+            If given, this class index does not contribute to the returned score, regardless of reduction method.
+            Has no effect if given an int that is not in the range [0, num_classes-1].
+            By default, no index is ignored, and all classes are used.
+            IMPORTANT: reduction="none" alongside with a list of ignored indices is not supported and will raise an error.
+        reduction: a method to reduce metric score over labels:
+
+            - ``'elementwise_mean'``: takes the mean (default)
+            - ``'sum'``: takes the sum
+            - ``'none'``: no reduction will be applied
+
+        metrics_args_prep_fn: Callable, inputs preprocess function applied on preds, target before updating metrics.
+            By default set to PreprocessSegmentationMetricsArgs(apply_arg_max=True)
+    """
+
+    def __init__(self, ignore_label: Union[int, List[int]] = -100, dist_sync_on_step=False, metrics_args_prep_fn: Optional[AbstractMetricsArgsPrepFn] = None):
         super().__init__(dist_sync_on_step=dist_sync_on_step)
         self.ignore_label = ignore_label
         self.greater_is_better = True
         self.add_state("total_correct", default=torch.tensor(0.0), dist_reduce_fx="sum")
         self.add_state("total_label", default=torch.tensor(0.0), dist_reduce_fx="sum")
         self.metrics_args_prep_fn = metrics_args_prep_fn or PreprocessSegmentationMetricsArgs(apply_arg_max=True)
 
     def update(self, preds: torch.Tensor, target: torch.Tensor):
         predict, target = self.metrics_args_prep_fn(preds, target)
+        labeled_mask = self._handle_multiple_ignored_inds(target)
 
-        labeled_mask = target.ne(self.ignore_label)
         pixel_labeled = torch.sum(labeled_mask)
         pixel_correct = torch.sum((predict == target) * labeled_mask)
         self.total_correct += pixel_correct
         self.total_label += pixel_labeled
 
+    def _handle_multiple_ignored_inds(self, target):
+        if isinstance(self.ignore_label, typing.Iterable):
+            evaluated_classes_mask = torch.ones_like(target)
+            for ignored_label in self.ignore_label:
+                evaluated_classes_mask = evaluated_classes_mask.masked_fill(target.eq(ignored_label), 0)
+        else:
+            evaluated_classes_mask = target.ne(self.ignore_label)
+
+        return evaluated_classes_mask
+
     def compute(self):
         _total_correct = self.total_correct.cpu().detach().numpy().astype("int64")
         _total_label = self.total_label.cpu().detach().numpy().astype("int64")
         pix_acc = np.float64(1.0) * _total_correct / (np.spacing(1, dtype=np.float64) + _total_label)
         return pix_acc
 
 
+def _handle_multiple_ignored_inds(ignore_index: Union[int, List[int]], num_classes: int):
+    """
+    Helper method for variable assignment, prior to the
+
+    super().__init__(num_classes=num_classes, dist_sync_on_step=dist_sync_on_step, ignore_index=ignore_index, reduction=reduction, threshold=threshold)
+
+    call in segmentation metrics inheriting from torchmetrics.JaccardIndex.
+    When ignore_index is list, the num_classes being passed to the torchmetrics.JaccardIndex c'tor is set to be the one after
+     mapping of the ignored indices in ignore_index_list to 0. Hence, we set:
+      ignore_index=0,
+    And since we map all of the ignored indices to 0, it is if we removed them and introduces a new index:
+      num_classes = num_classes - len(ignore_index_list) +1
+    Unfiltered num_classes is used in .update() for mapping of the original indice values.
+    Sets ignore_index to 0
+    :param ignore_index: list or single int representing the class ind(ices) to ignore.
+    :param num_classes: int, num_classes (original, before mapping) being passed to segmentation metric classesץ
+    :return:ignore_index, ignore_index_list, num_classes, unfiltered_num_classesignore_index, ignore_index_list, num_classes, unfiltered_num_classes
+    """
+    if isinstance(ignore_index, typing.Iterable):
+        ignore_index_list = ignore_index
+        unfiltered_num_classes = num_classes
+        num_classes = num_classes - len(ignore_index_list) + 1
+        ignore_index = 0
+    else:
+        unfiltered_num_classes = num_classes
+        ignore_index_list = None
+    return ignore_index, ignore_index_list, num_classes, unfiltered_num_classes
+
+
 @register_metric(Metrics.IOU)
 class IoU(torchmetrics.JaccardIndex):
+    """
+    IoU Metric
+
+    Args:
+        num_classes: Number of classes in the dataset.
+        ignore_index: Optional[Union[int, List[int]]], specifying a target class(es) to ignore.
+            If given, this class index does not contribute to the returned score, regardless of reduction method.
+            Has no effect if given an int that is not in the range [0, num_classes-1].
+            By default, no index is ignored, and all classes are used.
+            IMPORTANT: reduction="none" alongside with a list of ignored indices is not supported and will raise an error.
+        threshold: Threshold value for binary or multi-label probabilities.
+        reduction: a method to reduce metric score over labels:
+
+            - ``'elementwise_mean'``: takes the mean (default)
+            - ``'sum'``: takes the sum
+            - ``'none'``: no reduction will be applied
+
+        metrics_args_prep_fn: Callable, inputs preprocess function applied on preds, target before updating metrics.
+            By default set to PreprocessSegmentationMetricsArgs(apply_arg_max=True)
+    """
+
     def __init__(
         self,
         num_classes: int,
         dist_sync_on_step: bool = False,
-        ignore_index: Optional[int] = None,
+        ignore_index: Optional[Union[int, List[int]]] = None,
         reduction: str = "elementwise_mean",
         threshold: float = 0.5,
         metrics_args_prep_fn: Optional[AbstractMetricsArgsPrepFn] = None,
     ):
 
         if num_classes <= 1:
             raise ValueError(f"IoU class only for multi-class usage! For binary usage, please call {BinaryIOU.__name__}")
+        if isinstance(ignore_index, typing.Iterable) and reduction == "none":
+            raise ValueError("passing multiple ignore indices ")
+        ignore_index, ignore_index_list, num_classes, unfiltered_num_classes = _handle_multiple_ignored_inds(ignore_index, num_classes)
 
         super().__init__(num_classes=num_classes, dist_sync_on_step=dist_sync_on_step, ignore_index=ignore_index, reduction=reduction, threshold=threshold)
+
+        self.unfiltered_num_classes = unfiltered_num_classes
+        self.ignore_index_list = ignore_index_list
         self.metrics_args_prep_fn = metrics_args_prep_fn or PreprocessSegmentationMetricsArgs(apply_arg_max=True)
         self.greater_is_better = True
 
     def update(self, preds, target: torch.Tensor):
         preds, target = self.metrics_args_prep_fn(preds, target)
+        if self.ignore_index_list is not None:
+            target = _map_ignored_inds(target, self.ignore_index_list, self.unfiltered_num_classes)
+            preds = _map_ignored_inds(preds, self.ignore_index_list, self.unfiltered_num_classes)
         super().update(preds=preds, target=target)
 
 
 @register_metric(Metrics.DICE)
 class Dice(torchmetrics.JaccardIndex):
+    """
+    Dice Coefficient Metric
+
+    Args:
+        num_classes: Number of classes in the dataset.
+        ignore_index: Optional[Union[int, List[int]]], specifying a target class(es) to ignore.
+            If given, this class index does not contribute to the returned score, regardless of reduction method.
+            Has no effect if given an int that is not in the range [0, num_classes-1].
+            By default, no index is ignored, and all classes are used.
+            IMPORTANT: reduction="none" alongside with a list of ignored indices is not supported and will raise an error.
+        threshold: Threshold value for binary or multi-label probabilities.
+        reduction: a method to reduce metric score over labels:
+
+            - ``'elementwise_mean'``: takes the mean (default)
+            - ``'sum'``: takes the sum
+            - ``'none'``: no reduction will be applied
+
+        metrics_args_prep_fn: Callable, inputs preprocess function applied on preds, target before updating metrics.
+            By default set to PreprocessSegmentationMetricsArgs(apply_arg_max=True)
+    """
+
     def __init__(
         self,
         num_classes: int,
         dist_sync_on_step: bool = False,
         ignore_index: Optional[int] = None,
         reduction: str = "elementwise_mean",
         threshold: float = 0.5,
         metrics_args_prep_fn: Optional[AbstractMetricsArgsPrepFn] = None,
     ):
 
         if num_classes <= 1:
             raise ValueError(f"Dice class only for multi-class usage! For binary usage, please call {BinaryDice.__name__}")
 
+        ignore_index, ignore_index_list, num_classes, unfiltered_num_classes = _handle_multiple_ignored_inds(ignore_index, num_classes)
+
         super().__init__(num_classes=num_classes, dist_sync_on_step=dist_sync_on_step, ignore_index=ignore_index, reduction=reduction, threshold=threshold)
+
+        self.ignore_index_list = ignore_index_list
+        self.unfiltered_num_classes = unfiltered_num_classes
         self.metrics_args_prep_fn = metrics_args_prep_fn or PreprocessSegmentationMetricsArgs(apply_arg_max=True)
         self.greater_is_better = True
 
     def update(self, preds, target: torch.Tensor):
         preds, target = self.metrics_args_prep_fn(preds, target)
+        if self.ignore_index_list is not None:
+            target = _map_ignored_inds(target, self.ignore_index_list, self.unfiltered_num_classes)
+            preds = _map_ignored_inds(preds, self.ignore_index_list, self.unfiltered_num_classes)
         super().update(preds=preds, target=target)
 
     def compute(self) -> torch.Tensor:
         """Computes Dice coefficient"""
         return _dice_from_confmat(self.confmat, self.num_classes, self.ignore_index, self.absent_score, self.reduction)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## super_gradients/training/models/__init__.py

```diff
@@ -66,15 +66,15 @@
 from super_gradients.training.models.classification_models.vit import ViT, ViTBase, ViTLarge, ViTHuge
 
 # Detection models
 from super_gradients.training.models.detection_models.csp_darknet53 import CSPDarknet53, SPP
 from super_gradients.training.models.detection_models.pp_yolo_e import PPYoloE, PPYoloE_S, PPYoloE_M, PPYoloE_L, PPYoloE_X
 from super_gradients.training.models.detection_models.darknet53 import Darknet53, Darknet53Base
 from super_gradients.training.models.detection_models.ssd import SSDMobileNetV1, SSDLiteMobileNetV2
-from super_gradients.training.models.detection_models.yolo_base import YoloBase, YoloPostPredictionCallback
+from super_gradients.training.models.detection_models.yolo_base import YoloBase, YoloXPostPredictionCallback, YoloPostPredictionCallback
 from super_gradients.training.models.detection_models.yolox import YoloX_N, YoloX_T, YoloX_S, YoloX_M, YoloX_L, YoloX_X, CustomYoloX
 from super_gradients.training.models.detection_models.customizable_detector import CustomizableDetector
 from super_gradients.training.models.detection_models.yolo_nas import (
     YoloNASStage,
     YoloNASStem,
     YoloNASDownStage,
     YoloNASUpStage,
@@ -287,14 +287,15 @@
     "YoloX_T",
     "YoloX_S",
     "YoloX_M",
     "YoloX_L",
     "YoloX_X",
     "CustomYoloX",
     "YoloPostPredictionCallback",
+    "YoloXPostPredictionCallback",
     "CustomizableDetector",
     "ShelfNet50",
     "ShelfNet101",
     "ShelfNetHW",
     "ShelfNetLW",
     "ShelfNetBase",
     "ShelfNet503343",
```

## super_gradients/training/models/model_factory.py

```diff
@@ -22,27 +22,34 @@
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.utils.sg_trainer_utils import get_callable_param_names
 from super_gradients.training.processing.processing import get_pretrained_processing_params
 
 logger = get_logger(__name__)
 
 
-def get_architecture(model_name: str, arch_params: HpmStruct, download_required_code: bool = True) -> Tuple[Type[torch.nn.Module], HpmStruct, str, bool]:
+def get_architecture(
+    model_name: str, arch_params: HpmStruct, download_required_code: bool = True, download_platform_weights: bool = True
+) -> Tuple[Type[torch.nn.Module], HpmStruct, str, bool]:
     """
     Get the corresponding architecture class.
 
     :param model_name:          Define the model's architecture from models/ALL_ARCHITECTURES
     :param arch_params:         Architecture hyper parameters. e.g.: block, num_blocks, etc.
     :param download_required_code: if model is not found in SG and is downloaded from a remote client, overriding this parameter with False
                                         will prevent additional code from being downloaded. This affects only models from remote client.
 
+    :param download_platform_weights:  bool, when getting a model from the platform, whether to downlaod the pretrained weights as well.
+        In any other case this parameter will be ignored. (default=True).
+
     :return:
         - architecture_cls:     Class of the model
         - arch_params:          Might be updated if loading from remote deci lab
-        - pretrained_weights_path:   path to the pretrained weights from deci lab (None for local models).
+        - pretrained_weights_path:   path to the pretrained weights from deci lab (None for local models or when deci
+            client is not enabled).
+
         - is_remote:            True if loading from remote deci lab
     """
     pretrained_weights_path = None
     is_remote = False
     if not isinstance(model_name, str):
         raise ValueError("Parameter model_name is expected to be a string.")
 
@@ -58,16 +65,18 @@
                     f'The required model "{model_name}", was not found in SuperGradients and remote deci-lab. '
                     f"See docs or all_architectures.py for supported model names."
                 )
 
             if download_required_code:  # Some extra code might be required to instantiate the arch params.
                 deci_client.download_and_load_model_additional_code(model_name, target_path=str(Path.cwd()))
             _arch_params = hydra.utils.instantiate(_arch_params)
-
-            pretrained_weights_path = deci_client.get_model_weights(model_name)
+            if download_platform_weights:
+                pretrained_weights_path = deci_client.get_model_weights(model_name)
+            else:
+                pretrained_weights_path = None
             model_name = _arch_params["model_name"]
             del _arch_params["model_name"]
             _arch_params = HpmStruct(**_arch_params)
             _arch_params.override(**arch_params.to_dict())
             arch_params, is_remote = _arch_params, True
         else:
             raise UnknownTypeException(
@@ -95,16 +104,18 @@
                                 will prevent additional code from being downloaded. This affects only models from remote client.
 
     :return:                    Instantiated model i.e torch.nn.Module, architecture_class (will be none when architecture is not str)
     """
     if arch_params is None:
         arch_params = {}
     arch_params = core_utils.HpmStruct(**arch_params)
-
-    architecture_cls, arch_params, pretrained_weights_path, is_remote = get_architecture(model_name, arch_params, download_required_code)
+    download_platform_weights = isinstance(pretrained_weights, str) and pretrained_weights.startswith("platform/")
+    architecture_cls, arch_params, pretrained_weights_path, is_remote = get_architecture(
+        model_name, arch_params, download_required_code, download_platform_weights
+    )
 
     if not issubclass(architecture_cls, SgModule):
         net = architecture_cls(**arch_params.to_dict(include_schema=False))
     else:
         if core_utils.get_param(arch_params, "num_classes"):
             logger.warning(
                 "Passing num_classes through arch_params is deprecated and will be removed in the next version. " "Pass num_classes explicitly to models.get"
@@ -113,26 +124,29 @@
 
         if num_classes is not None:
             arch_params.override(num_classes=num_classes)
 
         if pretrained_weights is None and num_classes is None:
             raise ValueError("num_classes or pretrained_weights must be passed to determine net's structure.")
 
-        if pretrained_weights:
+        if pretrained_weights and pretrained_weights in PRETRAINED_NUM_CLASSES.keys():
             num_classes_new_head = core_utils.get_param(arch_params, "num_classes", PRETRAINED_NUM_CLASSES[pretrained_weights])
             arch_params.num_classes = PRETRAINED_NUM_CLASSES[pretrained_weights]
+        elif pretrained_weights and pretrained_weights is None:
+            raise ValueError(f"Unknown pretrained_weights - couldn't find pretrained weights in {PRETRAINED_NUM_CLASSES.keys()} or platform.")
 
-        # Most of the SG models work with a single params names "arch_params" of type HpmStruct, but a few take **kwargs instead
+        # Most of the SG models work with a single params names "arch_params" of type HpmStruct, but a few take
+        # **kwargs instead
         if "arch_params" not in get_callable_param_names(architecture_cls):
             net = architecture_cls(**arch_params.to_dict(include_schema=False))
         else:
             net = architecture_cls(arch_params=arch_params)
 
         if pretrained_weights:
-            if is_remote:
+            if is_remote and pretrained_weights_path:
                 load_pretrained_weights_local(net, model_name, pretrained_weights_path)
             else:
                 load_pretrained_weights(net, model_name, pretrained_weights)
 
             if num_classes_new_head != arch_params.num_classes:
                 net.replace_head(new_num_classes=num_classes_new_head)
                 arch_params.num_classes = num_classes_new_head
@@ -170,15 +184,15 @@
     download_required_code: bool = True,
     checkpoint_num_classes: int = None,
 ) -> Union[SgModule, torch.nn.Module]:
     """
     :param model_name:          Defines the model's architecture from models/ALL_ARCHITECTURES
     :param arch_params:         Architecture hyper parameters. e.g.: block, num_blocks, etc.
     :param num_classes:         Number of classes (defines the net's structure).
-                                    If None is given, will try to derrive from pretrained_weight's corresponding dataset.
+                                    If None is given, will try to derive from pretrained_weight's corresponding dataset.
     :param strict_load:         See super_gradients.common.data_types.enum.strict_load.StrictLoad class documentation for details
                                     (default=NO_KEY_MATCHING to suport SG trained checkpoints)
     :param checkpoint_path:     The path to the external checkpoint to be loaded. Can be absolute or relative (ie: path/to/checkpoint.pth) path or URL.
                                     If provided, will automatically attempt to load the checkpoint.
     :param pretrained_weights:  Describe the dataset of the pretrained weights (for example "imagenent").
     :param load_backbone:       Load the provided checkpoint to model.backbone instead of model.
     :param download_required_code: if model is not found in SG and is downloaded from a remote client, overriding this parameter with False
```

## super_gradients/training/models/predictions.py

```diff
@@ -1,55 +1,11 @@
-from typing import Tuple
-from abc import ABC
-from dataclasses import dataclass
+from super_gradients.training.utils.predict import Prediction, DetectionPrediction
+import warnings
 
-import numpy as np
+warnings.warn(
+    "Importing from super_gradients.training.models.predictions is deprecated. "
+    "Please update your code to import from super_gradients.training.utils.predict instead.",
+    DeprecationWarning,
+)
 
-from super_gradients.common.factories.bbox_format_factory import BBoxFormatFactory
-from super_gradients.training.datasets.data_formats.bbox_formats import convert_bboxes
 
-
-@dataclass
-class Prediction(ABC):
-    pass
-
-
-@dataclass
-class DetectionPrediction(Prediction):
-    """Represents a detection prediction, with bboxes represented in xyxy format."""
-
-    bboxes_xyxy: np.ndarray
-    confidence: np.ndarray
-    labels: np.ndarray
-
-    def __init__(self, bboxes: np.ndarray, bbox_format: str, confidence: np.ndarray, labels: np.ndarray, image_shape: Tuple[int, int]):
-        """
-        :param bboxes:      BBoxes in the format specified by bbox_format
-        :param bbox_format: BBoxes format that can be a string ("xyxy", "cxywh", ...)
-        :param confidence:  Confidence scores for each bounding box
-        :param labels:      Labels for each bounding box.
-        :param image_shape: Shape of the image the prediction is made on, (H, W). This is used to convert bboxes to xyxy format
-        """
-        self._validate_input(bboxes, confidence, labels)
-
-        factory = BBoxFormatFactory()
-        bboxes_xyxy = convert_bboxes(
-            bboxes=bboxes,
-            image_shape=image_shape,
-            source_format=factory.get(bbox_format),
-            target_format=factory.get("xyxy"),
-            inplace=False,
-        )
-
-        self.bboxes_xyxy = bboxes_xyxy
-        self.confidence = confidence
-        self.labels = labels
-
-    def _validate_input(self, bboxes: np.ndarray, confidence: np.ndarray, labels: np.ndarray) -> None:
-        n_bboxes, n_confidences, n_labels = bboxes.shape[0], confidence.shape[0], labels.shape[0]
-        if n_bboxes != n_confidences != n_labels:
-            raise ValueError(
-                f"The number of bounding boxes ({n_bboxes}) does not match the number of confidence scores ({n_confidences}) and labels ({n_labels})."
-            )
-
-    def __len__(self):
-        return len(self.bboxes_xyxy)
+__all__ = ["Prediction", "DetectionPrediction"]
```

## super_gradients/training/models/classification_models/regnet.py

```diff
@@ -174,20 +174,20 @@
     # We need to derive block width and number of blocks from initial parameters.
     parameterized_width = initial_width + slope * np.arange(network_depth)  # From equation 2
     parameterized_block = np.log(parameterized_width / initial_width) / np.log(quantized_param)  # From equation 3
     parameterized_block = np.round(parameterized_block)
     quantized_width = initial_width * np.power(quantized_param, parameterized_block)
     # We need to convert quantized_width to make sure that it is divisible by 8
     quantized_width = 8 * np.round(quantized_width / 8)
-    ls_block_width, ls_num_blocks = np.unique(quantized_width.astype(np.int), return_counts=True)
+    ls_block_width, ls_num_blocks = np.unique(quantized_width.astype(np.int32), return_counts=True)
     # At this points, for each stage, the above-calculated block width could be incompatible to group width
     # due to bottleneck ratio. Hence, we need to adjust the formers.
     # Group width could be swapped to number of groups, since their multiplication is block width
     ls_group_width = np.array([min(group_width, block_width // bottleneck_ratio) for block_width in ls_block_width])
-    ls_block_width = (np.round(ls_block_width // bottleneck_ratio / group_width) * group_width).astype(np.int).tolist()
+    ls_block_width = (np.round(ls_block_width // bottleneck_ratio / group_width) * group_width).astype(np.int32).tolist()
     ls_bottleneck_ratio = [bottleneck_ratio for _ in range(len(ls_block_width))]
     return ls_num_blocks, ls_block_width, ls_bottleneck_ratio, ls_group_width.tolist()
 
 
 class RegNetX(AnyNetX):
     def __init__(
         self, initial_width, slope, quantized_param, network_depth, bottleneck_ratio, group_width, stride, arch_params, se_ratio=None, input_channels=3
```

## super_gradients/training/models/classification_models/resnet.py

```diff
@@ -5,25 +5,25 @@
     Deep Residual Learning for Image Recognition. arXiv:1512.03385
 
 Pre-trained ImageNet models: 'deci-model-repository/resnet?/ckpt_best.pth' => ? = the type of resnet (e.g. 18, 34...)
 Pre-trained CIFAR10 models: 'deci-model-repository/CIFAR_NAS_#?_????_?/ckpt_best.pth' => ? = num of model, structure, width_mult
 
 Code adapted from https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py
 """
+from collections import OrderedDict
 
 import torch.nn as nn
 import torch.nn.functional as F
-from collections import OrderedDict
+from super_gradients.training.models.sg_module import SgModule
 
+from super_gradients.common.object_names import Models
+from super_gradients.common.registry.registry import register_model
 from super_gradients.modules.utils import width_multiplier
-from super_gradients.training.models import SgModule
 from super_gradients.training.utils import get_param
 from super_gradients.training.utils.regularization_utils import DropPath
-from super_gradients.common.registry.registry import register_model
-from super_gradients.common.object_names import Models
 
 
 class BasicResNetBlock(nn.Module):
     def __init__(self, in_planes, planes, stride=1, expansion=1, final_relu=True, droppath_prob=0.0):
         super(BasicResNetBlock, self).__init__()
         self.expansion = expansion
         self.conv1 = nn.Conv2d(in_planes, planes, kernel_size=3, stride=stride, padding=1, bias=False)
```

## super_gradients/training/models/detection_models/csp_resnet.py

```diff
@@ -202,15 +202,15 @@
                 )
                 for i in range(n)
             ]
         )
 
         self._out_channels = channels[1:]
         self._out_strides = [4 * 2**i for i in range(n)]
-        self.return_idx = return_idx
+        self.return_idx = tuple(return_idx)
 
         if pretrained_weights:
             if isinstance(pretrained_weights, (str, Path)) and os.path.isfile(str(pretrained_weights)):
                 state_dict = torch.load(str(pretrained_weights), map_location="cpu")
             elif isinstance(pretrained_weights, str) and pretrained_weights.startswith("https://"):
                 with wait_for_the_master(get_local_rank()):
                     state_dict = torch.hub.load_state_dict_from_url(pretrained_weights, map_location="cpu")
```

## super_gradients/training/models/detection_models/customizable_detector.py

```diff
@@ -15,15 +15,15 @@
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.module_interfaces import SupportsReplaceNumClasses
 from super_gradients.modules.head_replacement_utils import replace_num_classes_with_random_weights
 from super_gradients.training.utils.utils import HpmStruct, arch_params_deprecated
 from super_gradients.training.models.sg_module import SgModule
 import super_gradients.common.factories.detection_modules_factory as det_factory
-from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
+from super_gradients.training.utils.predict import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
 from super_gradients.training.utils.detection_utils import DetectionPostPredictionCallback
 from super_gradients.training.utils.media.image import ImageSource
 
 
 class CustomizableDetector(SgModule):
@@ -160,25 +160,33 @@
             image_processor=self._image_processor,
             post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
             class_names=self._class_names,
             fuse_model=fuse_model,
         )
         return pipeline
 
-    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> ImagesDetectionPrediction:
+    def predict(
+        self,
+        images: ImageSource,
+        iou: Optional[float] = None,
+        conf: Optional[float] = None,
+        batch_size: int = 32,
+        fuse_model: bool = True,
+    ) -> ImagesDetectionPrediction:
         """Predict an image or a list of images.
 
-        :param images:  Images to predict.
-        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
-        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
-                        If None, the default value associated to the training is used.
-        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+        :param images:      Images to predict.
+        :param iou:         (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:        (Optional) Below the confidence threshold, prediction are discarded.
+                            If None, the default value associated to the training is used.
+        :param batch_size:  Maximum number of images to process at the same time.
+        :param fuse_model:  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
         pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
-        return pipeline(images)  # type: ignore
+        return pipeline(images, batch_size=batch_size)  # type: ignore
 
     def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True):
         """Predict using webcam.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
```

## super_gradients/training/models/detection_models/yolo_base.py

```diff
@@ -1,8 +1,9 @@
 import math
+import warnings
 from typing import Union, Type, List, Tuple, Optional
 from functools import lru_cache
 
 import torch
 import torch.nn as nn
 
 from super_gradients.common.decorators.factory_decorator import resolve_param
@@ -10,15 +11,15 @@
 from super_gradients.modules import CrossModelSkipConnection, Conv
 from super_gradients.training.models.classification_models.regnet import AnyNetX, Stage
 from super_gradients.training.models.detection_models.csp_darknet53 import GroupedConvBlock, CSPDarknet53, get_yolo_type_params, SPP
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.utils import torch_version_is_greater_or_equal
 from super_gradients.training.utils.detection_utils import non_max_suppression, matrix_non_max_suppression, NMS_Type, DetectionPostPredictionCallback, Anchors
 from super_gradients.training.utils.utils import HpmStruct, check_img_size_divisibility, get_param
-from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
+from super_gradients.training.utils.predict import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
 from super_gradients.training.utils.media.image import ImageSource
 
 
 COCO_DETECTION_80_CLASSES_BBOX_ANCHORS = Anchors(
     [[10, 13, 16, 30, 33, 23], [30, 61, 62, 45, 59, 119], [116, 90, 156, 198, 373, 326]], strides=[8, 16, 32]
@@ -54,62 +55,109 @@
     "xhead_groups": None,  # (has an impact only if yolo_type is yoloX)
     # Num groups in convs in classification and regression branches of the detecting blocks;
     # if None default groups will be used according to conv type
     # (1 for Conv and depthwise for GroupedConvBlock)
 }
 
 
-class YoloPostPredictionCallback(DetectionPostPredictionCallback):
-    """Non-Maximum Suppression (NMS) module"""
+class YoloXPostPredictionCallback(DetectionPostPredictionCallback):
+    """Post-prediction callback to decode YoloX model's output and apply Non-Maximum Suppression (NMS) to get
+    the final predictions.
+    """
 
     def __init__(
         self,
         conf: float = 0.001,
         iou: float = 0.6,
         classes: List[int] = None,
         nms_type: NMS_Type = NMS_Type.ITERATIVE,
         max_predictions: int = 300,
         with_confidence: bool = True,
+        class_agnostic_nms: bool = False,
+        multi_label_per_box: bool = True,
     ):
         """
         :param conf: confidence threshold
         :param iou: IoU threshold                                       (used in NMS_Type.ITERATIVE)
         :param classes: (optional list) filter by class                 (used in NMS_Type.ITERATIVE)
         :param nms_type: the type of nms to use (iterative or matrix)
         :param max_predictions: maximum number of boxes to output       (used in NMS_Type.MATRIX)
         :param with_confidence: in NMS, whether to multiply objectness  (used in NMS_Type.ITERATIVE)
                                 score with class score
+        :param class_agnostic_nms: indicates how boxes of different classes will be treated during
+                                   NMS step (used in NMS_Type.ITERATIVE and NMS_Type.MATRIX)
+                                   True - NMS will be performed on all classes together.
+                                   False - NMS will be performed on each class separately (default).
+        :param multi_label_per_box: controls whether to decode multiple labels per box (used in NMS_Type.ITERATIVE)
+                                    True - each anchor can produce multiple labels of different classes
+                                           that pass confidence threshold check (default).
+                                    False - each anchor can produce only one label of the class with the highest score.
         """
-        super(YoloPostPredictionCallback, self).__init__()
+        super(YoloXPostPredictionCallback, self).__init__()
         self.conf = conf
         self.iou = iou
         self.classes = classes
         self.nms_type = nms_type
         self.max_pred = max_predictions
         self.with_confidence = with_confidence
+        self.class_agnostic_nms = class_agnostic_nms
+        self.multi_label_per_box = multi_label_per_box
 
-    def forward(self, x, device: str = None):
+    def forward(self, x: Union[torch.Tensor, Tuple[torch.Tensor, List[torch.Tensor]]], device: str = None):
         """Apply NMS to the raw output of the model and keep only top `max_predictions` results.
 
         :param x: Raw output of the model, with x[0] expected to be a list of Tensors of shape (cx, cy, w, h, confidence, cls0, cls1, ...)
         :return: List of Tensors of shape (x1, y1, x2, y2, conf, cls)
         """
+        # Use the main output features in case of multiple outputs.
+        if isinstance(x, (tuple, list)):
+            x = x[0]
 
         if self.nms_type == NMS_Type.ITERATIVE:
-            nms_result = non_max_suppression(x[0], conf_thres=self.conf, iou_thres=self.iou, with_confidence=self.with_confidence)
+            nms_result = non_max_suppression(
+                x,
+                conf_thres=self.conf,
+                iou_thres=self.iou,
+                with_confidence=self.with_confidence,
+                multi_label_per_box=self.multi_label_per_box,
+                class_agnostic_nms=self.class_agnostic_nms,
+            )
         else:
-            nms_result = matrix_non_max_suppression(x[0], conf_thres=self.conf, max_num_of_detections=self.max_pred)
+            nms_result = matrix_non_max_suppression(x, conf_thres=self.conf, max_num_of_detections=self.max_pred, class_agnostic_nms=self.class_agnostic_nms)
 
         return self._filter_max_predictions(nms_result)
 
     def _filter_max_predictions(self, res: List) -> List:
         res[:] = [im[: self.max_pred] if (im is not None and im.shape[0] > self.max_pred) else im for im in res]
         return res
 
 
+class YoloPostPredictionCallback(YoloXPostPredictionCallback):
+    def __init__(
+        self,
+        conf: float = 0.001,
+        iou: float = 0.6,
+        classes: List[int] = None,
+        nms_type: NMS_Type = NMS_Type.ITERATIVE,
+        max_predictions: int = 300,
+        with_confidence: bool = True,
+    ):
+        warnings.warn("YoloPostPredictionCallback is deprecated since SG 3.1.3, please use YoloXPostPredictionCallback instead", DeprecationWarning)
+        super().__init__(
+            conf=conf,
+            iou=iou,
+            classes=classes,
+            nms_type=nms_type,
+            max_predictions=max_predictions,
+            with_confidence=with_confidence,
+            class_agnostic_nms=False,
+            multi_label_per_box=True,
+        )
+
+
 class Concat(nn.Module):
     """CONCATENATE A LIST OF TENSORS ALONG DIMENSION"""
 
     def __init__(self, dimension=1):
         super().__init__()
         self.dimension = dimension
 
@@ -423,15 +471,15 @@
         self._class_names: Optional[List[str]] = None
         self._image_processor: Optional[Processing] = None
         self._default_nms_iou: Optional[float] = None
         self._default_nms_conf: Optional[float] = None
 
     @staticmethod
     def get_post_prediction_callback(conf: float, iou: float) -> DetectionPostPredictionCallback:
-        return YoloPostPredictionCallback(conf=conf, iou=iou)
+        return YoloXPostPredictionCallback(conf=conf, iou=iou)
 
     @resolve_param("image_processor", ProcessingFactory())
     def set_dataset_processing_params(
         self,
         class_names: Optional[List[str]] = None,
         image_processor: Optional[Processing] = None,
         iou: Optional[float] = None,
@@ -471,25 +519,33 @@
             image_processor=self._image_processor,
             post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
             class_names=self._class_names,
             fuse_model=fuse_model,
         )
         return pipeline
 
-    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> ImagesDetectionPrediction:
+    def predict(
+        self,
+        images: ImageSource,
+        iou: Optional[float] = None,
+        conf: Optional[float] = None,
+        batch_size: int = 32,
+        fuse_model: bool = True,
+    ) -> ImagesDetectionPrediction:
         """Predict an image or a list of images.
 
-        :param images:  Images to predict.
-        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
-        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
-                        If None, the default value associated to the training is used.
-        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+        :param images:      Images to predict.
+        :param iou:         (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:        (Optional) Below the confidence threshold, prediction are discarded.
+                            If None, the default value associated to the training is used.
+        :param batch_size:  Maximum number of images to process at the same time.
+        :param fuse_model:  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
         pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
-        return pipeline(images)  # type: ignore
+        return pipeline(images, batch_size=batch_size)  # type: ignore
 
     def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True):
         """Predict using webcam.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
```

## super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py

```diff
@@ -11,15 +11,18 @@
 
     def __init__(self, score_threshold: float, nms_threshold: float, nms_top_k: int, max_predictions: int, multi_label_per_box: bool = True):
         """
         :param score_threshold: Predictions confidence threshold. Predictions with score lower than score_threshold will not participate in Top-K & NMS
         :param iou: IoU threshold for NMS step.
         :param nms_top_k: Number of predictions participating in NMS step
         :param max_predictions: maximum number of boxes to return after NMS step
-
+        :param multi_label_per_box: controls whether to decode multiple labels per box.
+                                    True - each anchor can produce multiple labels of different classes
+                                           that pass confidence threshold check (default).
+                                    False - each anchor can produce only one label of the class with the highest score.
         """
         super(PPYoloEPostPredictionCallback, self).__init__()
         self.score_threshold = score_threshold
         self.nms_threshold = nms_threshold
         self.nms_top_k = nms_top_k
         self.max_predictions = max_predictions
         self.multi_label_per_box = multi_label_per_box
```

## super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py

```diff
@@ -12,15 +12,15 @@
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.models.detection_models.csp_resnet import CSPResNetBackbone
 from super_gradients.training.models.detection_models.pp_yolo_e.pan import PPYoloECSPPAN
 from super_gradients.training.models.detection_models.pp_yolo_e.pp_yolo_head import PPYOLOEHead
 from super_gradients.training.utils import HpmStruct
 from super_gradients.training.models.arch_params_factory import get_arch_params
 from super_gradients.training.models.detection_models.pp_yolo_e.post_prediction_callback import PPYoloEPostPredictionCallback, DetectionPostPredictionCallback
-from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
+from super_gradients.training.utils.predict import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
 from super_gradients.training.utils.media.image import ImageSource
 
 
 class PPYoloE(SgModule):
     def __init__(self, arch_params):
@@ -82,25 +82,33 @@
             model=self,
             image_processor=self._image_processor,
             post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
             class_names=self._class_names,
         )
         return pipeline
 
-    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> ImagesDetectionPrediction:
+    def predict(
+        self,
+        images: ImageSource,
+        iou: Optional[float] = None,
+        conf: Optional[float] = None,
+        batch_size: int = 32,
+        fuse_model: bool = True,
+    ) -> ImagesDetectionPrediction:
         """Predict an image or a list of images.
 
-        :param images:  Images to predict.
-        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
-        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
-                        If None, the default value associated to the training is used.
-        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+        :param images:      Images to predict.
+        :param iou:         (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:        (Optional) Below the confidence threshold, prediction are discarded.
+                            If None, the default value associated to the training is used.
+        :param batch_size:  Maximum number of images to process at the same time.
+        :param fuse_model:  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
         pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
-        return pipeline(images)  # type: ignore
+        return pipeline(images, batch_size=batch_size)  # type: ignore
 
     def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True):
         """Predict using webcam.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
```

## super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py

```diff
@@ -121,15 +121,15 @@
         :param width_mult: A scaling factor applied to in_channels in order.
         """
         super(PPYOLOEHead, self).__init__()
         in_channels = [max(round(c * width_mult), 1) for c in in_channels]
 
         self.in_channels = tuple(in_channels)
         self.num_classes = num_classes
-        self.fpn_strides = fpn_strides
+        self.fpn_strides = tuple(fpn_strides)
         self.grid_cell_scale = grid_cell_scale
         self.grid_cell_offset = grid_cell_offset
         self.reg_max = reg_max
         self.eval_size = eval_size
 
         # stem
         self.stem_cls = nn.ModuleList()
```

## super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py

```diff
@@ -14,24 +14,37 @@
 from super_gradients.training.models.detection_models.pp_yolo_e.pp_yolo_head import generate_anchors_for_grid_cell
 from super_gradients.training.utils import HpmStruct, torch_version_is_greater_or_equal
 from super_gradients.training.utils.bbox_utils import batch_distance2bbox
 
 
 @register_detection_module()
 class YoloNASDFLHead(BaseDetectionModule, SupportsReplaceNumClasses):
-    def __init__(self, in_channels: int, inter_channels: int, width_mult: float, first_conv_group_size: int, num_classes: int, stride: int, reg_max: int):
+    def __init__(
+        self,
+        in_channels: int,
+        inter_channels: int,
+        width_mult: float,
+        first_conv_group_size: int,
+        num_classes: int,
+        stride: int,
+        reg_max: int,
+        cls_dropout_rate: float = 0.0,
+        reg_dropout_rate: float = 0.0,
+    ):
         """
         Initialize the YoloNASDFLHead
         :param in_channels: Input channels
         :param inter_channels: Intermediate number of channels
         :param width_mult: Width multiplier
         :param first_conv_group_size: Group size
         :param num_classes: Number of detection classes
         :param stride: Output stride for this head
         :param reg_max: Number of bins in the regression head
+        :param cls_dropout_rate: Dropout rate for the classification head
+        :param reg_dropout_rate: Dropout rate for the regression head
         """
         super().__init__(in_channels)
 
         inter_channels = width_multiplier(inter_channels, width_mult, 8)
         if first_conv_group_size == 0:
             groups = 0
         elif first_conv_group_size == -1:
@@ -47,14 +60,17 @@
 
         first_reg_conv = [ConvBNReLU(inter_channels, inter_channels, kernel_size=3, stride=1, padding=1, groups=groups, bias=False)] if groups else []
         self.reg_convs = nn.Sequential(*first_reg_conv, ConvBNReLU(inter_channels, inter_channels, kernel_size=3, stride=1, padding=1, bias=False))
 
         self.cls_pred = nn.Conv2d(inter_channels, self.num_classes, 1, 1, 0)
         self.reg_pred = nn.Conv2d(inter_channels, 4 * (reg_max + 1), 1, 1, 0)
 
+        self.cls_dropout_rate = nn.Dropout2d(cls_dropout_rate) if cls_dropout_rate > 0 else nn.Identity()
+        self.reg_dropout_rate = nn.Dropout2d(reg_dropout_rate) if reg_dropout_rate > 0 else nn.Identity()
+
         self.grid = torch.zeros(1)
         self.stride = stride
 
         self.prior_prob = 1e-2
         self._initialize_biases()
 
     def replace_num_classes(self, num_classes: int, compute_new_weights_fn: Callable[[nn.Module, int], nn.Module]):
@@ -65,17 +81,19 @@
     def out_channels(self):
         return None
 
     def forward(self, x):
         x = self.stem(x)
 
         cls_feat = self.cls_convs(x)
+        cls_feat = self.cls_dropout_rate(cls_feat)
         cls_output = self.cls_pred(cls_feat)
 
         reg_feat = self.reg_convs(x)
+        reg_feat = self.reg_dropout_rate(reg_feat)
         reg_output = self.reg_pred(reg_feat)
 
         return reg_output, cls_output
 
     def _initialize_biases(self):
         prior_bias = -math.log((1 - self.prior_prob) / self.prior_prob)
         torch.nn.init.constant_(self.cls_pred.bias, prior_bias)
```

## super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py

```diff
@@ -1,11 +1,12 @@
 from functools import partial
-from typing import Type, List
+from typing import Type, List, Iterable, Union
 
 import torch
+from super_gradients.training.utils.regularization_utils import DropPath
 from torch import nn, Tensor
 
 from super_gradients.common.registry import register_detection_module
 from super_gradients.modules import Residual, BaseDetectionModule
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.activations_type_factory import ActivationsTypeFactory
 from super_gradients.modules import QARepVGGBlock, Conv
@@ -16,39 +17,49 @@
 
 class YoloNASBottleneck(nn.Module):
     """
     A bottleneck block for YoloNAS. Consists of two consecutive blocks and optional residual connection.
     """
 
     def __init__(
-        self, input_channels: int, output_channels: int, block_type: Type[nn.Module], activation_type: Type[nn.Module], shortcut: bool, use_alpha: bool
+        self,
+        input_channels: int,
+        output_channels: int,
+        block_type: Type[nn.Module],
+        activation_type: Type[nn.Module],
+        shortcut: bool,
+        use_alpha: bool,
+        drop_path_rate: float = 0.0,
     ):
         """
         Initialize the YoloNASBottleneck block
 
         :param input_channels: Number of input channels
         :param output_channels: Number of output channels
         :param block_type: Type of the convolutional block
         :param activation_type: Activation type for the convolutional block
         :param shortcut: If True, adds the residual connection from input to output.
         :param use_alpha: If True, adds the learnable alpha parameter (multiplier for the residual connection).
+        :param drop_path_rate: Drop path rate for the residual path of the block
         """
         super().__init__()
 
         self.cv1 = block_type(input_channels, output_channels, activation_type=activation_type)
         self.cv2 = block_type(output_channels, output_channels, activation_type=activation_type)
         self.add = shortcut and input_channels == output_channels
         self.shortcut = Residual() if self.add else None
+        self.drop_path = DropPath(drop_path_rate) if drop_path_rate > 0.0 else nn.Identity()
         if use_alpha:
             self.alpha = torch.nn.Parameter(torch.tensor([1.0]), requires_grad=True)
         else:
             self.alpha = 1.0
 
     def forward(self, x):
-        return self.alpha * self.shortcut(x) + self.cv2(self.cv1(x)) if self.add else self.cv2(self.cv1(x))
+        y = self.drop_path(self.cv2(self.cv1(x)))
+        return self.alpha * self.shortcut(x) + y if self.add else y
 
 
 class SequentialWithIntermediates(nn.Sequential):
     """
     A Sequential module that can return all intermediate values as a list of Tensors
     """
 
@@ -79,42 +90,62 @@
         block_type: Type[nn.Module],
         activation_type: Type[nn.Module],
         shortcut: bool = True,
         use_alpha: bool = True,
         expansion: float = 0.5,
         hidden_channels: int = None,
         concat_intermediates: bool = False,
+        drop_path_rates: Union[Iterable[float], None] = None,
+        dropout_rate: float = 0.0,
     ):
         """
 
         :param in_channels: Number of input channels.
         :param out_channels:  Number of output channels.
         :param num_bottlenecks: Number of bottleneck blocks.
         :param block_type: Bottleneck block type.
         :param activation_type: Activation type for all blocks.
         :param shortcut: If True, adds the residual connection from input to output.
         :param use_alpha: If True, adds the learnable alpha parameter (multiplier for the residual connection).
         :param expansion: If hidden_channels is None, hidden_channels is set to in_channels * expansion.
         :param hidden_channels: If not None, sets the number of hidden channels used inside the bottleneck blocks.
         :param concat_intermediates:
+        :param drop_path_rates: List of drop path probabilities for each bottleneck block.
+                                Must have the length equal to the num_bottlenecks or None.
+        :param dropout_rate: Dropout probability before the last convolution in this layer.
         """
+        if drop_path_rates is None:
+            drop_path_rates = [0.0] * num_bottlenecks
+        else:
+            drop_path_rates = tuple(drop_path_rates)
+        if len(drop_path_rates) != num_bottlenecks:
+            raise ValueError(
+                f"Argument drop_path_rates ({drop_path_rates}, len {len(drop_path_rates)} "
+                f"must have the length equal to the num_bottlenecks ({num_bottlenecks})."
+            )
+
         super(YoloNASCSPLayer, self).__init__()
         if hidden_channels is None:
             hidden_channels = int(out_channels * expansion)
         self.conv1 = Conv(in_channels, hidden_channels, 1, stride=1, activation_type=activation_type)
         self.conv2 = Conv(in_channels, hidden_channels, 1, stride=1, activation_type=activation_type)
         self.conv3 = Conv(hidden_channels * (2 + concat_intermediates * num_bottlenecks), out_channels, 1, stride=1, activation_type=activation_type)
-        module_list = [YoloNASBottleneck(hidden_channels, hidden_channels, block_type, activation_type, shortcut, use_alpha) for _ in range(num_bottlenecks)]
+        module_list = [
+            YoloNASBottleneck(hidden_channels, hidden_channels, block_type, activation_type, shortcut, use_alpha, drop_path_rate=drop_path_rates[i])
+            for i in range(num_bottlenecks)
+        ]
         self.bottlenecks = SequentialWithIntermediates(concat_intermediates, *module_list)
+        self.dropout = nn.Dropout2d(dropout_rate, inplace=True) if dropout_rate > 0.0 else nn.Identity()
 
     def forward(self, x: Tensor) -> Tensor:
         x_1 = self.conv1(x)
         x_1 = self.bottlenecks(x_1)
         x_2 = self.conv2(x)
         x = torch.cat((*x_1, x_2), dim=1)
+        x = self.dropout(x)
         return self.conv3(x)
 
 
 @register_detection_module()
 class YoloNASStem(BaseDetectionModule):
     """
     Stem module for YoloNAS. Consists of a single QARepVGGBlock with stride of two.
@@ -149,36 +180,43 @@
         self,
         in_channels: int,
         out_channels: int,
         num_blocks: int,
         activation_type: Type[nn.Module],
         hidden_channels: int = None,
         concat_intermediates: bool = False,
+        drop_path_rates: Union[Iterable[float], None] = None,
+        dropout_rate: float = 0.0,
     ):
         """
         Initialize the YoloNASStage module
         :param in_channels: Number of input channels
         :param out_channels: Number of output channels
         :param num_blocks: Number of bottleneck blocks in the YoloNASCSPLayer
         :param activation_type: Activation type for all blocks
         :param hidden_channels: If not None, sets the number of hidden channels used inside the bottleneck blocks.
         :param concat_intermediates: If True, concatenates the intermediate values from the YoloNASCSPLayer.
+        :param drop_path_rates: List of drop path probabilities for each bottleneck block.
+                                Must have the length equal to the num_blocks or None.
+        :param dropout_rate: Dropout probability before the last convolution in this layer.
         """
         super().__init__(in_channels)
         self._out_channels = out_channels
         self.downsample = QARepVGGBlock(in_channels, out_channels, stride=2, activation_type=activation_type, use_residual_connection=False)
         self.blocks = YoloNASCSPLayer(
             out_channels,
             out_channels,
             num_blocks,
             QARepVGGBlock,
             activation_type,
             True,
             hidden_channels=hidden_channels,
             concat_intermediates=concat_intermediates,
+            drop_path_rates=drop_path_rates,
+            dropout_rate=dropout_rate,
         )
 
     @property
     def out_channels(self):
         return self._out_channels
 
     def forward(self, x):
@@ -199,14 +237,16 @@
         width_mult: float,
         num_blocks: int,
         depth_mult: float,
         activation_type: Type[nn.Module],
         hidden_channels: int = None,
         concat_intermediates: bool = False,
         reduce_channels: bool = False,
+        drop_path_rates: Union[Iterable[float], None] = None,
+        dropout_rate: float = 0.0,
     ):
         """
         Initialize the YoloNASUpStage module
         :param in_channels: Number of input channels
         :param out_channels: Number of output channels
         :param width_mult: Multiplier for the number of channels in the stage.
         :param num_blocks: Number of bottleneck blocks
@@ -245,14 +285,16 @@
             after_concat_channels,
             out_channels,
             num_blocks,
             QARepVGGBlock,
             activation_type,
             hidden_channels=hidden_channels,
             concat_intermediates=concat_intermediates,
+            drop_path_rates=drop_path_rates,
+            dropout_rate=dropout_rate,
         )
 
         self._out_channels = [out_channels, out_channels]
 
     @property
     def out_channels(self):
         return self._out_channels
@@ -282,14 +324,16 @@
         out_channels: int,
         width_mult: float,
         num_blocks: int,
         depth_mult: float,
         activation_type: Type[nn.Module],
         hidden_channels: int = None,
         concat_intermediates: bool = False,
+        drop_path_rates: Union[Iterable[float], None] = None,
+        dropout_rate: float = 0.0,
     ):
         """
         Initializes a YoloNASDownStage.
 
         :param in_channels: Number of input channels.
         :param out_channels: Number of output channels.
         :param width_mult: Multiplier for the number of channels in the stage.
@@ -312,14 +356,16 @@
             in_channels=after_concat_channels,
             out_channels=out_channels,
             num_bottlenecks=num_blocks,
             block_type=partial(Conv, kernel=3, stride=1),
             activation_type=activation_type,
             hidden_channels=hidden_channels,
             concat_intermediates=concat_intermediates,
+            drop_path_rates=drop_path_rates,
+            dropout_rate=dropout_rate,
         )
 
         self._out_channels = out_channels
 
     @property
     def out_channels(self):
         return self._out_channels
```

## super_gradients/training/models/pose_estimation_models/dekr_hrnet.py

```diff
@@ -7,30 +7,40 @@
 # ------------------------------------------------------------------------------
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import copy
-from typing import Mapping, Any, Tuple
+from functools import lru_cache
+from typing import Mapping, Any, Tuple, Optional, List, Union
 
+import numpy as np
 import torch
 import torch.nn.functional as F
 import torchvision
 from torch import nn
 
+from super_gradients.common.decorators.factory_decorator import resolve_param
+from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.common.abstractions.abstract_logger import get_logger
+from super_gradients.training.utils.predict import ImagesPoseEstimationPrediction
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.models.arch_params_factory import get_arch_params
 
 __all__ = ["DEKRPoseEstimationModel", "DEKRW32NODC"]
 
-from super_gradients.training.utils import HpmStruct
+from super_gradients.training.pipelines.pipelines import PoseEstimationPipeline
+
+from super_gradients.training.processing.processing import Processing
+
+from super_gradients.training.utils import HpmStruct, DEKRPoseEstimationDecodeCallback
+from super_gradients.training.utils.media.image import ImageSource
 
 logger = get_logger(__name__)
 
 
 class BasicBlock(nn.Module):
     """
     ResNet basic block
@@ -314,30 +324,40 @@
             transition_layer = self._make_transition_layer(num_channels_last, num_channels)
             setattr(self, "transition{}".format(i + 1), transition_layer)
 
             stage, num_channels_last = self._make_stage(self.stages_spec, i, num_channels, True)
             setattr(self, "stage{}".format(i + 2), stage)
 
         # build head net
-        inp_channels = int(sum(self.stages_spec.NUM_CHANNELS[-1]))
-        config_heatmap = self.spec.HEAD_HEATMAP
-        config_offset = self.spec.HEAD_OFFSET
+        self.head_inp_channels = int(sum(self.stages_spec.NUM_CHANNELS[-1]))
+        self.config_heatmap = self.spec.HEAD_HEATMAP
+        self.config_offset = self.spec.HEAD_OFFSET
         self.num_joints = arch_params.num_classes
         self.num_offset = self.num_joints * 2
         self.num_joints_with_center = self.num_joints + 1
-        self.offset_prekpt = config_offset["NUM_CHANNELS_PERKPT"]
+        self.offset_prekpt = self.config_offset["NUM_CHANNELS_PERKPT"]
 
         offset_channels = self.num_joints * self.offset_prekpt
-        self.transition_heatmap = self._make_transition_for_head(inp_channels, config_heatmap["NUM_CHANNELS"])
-        self.transition_offset = self._make_transition_for_head(inp_channels, offset_channels)
-        self.head_heatmap = self._make_heatmap_head(config_heatmap)
-        self.offset_feature_layers, self.offset_final_layer = self._make_separete_regression_head(config_offset)
-        self.heatmap_activation = nn.Sigmoid() if config_heatmap["HEATMAP_APPLY_SIGMOID"] else nn.Identity()
+        self.transition_heatmap = self._make_transition_for_head(self.head_inp_channels, self.config_heatmap["NUM_CHANNELS"])
+        self.transition_offset = self._make_transition_for_head(self.head_inp_channels, offset_channels)
+        self.head_heatmap = self._make_heatmap_head(self.config_heatmap)
+        self.offset_feature_layers, self.offset_final_layer = self._make_separete_regression_head(self.config_offset)
+        self.heatmap_activation = nn.Sigmoid() if self.config_heatmap["HEATMAP_APPLY_SIGMOID"] else nn.Identity()
         self.init_weights()
 
+    def replace_head(self, new_num_classes: int):
+        self.num_joints = new_num_classes
+        self.num_offset = new_num_classes * 2
+        self.num_joints_with_center = new_num_classes + 1
+
+        offset_channels = self.num_joints * self.offset_prekpt
+        self.head_heatmap = self._make_heatmap_head(self.config_heatmap)
+        self.transition_offset = self._make_transition_for_head(self.head_inp_channels, offset_channels)
+        self.offset_feature_layers, self.offset_final_layer = self._make_separete_regression_head(self.config_offset)
+
     def _make_transition_for_head(self, inplanes: int, outplanes: int) -> nn.Module:
         transition_layer = [nn.Conv2d(inplanes, outplanes, 1, 1, 0, bias=False), nn.BatchNorm2d(outplanes), nn.ReLU(True)]
         return nn.Sequential(*transition_layer)
 
     def _make_heatmap_head(self, layer_config: Mapping[str, Any]) -> nn.ModuleList:
         heatmap_head_layers = []
 
@@ -516,25 +536,118 @@
                 if hasattr(m, "bias"):
                     nn.init.constant_(m.transform_matrix_conv.bias, 0)
             if hasattr(m, "translation_conv"):
                 nn.init.constant_(m.translation_conv.weight, 0)
                 if hasattr(m, "bias"):
                     nn.init.constant_(m.translation_conv.bias, 0)
 
+    @staticmethod
+    def get_post_prediction_callback(conf: float = 0.05):
+        return DEKRPoseEstimationDecodeCallback(
+            min_confidence=conf,
+            keypoint_threshold=0.05,
+            nms_threshold=0.05,
+            apply_sigmoid=True,
+            max_num_people=30,
+            nms_num_threshold=8,
+            output_stride=4,
+        )
+
+    @resolve_param("image_processor", ProcessingFactory())
+    def set_dataset_processing_params(
+        self,
+        edge_links: Union[np.ndarray, List[Tuple[int, int]]],
+        edge_colors: Union[np.ndarray, List[Tuple[int, int, int]]],
+        keypoint_colors: Union[np.ndarray, List[Tuple[int, int, int]]],
+        image_processor: Optional[Processing] = None,
+        conf: Optional[float] = None,
+    ) -> None:
+        """Set the processing parameters for the dataset.
+
+        :param image_processor: (Optional) Image processing objects to reproduce the dataset preprocessing used for training.
+        :param conf:            (Optional) Below the confidence threshold, prediction are discarded
+        """
+        self._edge_links = edge_links or self._edge_links
+        self._edge_colors = edge_colors or self._edge_colors
+        self._keypoint_colors = keypoint_colors or self._keypoint_colors
+        self._image_processor = image_processor or self._image_processor
+        self._default_nms_conf = conf or self._default_nms_conf
+
+    @lru_cache(maxsize=1)
+    def _get_pipeline(self, conf: Optional[float] = None, fuse_model: bool = True) -> PoseEstimationPipeline:
+        """Instantiate the prediction pipeline of this model.
+
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+        """
+        if None in (self._edge_links, self._image_processor, self._default_nms_conf):
+            raise RuntimeError(
+                "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
+            )
+
+        conf = conf or self._default_nms_conf
 
-POSE_DEKR_W32_NO_DC_ARCH_PARAMS = get_arch_params("pose_dekr_w32_no_dc_arch_params")
+        if len(self._keypoint_colors) != self.num_joints:
+            raise RuntimeError(
+                "The number of colors for the keypoints ({}) does not match the number of joints ({})".format(len(self._keypoint_colors), self.num_joints)
+            )
+        if len(self._edge_colors) != len(self._edge_links):
+            raise RuntimeError(
+                "The number of colors for the joints ({}) does not match the number of joint links ({})".format(len(self._edge_colors), len(self._edge_links))
+            )
+
+        pipeline = PoseEstimationPipeline(
+            model=self,
+            image_processor=self._image_processor,
+            edge_links=self._edge_links,
+            edge_colors=self._edge_colors,
+            keypoint_colors=self._keypoint_colors,
+            post_prediction_callback=self.get_post_prediction_callback(conf=conf),
+            fuse_model=fuse_model,
+        )
+        return pipeline
+
+    def predict(self, images: ImageSource, conf: Optional[float] = None, batch_size: int = 32, fuse_model: bool = True) -> ImagesPoseEstimationPrediction:
+        """Predict an image or a list of images.
+
+        :param images:  Images to predict.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        :param batch_size:  Maximum number of images to process at the same time.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+        """
+        pipeline = self._get_pipeline(conf=conf, fuse_model=fuse_model)
+        return pipeline(images, batch_size=batch_size)  # type: ignore
+
+    def predict_webcam(self, conf: Optional[float] = None, fuse_model: bool = True):
+        """Predict using webcam.
+
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+        """
+        pipeline = self._get_pipeline(conf=conf, fuse_model=fuse_model)
+        pipeline.predict_webcam()
+
+    def train(self, mode: bool = True):
+        self._get_pipeline.cache_clear()
+        torch.cuda.empty_cache()
+        return super().train(mode)
 
 
 @register_model(Models.DEKR_W32_NO_DC)
 class DEKRW32NODC(DEKRPoseEstimationModel):
     """
     DEKR-W32 model for pose estimation without deformable convolutions.
     """
 
     def __init__(self, arch_params):
+        POSE_DEKR_W32_NO_DC_ARCH_PARAMS = get_arch_params("pose_dekr_w32_no_dc_arch_params")
+
         merged_arch_params = HpmStruct(**copy.deepcopy(POSE_DEKR_W32_NO_DC_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
         super().__init__(merged_arch_params)
 
 
 class DEKRWrapper(nn.Module):
     def __init__(self, model: DEKRPoseEstimationModel, apply_sigmoid=False):
@@ -548,19 +661,20 @@
         if self.apply_sigmoid:
             heatmap = torch.sigmoid(heatmap)
 
         return heatmap, offsets
 
 
 class DEKRHorisontalFlipWrapper(nn.Module):
-    def __init__(self, model: DEKRPoseEstimationModel, flip_indexes_heatmap, flip_indexes_offset, apply_sigmoid=False):
+    def __init__(self, model: DEKRPoseEstimationModel, flip_indexes, apply_sigmoid=False):
         super().__init__()
         self.model = model
-        self.flip_indexes_heatmap = torch.tensor(flip_indexes_heatmap).long()
-        self.flip_indexes_offset = torch.tensor(flip_indexes_offset).long()
+        # In DEKR the heatmap has one more channel for the center point of the pose, which is the last channel and it is not flipped
+        self.flip_indexes_heatmap = torch.tensor(list(flip_indexes) + [len(flip_indexes)]).long()
+        self.flip_indexes_offset = torch.tensor(flip_indexes).long()
         self.apply_sigmoid = apply_sigmoid
 
     def forward(self, inputs):
 
         input_flip = inputs.flip(3)
         input_flip[:, :, :, :-3] = input_flip[:, :, :, 3:]
```

## super_gradients/training/models/pose_estimation_models/rescoring_net.py

```diff
@@ -20,58 +20,58 @@
     joint configurations. So it may downweight confidence of impossible joint configurations.
 
     The model is a simple 3-layer MLP with ReLU activation. The input is the concatenation of the predicted poses and prior
     information in the form of the joint links. See RescoringNet.get_feature() for details.
     The output is a single scalar value.
     """
 
-    def __init__(self, num_classes: int, hidden_channels: int, num_layers: int, joint_links: List[Tuple[int, int]]):
+    def __init__(self, num_classes: int, hidden_channels: int, num_layers: int, edge_links: List[Tuple[int, int]]):
         super(PoseRescoringNet, self).__init__()
-        in_channels = len(joint_links) * 2 + len(joint_links) + num_classes  # [joint_relate, joint_length, visibility]
+        in_channels = len(edge_links) * 2 + len(edge_links) + num_classes  # [joint_relate, joint_length, visibility]
         layers = []
         for _ in range(num_layers):
             layers.append(nn.Linear(in_channels, hidden_channels, bias=True))
             layers.append(nn.ReLU())
             in_channels = hidden_channels
         self.layers = nn.Sequential(*layers)
         self.final = nn.Linear(hidden_channels, 1, bias=True)
-        self.joint_links = torch.tensor(joint_links).long()
+        self.edge_links = torch.tensor(edge_links).long()
 
     def forward(self, poses: Tensor) -> Tuple[Tensor, Tensor]:
         """
 
         :param x: Predicted poses or shape [N, J, 3] or [B, N, J, 3]
         :return: Tuple of input poses and corresponding scores
         """
 
-        x = self.get_feature(poses, self.joint_links)
+        x = self.get_feature(poses, self.edge_links)
         x = self.layers(x)
         y_pred = self.final(x)
         return poses, y_pred
 
     def init_weights(self):
         for m in self.modules():
             if isinstance(m, nn.Linear):
                 nn.init.kaiming_uniform_(m.weight, a=1)
                 nn.init.constant_(m.bias, 0)
 
     @classmethod
-    def get_feature(cls, poses: Tensor, joint_links: Tensor) -> Tensor:
+    def get_feature(cls, poses: Tensor, edge_links: Tensor) -> Tensor:
         """
         Compute the feature vector input to the rescoring network.
 
         :param poses: [N, J, 3] Predicted poses
-        :param joint_links: [L,2] List of joint indices
+        :param edge_links: [L,2] List of joint indices
         :return: [N, L*2+L+J] Feature vector
         """
         joint_xy = poses[..., :2]
         visibility = poses[..., 2]
 
-        joint_1 = joint_links[:, 0]
-        joint_2 = joint_links[:, 1]
+        joint_1 = edge_links[:, 0]
+        joint_2 = edge_links[:, 1]
 
         # To get the Delta x Delta y
         joint_relate = joint_xy[..., joint_1, :] - joint_xy[..., joint_2, :]  # [N, L, 2]
         joint_length = ((joint_relate**2)[..., 0] + (joint_relate**2)[..., 1]) ** (0.5)  # [N, L]
 
         # To use the torso distance to normalize
         normalize = (joint_length[..., 9] + joint_length[..., 11]) / 2  # [N] # NOTE: THIS IS COCO-SPECIFIC
@@ -95,9 +95,9 @@
         RESCORING_POSE_DEKR_ARCH_PARAMS = get_arch_params("pose_dekr_coco_rescoring_arch_params")
         merged_arch_params = HpmStruct(**copy.deepcopy(RESCORING_POSE_DEKR_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
         super().__init__(
             num_classes=merged_arch_params.num_classes,
             hidden_channels=merged_arch_params.hidden_channels,
             num_layers=merged_arch_params.num_layers,
-            joint_links=merged_arch_params.joint_links,
+            edge_links=merged_arch_params.edge_links,
         )
```

## super_gradients/training/pipelines/pipelines.py

```diff
@@ -2,33 +2,42 @@
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple, Union, Iterable
 from contextlib import contextmanager
 from tqdm import tqdm
 
 import numpy as np
 import torch
-from super_gradients.training.utils.utils import generate_batch
-from super_gradients.training.utils.media.video import load_video, includes_video_extension
-from super_gradients.training.utils.media.image import ImageSource, check_image_typing
-from super_gradients.training.utils.media.stream import WebcamStreaming
-from super_gradients.training.utils.detection_utils import DetectionPostPredictionCallback
-from super_gradients.training.models.sg_module import SgModule
-from super_gradients.training.models.prediction_results import (
+
+from super_gradients.training.utils.predict import (
+    ImagePoseEstimationPrediction,
+    ImagesPoseEstimationPrediction,
+    VideoPoseEstimationPrediction,
     ImagesDetectionPrediction,
     VideoDetectionPrediction,
     ImagePrediction,
     ImageDetectionPrediction,
     ImagesPredictions,
     VideoPredictions,
+    Prediction,
+    DetectionPrediction,
+    PoseEstimationPrediction,
+    ImageClassificationPrediction,
+    ImagesClassificationPrediction,
+    ClassificationPrediction,
 )
-from super_gradients.training.models.predictions import Prediction, DetectionPrediction
+from torch.nn.functional import softmax
+from super_gradients.training.utils.utils import generate_batch
+from super_gradients.training.utils.media.video import load_video, includes_video_extension
+from super_gradients.training.utils.media.image import ImageSource, check_image_typing
+from super_gradients.training.utils.media.stream import WebcamStreaming
+from super_gradients.training.utils.detection_utils import DetectionPostPredictionCallback
+from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.processing.processing import Processing, ComposeProcessing
 from super_gradients.common.abstractions.abstract_logger import get_logger
 
-
 logger = get_logger(__name__)
 
 
 @contextmanager
 def eval_mode(model: SgModule) -> None:
     """Set a model in evaluation mode, undo at the end.
 
@@ -43,27 +52,30 @@
 class Pipeline(ABC):
     """An abstract base class representing a processing pipeline for a specific task.
     The pipeline includes loading images, preprocessing, prediction, and postprocessing.
 
     :param model:           The model used for making predictions.
     :param image_processor: A single image processor or a list of image processors for preprocessing and postprocessing the images.
     :param device:          The device on which the model will be run. If None, will run on current model device. Use "cuda" for GPU support.
+    :param dtype:           Specify the dtype of the inputs. If None, will use the dtype of the model's parameters.
     :param fuse_model:                  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
     """
 
     def __init__(
         self,
         model: SgModule,
         image_processor: Union[Processing, List[Processing]],
         class_names: List[str],
         device: Optional[str] = None,
         fuse_model: bool = True,
+        dtype: Optional[torch.dtype] = None,
     ):
         self.device = device or next(model.parameters()).device
         self.model = model.to(self.device)
+        self.dtype = dtype or next(model.parameters()).dtype
         self.class_names = class_names
 
         if isinstance(image_processor, list):
             image_processor = ComposeProcessing(image_processor)
         self.image_processor = image_processor
 
         self.fuse_model = fuse_model  # If True, the model will be fused in the first forward pass, to make sure it gets the right input_size
@@ -82,15 +94,15 @@
             - str:              A string representing either a video, an image or an URL.
             - numpy.ndarray:    A numpy array representing the image
             - torch.Tensor:     A PyTorch tensor representing the image
             - PIL.Image.Image:  A PIL Image object
             - List:             A list of images of any of the above image types (list of videos not supported).
 
         :param inputs:      inputs to the model, which can be any of the above-mentioned types.
-        :param batch_size:  Number of images to be processed at the same time.
+        :param batch_size:  Maximum number of images to process at the same time.
         :return:            Results of the prediction.
         """
 
         if includes_video_extension(inputs):
             return self.predict_video(inputs, batch_size)
         elif check_image_typing(inputs):
             return self.predict_images(inputs, batch_size)
@@ -167,14 +179,15 @@
             preprocessed_image, processing_metadata = self.image_processor.preprocess_image(image=image.copy())
             preprocessed_images.append(preprocessed_image)
             processing_metadatas.append(processing_metadata)
 
         # Predict
         with eval_mode(self.model), torch.no_grad(), torch.cuda.amp.autocast():
             torch_inputs = torch.from_numpy(np.array(preprocessed_images)).to(self.device)
+            torch_inputs = torch_inputs.to(self.dtype)
             if self.fuse_model:
                 self._fuse_model(torch_inputs)
             model_output = self.model(torch_inputs)
             predictions = self._decode_model_output(model_output, model_input=torch_inputs)
 
         # Postprocess
         postprocessed_predictions = []
@@ -294,7 +307,138 @@
         return ImagesDetectionPrediction(_images_prediction_lst=images_predictions)
 
     def _combine_image_prediction_to_video(
         self, images_predictions: Iterable[ImageDetectionPrediction], fps: float, n_images: Optional[int] = None
     ) -> VideoDetectionPrediction:
         images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Video")]
         return VideoDetectionPrediction(_images_prediction_lst=images_predictions, fps=fps)
+
+
+class PoseEstimationPipeline(Pipeline):
+    """Pipeline specifically designed for pose estimation tasks.
+    The pipeline includes loading images, preprocessing, prediction, and postprocessing.
+
+    :param model:                       The object detection model (instance of SgModule) used for making predictions.
+    :param post_prediction_callback:    Callback function to process raw predictions from the model.
+    :param image_processor:             Single image processor or a list of image processors for preprocessing and postprocessing the images.
+    :param device:                      The device on which the model will be run. If None, will run on current model device. Use "cuda" for GPU support.
+    :param fuse_model:                  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+    """
+
+    def __init__(
+        self,
+        model: SgModule,
+        edge_links: Union[np.ndarray, List[Tuple[int, int]]],
+        edge_colors: Union[np.ndarray, List[Tuple[int, int, int]]],
+        keypoint_colors: Union[np.ndarray, List[Tuple[int, int, int]]],
+        post_prediction_callback,
+        device: Optional[str] = None,
+        image_processor: Optional[Processing] = None,
+        fuse_model: bool = True,
+    ):
+        super().__init__(model=model, device=device, image_processor=image_processor, class_names=None, fuse_model=fuse_model)
+        self.post_prediction_callback = post_prediction_callback
+        self.edge_links = np.asarray(edge_links, dtype=int)
+        self.edge_colors = np.asarray(edge_colors, dtype=int)
+        self.keypoint_colors = np.asarray(keypoint_colors, dtype=int)
+
+    def _decode_model_output(self, model_output: Union[List, Tuple, torch.Tensor], model_input: np.ndarray) -> List[PoseEstimationPrediction]:
+        """Decode the model output, by applying post prediction callback. This includes NMS.
+
+        :param model_output:    Direct output of the model, without any post-processing.
+        :param model_input:     Model input (i.e. images after preprocessing).
+        :return:                Predicted Bboxes.
+        """
+        all_poses, all_scores = self.post_prediction_callback(model_output)
+
+        predictions = []
+        for poses, scores, image in zip(all_poses, all_scores, model_input):
+            predictions.append(
+                PoseEstimationPrediction(
+                    poses=poses,
+                    scores=scores,
+                    image_shape=image.shape,
+                    edge_links=self.edge_links,
+                    edge_colors=self.edge_colors,
+                    keypoint_colors=self.keypoint_colors,
+                )
+            )
+
+        return predictions
+
+    def _instantiate_image_prediction(self, image: np.ndarray, prediction: PoseEstimationPrediction) -> ImagePrediction:
+        return ImagePoseEstimationPrediction(image=image, prediction=prediction, class_names=self.class_names)
+
+    def _combine_image_prediction_to_images(
+        self, images_predictions: Iterable[PoseEstimationPrediction], n_images: Optional[int] = None
+    ) -> ImagesPoseEstimationPrediction:
+        if n_images is not None and n_images == 1:
+            # Do not show tqdm progress bar if there is only one image
+            images_predictions = [next(iter(images_predictions))]
+        else:
+            images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Images")]
+
+        return ImagesPoseEstimationPrediction(_images_prediction_lst=images_predictions)
+
+    def _combine_image_prediction_to_video(
+        self, images_predictions: Iterable[ImageDetectionPrediction], fps: float, n_images: Optional[int] = None
+    ) -> VideoPoseEstimationPrediction:
+        images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Video")]
+        return VideoPoseEstimationPrediction(_images_prediction_lst=images_predictions, fps=fps)
+
+
+class ClassificationPipeline(Pipeline):
+    """Pipeline specifically designed for Image Classification tasks.
+    The pipeline includes loading images, preprocessing, prediction, and postprocessing.
+
+    :param model:                       The classification model (instance of SgModule) used for making predictions.
+    :param class_names:                 List of class names corresponding to the model's output classes.
+    :param image_processor:             Single image processor or a list of image processors for preprocessing and postprocessing the images.
+    :param device:                      The device on which the model will be run. If None, will run on current model device. Use "cuda" for GPU support.
+    :param fuse_model:                  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
+    """
+
+    def __init__(
+        self,
+        model: SgModule,
+        class_names: List[str],
+        device: Optional[str] = None,
+        image_processor: Optional[Processing] = None,
+        fuse_model: bool = True,
+    ):
+        super().__init__(model=model, device=device, image_processor=image_processor, class_names=class_names, fuse_model=fuse_model)
+
+    def _decode_model_output(self, model_output: Union[List, Tuple, torch.Tensor], model_input: np.ndarray) -> List[ClassificationPrediction]:
+        """Decode the model output
+
+        :param model_output:    Direct output of the model, without any post-processing.
+        :param model_input:     Model input (i.e. images after preprocessing).
+        :return:                Predicted Bboxes.
+        """
+        confidence_predictions, classifier_predictions = torch.max(model_output, 1)
+
+        classifier_predictions = classifier_predictions.detach().cpu().numpy()
+        confidence_predictions = softmax(confidence_predictions).detach().cpu().numpy()
+
+        predictions = list()
+        for prediction, confidence, image_input in zip(classifier_predictions, confidence_predictions, model_input):
+            predictions.append(ClassificationPrediction(confidence=float(confidence), labels=int(prediction), image_shape=image_input.shape))
+        return predictions
+
+    def _instantiate_image_prediction(self, image: np.ndarray, prediction: ClassificationPrediction) -> ImagePrediction:
+        return ImageClassificationPrediction(image=image, prediction=prediction, class_names=self.class_names)
+
+    def _combine_image_prediction_to_images(
+        self, images_predictions: Iterable[ImageClassificationPrediction], n_images: Optional[int] = None
+    ) -> ImagesClassificationPrediction:
+        if n_images is not None and n_images == 1:
+            # Do not show tqdm progress bar if there is only one image
+            images_predictions = [next(iter(images_predictions))]
+        else:
+            images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Images")]
+
+        return ImagesClassificationPrediction(_images_prediction_lst=images_predictions)
+
+    def _combine_image_prediction_to_video(
+        self, images_predictions: Iterable[ImageDetectionPrediction], fps: float, n_images: Optional[int] = None
+    ) -> ImagesClassificationPrediction:
+        raise NotImplementedError("This feature is not available for Classification task")
```

## super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py

```diff
@@ -102,22 +102,23 @@
             arch_params=cfg.arch_params,
             strict_load=cfg.checkpoint_params.strict_load,
             pretrained_weights=cfg.checkpoint_params.pretrained_weights,
             checkpoint_path=cfg.checkpoint_params.checkpoint_path,
             load_backbone=cfg.checkpoint_params.load_backbone,
         )
         tmp_cfg = deepcopy(cfg)
-        tmp_cfg.training_hyperparamsbatch_accumulate = 1
-        tmp_cfg.training_hyperparamsmax_train_batches = self.num_forward_passes
-        tmp_cfg.training_hyperparamsrun_validation_freq = 2
-        tmp_cfg.training_hyperparamssilent_mode = True
-        tmp_cfg.training_hyperparamssave_model = False
-        tmp_cfg.training_hyperparamsmax_epochs = 1
-        tmp_cfg.training_hyperparamsaverage_best_models = False
-        tmp_cfg.training_hyperparamskill_ddp_pgroup_on_end = False
+        tmp_cfg.training_hyperparams.batch_accumulate = 1
+        tmp_cfg.training_hyperparams.max_train_batches = self.num_forward_passes
+        tmp_cfg.training_hyperparams.run_validation_freq = 2
+        tmp_cfg.training_hyperparams.run_test_freq = 2
+        tmp_cfg.training_hyperparams.silent_mode = True
+        tmp_cfg.training_hyperparams.save_model = False
+        tmp_cfg.training_hyperparams.max_epochs = 1
+        tmp_cfg.training_hyperparams.average_best_models = False
+        tmp_cfg.training_hyperparams.kill_ddp_pgroup_on_end = False
         tmp_cfg.pre_launch_callbacks_list = []
 
         fastest_batch_time = np.inf
         fastest_batch_size = curr_batch_size
 
         bs_found = False
```

## super_gradients/training/processing/processing.py

```diff
@@ -1,26 +1,29 @@
-from typing import Tuple, List, Union
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from typing import Tuple, List, Union
 
 import numpy as np
+from PIL import Image
 
+from super_gradients.common.object_names import Processings
 from super_gradients.common.registry.registry import register_processing
-from super_gradients.training.datasets.datasets_conf import COCO_DETECTION_CLASSES_LIST
-from super_gradients.training.models.predictions import Prediction, DetectionPrediction
+from super_gradients.training.datasets.datasets_conf import COCO_DETECTION_CLASSES_LIST, IMAGENET_CLASSES
 from super_gradients.training.transforms.utils import (
     _rescale_image,
     _rescale_bboxes,
     _get_center_padding_coordinates,
     _get_bottom_right_padding_coordinates,
     _pad_image,
     _shift_bboxes,
     PaddingCoordinates,
+    _rescale_keypoints,
+    _shift_keypoints,
 )
-from super_gradients.common.object_names import Processings
+from super_gradients.training.utils.predict import Prediction, DetectionPrediction, PoseEstimationPrediction
 
 
 @dataclass
 class ProcessingMetadata(ABC):
     """Metadata including information to postprocess a prediction."""
 
 
@@ -192,37 +195,73 @@
         return predictions
 
     @abstractmethod
     def _get_padding_params(self, input_shape: Tuple[int, int]) -> PaddingCoordinates:
         pass
 
 
+class _KeypointsPadding(Processing, ABC):
+    """Base class for keypoints padding methods. One should implement the `_get_padding_params` method to work with a custom padding method.
+
+    Note: This transformation assume that dimensions of input image is equal or less than `output_shape`.
+
+    :param output_shape: Output image shape (H, W)
+    :param pad_value:   Padding value for image
+    """
+
+    def __init__(self, output_shape: Tuple[int, int], pad_value: int):
+        self.output_shape = output_shape
+        self.pad_value = pad_value
+
+    def preprocess_image(self, image: np.ndarray) -> Tuple[np.ndarray, DetectionPadToSizeMetadata]:
+        padding_coordinates = self._get_padding_params(input_shape=image.shape)
+        processed_image = _pad_image(image=image, padding_coordinates=padding_coordinates, pad_value=self.pad_value)
+        return processed_image, DetectionPadToSizeMetadata(padding_coordinates=padding_coordinates)
+
+    def postprocess_predictions(self, predictions: PoseEstimationPrediction, metadata: DetectionPadToSizeMetadata) -> PoseEstimationPrediction:
+        predictions.poses = _shift_keypoints(
+            targets=predictions.poses,
+            shift_h=-metadata.padding_coordinates.top,
+            shift_w=-metadata.padding_coordinates.left,
+        )
+        return predictions
+
+    @abstractmethod
+    def _get_padding_params(self, input_shape: Tuple[int, int]) -> PaddingCoordinates:
+        pass
+
+
 @register_processing(Processings.DetectionCenterPadding)
 class DetectionCenterPadding(_DetectionPadding):
     def _get_padding_params(self, input_shape: Tuple[int, int]) -> PaddingCoordinates:
         return _get_center_padding_coordinates(input_shape=input_shape, output_shape=self.output_shape)
 
 
 @register_processing(Processings.DetectionBottomRightPadding)
 class DetectionBottomRightPadding(_DetectionPadding):
     def _get_padding_params(self, input_shape: Tuple[int, int]) -> PaddingCoordinates:
         return _get_bottom_right_padding_coordinates(input_shape=input_shape, output_shape=self.output_shape)
 
 
+@register_processing(Processings.KeypointsBottomRightPadding)
+class KeypointsBottomRightPadding(_KeypointsPadding):
+    def _get_padding_params(self, input_shape: Tuple[int, int]) -> PaddingCoordinates:
+        return _get_bottom_right_padding_coordinates(input_shape=input_shape, output_shape=self.output_shape)
+
+
 class _Rescale(Processing, ABC):
     """Resize image to given image dimensions WITHOUT preserving aspect ratio.
 
     :param output_shape: (H, W)
     """
 
     def __init__(self, output_shape: Tuple[int, int]):
         self.output_shape = output_shape
 
     def preprocess_image(self, image: np.ndarray) -> Tuple[np.ndarray, RescaleMetadata]:
-
         scale_factor_h, scale_factor_w = self.output_shape[0] / image.shape[0], self.output_shape[1] / image.shape[1]
         rescaled_image = _rescale_image(image, target_shape=self.output_shape)
 
         return rescaled_image, RescaleMetadata(original_shape=image.shape[:2], scale_factor_h=scale_factor_h, scale_factor_w=scale_factor_w)
 
 
 class _LongestMaxSizeRescale(Processing, ABC):
@@ -255,14 +294,73 @@
 @register_processing(Processings.DetectionLongestMaxSizeRescale)
 class DetectionLongestMaxSizeRescale(_LongestMaxSizeRescale):
     def postprocess_predictions(self, predictions: DetectionPrediction, metadata: RescaleMetadata) -> DetectionPrediction:
         predictions.bboxes_xyxy = _rescale_bboxes(targets=predictions.bboxes_xyxy, scale_factors=(1 / metadata.scale_factor_h, 1 / metadata.scale_factor_w))
         return predictions
 
 
+@register_processing(Processings.KeypointsLongestMaxSizeRescale)
+class KeypointsLongestMaxSizeRescale(_LongestMaxSizeRescale):
+    def postprocess_predictions(self, predictions: PoseEstimationPrediction, metadata: RescaleMetadata) -> PoseEstimationPrediction:
+        predictions.poses = _rescale_keypoints(targets=predictions.poses, scale_factors=(1 / metadata.scale_factor_h, 1 / metadata.scale_factor_w))
+        return predictions
+
+
+class ClassificationProcess(Processing, ABC):
+    def postprocess_predictions(self, predictions: Prediction, metadata: None) -> Prediction:
+        return predictions
+
+
+@register_processing(Processings.Resize)
+class Resize(ClassificationProcess):
+    def __init__(self, size: int = 224):
+        super().__init__()
+        self.size = size
+
+    def preprocess_image(self, image: np.ndarray) -> Tuple[np.ndarray, None]:
+        """Resize an image.
+
+        :param image: Image, in (H, W, C) format.
+        :return:      The resized image.
+        """
+        image = Image.fromarray(image)
+        resized_image = image.resize((self.size, self.size))
+        resized_image = np.array(resized_image)
+
+        return resized_image, None
+
+
+@register_processing(Processings.CenterCrop)
+class CenterCrop(ClassificationProcess):
+    """
+    :param size: Desired output size of the crop.
+    """
+
+    def __init__(self, size: int = 224):
+        super().__init__()
+        self.size = size
+
+    def preprocess_image(self, image: np.ndarray) -> Tuple[np.ndarray, None]:
+        """Crops the given image at the center.
+
+        :param image: Image, in (H, W, C) format.
+        :return:      The center cropped image.
+        """
+        height, width = image.shape[0], image.shape[1]
+
+        # Calculate the start and end coordinates of the crop.
+        start_x = (width - self.size) // 2
+        start_y = (height - self.size) // 2
+        end_x = start_x + self.size
+        end_y = start_y + self.size
+
+        cropped_image = image[start_y:end_y, start_x:end_x]
+        return cropped_image, None
+
+
 def default_yolox_coco_processing_params() -> dict:
     """Processing parameters commonly used for training YoloX on COCO dataset.
     TODO: remove once we load it from the checkpoint
     """
 
     image_processor = ComposeProcessing(
         [
@@ -324,19 +422,119 @@
         image_processor=image_processor,
         iou=0.7,
         conf=0.25,
     )
     return params
 
 
+def default_dekr_coco_processing_params() -> dict:
+    """Processing parameters commonly used for training DEKR on COCO dataset."""
+
+    image_processor = ComposeProcessing(
+        [
+            ReverseImageChannels(),
+            KeypointsLongestMaxSizeRescale(output_shape=(640, 640)),
+            KeypointsBottomRightPadding(output_shape=(640, 640), pad_value=127),
+            StandardizeImage(max_value=255.0),
+            NormalizeImage(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+            ImagePermute(permutation=(2, 0, 1)),
+        ]
+    )
+
+    edge_links = [
+        [0, 1],
+        [0, 2],
+        [1, 2],
+        [1, 3],
+        [2, 4],
+        [3, 5],
+        [4, 6],
+        [5, 6],
+        [5, 7],
+        [5, 11],
+        [6, 8],
+        [6, 12],
+        [7, 9],
+        [8, 10],
+        [11, 12],
+        [11, 13],
+        [12, 14],
+        [13, 15],
+        [14, 16],
+    ]
+
+    edge_colors = [
+        (214, 39, 40),  # Nose -> LeftEye
+        (148, 103, 189),  # Nose -> RightEye
+        (44, 160, 44),  # LeftEye -> RightEye
+        (140, 86, 75),  # LeftEye -> LeftEar
+        (227, 119, 194),  # RightEye -> RightEar
+        (127, 127, 127),  # LeftEar -> LeftShoulder
+        (188, 189, 34),  # RightEar -> RightShoulder
+        (127, 127, 127),  # Shoulders
+        (188, 189, 34),  # LeftShoulder -> LeftElbow
+        (140, 86, 75),  # LeftTorso
+        (23, 190, 207),  # RightShoulder -> RightElbow
+        (227, 119, 194),  # RightTorso
+        (31, 119, 180),  # LeftElbow -> LeftArm
+        (255, 127, 14),  # RightElbow -> RightArm
+        (148, 103, 189),  # Waist
+        (255, 127, 14),  # Left Hip -> Left Knee
+        (214, 39, 40),  # Right Hip -> Right Knee
+        (31, 119, 180),  # Left Knee -> Left Ankle
+        (44, 160, 44),  # Right Knee -> Right Ankle
+    ]
+
+    keypoint_colors = [
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+        (31, 119, 180),
+        (148, 103, 189),
+    ]
+    params = dict(image_processor=image_processor, conf=0.05, edge_links=edge_links, edge_colors=edge_colors, keypoint_colors=keypoint_colors)
+    return params
+
+
+def default_resnet_imagenet_processing_params() -> dict:
+    """Processing parameters commonly used for training resnet on Imagenet dataset."""
+    image_processor = ComposeProcessing(
+        [Resize(size=256), CenterCrop(size=224), NormalizeImage(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]), StandardizeImage(), ImagePermute()]
+    )
+    params = dict(
+        class_names=IMAGENET_CLASSES,
+        image_processor=image_processor,
+    )
+    return params
+
+
 def get_pretrained_processing_params(model_name: str, pretrained_weights: str) -> dict:
     """Get the processing parameters for a pretrained model.
     TODO: remove once we load it from the checkpoint
     """
     if pretrained_weights == "coco":
         if "yolox" in model_name:
             return default_yolox_coco_processing_params()
         elif "ppyoloe" in model_name:
             return default_ppyoloe_coco_processing_params()
         elif "yolo_nas" in model_name:
             return default_yolo_nas_coco_processing_params()
+
+    if pretrained_weights == "coco_pose" and model_name in ("dekr_w32_no_dc", "dekr_custom"):
+        return default_dekr_coco_processing_params()
+
+    if pretrained_weights == "imagenet" and model_name == "resnet18":
+        return default_resnet_imagenet_processing_params()
+
     return dict()
```

## super_gradients/training/sg_trainer/sg_trainer.py

```diff
@@ -1,13 +1,13 @@
 import copy
 import inspect
 import os
 from copy import deepcopy
 from pathlib import Path
-from typing import Union, Tuple, Mapping, Dict, Any, List
+from typing import Union, Tuple, Mapping, Dict, Any, List, Optional
 
 import hydra
 import numpy as np
 import torch
 import torch.cuda
 import torch.nn
 import torchmetrics
@@ -16,43 +16,45 @@
 from torch import nn
 from torch.cuda.amp import GradScaler, autocast
 from torch.utils.data import DataLoader, SequentialSampler
 from torch.utils.data.distributed import DistributedSampler
 from torchmetrics import MetricCollection, Metric
 from tqdm import tqdm
 
+from super_gradients import is_distributed
 from super_gradients.common.environment.checkpoints_dir_utils import get_checkpoints_dir_path, get_ckpt_local_path
 from super_gradients.module_interfaces import HasPreprocessingParams, HasPredict
 from super_gradients.modules.repvgg_block import fuse_repvgg_blocks_residual_branches
 
 from super_gradients.training.utils.sg_trainer_utils import get_callable_param_names
+from super_gradients.training.utils.callbacks.callbacks import create_lr_scheduler_callback, LRSchedulerCallback
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.sg_loggers.abstract_sg_logger import AbstractSGLogger
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.data_types.enum import MultiGPUMode, StrictLoad, EvaluationType
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.callbacks_factory import CallbacksFactory
 from super_gradients.common.factories.list_factory import ListFactory
 from super_gradients.common.factories.losses_factory import LossesFactory
 from super_gradients.common.factories.metrics_factory import MetricsFactory
 
 from super_gradients.training import utils as core_utils, models, dataloaders
 from super_gradients.training.datasets.samplers import RepeatAugSampler
-from super_gradients.training.exceptions.sg_trainer_exceptions import UnsupportedOptimizerFormat
+from super_gradients.common.exceptions.sg_trainer_exceptions import UnsupportedOptimizerFormat
 from super_gradients.training.metrics.metric_utils import (
     get_metrics_titles,
     get_metrics_results_tuple,
     get_logging_values,
     get_metrics_dict,
     get_train_loop_description_dict,
 )
 from super_gradients.training.models import SgModule, get_model_name
 from super_gradients.common.registry.registry import ARCHITECTURES, SG_LOGGERS
 from super_gradients.training.pretrained_models import PRETRAINED_NUM_CLASSES
-from super_gradients.training.utils import sg_trainer_utils, get_param
+from super_gradients.training.utils import sg_trainer_utils, get_param, torch_version_is_greater_or_equal
 from super_gradients.training.utils.distributed_training_utils import (
     MultiGPUModeAutocastWrapper,
     reduce_results_tuple_for_ddp,
     compute_precise_bn_stats,
     setup_device,
     get_gpu_mem_utilization,
     get_world_size,
@@ -62,33 +64,32 @@
     is_ddp_subprocess,
     wait_for_the_master,
     DDPNotSetupException,
 )
 from super_gradients.training.utils.ema import ModelEMA
 from super_gradients.training.utils.optimizer_utils import build_optimizer
 from super_gradients.training.utils.sg_trainer_utils import MonitoredValue, log_main_training_params
-from super_gradients.training.utils.utils import fuzzy_idx_in_list
+from super_gradients.training.utils.utils import fuzzy_idx_in_list, unwrap_model
 from super_gradients.training.utils.weight_averaging_utils import ModelWeightAveraging
 from super_gradients.training.metrics import Accuracy, Top5
 from super_gradients.training.utils import random_seed
 from super_gradients.training.utils.checkpoint_utils import (
     read_ckpt_state_dict,
     load_checkpoint_to_model,
     load_pretrained_weights,
 )
 from super_gradients.training.datasets.datasets_utils import DatasetStatisticsTensorboardLogger
 from super_gradients.training.utils.callbacks import (
     CallbackHandler,
     Phase,
     PhaseContext,
     MetricsUpdateCallback,
-    ContextSgMethods,
     LRCallbackBase,
 )
-from super_gradients.common.registry.registry import LR_SCHEDULERS_CLS_DICT, LR_WARMUP_CLS_DICT
+from super_gradients.common.registry.registry import LR_WARMUP_CLS_DICT
 from super_gradients.common.environment.device_utils import device_config
 from super_gradients.training.utils import HpmStruct
 from super_gradients.common.environment.cfg_utils import load_experiment_cfg, add_params_to_cfg, load_recipe
 from super_gradients.common.factories.pre_launch_callbacks_factory import PreLaunchCallbacksFactory
 from super_gradients.training.params import TrainingParams
 
 logger = get_logger(__name__)
@@ -146,15 +147,15 @@
             )
 
         if require_ddp_setup():
             raise DDPNotSetupException()
 
         # SET THE EMPTY PROPERTIES
         self.net, self.architecture, self.arch_params, self.dataset_interface = None, None, None, None
-        self.train_loader, self.valid_loader = None, None
+        self.train_loader, self.valid_loader, self.test_loaders = None, None, {}
         self.ema = None
         self.ema_model = None
         self.sg_logger = None
         self.update_param_groups = None
         self.criterion = None
         self.training_params = None
         self.scaler = None
@@ -177,16 +178,17 @@
         self.strict_load = StrictLoad.ON
         self.load_ema_as_net = False
         self.ckpt_best_name = "ckpt_best.pth"
         self._first_backward = True
 
         # METRICS
         self.loss_logging_items_names = None
-        self.train_metrics = None
-        self.valid_metrics = None
+        self.train_metrics: Optional[MetricCollection] = None
+        self.valid_metrics: Optional[MetricCollection] = None
+        self.test_metrics: Optional[MetricCollection] = None
         self.greater_metric_to_watch_is_better = None
         self.metric_to_watch = None
         self.greater_train_metrics_is_better: Dict[str, bool] = {}  # For each metric, indicates if greater is better
         self.greater_valid_metrics_is_better: Dict[str, bool] = {}
 
         # SETTING THE PROPERTIES FROM THE CONSTRUCTOR
         self.experiment_name = experiment_name
@@ -204,18 +206,20 @@
 
         default_train_metrics, default_valid_metrics = MetricCollection([Accuracy(), Top5()]), MetricCollection([Accuracy(), Top5()])
 
         self.train_metrics, self.valid_metrics = default_train_metrics, default_valid_metrics
 
         self.train_monitored_values = {}
         self.valid_monitored_values = {}
+        self.test_monitored_values = {}
         self.max_train_batches = None
         self.max_valid_batches = None
 
         self._epoch_start_logging_values = {}
+        self._torch_lr_scheduler = None
 
     @property
     def device(self) -> str:
         return device_config.device
 
     @classmethod
     def train_from_config(cls, cfg: Union[DictConfig, dict]) -> Tuple[nn.Module, Tuple]:
@@ -267,14 +271,15 @@
 
         recipe_logged_cfg = {"recipe_config": OmegaConf.to_container(cfg, resolve=True)}
         # TRAIN
         res = trainer.train(
             model=model,
             train_loader=train_dataloader,
             valid_loader=val_dataloader,
+            test_loaders=None,  # TODO: Add option to set test_loaders in recipe
             training_params=cfg.training_hyperparams,
             additional_configs_to_log=recipe_logged_cfg,
         )
 
         return model, res
 
     @classmethod
@@ -320,20 +325,22 @@
         trainer = Trainer(experiment_name=cfg.experiment_name, ckpt_root_dir=cfg.ckpt_root_dir)
 
         # INSTANTIATE DATA LOADERS
         val_dataloader = dataloaders.get(
             name=cfg.val_dataloader, dataset_params=cfg.dataset_params.val_dataset_params, dataloader_params=cfg.dataset_params.val_dataloader_params
         )
 
-        if cfg.checkpoint_params.pretrained_weights is None and cfg.checkpoint_params.checkpoint_path is None:
+        if cfg.checkpoint_params.checkpoint_path is None:
             logger.info(
                 "checkpoint_params.checkpoint_path was not provided, " "so the recipe will be evaluated using checkpoints_dir/training_hyperparams.ckpt_name"
             )
-            checkpoints_dir = Path(get_checkpoints_dir_path(experiment_name=cfg.experiment_name, ckpt_root_dir=cfg.ckpt_root_dir))
-            cfg.checkpoint_params.checkpoint_path = str(checkpoints_dir / cfg.training_hyperparams.ckpt_name)
+            checkpoints_dir = get_checkpoints_dir_path(experiment_name=cfg.experiment_name, ckpt_root_dir=cfg.ckpt_root_dir)
+            checkpoint_path = os.path.join(checkpoints_dir, cfg.training_hyperparams.ckpt_name)
+            if os.path.exists(checkpoint_path):
+                cfg.checkpoint_params.checkpoint_path = checkpoint_path
 
         logger.info(f"Evaluating checkpoint: {cfg.checkpoint_params.checkpoint_path}")
 
         # BUILD NETWORK
         model = models.get(
             model_name=cfg.architecture,
             num_classes=cfg.arch_params.num_classes,
@@ -371,78 +378,54 @@
         :param ckpt_root_dir:       Directory including the checkpoints
         """
         logger.info("Evaluate checkpoint")
         cfg = load_experiment_cfg(experiment_name, ckpt_root_dir)
         add_params_to_cfg(cfg, params=["training_hyperparams.resume=True", f"ckpt_name={ckpt_name}"])
         cls.evaluate_from_recipe(cfg)
 
-    def _set_dataset_params(self):
-        self.dataset_params = {
-            "train_dataset_params": self.train_loader.dataset.dataset_params if hasattr(self.train_loader.dataset, "dataset_params") else None,
-            "train_dataloader_params": self.train_loader.dataloader_params if hasattr(self.train_loader, "dataloader_params") else None,
-            "valid_dataset_params": self.valid_loader.dataset.dataset_params if hasattr(self.valid_loader.dataset, "dataset_params") else None,
-            "valid_dataloader_params": self.valid_loader.dataloader_params if hasattr(self.valid_loader, "dataloader_params") else None,
-        }
-        self.dataset_params = HpmStruct(**self.dataset_params)
-
     def _net_to_device(self):
         """
         Manipulates self.net according to device.multi_gpu
         """
         self.net.to(device_config.device)
 
         # FOR MULTI-GPU TRAINING (not distributed)
         sync_bn = core_utils.get_param(self.training_params, "sync_bn", default_val=False)
         if device_config.multi_gpu == MultiGPUMode.DATA_PARALLEL:
             self.net = torch.nn.DataParallel(self.net, device_ids=get_device_ids())
         elif device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL:
             if sync_bn:
                 if not self.ddp_silent_mode:
                     logger.info("DDP - Using Sync Batch Norm... Training time will be affected accordingly")
-                self.net = torch.nn.SyncBatchNorm.convert_sync_batchnorm(self.net).to(device_config.device)
+                self.net = torch.nn.SyncBatchNorm.convert_sync_batchnorm(self.net)
 
             local_rank = int(device_config.device.split(":")[1])
             self.net = torch.nn.parallel.DistributedDataParallel(self.net, device_ids=[local_rank], output_device=local_rank, find_unused_parameters=True)
 
-        else:
-            self.net = core_utils.WrappedModel(self.net)
-
-    def _train_epoch(self, epoch: int, silent_mode: bool = False) -> tuple:
+    def _train_epoch(self, context: PhaseContext, silent_mode: bool = False) -> tuple:
         """
         train_epoch - A single epoch training procedure
             :param optimizer:   The optimizer for the network
             :param epoch:       The current epoch
             :param silent_mode: No verbosity
         """
         # SET THE MODEL IN training STATE
         self.net.train()
 
         # THE DISABLE FLAG CONTROLS WHETHER THE PROGRESS BAR IS SILENT OR PRINTS THE LOGS
         with tqdm(self.train_loader, bar_format="{l_bar}{bar:10}{r_bar}", dynamic_ncols=True, disable=silent_mode) as progress_bar_train_loader:
-            progress_bar_train_loader.set_description(f"Train epoch {epoch}")
+            progress_bar_train_loader.set_description(f"Train epoch {context.epoch}")
 
             # RESET/INIT THE METRIC LOGGERS
             self._reset_metrics()
 
             self.train_metrics.to(device_config.device)
             loss_avg_meter = core_utils.utils.AverageMeter()
 
-            context = PhaseContext(
-                epoch=epoch,
-                optimizer=self.optimizer,
-                metrics_compute_fn=self.train_metrics,
-                loss_avg_meter=loss_avg_meter,
-                criterion=self.criterion,
-                device=device_config.device,
-                lr_warmup_epochs=self.training_params.lr_warmup_epochs,
-                sg_logger=self.sg_logger,
-                train_loader=self.train_loader,
-                context_methods=self._get_context_methods(Phase.TRAIN_BATCH_END),
-                ddp_silent_mode=self.ddp_silent_mode,
-            )
+            context.update_context(loss_avg_meter=loss_avg_meter, metrics_compute_fn=self.train_metrics)
 
             for batch_idx, batch_items in enumerate(progress_bar_train_loader):
                 batch_items = core_utils.tensor_container_to_device(batch_items, device_config.device, non_blocking=True)
                 inputs, targets, additional_batch_items = sg_trainer_utils.unpack_batch_items(batch_items)
 
                 if self.pre_prediction_callback is not None:
                     inputs, targets = self.pre_prediction_callback(inputs, targets, batch_idx)
@@ -460,15 +443,15 @@
 
                 context.update_context(preds=outputs, loss_log_items=loss_log_items)
                 self.phase_callback_handler.on_train_batch_loss_end(context)
 
                 if not self.ddp_silent_mode and batch_idx == 0:
                     self._epoch_start_logging_values = self._get_epoch_start_logging_values()
 
-                self._backward_step(loss, epoch, batch_idx, context)
+                self._backward_step(loss, context.epoch, batch_idx, context)
 
                 # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
                 logging_values = loss_avg_meter.average + get_metrics_results_tuple(self.train_metrics)
                 gpu_memory_utilization = get_gpu_mem_utilization() / 1e9 if torch.cuda.is_available() else 0
 
                 # RENDER METRICS PROGRESS
                 pbar_message_dict = get_train_loop_description_dict(
@@ -510,36 +493,55 @@
                 + ", and "
                 + str(len(self.loss_logging_items_names))
             )
         # RETURN AND THE LOSS LOGGING ITEMS COMPUTED DURING LOSS FORWARD PASS
         return loss, loss_logging_items
 
     def _init_monitored_items(self):
-        self.metric_idx_in_results_tuple = fuzzy_idx_in_list(self.metric_to_watch, self.loss_logging_items_names + get_metrics_titles(self.valid_metrics))
         # Instantiate the values to monitor (loss/metric)
         for loss_name in self.loss_logging_items_names:
             self.train_monitored_values[loss_name] = MonitoredValue(name=loss_name, greater_is_better=False)
             self.valid_monitored_values[loss_name] = MonitoredValue(name=loss_name, greater_is_better=False)
 
         for metric_name in get_metrics_titles(self.train_metrics):
             self.train_monitored_values[metric_name] = MonitoredValue(name=metric_name, greater_is_better=self.greater_train_metrics_is_better.get(metric_name))
 
         for metric_name in get_metrics_titles(self.valid_metrics):
             self.valid_monitored_values[metric_name] = MonitoredValue(name=metric_name, greater_is_better=self.greater_valid_metrics_is_better.get(metric_name))
 
-        self.results_titles = ["Train_" + t for t in self.loss_logging_items_names + get_metrics_titles(self.train_metrics)] + [
-            "Valid_" + t for t in self.loss_logging_items_names + get_metrics_titles(self.valid_metrics)
-        ]
+        for dataset_name in self.test_loaders.keys():
+            for loss_name in self.loss_logging_items_names:
+                loss_full_name = f"{dataset_name}:{loss_name}" if dataset_name else loss_name
+                self.test_monitored_values[loss_full_name] = MonitoredValue(
+                    name=f"{dataset_name}:{loss_name}",
+                    greater_is_better=False,
+                )
+            for metric_name in get_metrics_titles(self.test_metrics):
+                metric_full_name = f"{dataset_name}:{metric_name}" if dataset_name else metric_name
+                self.test_monitored_values[metric_full_name] = MonitoredValue(
+                    name=metric_full_name,
+                    greater_is_better=self.greater_valid_metrics_is_better.get(metric_name),
+                )
+
+        # make sure the metric_to_watch is an exact match
+        metric_titles = self.loss_logging_items_names + get_metrics_titles(self.valid_metrics)
+        metric_to_watch_idx = fuzzy_idx_in_list(self.metric_to_watch, metric_titles)
+        metric_to_watch = metric_titles[metric_to_watch_idx]
+        if metric_to_watch != self.metric_to_watch:
+            logger.warning(
+                f"No exact match found for `metric_to_watch={self.metric_to_watch}`. It should be one of {metric_titles}. \n"
+                f"`metric_to_watch={metric_to_watch} will be used instead.`"
+            )
+            self.metric_to_watch = metric_to_watch
 
         if self.training_params.average_best_models:
             self.model_weight_averaging = ModelWeightAveraging(
                 ckpt_dir=self.checkpoints_dir_path,
                 greater_is_better=self.greater_metric_to_watch_is_better,
                 metric_to_watch=self.metric_to_watch,
-                metric_idx=self.metric_idx_in_results_tuple,
                 load_checkpoint=self.load_checkpoint,
             )
 
     def _backward_step(self, loss: torch.Tensor, epoch: int, batch_idx: int, context: PhaseContext, *args, **kwargs) -> None:
         """
         Run backprop on the loss and perform a step
         :param loss: The value computed by the loss function
@@ -577,47 +579,48 @@
             # RUN PHASE CALLBACKS
             self.phase_callback_handler.on_train_batch_gradient_step_end(context)
 
     def _save_checkpoint(
         self,
         optimizer: torch.optim.Optimizer = None,
         epoch: int = None,
-        validation_results_tuple: tuple = None,
+        validation_results_dict: Optional[Dict[str, float]] = None,
         context: PhaseContext = None,
     ) -> None:
         """
         Save the current state dict as latest (always), best (if metric was improved), epoch# (if determined in training
         params)
         """
         # WHEN THE validation_results_tuple IS NONE WE SIMPLY SAVE THE state_dict AS LATEST AND Return
-        if validation_results_tuple is None:
+        if validation_results_dict is None:
             self.sg_logger.add_checkpoint(tag="ckpt_latest_weights_only.pth", state_dict={"net": self.net.state_dict()}, global_step=epoch)
             return
 
         # COMPUTE THE CURRENT metric
         # IF idx IS A LIST - SUM ALL THE VALUES STORED IN THE LIST'S INDICES
-        metric = (
-            validation_results_tuple[self.metric_idx_in_results_tuple]
-            if isinstance(self.metric_idx_in_results_tuple, int)
-            else sum([validation_results_tuple[idx] for idx in self.metric_idx_in_results_tuple])
-        )
+        metric = validation_results_dict[self.metric_to_watch]
 
         # BUILD THE state_dict
-        state = {"net": self.net.state_dict(), "acc": metric, "epoch": epoch}
+        state = {"net": unwrap_model(self.net).state_dict(), "acc": metric, "epoch": epoch}
+
         if optimizer is not None:
             state["optimizer_state_dict"] = optimizer.state_dict()
 
         if self.scaler is not None:
             state["scaler_state_dict"] = self.scaler.state_dict()
 
         if self.ema:
-            state["ema_net"] = self.ema_model.ema.state_dict()
+            state["ema_net"] = unwrap_model(self.ema_model.ema).state_dict()
+
+        processing_params = self._get_preprocessing_from_valid_loader()
+        if processing_params is not None:
+            state["processing_params"] = processing_params
 
-        if isinstance(self.net.module, HasPredict) and isinstance(self.valid_loader.dataset, HasPreprocessingParams):
-            state["processing_params"] = self.valid_loader.dataset.get_dataset_preprocessing_params()
+        if self._torch_lr_scheduler is not None:
+            state["torch_scheduler_state_dict"] = self._torch_lr_scheduler.state_dict()
 
         # SAVES CURRENT MODEL AS ckpt_latest
         self.sg_logger.add_checkpoint(tag="ckpt_latest.pth", state_dict=state, global_step=epoch)
 
         # SAVE MODEL AT SPECIFIC EPOCHS DETERMINED BY save_ckpt_epoch_list
         if epoch in self.training_params.save_ckpt_epoch_list:
             self.sg_logger.add_checkpoint(tag=f"ckpt_epoch_{epoch}.pth", state_dict=state, global_step=epoch)
@@ -632,54 +635,70 @@
             self.phase_callback_handler.on_validation_end_best_epoch(context)
 
             if isinstance(metric, torch.Tensor):
                 metric = metric.item()
             logger.info("Best checkpoint overriden: validation " + self.metric_to_watch + ": " + str(metric))
 
         if self.training_params.average_best_models:
-            net_for_averaging = self.ema_model.ema if self.ema else self.net
-            state["net"] = self.model_weight_averaging.get_average_model(net_for_averaging, validation_results_tuple=validation_results_tuple)
+            net_for_averaging = unwrap_model(self.ema_model.ema if self.ema else self.net)
+
+            state["net"] = self.model_weight_averaging.get_average_model(net_for_averaging, validation_results_dict=validation_results_dict)
             self.sg_logger.add_checkpoint(tag=self.average_model_checkpoint_filename, state_dict=state, global_step=epoch)
 
     def _prep_net_for_train(self) -> None:
         if self.arch_params is None:
             self._init_arch_params()
 
         # TODO: REMOVE THE BELOW LINE (FOR BACKWARD COMPATIBILITY)
         if self.checkpoint_params is None:
             self.checkpoint_params = HpmStruct(load_checkpoint=self.training_params.resume)
 
         self._net_to_device()
 
         # SET THE FLAG FOR DIFFERENT PARAMETER GROUP OPTIMIZER UPDATE
-        self.update_param_groups = hasattr(self.net.module, "update_param_groups")
+        self.update_param_groups = hasattr(unwrap_model(self.net), "update_param_groups")
 
         self.checkpoint = {}
         self.strict_load = core_utils.get_param(self.training_params, "resume_strict_load", StrictLoad.ON)
         self.load_ema_as_net = False
         self.load_checkpoint = core_utils.get_param(self.training_params, "resume", False)
         self.external_checkpoint_path = core_utils.get_param(self.training_params, "resume_path")
         self.ckpt_name = core_utils.get_param(self.training_params, "ckpt_name", "ckpt_latest.pth")
         self.resume_from_remote_sg_logger = core_utils.get_param(self.training_params, "resume_from_remote_sg_logger", False)
         self.load_checkpoint = self.load_checkpoint or self.external_checkpoint_path is not None or self.resume_from_remote_sg_logger
 
+        if self.training_params.torch_compile:
+            if torch_version_is_greater_or_equal(2, 0):
+                logger.info("Using torch.compile feature. Compiling model. This may take a few minutes")
+                self.net = torch.compile(self.net, **self.training_params.torch_compile_options)
+                logger.info("Model compilation complete. Continuing training")
+                if is_distributed():
+                    torch.distributed.barrier()
+            else:
+                logger.warning(
+                    "Your recipe has requested use of torch.compile. "
+                    f"However torch.compile is not supported in this version of PyTorch ({torch.__version__}). "
+                    "A Pytorch 2.0 or greater version is required. Ignoring torch_compile flag"
+                )
+
     def _init_arch_params(self) -> None:
         default_arch_params = HpmStruct()
         arch_params = getattr(self.net, "arch_params", default_arch_params)
         self.arch_params = default_arch_params
         if arch_params is not None:
             self.arch_params.override(**arch_params.to_dict())
 
     # FIXME - we need to resolve flake8's 'function is too complex' for this function
     def train(
         self,
         model: nn.Module,
         training_params: dict = None,
         train_loader: DataLoader = None,
         valid_loader: DataLoader = None,
+        test_loaders: Dict[str, DataLoader] = None,
         additional_configs_to_log: Dict = None,
     ):  # noqa: C901
         """
 
         train - Trains the Model
 
         IMPORTANT NOTE: Additional batch parameters can be added as a third item (optional) if a tuple is returned by
@@ -688,14 +707,15 @@
 
             :param additional_configs_to_log: Dict, dictionary containing configs that will be added to the training's
                 sg_logger. Format should be {"Config_title_1": {...}, "Config_title_2":{..}}.
             :param model: torch.nn.Module, model to train.
 
             :param train_loader: Dataloader for train set.
             :param valid_loader: Dataloader for validation.
+            :param test_loaders: Dictionary of test loaders. The key will be used as the dataset name.
             :param training_params:
 
                 - `resume` : bool (default=False)
 
                     Whether to continue training from ckpt with the same experiment name
                      (i.e resume from CKPT_ROOT_DIR/EXPERIMENT_NAME/CKPT_NAME)
 
@@ -717,27 +737,60 @@
                     List of fixed epoch numbers to perform learning rate updates when `lr_mode='step'`.
 
                 - `lr_decay_factor` : float
 
                     Decay factor to apply to the learning rate at each update when `lr_mode='step'`.
 
 
-                -  `lr_mode` : str
+                -  `lr_mode` : Union[str, Mapping],
+
+                    When str:
 
                     Learning rate scheduling policy, one of ['step','poly','cosine','function'].
 
                     'step' refers to constant updates at epoch numbers passed through `lr_updates`. Each update decays the learning rate by `lr_decay_factor`.
 
                     'cosine' refers to the Cosine Anealing policy as mentioned in https://arxiv.org/abs/1608.03983.
                       The final learning rate ratio is controlled by `cosine_final_lr_ratio` training parameter.
 
                     'poly' refers to the polynomial decrease: in each epoch iteration `self.lr = self.initial_lr * pow((1.0 - (current_iter / max_iter)), 0.9)`
 
                     'function' refers to a user-defined learning rate scheduling function, that is passed through `lr_schedule_function`.
 
+
+
+                    When Mapping, refers to a torch.optim.lr_scheduler._LRScheduler, following the below API:
+
+                        lr_mode = {LR_SCHEDULER_CLASS_NAME: {**LR_SCHEDULER_KWARGS, "phase": XXX, "metric_name": XXX)
+
+                        Where "phase" (of Phase type) controls when to call torch.optim.lr_scheduler._LRScheduler.step().
+
+                        The "metric_name" refers to the metric to watch (See docs for "metric_to_watch" in train(...)
+                         https://docs.deci.ai/super-gradients/docstring/training/sg_trainer.html) when using
+                          ReduceLROnPlateau. In any other case this kwarg is ignored.
+
+                        **LR_SCHEDULER_KWARGS are simply passed to the torch scheduler's __init__.
+
+
+                        For example:
+                            lr_mode = {"StepLR": {"gamma": 0.1, "step_size": 1, "phase": Phase.TRAIN_EPOCH_END}}
+                            is equivalent to following training code:
+
+                                from torch.optim.lr_scheduler import StepLR
+                                ...
+                                optimizer = ....
+                                scheduler = StepLR(optimizer=optimizer, gamma=0.1, step_size=1)
+
+                                for epoch in num_epochs:
+                                    train_epoch(...)
+                                    scheduler.step()
+                                    ....
+
+
+
                 - `lr_schedule_function` : Union[callable,None]
 
                     Learning rate scheduling function to be used when `lr_mode` is 'function'.
 
                 - `warmup_mode`: Union[str, Type[LRCallbackBase], None]
 
                     If not None, define how the learning rate will be increased during the warmup phase.
@@ -917,15 +970,20 @@
                 - `load_opt_params` : bool (default=True)
 
                     Whether to load the optimizers parameters as well when loading a model's checkpoint.
 
                 - `run_validation_freq` : int (default=1)
 
                     The frequency in which validation is performed during training (i.e the validation is ran every
-                     `run_validation_freq` epochs.
+                     `run_validation_freq` epochs). Also applies to test set if you provided one.
+
+                - `run_test_freq` : int (default=1)
+
+                    The frequency in which test is performed during training (i.e the test is ran every
+                     `run_test_freq` epochs). Only applies if you provided a test set.
 
                 - `save_model` : bool (default=True)
 
                     Whether to save the model checkpoints.
 
                 - `silent_mode` : bool
 
@@ -1021,29 +1079,32 @@
         """
         global logger
         if training_params is None:
             training_params = dict()
 
         self.train_loader = train_loader if train_loader is not None else self.train_loader
         self.valid_loader = valid_loader if valid_loader is not None else self.valid_loader
+        self.test_loaders = test_loaders if test_loaders is not None else {}
 
         if self.train_loader is None:
             raise ValueError("No `train_loader` found. Please provide a value for `train_loader`")
 
         if self.valid_loader is None:
             raise ValueError("No `valid_loader` found. Please provide a value for `valid_loader`")
 
+        if self.test_loaders is not None and not isinstance(self.test_loaders, dict):
+            raise ValueError("`test_loaders` must be a dictionary mapping dataset names to DataLoaders")
+
         if hasattr(self.train_loader, "batch_sampler") and self.train_loader.batch_sampler is not None:
             batch_size = self.train_loader.batch_sampler.batch_size
         else:
             batch_size = self.train_loader.batch_size
 
         if len(self.train_loader.dataset) % batch_size != 0 and not self.train_loader.drop_last:
             logger.warning("Train dataset size % batch_size != 0 and drop_last=False, this might result in smaller " "last batch.")
-        self._set_dataset_params()
 
         if device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL:
             # Note: the dataloader uses sampler of the batch_sampler when it is not None.
             train_sampler = self.train_loader.batch_sampler.sampler if self.train_loader.batch_sampler is not None else self.train_loader.sampler
             if isinstance(train_sampler, SequentialSampler):
                 raise ValueError(
                     "You are using a SequentialSampler on you training dataloader, while working on DDP. "
@@ -1054,26 +1115,28 @@
                     "The training sampler you are using might not support DDP. "
                     "If it doesnt, please use one of the following sampler: DistributedSampler, RepeatAugSampler"
                 )
         self.training_params = TrainingParams()
         self.training_params.override(**training_params)
 
         self.net = model
+
         self._prep_net_for_train()
         if not self.ddp_silent_mode:
             self._initialize_sg_logger_objects(additional_configs_to_log)
         self._load_checkpoint_to_model()
 
         # SET RANDOM SEED
         random_seed(is_ddp=device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL, device=device_config.device, seed=self.training_params.seed)
 
         silent_mode = self.training_params.silent_mode or self.ddp_silent_mode
         # METRICS
         self._set_train_metrics(train_metrics_list=self.training_params.train_metrics_list)
         self._set_valid_metrics(valid_metrics_list=self.training_params.valid_metrics_list)
+        self.test_metrics = self.valid_metrics.clone()
 
         # Store the metric to follow (loss\accuracy) and initialize as the worst value
         self.metric_to_watch = self.training_params.metric_to_watch
         self.greater_metric_to_watch_is_better = self.training_params.greater_metric_to_watch_is_better
 
         # Allowing loading instantiated loss or string
         if isinstance(self.training_params.loss, str):
@@ -1083,14 +1146,28 @@
             self.criterion = LossesFactory().get(self.training_params.loss)
 
         elif isinstance(self.training_params.loss, nn.Module):
             self.criterion = self.training_params.loss
 
         self.criterion.to(device_config.device)
 
+        if self.training_params.torch_compile_loss:
+            if torch_version_is_greater_or_equal(2, 0):
+                logger.info("Using torch.compile feature. Compiling loss. This may take a few minutes")
+                self.criterion = torch.compile(self.criterion, **self.training_params.torch_compile_options)
+                logger.info("Loss compilation complete. Continuing training")
+                if is_distributed():
+                    torch.distributed.barrier()
+            else:
+                logger.warning(
+                    "Your recipe has requested use of torch.compile. "
+                    f"However torch.compile is not supported in this version of PyTorch ({torch.__version__}). "
+                    "A Pytorch 2.0 or greater version is required. Ignoring torch_compile flag"
+                )
+
         self.max_epochs = self.training_params.max_epochs
 
         self.ema = self.training_params.ema
 
         self.precise_bn = self.training_params.precise_bn
         self.precise_bn_batch_size = self.training_params.precise_bn_batch_size
 
@@ -1104,37 +1181,26 @@
                 if "ema_net" in self.checkpoint.keys():
                     self.ema_model.ema.load_state_dict(self.checkpoint["ema_net"])
                 else:
                     self.ema = False
                     logger.warning("[Warning] Checkpoint does not include EMA weights, continuing training without EMA.")
 
         self.run_validation_freq = self.training_params.run_validation_freq
-        validation_results_tuple = (0, 0)
+        self.run_test_freq = self.training_params.run_test_freq
+
         inf_time = 0
         timer = core_utils.Timer(device_config.device)
 
         # IF THE LR MODE IS NOT DEFAULT TAKE IT FROM THE TRAINING PARAMS
         self.lr_mode = self.training_params.lr_mode
         load_opt_params = self.training_params.load_opt_params
 
         self.phase_callbacks = self.training_params.phase_callbacks or []
         self.phase_callbacks = ListFactory(CallbacksFactory()).get(self.phase_callbacks)
 
-        if self.lr_mode is not None:
-            sg_lr_callback_cls = LR_SCHEDULERS_CLS_DICT[self.lr_mode]
-            self.phase_callbacks.append(
-                sg_lr_callback_cls(
-                    train_loader_len=len(self.train_loader),
-                    net=self.net,
-                    training_params=self.training_params,
-                    update_param_groups=self.update_param_groups,
-                    **self.training_params.to_dict(),
-                )
-            )
-
         warmup_mode = self.training_params.warmup_mode
         warmup_callback_cls = None
         if isinstance(warmup_mode, str):
             warmup_callback_cls = LR_WARMUP_CLS_DICT[warmup_mode]
         elif isinstance(warmup_mode, type) and issubclass(warmup_mode, LRCallbackBase):
             warmup_callback_cls = warmup_mode
         elif warmup_mode is not None:
@@ -1151,40 +1217,60 @@
                     update_param_groups=self.update_param_groups,
                     **self.training_params.to_dict(),
                 )
             )
 
         self._add_metrics_update_callback(Phase.TRAIN_BATCH_END)
         self._add_metrics_update_callback(Phase.VALIDATION_BATCH_END)
+        self._add_metrics_update_callback(Phase.TEST_BATCH_END)
 
         self.phase_callback_handler = CallbackHandler(callbacks=self.phase_callbacks)
 
         if not self.ddp_silent_mode:
             if self.training_params.dataset_statistics:
                 dataset_statistics_logger = DatasetStatisticsTensorboardLogger(self.sg_logger)
-                dataset_statistics_logger.analyze(self.train_loader, all_classes=self.classes, title="Train-set", anchors=self.net.module.arch_params.anchors)
+                dataset_statistics_logger.analyze(
+                    self.train_loader, all_classes=self.classes, title="Train-set", anchors=unwrap_model(self.net).arch_params.anchors
+                )
                 dataset_statistics_logger.analyze(self.valid_loader, all_classes=self.classes, title="val-set")
 
         sg_trainer_utils.log_uncaught_exceptions(logger)
 
         if not self.load_checkpoint or self.load_weights_only:
             # WHEN STARTING TRAINING FROM SCRATCH, DO NOT LOAD OPTIMIZER PARAMS (EVEN IF LOADING BACKBONE)
             self.start_epoch = 0
             self._reset_best_metric()
             load_opt_params = False
 
         if isinstance(self.training_params.optimizer, str) or (
             inspect.isclass(self.training_params.optimizer) and issubclass(self.training_params.optimizer, torch.optim.Optimizer)
         ):
-            self.optimizer = build_optimizer(net=self.net, lr=self.training_params.initial_lr, training_params=self.training_params)
+            self.optimizer = build_optimizer(net=unwrap_model(self.net), lr=self.training_params.initial_lr, training_params=self.training_params)
         elif isinstance(self.training_params.optimizer, torch.optim.Optimizer):
             self.optimizer = self.training_params.optimizer
         else:
             raise UnsupportedOptimizerFormat()
 
+        if self.lr_mode is not None:
+            lr_scheduler_callback = create_lr_scheduler_callback(
+                lr_mode=self.lr_mode,
+                train_loader=self.train_loader,
+                net=self.net,
+                training_params=self.training_params,
+                update_param_groups=self.update_param_groups,
+                optimizer=self.optimizer,
+            )
+            self.phase_callbacks.append(lr_scheduler_callback)
+
+            # NEED ACCESS TO THE UNDERLYING TORCH SCHEDULER FOR LOADING/SAVING IT'S STATE_DICT
+            if isinstance(lr_scheduler_callback, LRSchedulerCallback):
+                self._torch_lr_scheduler = lr_scheduler_callback.scheduler
+                if self.load_checkpoint:
+                    self._torch_lr_scheduler.load_state_dict(self.checkpoint["torch_scheduler_state_dict"])
+
         # VERIFY GRADIENT CLIPPING VALUE
         if self.training_params.clip_grad_norm is not None and self.training_params.clip_grad_norm <= 0:
             raise TypeError("Params", "Invalid clip_grad_norm")
 
         if self.load_checkpoint and load_opt_params:
             self.optimizer.load_state_dict(self.checkpoint["optimizer_state_dict"])
 
@@ -1225,15 +1311,14 @@
             training_params=self.training_params,
             ddp_silent_mode=self.ddp_silent_mode,
             checkpoint_params=self.checkpoint_params,
             architecture=self.architecture,
             arch_params=self.arch_params,
             metric_to_watch=self.metric_to_watch,
             device=device_config.device,
-            context_methods=self._get_context_methods(Phase.PRE_TRAINING),
             ema_model=self.ema_model,
         )
         self.phase_callback_handler.on_training_start(context)
 
         first_batch = next(iter(self.train_loader))
         inputs, _, _ = sg_trainer_utils.unpack_batch_items(first_batch)
 
@@ -1242,15 +1327,18 @@
             num_gpus=get_world_size(),
             batch_size=len(inputs),
             batch_accumulate=self.batch_accumulate,
             train_dataset_length=len(self.train_loader.dataset),
             train_dataloader_len=len(self.train_loader),
         )
 
-        self._set_net_preprocessing_from_valid_loader()
+        processing_params = self._get_preprocessing_from_valid_loader()
+        if processing_params is not None:
+            unwrap_model(self.net).set_dataset_processing_params(**processing_params)
+
         try:
             # HEADERS OF THE TRAINING PROGRESS
             if not silent_mode:
                 logger.info(f"Started training for {self.max_epochs - self.start_epoch} epochs ({self.start_epoch}/" f"{self.max_epochs - 1})\n")
             for epoch in range(self.start_epoch, self.max_epochs):
                 if context.stop_training:
                     logger.info("Request to stop training has been received, stopping training")
@@ -1266,15 +1354,15 @@
                 if (
                     device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL
                     and hasattr(self.train_loader, "sampler")
                     and hasattr(self.train_loader.sampler, "set_epoch")
                 ):
                     self.train_loader.sampler.set_epoch(epoch)
 
-                train_metrics_tuple = self._train_epoch(epoch=epoch, silent_mode=silent_mode)
+                train_metrics_tuple = self._train_epoch(context=context, silent_mode=silent_mode)
 
                 # Phase.TRAIN_EPOCH_END
                 # RUN PHASE CALLBACKS
                 train_metrics_dict = get_metrics_dict(train_metrics_tuple, self.train_metrics, self.loss_logging_items_names)
 
                 context.update_context(metrics_dict=train_metrics_dict)
                 self.phase_callback_handler.on_train_loader_end(context)
@@ -1288,53 +1376,85 @@
                         compute_precise_bn_stats(
                             model=self.ema_model.ema,
                             loader=self.train_loader,
                             precise_bn_batch_size=self.precise_bn_batch_size,
                             num_gpus=get_world_size(),
                         )
 
-                # model switch - we replace self.net.module with the ema model for the testing and saving part
+                # model switch - we replace self.net with the ema model for the testing and saving part
                 # and then switch it back before the next training epoch
                 if self.ema:
                     self.ema_model.update_attr(self.net)
                     keep_model = self.net
                     self.net = self.ema_model.ema
 
                 # RUN TEST ON VALIDATION SET EVERY self.run_validation_freq EPOCHS
+                valid_metrics_dict = {}
                 if (epoch + 1) % self.run_validation_freq == 0:
                     self.phase_callback_handler.on_validation_loader_start(context)
                     timer.start()
-                    validation_results_tuple = self._validate_epoch(epoch=epoch, silent_mode=silent_mode)
+                    valid_metrics_dict = self._validate_epoch(context=context, silent_mode=silent_mode)
                     inf_time = timer.stop()
 
+                    self.valid_monitored_values = sg_trainer_utils.update_monitored_values_dict(
+                        monitored_values_dict=self.valid_monitored_values,
+                        new_values_dict=valid_metrics_dict,
+                    )  # TODO: Move this logic inside a MonitoredValues class
                     # Phase.VALIDATION_EPOCH_END
                     # RUN PHASE CALLBACKS
-                    valid_metrics_dict = get_metrics_dict(validation_results_tuple, self.valid_metrics, self.loss_logging_items_names)
-
                     context.update_context(metrics_dict=valid_metrics_dict)
                     self.phase_callback_handler.on_validation_loader_end(context)
 
+                test_metrics_dict = {}
+                if (epoch + 1) % self.run_test_freq == 0:
+                    self.phase_callback_handler.on_test_loader_start(context)
+                    for dataset_name, dataloader in self.test_loaders.items():
+                        dataset_metrics_dict = self._test_epoch(data_loader=dataloader, context=context, silent_mode=silent_mode, dataset_name=dataset_name)
+                        dataset_metrics_dict_with_name = {
+                            f"{dataset_name}:{metric_name}": metric_value for metric_name, metric_value in dataset_metrics_dict.items()
+                        }
+                        self.test_monitored_values = sg_trainer_utils.update_monitored_values_dict(
+                            monitored_values_dict=self.test_monitored_values,
+                            new_values_dict=dataset_metrics_dict_with_name,
+                        )  # TODO: Move this logic inside a MonitoredValues class
+
+                        test_metrics_dict.update(**dataset_metrics_dict_with_name)
+                    context.update_context(metrics_dict=test_metrics_dict)
+                    self.phase_callback_handler.on_test_loader_end(context)
+
                 if self.ema:
                     self.net = keep_model
 
                 if not self.ddp_silent_mode:
                     # SAVING AND LOGGING OCCURS ONLY IN THE MAIN PROCESS (IN CASES THERE ARE SEVERAL PROCESSES - DDP)
                     self._write_to_disk_operations(
-                        train_metrics=train_metrics_tuple,
-                        validation_results=validation_results_tuple,
+                        train_metrics_dict=train_metrics_dict,
+                        validation_results_dict=valid_metrics_dict,
+                        test_metrics_dict=test_metrics_dict,
                         lr_dict=self._epoch_start_logging_values,
                         inf_time=inf_time,
                         epoch=epoch,
                         context=context,
                     )
                     self.sg_logger.upload()
 
+                if not silent_mode:
+                    sg_trainer_utils.display_epoch_summary(
+                        epoch=context.epoch,
+                        n_digits=4,
+                        monitored_values_dict={
+                            "Train": self.train_monitored_values,
+                            "Validation": self.valid_monitored_values,
+                            "Test": self.test_monitored_values,
+                        },
+                    )
+
             # Evaluating the average model and removing snapshot averaging file if training is completed
             if self.training_params.average_best_models:
-                self._validate_final_average_model(cleanup_snapshots_pkl_file=True)
+                self._validate_final_average_model(context, cleanup_snapshots_pkl_file=True)
 
         except KeyboardInterrupt:
             logger.info(
                 "\n[MODEL TRAINING EXECUTION HAS BEEN INTERRUPTED]... Please wait until SOFT-TERMINATION process "
                 "finishes and saves all of the Model Checkpoints and log files before terminating..."
             )
             logger.info("For HARD Termination - Stop the process again")
@@ -1347,18 +1467,20 @@
 
             # PHASE.TRAIN_END
             self.phase_callback_handler.on_training_end(context)
 
             if not self.ddp_silent_mode:
                 self.sg_logger.close()
 
-    def _set_net_preprocessing_from_valid_loader(self):
-        if isinstance(self.net.module, HasPredict) and isinstance(self.valid_loader.dataset, HasPreprocessingParams):
+    def _get_preprocessing_from_valid_loader(self) -> Optional[dict]:
+        valid_loader = self.valid_loader
+
+        if isinstance(unwrap_model(self.net), HasPredict) and isinstance(valid_loader.dataset, HasPreprocessingParams):
             try:
-                self.net.module.set_dataset_processing_params(**self.valid_loader.dataset.get_dataset_preprocessing_params())
+                return valid_loader.dataset.get_dataset_preprocessing_params()
             except Exception as e:
                 logger.warning(
                     f"Could not set preprocessing pipeline from the validation dataset:\n {e}.\n Before calling"
                     "predict make sure to call set_dataset_processing_params."
                 )
 
     def _reset_best_metric(self):
@@ -1406,24 +1528,24 @@
             if device_config.multi_gpu == MultiGPUMode.DATA_PARALLEL:
                 # IN DATAPARALLEL MODE WE NEED TO WRAP THE FORWARD FUNCTION OF OUR MODEL SO IT WILL RUN WITH AUTOCAST.
                 # BUT SINCE THE MODULE IS CLONED TO THE DEVICES ON EACH FORWARD CALL OF A DATAPARALLEL MODEL,
                 # WE HAVE TO REGISTER THE WRAPPER BEFORE EVERY FORWARD CALL
                 def hook(module, _):
                     module.forward = MultiGPUModeAutocastWrapper(module.forward)
 
-                self.net.module.register_forward_pre_hook(hook=hook)
+                unwrap_model(self.net).register_forward_pre_hook(hook=hook)
 
             if self.load_checkpoint:
                 scaler_state_dict = core_utils.get_param(self.checkpoint, "scaler_state_dict")
                 if scaler_state_dict is None:
                     logger.warning("Mixed Precision - scaler state_dict not found in loaded model. This may case issues " "with loss scaling")
                 else:
                     self.scaler.load_state_dict(scaler_state_dict)
 
-    def _validate_final_average_model(self, cleanup_snapshots_pkl_file=False):
+    def _validate_final_average_model(self, context: PhaseContext, cleanup_snapshots_pkl_file=False):
         """
         Testing the averaged model by loading the last saved average checkpoint and running test.
         Will be loaded to each of DDP processes
         :param cleanup_pkl_file: a flag for deleting the 10 best snapshots dictionary
         """
         logger.info("RUNNING ADDITIONAL TEST ON THE AVERAGED MODEL...")
 
@@ -1432,39 +1554,43 @@
         average_model_ckpt_path = os.path.join(self.checkpoints_dir_path, self.average_model_checkpoint_filename)
         local_rank = get_local_rank()
 
         # WAIT FOR MASTER RANK TO SAVE THE CKPT BEFORE WE TRY TO READ IT.
         with wait_for_the_master(local_rank):
             average_model_sd = read_ckpt_state_dict(average_model_ckpt_path)["net"]
 
-        self.net.load_state_dict(average_model_sd)
+        unwrap_model(self.net).load_state_dict(average_model_sd)
         # testing the averaged model and save instead of best model if needed
-        averaged_model_results_tuple = self._validate_epoch(epoch=self.max_epochs)
+        context.update_context(epoch=self.max_epochs)
+        averaged_model_results_dict = self._validate_epoch(context=context)
+        self.valid_monitored_values = sg_trainer_utils.update_monitored_values_dict(
+            monitored_values_dict=self.valid_monitored_values,
+            new_values_dict=averaged_model_results_dict,
+        )  # TODO: Move this logic inside a MonitoredValues class
 
         # Reverting the current model
         self.net.load_state_dict(keep_state_dict)
 
         if not self.ddp_silent_mode:
-            average_model_tb_titles = ["Averaged Model " + x for x in self.results_titles[-1 * len(averaged_model_results_tuple) :]]
             write_struct = ""
-            for ind, title in enumerate(average_model_tb_titles):
-                write_struct += "%s: %.3f  \n  " % (title, averaged_model_results_tuple[ind])
-                self.sg_logger.add_scalar(title, averaged_model_results_tuple[ind], global_step=self.max_epochs)
+            for name, value in averaged_model_results_dict.items():
+                write_struct += "%s: %.3f  \n  " % (name, value)
+                self.sg_logger.add_scalar(name, value, global_step=self.max_epochs)
 
             self.sg_logger.add_text("Averaged_Model_Performance", write_struct, self.max_epochs)
             if cleanup_snapshots_pkl_file:
                 self.model_weight_averaging.cleanup()
 
     @property
     def get_arch_params(self):
         return self.arch_params.to_dict()
 
     @property
     def get_structure(self):
-        return self.net.module.structure
+        return unwrap_model(self.net).structure
 
     @property
     def get_architecture(self):
         return self.architecture
 
     def set_experiment_name(self, experiment_name):
         self.experiment_name = experiment_name
@@ -1488,15 +1614,16 @@
         if hasattr(self.net, "structure"):
             self.architecture = self.net.structure
 
         self.net.to(device_config.device)
 
         if device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL:
             logger.warning("Warning: distributed training is not supported in re_build_model()")
-        self.net = torch.nn.DataParallel(self.net, device_ids=get_device_ids()) if device_config.multi_gpu else core_utils.WrappedModel(self.net)
+        if device_config.multi_gpu == MultiGPUMode.DATA_PARALLEL:
+            self.net = torch.nn.DataParallel(self.net, device_ids=get_device_ids())
 
     @property
     def get_module(self):
         return self.net
 
     def set_module(self, module):
         self.net = module
@@ -1578,15 +1705,15 @@
             self.loss_logging_items_names = []
 
         if self.test_metrics is None:
             raise ValueError(
                 "Metrics are required to perform test. Pass them through test_metrics_list arg when "
                 "calling test or through training_params when calling train(...)"
             )
-        if self.test_loader is None:
+        if test_loader is None:
             raise ValueError("Test dataloader is required to perform test. Make sure to either pass it through " "test_loader arg.")
 
         # RESET METRIC RUNNERS
         self._reset_metrics()
         self.test_metrics.to(device_config.device)
 
         if self.arch_params is None:
@@ -1629,15 +1756,15 @@
             if issubclass(sg_logger_cls, BaseSGLogger):
                 sg_logger_params = {**sg_logger_params, **general_sg_logger_params}
 
             # Some sg_logger require model_name, but not all of them.
             if "model_name" in get_callable_param_names(sg_logger_cls.__init__):
                 if sg_logger_params.get("model_name") is None:
                     # Use the model name used in `models.get(...)` if relevant
-                    sg_logger_params["model_name"] = get_model_name(self.net.module)
+                    sg_logger_params["model_name"] = get_model_name(unwrap_model(self.net))
 
                 if sg_logger_params["model_name"] is None:
                     raise ValueError(
                         f'`model_name` is required to use `training_hyperparams.sg_logger="{sg_logger}"`.\n'
                         'Please set `training_hyperparams.sg_logger_params.model_name="<your-model-name>"`.\n'
                         "Note that specifying `model_name` is not required when the model was loaded using `models.get(...)`."
                     )
@@ -1670,36 +1797,53 @@
             "multi_gpu": str(device_config.multi_gpu),
             "device_type": torch.cuda.get_device_name(0) if torch.cuda.is_available() else "cpu",
         }
         # ADD INSTALLED PACKAGE LIST + THEIR VERSIONS
         if self.training_params.log_installed_packages:
             pkg_list = list(map(lambda pkg: str(pkg), _get_installed_distributions()))
             additional_log_items["installed_packages"] = pkg_list
+
+        dataset_params = {
+            "train_dataset_params": self.train_loader.dataset.dataset_params if hasattr(self.train_loader.dataset, "dataset_params") else None,
+            "train_dataloader_params": self.train_loader.dataloader_params if hasattr(self.train_loader, "dataloader_params") else None,
+            "valid_dataset_params": self.valid_loader.dataset.dataset_params if hasattr(self.valid_loader.dataset, "dataset_params") else None,
+            "valid_dataloader_params": self.valid_loader.dataloader_params if hasattr(self.valid_loader, "dataloader_params") else None,
+        }
         hyper_param_config = {
             "arch_params": self.arch_params.__dict__,
             "checkpoint_params": self.checkpoint_params.__dict__,
             "training_hyperparams": self.training_params.__dict__,
-            "dataset_params": self.dataset_params.__dict__,
+            "dataset_params": dataset_params,
             "additional_log_items": additional_log_items,
         }
         return hyper_param_config
 
-    def _write_to_disk_operations(self, train_metrics: tuple, validation_results: tuple, lr_dict: dict, inf_time: float, epoch: int, context: PhaseContext):
+    def _write_to_disk_operations(
+        self,
+        train_metrics_dict: dict,
+        validation_results_dict: dict,
+        test_metrics_dict: dict,
+        lr_dict: dict,
+        inf_time: float,
+        epoch: int,
+        context: PhaseContext,
+    ):
         """Run the various logging operations, e.g.: log file, Tensorboard, save checkpoint etc."""
-        # STORE VALUES IN A TENSORBOARD FILE
-        train_results = list(train_metrics) + list(validation_results) + [inf_time]
-        all_titles = self.results_titles + ["Inference Time"]
-
-        result_dict = {all_titles[i]: train_results[i] for i in range(len(train_results))}
+        result_dict = {
+            "Inference Time": inf_time,
+            **{f"Train_{k}": v for k, v in train_metrics_dict.items()},
+            **{f"Valid_{k}": v for k, v in validation_results_dict.items()},
+            **{f"Test_{k}": v for k, v in test_metrics_dict.items()},
+        }
         self.sg_logger.add_scalars(tag_scalar_dict=result_dict, global_step=epoch)
         self.sg_logger.add_scalars(tag_scalar_dict=lr_dict, global_step=epoch)
 
         # SAVE THE CHECKPOINT
         if self.training_params.save_model:
-            self._save_checkpoint(self.optimizer, epoch + 1, validation_results, context)
+            self._save_checkpoint(self.optimizer, epoch + 1, validation_results_dict, context)
 
     def _get_epoch_start_logging_values(self) -> dict:
         """Get all the values that should be logged at the start of each epoch.
         This is useful for values like Learning Rate that can change over an epoch."""
         lrs = [self.optimizer.param_groups[i]["lr"] for i in range(len(self.optimizer.param_groups))]
         lr_titles = ["LR/Param_group_" + str(i) for i in range(len(self.optimizer.param_groups))] if len(self.optimizer.param_groups) > 1 else ["LR"]
         lr_dict = {lr_titles[i]: lrs[i] for i in range(len(lrs))}
@@ -1712,15 +1856,15 @@
         loss: torch.nn.modules.loss._Loss = None,
         silent_mode: bool = False,
         test_metrics_list=None,
         loss_logging_items_names=None,
         metrics_progress_verbose=False,
         test_phase_callbacks=None,
         use_ema_net=True,
-    ) -> tuple:
+    ) -> Dict[str, float]:
         """
         Evaluates the model on given dataloader and metrics.
         :param model: model to perfrom test on. When none is given, will try to use self.net (defalut=None).
         :param test_loader: dataloader to perform test on.
         :param test_metrics_list: (list(torchmetrics.Metric)) metrics list for evaluation.
         :param silent_mode: (bool) controls verbosity
         :param metrics_progress_verbose: (bool) controls the verbosity of metrics progress (default=False). Slows down the program.
@@ -1749,66 +1893,83 @@
             test_phase_callbacks=test_phase_callbacks,
         )
 
         context = PhaseContext(
             criterion=self.criterion,
             device=self.device,
             sg_logger=self.sg_logger,
-            context_methods=self._get_context_methods(Phase.TEST_BATCH_END),
         )
         if test_metrics_list:
             context.update_context(test_metrics=self.test_metrics)
 
         self.phase_callback_handler.on_test_loader_start(context)
         test_results = self.evaluate(
-            data_loader=self.test_loader,
+            data_loader=test_loader,
             metrics=self.test_metrics,
             evaluation_type=EvaluationType.TEST,
             silent_mode=silent_mode,
             metrics_progress_verbose=metrics_progress_verbose,
         )
         self.phase_callback_handler.on_test_loader_end(context)
 
         # SWITCH BACK BETWEEN NETS SO AN ADDITIONAL TRAINING CAN BE DONE AFTER TEST
         if use_ema_net and self.ema_model is not None:
             self.net = keep_model
 
         self._first_backward = True
 
-        test_results = get_metrics_dict(test_results, self.test_metrics, self.loss_logging_items_names)
-
         return test_results
 
-    def _validate_epoch(self, epoch: int, silent_mode: bool = False) -> tuple:
+    def _validate_epoch(self, context: PhaseContext, silent_mode: bool = False) -> Dict[str, float]:
         """
         Runs evaluation on self.valid_loader, with self.valid_metrics.
 
         :param epoch: (int) epoch idx
         :param silent_mode: (bool) controls verbosity
 
         :return: results tuple (tuple) containing the loss items and metric values.
         """
-
         self.net.eval()
         self._reset_metrics()
         self.valid_metrics.to(device_config.device)
+        return self.evaluate(
+            data_loader=self.valid_loader, metrics=self.valid_metrics, evaluation_type=EvaluationType.VALIDATION, epoch=context.epoch, silent_mode=silent_mode
+        )
 
+    def _test_epoch(self, data_loader: DataLoader, context: PhaseContext, silent_mode: bool = False, dataset_name: str = "") -> Dict[str, float]:
+        """
+        Evaluate the input loader on given metrics.
+
+        :param epoch: (int) epoch idx
+        :param silent_mode: (bool) controls verbosity
+
+        :return: results tuple (tuple) containing the loss items and metric values.
+        """
+        self.net.eval()
+        self._reset_metrics()
+        self.test_metrics.to(device_config.device)
         return self.evaluate(
-            data_loader=self.valid_loader, metrics=self.valid_metrics, evaluation_type=EvaluationType.VALIDATION, epoch=epoch, silent_mode=silent_mode
+            data_loader=data_loader,
+            metrics=self.test_metrics,
+            evaluation_type=EvaluationType.TEST,
+            epoch=context.epoch,
+            silent_mode=silent_mode,
+            dataset_name=dataset_name,
         )
 
     def evaluate(
         self,
         data_loader: torch.utils.data.DataLoader,
         metrics: MetricCollection,
         evaluation_type: EvaluationType,
         epoch: int = None,
         silent_mode: bool = False,
         metrics_progress_verbose: bool = False,
-    ):
+        dataset_name: str = "",
+    ) -> Dict[str, float]:
         """
         Evaluates the model on given dataloader and metrics.
 
         :param data_loader: dataloader to perform evaluataion on
         :param metrics: (MetricCollection) metrics for evaluation
         :param evaluation_type: (EvaluationType) controls which phase callbacks will be used (for example, on batch end,
             when evaluation_type=EvaluationType.VALIDATION the Phase.VALIDATION_BATCH_END callbacks will be triggered)
@@ -1818,33 +1979,37 @@
             Slows down the program significantly.
 
         :return: results tuple (tuple) containing the loss items and metric values.
         """
 
         # THE DISABLE FLAG CONTROLS WHETHER THE PROGRESS BAR IS SILENT OR PRINTS THE LOGS
         loss_avg_meter = core_utils.utils.AverageMeter()
-        logging_values = None
 
         lr_warmup_epochs = self.training_params.lr_warmup_epochs if self.training_params else None
         context = PhaseContext(
             epoch=epoch,
             metrics_compute_fn=metrics,
             loss_avg_meter=loss_avg_meter,
             criterion=self.criterion,
             device=device_config.device,
             lr_warmup_epochs=lr_warmup_epochs,
             sg_logger=self.sg_logger,
-            context_methods=self._get_context_methods(Phase.VALIDATION_BATCH_END),
+            train_loader=self.train_loader,
+            valid_loader=self.valid_loader,
         )
 
         with tqdm(data_loader, bar_format="{l_bar}{bar:10}{r_bar}", dynamic_ncols=True, disable=silent_mode) as progress_bar_data_loader:
 
             if not silent_mode:
                 # PRINT TITLES
-                pbar_start_msg = f"Validation epoch {epoch}" if evaluation_type == EvaluationType.VALIDATION else "Test"
+                pbar_start_msg = "Validating" if evaluation_type == EvaluationType.VALIDATION else "Testing"
+                if dataset_name:
+                    pbar_start_msg += f' dataset="{dataset_name}:"'
+                if epoch:
+                    pbar_start_msg += f" epoch {epoch}"
                 progress_bar_data_loader.set_description(pbar_start_msg)
 
             with torch.no_grad():
                 for batch_idx, batch_items in enumerate(progress_bar_data_loader):
                     batch_items = core_utils.tensor_container_to_device(batch_items, device_config.device, non_blocking=True)
                     inputs, targets, additional_batch_items = sg_trainer_utils.unpack_batch_items(batch_items)
 
@@ -1876,44 +2041,31 @@
                         pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
 
                         progress_bar_data_loader.set_postfix(**pbar_message_dict)
 
                     if evaluation_type == EvaluationType.VALIDATION and self.max_valid_batches is not None and self.max_valid_batches - 1 <= batch_idx:
                         break
 
+            logging_values = get_logging_values(loss_avg_meter, metrics, self.criterion)
             # NEED TO COMPUTE METRICS FOR THE FIRST TIME IF PROGRESS VERBOSITY IS NOT SET
             if not metrics_progress_verbose:
                 # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
-                logging_values = get_logging_values(loss_avg_meter, metrics, self.criterion)
                 pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
 
                 progress_bar_data_loader.set_postfix(**pbar_message_dict)
 
             # TODO: SUPPORT PRINTING AP PER CLASS- SINCE THE METRICS ARE NOT HARD CODED ANYMORE (as done in
             #  calc_batch_prediction_accuracy_per_class in metric_utils.py), THIS IS ONLY RELEVANT WHEN CHOOSING
             #  DETECTIONMETRICS, WHICH ALREADY RETURN THE METRICS VALUEST HEMSELVES AND NOT THE ITEMS REQUIRED FOR SUCH
             #  COMPUTATION. ALSO REMOVE THE BELOW LINES BY IMPLEMENTING CRITERION AS A TORCHMETRIC.
 
             if device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL:
                 logging_values = reduce_results_tuple_for_ddp(logging_values, next(self.net.parameters()).device)
 
-            pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
-
-            self.valid_monitored_values = sg_trainer_utils.update_monitored_values_dict(
-                monitored_values_dict=self.valid_monitored_values, new_values_dict=pbar_message_dict
-            )
-
-            if not silent_mode and evaluation_type == EvaluationType.VALIDATION:
-                progress_bar_data_loader.write("===========================================================")
-                sg_trainer_utils.display_epoch_summary(
-                    epoch=context.epoch, n_digits=4, train_monitored_values=self.train_monitored_values, valid_monitored_values=self.valid_monitored_values
-                )
-                progress_bar_data_loader.write("===========================================================")
-
-        return logging_values
+        return get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
 
     def _instantiate_net(
         self, architecture: Union[torch.nn.Module, SgModule.__class__, str], arch_params: dict, checkpoint_params: dict, *args, **kwargs
     ) -> tuple:
         """
         Instantiates nn.Module according to architecture and arch_params, and handles pretrained weights and the required
             module manipulation (i.e head replacement).
@@ -1987,44 +2139,14 @@
         """
         Setter for self.ema
 
         :param val: bool, value to set ema
         """
         self.ema = val
 
-    def _get_context_methods(self, phase: Phase) -> ContextSgMethods:
-        """
-        Returns ContextSgMethods holding the methods that should be accessible through phase callbacks to the user at
-         the specific phase
-
-        :param phase: Phase, controls what methods should be returned.
-        :return: ContextSgMethods holding methods from self.
-        """
-        if phase in [
-            Phase.PRE_TRAINING,
-            Phase.TRAIN_EPOCH_START,
-            Phase.TRAIN_EPOCH_END,
-            Phase.VALIDATION_EPOCH_END,
-            Phase.VALIDATION_EPOCH_END,
-            Phase.POST_TRAINING,
-            Phase.VALIDATION_END_BEST_EPOCH,
-        ]:
-            context_methods = ContextSgMethods(
-                get_net=self.get_net,
-                set_net=self.set_net,
-                set_ckpt_best_name=self.set_ckpt_best_name,
-                reset_best_metric=self._reset_best_metric,
-                validate_epoch=self._validate_epoch,
-                set_ema=self.set_ema,
-            )
-        else:
-            context_methods = ContextSgMethods()
-
-        return context_methods
-
     def _init_loss_logging_names(self, loss_logging_items):
         criterion_name = self.criterion.__class__.__name__
         component_names = None
         if hasattr(self.criterion, "component_names"):
             component_names = self.criterion.component_names
         elif len(loss_logging_items) > 1:
             component_names = ["loss_" + str(i) for i in range(len(loss_logging_items))]
@@ -2068,15 +2190,17 @@
 
         # TRIGGER CFG MODIFYING CALLBACKS
         cfg = cls._trigger_cfg_modifying_callbacks(cfg)
 
         quantization_params = get_param(cfg, "quantization_params")
 
         if quantization_params is None:
-            raise logger.warning("Your recipe does not include quantization_params. Using default quantization params.")
+            logger.warning("Your recipe does not include quantization_params. Using default quantization params.")
+            quantization_params = load_recipe("quantization_params/default_quantization_params").quantization_params
+            cfg.quantization_params = quantization_params
 
         if get_param(cfg.checkpoint_params, "checkpoint_path") is None and get_param(cfg.checkpoint_params, "pretrained_weights") is None:
             raise ValueError("Starting checkpoint / pretrained weights are a must for QAT finetuning.")
 
         num_gpus = core_utils.get_param(cfg, "num_gpus")
         multi_gpu = core_utils.get_param(cfg, "multi_gpu")
         device = core_utils.get_param(cfg, "device")
```

## super_gradients/training/transforms/keypoint_transforms.py

```diff
@@ -1,21 +1,22 @@
 import random
 from abc import abstractmethod
-from typing import Tuple, List, Iterable, Union, Optional
+from typing import Tuple, List, Iterable, Union, Optional, Dict
 
 import cv2
 import numpy as np
+import torch
 from torch import Tensor
-from torchvision.transforms import functional as F
 
-from super_gradients.common.object_names import Transforms
+from super_gradients.common.object_names import Transforms, Processings
 from super_gradients.common.registry.registry import register_transform
 
 __all__ = [
     "KeypointsImageNormalize",
+    "KeypointsImageStandardize",
     "KeypointsImageToTensor",
     "KeypointsPadIfNeeded",
     "KeypointsLongestMaxSize",
     "KeypointTransform",
     "KeypointsCompose",
     "KeypointsRandomHorizontalFlip",
     "KeypointsRandomAffineTransform",
@@ -24,15 +25,15 @@
 
 from super_gradients.training.datasets.data_formats.bbox_formats.xywh import xywh_to_xyxy, xyxy_to_xywh
 
 
 @register_transform(Transforms.KeypointTransform)
 class KeypointTransform(object):
     """
-    Base class for all transforms for keypoints augmnetation.
+    Base class for all transforms for keypoints augmentation.
     All transforms subclassing it should implement __call__ method which takes image, mask and keypoints as input and
     returns transformed image, mask and keypoints.
     """
 
     @abstractmethod
     def __call__(
         self, image: np.ndarray, mask: np.ndarray, joints: np.ndarray, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]
@@ -45,53 +46,105 @@
         :param joints: Numpy array of [NumInstances, NumJoints, 3] shape. Last dimension contains (x,y,visibility) for each joint.
         :param areas: (Optional) Numpy array of [N] shape with area of each instance
         :param bboxes: (Optional) Numpy array of [N,4] shape with bounding box of each instance (XYWH)
         :return: (image, mask, joints)
         """
         raise NotImplementedError
 
+    def get_equivalent_preprocessing(self) -> List:
+        raise NotImplementedError
+
 
 class KeypointsCompose(KeypointTransform):
     def __init__(self, transforms: List[KeypointTransform]):
         self.transforms = transforms
 
     def __call__(
         self, image: np.ndarray, mask: np.ndarray, joints: np.ndarray, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]
     ) -> Tuple[Union[np.ndarray, Tensor], np.ndarray, np.ndarray, Optional[np.ndarray], Optional[np.ndarray]]:
         for t in self.transforms:
             image, mask, joints, areas, bboxes = t(image, mask, joints, areas, bboxes)
         return image, mask, joints, areas, bboxes
 
+    def get_equivalent_preprocessing(self) -> List:
+        preprocessing = []
+        for t in self.transforms:
+            preprocessing += t.get_equivalent_preprocessing()
+        return preprocessing
+
+    def __repr__(self):
+        format_string = self.__class__.__name__ + "("
+        for t in self.transforms:
+            format_string += f"\t{repr(t)}"
+        format_string += "\n)"
+        return format_string
+
 
 @register_transform(Transforms.KeypointsImageToTensor)
 class KeypointsImageToTensor(KeypointTransform):
     """
     Convert image from numpy array to tensor and permute axes to [C,H,W].
-    This function also divides image by 255.0 to convert it to [0,1] range.
     """
 
     def __call__(self, image: np.ndarray, mask: np.ndarray, joints: np.ndarray, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]):
-        return F.to_tensor(image), mask, joints, areas, bboxes
+        image = torch.from_numpy(np.transpose(image, (2, 0, 1))).float()
+        return image, mask, joints, areas, bboxes
+
+    def get_equivalent_preprocessing(self) -> List:
+        return [
+            {Processings.ImagePermute: {"permutation": (2, 0, 1)}},
+        ]
+
+    def __repr__(self):
+        return self.__class__.__name__ + f"(permutation={self.permutation})"
+
+
+@register_transform(Transforms.KeypointsImageStandardize)
+class KeypointsImageStandardize(KeypointTransform):
+    """
+    Standardize image pixel values with img/max_val
+
+    :param max_val: Current maximum value of the image pixels. (usually 255)
+    """
+
+    def __init__(self, max_value: float = 255.0):
+        super().__init__()
+        self.max_value = max_value
+
+    def __call__(self, image: np.ndarray, mask: np.ndarray, joints: np.ndarray, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]):
+        image = (image / self.max_value).astype(np.float32)
+        return image, mask, joints, areas, bboxes
+
+    def get_equivalent_preprocessing(self) -> List[Dict]:
+        return [{Processings.StandardizeImage: {"max_value": self.max_value}}]
+
+    def __repr__(self):
+        return self.__class__.__name__ + f"(max_value={self.max_value})"
 
 
 @register_transform(Transforms.KeypointsImageNormalize)
 class KeypointsImageNormalize(KeypointTransform):
     """
-    Normalize image with mean and std. Note this transform should come after KeypointsImageToTensor
-    since it operates on torch Tensor and not numpy array.
+    Normalize image with mean and std.
     """
 
     def __init__(self, mean, std):
-        self.mean = mean
-        self.std = std
+        self.mean = np.array(list(mean)).reshape((1, 1, -1)).astype(np.float32)
+        self.std = np.array(list(std)).reshape((1, 1, -1)).astype(np.float32)
 
     def __call__(self, image: np.ndarray, mask: np.ndarray, joints: np.ndarray, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]):
-        image = F.normalize(image, mean=self.mean, std=self.std)
+        image = (image - self.mean) / self.std
         return image, mask, joints, areas, bboxes
 
+    def __repr__(self):
+        return self.__class__.__name__ + f"(mean={self.mean}, std={self.std})"
+
+    def get_equivalent_preprocessing(self) -> List:
+        return [{Processings.NormalizeImage: {"mean": self.mean, "std": self.std}}]
+
 
 @register_transform(Transforms.KeypointsRandomHorizontalFlip)
 class KeypointsRandomHorizontalFlip(KeypointTransform):
     """
     Flip image, mask and joints horizontally with a given probability.
     """
 
@@ -102,14 +155,17 @@
                            So this array contains order of keypoints on the flipped image. This is dataset specific and depends on
                            how keypoints are defined in dataset.
         :param prob: Probability of flipping
         """
         self.flip_index = flip_index
         self.prob = prob
 
+    def __repr__(self):
+        return self.__class__.__name__ + f"(flip_index={self.flip_index}, prob={self.prob})"
+
     def __call__(self, image, mask, joints, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]):
         if image.shape[:2] != mask.shape[:2]:
             raise RuntimeError(f"Image shape ({image.shape[:2]}) does not match mask shape ({mask.shape[:2]}).")
 
         if random.random() < self.prob:
             image = self.apply_to_image(image)
             mask = self.apply_to_image(mask)
@@ -132,14 +188,17 @@
         return keypoints
 
     def apply_to_bboxes(self, bboxes, cols):
         bboxes = bboxes.copy()
         bboxes[:, 0] = cols - (bboxes[:, 0] + bboxes[:, 2])
         return bboxes
 
+    def get_equivalent_preprocessing(self) -> List:
+        raise RuntimeError("KeypointsRandomHorizontalFlip does not have equivalent preprocessing.")
+
 
 @register_transform(Transforms.KeypointsRandomVerticalFlip)
 class KeypointsRandomVerticalFlip(KeypointTransform):
     """
     Flip image, mask and joints vertically with a given probability.
     """
 
@@ -171,14 +230,20 @@
         return keypoints
 
     def apply_to_bboxes(self, bboxes, rows):
         bboxes = bboxes.copy()
         bboxes[:, 1] = rows - (bboxes[:, 1] + bboxes[:, 3]) - 1
         return bboxes
 
+    def get_equivalent_preprocessing(self) -> List:
+        raise RuntimeError("KeypointsRandomHorizontalFlip does not have equivalent preprocessing.")
+
+    def __repr__(self):
+        return self.__class__.__name__ + f"(prob={self.prob})"
+
 
 @register_transform(Transforms.KeypointsLongestMaxSize)
 class KeypointsLongestMaxSize(KeypointTransform):
     """
     Resize image, mask and joints to ensure that resulting image does not exceed max_sizes (rows, cols).
     """
 
@@ -231,14 +296,24 @@
         keypoints[:, :, 0:2] *= scale
         return keypoints
 
     @classmethod
     def apply_to_bboxes(cls, bboxes, scale):
         return bboxes * scale
 
+    def __repr__(self):
+        return (
+            self.__class__.__name__ + f"(max_height={self.max_height}, "
+            f"max_width={self.max_width}, "
+            f"interpolation={self.interpolation}, prob={self.prob})"
+        )
+
+    def get_equivalent_preprocessing(self) -> List:
+        return [{Processings.KeypointsLongestMaxSizeRescale: {"output_shape": (self.max_height, self.max_width)}}]
+
 
 @register_transform(Transforms.KeypointsPadIfNeeded)
 class KeypointsPadIfNeeded(KeypointTransform):
     """
     Pad image and mask to ensure that resulting image size is not less than `output_size` (rows, cols).
     Image and mask padded from right and bottom, thus joints remains unchanged.
     """
@@ -248,33 +323,45 @@
 
         :param output_size: Desired image size (rows, cols)
         :param image_pad_value: Padding value of image
         :param mask_pad_value: Padding value for mask
         """
         self.min_height = min_height
         self.min_width = min_width
-        self.image_pad_value = tuple(image_pad_value) if isinstance(image_pad_value, Iterable) else int(image_pad_value)
+        self.image_pad_value = image_pad_value
         self.mask_pad_value = mask_pad_value
 
     def __call__(self, image, mask, joints, areas: Optional[np.ndarray], bboxes: Optional[np.ndarray]):
         height, width = image.shape[:2]
 
         pad_bottom = max(0, self.min_height - height)
         pad_right = max(0, self.min_width - width)
 
-        image = cv2.copyMakeBorder(image, top=0, bottom=pad_bottom, left=0, right=pad_right, value=self.image_pad_value, borderType=cv2.BORDER_CONSTANT)
+        image_pad_value = tuple(self.image_pad_value) if isinstance(self.image_pad_value, Iterable) else tuple([self.image_pad_value] * image.shape[-1])
+        image = cv2.copyMakeBorder(image, top=0, bottom=pad_bottom, left=0, right=pad_right, value=image_pad_value, borderType=cv2.BORDER_CONSTANT)
 
         original_dtype = mask.dtype
         mask = cv2.copyMakeBorder(
             mask.astype(np.uint8), top=0, bottom=pad_bottom, left=0, right=pad_right, value=self.mask_pad_value, borderType=cv2.BORDER_CONSTANT
         )
         mask = mask.astype(original_dtype)
 
         return image, mask, joints, areas, bboxes
 
+    def __repr__(self):
+        return (
+            self.__class__.__name__ + f"(min_height={self.min_height}, "
+            f"min_width={self.min_width}, "
+            f"image_pad_value={self.image_pad_value}, "
+            f"mask_pad_value={self.mask_pad_value})"
+        )
+
+    def get_equivalent_preprocessing(self) -> List:
+        return [{Processings.KeypointsBottomRightPadding: {"output_shape": (self.min_height, self.min_width), "pad_value": self.image_pad_value}}]
+
 
 @register_transform(Transforms.KeypointsRandomAffineTransform)
 class KeypointsRandomAffineTransform(KeypointTransform):
     """
     Apply random affine transform to image, mask and joints.
     """
 
@@ -295,18 +382,29 @@
         :param max_scale: Lower bound for the scale change. For +- 20% size jitter this should be 1.2
         :param max_translate: Max translation offset in percents of image size
         """
         self.max_rotation = max_rotation
         self.min_scale = min_scale
         self.max_scale = max_scale
         self.max_translate = max_translate
-        self.image_pad_value = tuple(image_pad_value) if isinstance(image_pad_value, Iterable) else int(image_pad_value)
+        self.image_pad_value = image_pad_value
         self.mask_pad_value = mask_pad_value
         self.prob = prob
 
+    def __repr__(self):
+        return (
+            self.__class__.__name__ + f"(max_rotation={self.max_rotation}, "
+            f"min_scale={self.min_scale}, "
+            f"max_scale={self.max_scale}, "
+            f"max_translate={self.max_translate}, "
+            f"image_pad_value={self.image_pad_value}, "
+            f"mask_pad_value={self.mask_pad_value}, "
+            f"prob={self.prob})"
+        )
+
     def _get_affine_matrix(self, img, angle, scale, dx, dy):
         """
 
         :param center: (x,y)
         :param scale:
         :param output_size: (rows, cols)
         :param rot:
@@ -333,16 +431,18 @@
             scale = random.uniform(self.min_scale, self.max_scale)
             dx = random.uniform(-self.max_translate, self.max_translate)
             dy = random.uniform(-self.max_translate, self.max_translate)
 
             mat_output = self._get_affine_matrix(image, angle, scale, dx, dy)
             mat_output = mat_output[:2]
 
+            image_pad_value = tuple(self.image_pad_value) if isinstance(self.image_pad_value, Iterable) else tuple([self.image_pad_value] * image.shape[-1])
+
             mask = self.apply_to_image(mask, mat_output, cv2.INTER_NEAREST, self.mask_pad_value, cv2.BORDER_CONSTANT)
-            image = self.apply_to_image(image, mat_output, cv2.INTER_LINEAR, self.image_pad_value, cv2.BORDER_CONSTANT)
+            image = self.apply_to_image(image, mat_output, cv2.INTER_LINEAR, image_pad_value, cv2.BORDER_CONSTANT)
 
             joints = self.apply_to_keypoints(joints, mat_output, image.shape)
 
             if bboxes is not None:
                 bboxes = self.apply_to_bboxes(bboxes, mat_output)
 
             if areas is not None:
@@ -399,7 +499,10 @@
             image,
             mat,
             dsize=(image.shape[1], image.shape[0]),
             flags=interpolation,
             borderValue=padding_value,
             borderMode=padding_mode,
         )
+
+    def get_equivalent_preprocessing(self) -> List:
+        raise RuntimeError(f"{self.__class__} does not have equivalent preprocessing.")
```

## super_gradients/training/transforms/transforms.py

```diff
@@ -1,10 +1,11 @@
 import collections
 import math
 import random
+import warnings
 from numbers import Number
 from typing import Optional, Union, Tuple, List, Sequence, Dict
 
 import cv2
 import numpy as np
 import torch.nn
 from PIL import Image, ImageFilter, ImageOps
@@ -650,16 +651,18 @@
         if self.enable_mixup and random.random() < self.prob:
             origin_img, origin_labels = sample["image"], sample["target"]
             target_dim = self.input_dim if self.input_dim is not None else sample["image"].shape[:2]
 
             cp_sample = sample["additional_samples"][0]
             img, cp_labels = cp_sample["image"], cp_sample["target"]
             cp_boxes = cp_labels[:, :4]
-
-            img, cp_boxes = _mirror(img, cp_boxes, self.flip_prob)
+            if random.random() < self.prob:
+                _, width, _ = img.shape
+                img = _flip_horizontal_image(img)
+                cp_boxes = _flip_horizontal_boxes(cp_boxes, width)
             # PLUG IN TARGET THE FLIPPED BOXES
             cp_labels[:, :4] = cp_boxes
 
             jit_factor = random.uniform(*self.mixup_scale)
 
             if len(img.shape) == 3:
                 cp_img = np.ones((target_dim[0], target_dim[1], 3), dtype=np.uint8) * self.border_value
@@ -772,26 +775,28 @@
 
 @register_transform(Transforms.DetectionPaddedRescale)
 class DetectionPaddedRescale(DetectionTransform):
     """
     Preprocessing transform to be applied last of all transforms for validation.
 
     Image- Rescales and pads to self.input_dim.
-    Targets- pads targets to max_targets, moves the class label to first index, converts boxes format- xyxy -> cxcywh.
+    Targets- moves the class label to first index, converts boxes format- xyxy -> cxcywh.
 
     :param input_dim:   Final input dimension (default=(640,640))
     :param swap:        Image axis's to be rearranged.
-    :param max_targets:
     :param pad_value:   Padding value for image.
     """
 
-    def __init__(self, input_dim: Union[int, Tuple[int, int], None], swap: Tuple[int, ...] = (2, 0, 1), max_targets: int = 50, pad_value: int = 114):
+    def __init__(
+        self, input_dim: Union[int, Tuple[int, int], None], swap: Tuple[int, ...] = (2, 0, 1), max_targets: Optional[int] = None, pad_value: int = 114
+    ):
+        super().__init__()
+        _max_targets_deprication(max_targets)
         self.swap = swap
         self.input_dim = ensure_is_tuple_of_two(input_dim)
-        self.max_targets = max_targets
         self.pad_value = pad_value
 
     def __call__(self, sample: dict) -> dict:
         img, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
         img, r = _rescale_and_pad_to_size(img, self.input_dim, self.swap, self.pad_value)
 
         sample["image"] = img
@@ -810,32 +815,65 @@
 
 @register_transform(Transforms.DetectionHorizontalFlip)
 class DetectionHorizontalFlip(DetectionTransform):
     """
     Horizontal Flip for Detection
 
     :param prob:        Probability of applying horizontal flip
-    :param max_targets: Max objects in single image, padding target to this size in case of empty image.
     """
 
-    def __init__(self, prob: float, max_targets: int = 120):
+    def __init__(self, prob: float, max_targets: Optional[int] = None):
         super(DetectionHorizontalFlip, self).__init__()
+        _max_targets_deprication(max_targets)
         self.prob = prob
-        self.max_targets = max_targets
 
     def __call__(self, sample):
         image, targets = sample["image"], sample["target"]
-        boxes = targets[:, :4]
-        if len(boxes) == 0:
-            targets = np.zeros((self.max_targets, 5), dtype=np.float32)
-            boxes = targets[:, :4]
-        image, boxes = _mirror(image, boxes, self.prob)
-        targets[:, :4] = boxes
+        crowd_targets = sample.get("crowd_targets")
+        if len(targets) == 0:
+            targets = np.zeros((0, 5), dtype=np.float32)
+        if random.random() < self.prob:
+            image = _flip_horizontal_image(image)
+            _, width, _ = image.shape
+            targets[:, :4] = _flip_horizontal_boxes(targets[:, :4], width)
+            if crowd_targets is not None:
+                crowd_targets = _flip_horizontal_boxes(crowd_targets, width)
+        sample["image"] = image
         sample["target"] = targets
+        sample["crowd_targets"] = crowd_targets
+        return sample
+
+
+@register_transform(Transforms.DetectionVerticalFlip)
+class DetectionVerticalFlip(DetectionTransform):
+    """
+    Vertical Flip for Detection
+
+    :param prob:        Probability of applying vertical flip
+    """
+
+    def __init__(self, prob: float, max_targets: Optional[int] = None):
+        super(DetectionVerticalFlip, self).__init__()
+        _max_targets_deprication(max_targets)
+        self.prob = prob
+
+    def __call__(self, sample):
+        image, targets = sample["image"], sample["target"]
+        crowd_targets = sample.get("crowd_targets")
+        if len(targets) == 0:
+            targets = np.zeros((0, 5), dtype=np.float32)
+        if random.random() < self.prob:
+            image = _flip_vertical_image(image)
+            height, _, _ = image.shape
+            targets[:, :4] = _flip_vertical_boxes(targets[:, :4], height)
+            if crowd_targets is not None:
+                crowd_targets[:, :4] = _flip_vertical_boxes(crowd_targets[:, :4], height)
         sample["image"] = image
+        sample["target"] = targets
+        sample["crowd_targets"] = crowd_targets
         return sample
 
 
 @register_transform(Transforms.DetectionRescale)
 class DetectionRescale(DetectionTransform):
     """
     Resize image and bounding boxes to given image dimensions without preserving aspect ratio
@@ -1008,38 +1046,37 @@
 
     Convert targets in input_format to output_format, filter small bboxes and pad targets.
 
     :param input_dim:          Shape of the images to transform.
     :param input_format:       Format of the input targets. For instance [xmin, ymin, xmax, ymax, cls_id] refers to XYXY_LABEL.
     :param output_format:      Format of the output targets. For instance [xmin, ymin, xmax, ymax, cls_id] refers to XYXY_LABEL
     :param min_bbox_edge_size: bboxes with edge size lower then this values will be removed.
-    :param max_targets:        Max objects in single image, padding target to this size.
     """
 
     @resolve_param("input_format", ConcatenatedTensorFormatFactory())
     @resolve_param("output_format", ConcatenatedTensorFormatFactory())
     def __init__(
         self,
         input_dim: Union[int, Tuple[int, int], None] = None,
         input_format: ConcatenatedTensorFormat = XYXY_LABEL,
         output_format: ConcatenatedTensorFormat = LABEL_CXCYWH,
         min_bbox_edge_size: float = 1,
-        max_targets: int = 120,
+        max_targets: Optional[int] = None,
     ):
         super(DetectionTargetsFormatTransform, self).__init__()
+        _max_targets_deprication(max_targets)
         if isinstance(input_format, DetectionTargetsFormat) or isinstance(output_format, DetectionTargetsFormat):
             raise TypeError(
                 "DetectionTargetsFormat is not supported for input_format and output_format starting from super_gradients==3.0.7.\n"
                 "You can either:\n"
                 "\t - use builtin format among super_gradients.training.datasets.data_formats.default_formats.<FORMAT_NAME> (e.g. XYXY_LABEL, CXCY_LABEL, ..)\n"
                 "\t - define your custom format using super_gradients.training.datasets.data_formats.formats.ConcatenatedTensorFormat\n"
             )
         self.input_format = input_format
         self.output_format = output_format
-        self.max_targets = max_targets
         self.min_bbox_edge_size = min_bbox_edge_size
         self.input_dim = None
 
         if input_dim is not None:
             input_dim = ensure_is_tuple_of_two(input_dim)
             self._setup_input_dim_related_params(input_dim)
 
@@ -1062,33 +1099,25 @@
             sample["crowd_target"] = self.apply_on_targets(sample["crowd_target"])
         return sample
 
     def apply_on_targets(self, targets: np.ndarray) -> np.ndarray:
         """Convert targets in input_format to output_format, filter small bboxes and pad targets"""
         targets = self.targets_format_converter(targets)
         targets = self.filter_small_bboxes(targets)
-        targets = self.pad_targets(targets)
-        return targets
+        return np.ascontiguousarray(targets, dtype=np.float32)
 
     def filter_small_bboxes(self, targets: np.ndarray) -> np.ndarray:
         """Filter bboxes smaller than specified threshold."""
 
         def _is_big_enough(bboxes: np.ndarray) -> np.ndarray:
             return np.minimum(bboxes[:, 2], bboxes[:, 3]) > self.min_bbox_edge_size
 
         targets = filter_on_bboxes(fn=_is_big_enough, tensor=targets, tensor_format=self.output_format)
         return targets
 
-    def pad_targets(self, targets: np.ndarray) -> np.ndarray:
-        """Pad targets."""
-        padded_targets = np.zeros((self.max_targets, targets.shape[-1]))
-        padded_targets[range(len(targets))[: self.max_targets]] = targets[: self.max_targets]
-        padded_targets = np.ascontiguousarray(padded_targets, dtype=np.float32)
-        return padded_targets
-
     def get_equivalent_preprocessing(self) -> List:
         return []
 
 
 def get_aug_params(value: Union[tuple, float], center: float = 0) -> float:
     """
     Generates a random value for augmentations as described below
@@ -1281,29 +1310,50 @@
     box2 = box2.T
     w1, h1 = box1[2] - box1[0], box1[3] - box1[1]
     w2, h2 = box2[2] - box2[0], box2[3] - box2[1]
     ar = np.maximum(w2 / (h2 + 1e-16), h2 / (w2 + 1e-16))  # aspect ratio
     return (w2 > wh_thr) & (h2 > wh_thr) & (w2 * h2 / (w1 * h1 + 1e-16) > area_thr) & (ar < ar_thr)  # candidates
 
 
-def _mirror(image, boxes, prob=0.5):
+def _flip_horizontal_image(image: np.ndarray) -> np.ndarray:
+    """
+    Horizontally flips image
+    :param image: image to be flipped.
+    :return: flipped_image
     """
-    Horizontal flips image and bboxes with probability prob.
+    return image[:, ::-1]
 
-    :param image: (np.array) image to be flipped.
-    :param boxes: (np.array) bboxes to be modified.
-    :param prob: probability to perform flipping.
-    :return: flipped_image, flipped_bboxes
-    """
-    flipped_boxes = boxes.copy()
-    _, width, _ = image.shape
-    if random.random() < prob:
-        image = image[:, ::-1]
-        flipped_boxes[:, 0::2] = width - boxes[:, 2::-2]
-    return image, flipped_boxes
+
+def _flip_horizontal_boxes(boxes: np.ndarray, img_width: int) -> np.ndarray:
+    """
+    Horizontally flips bboxes
+    :param boxes: bboxes to be flipped. (xyxy format)
+    :return: flipped_boxes
+    """
+    boxes[:, [0, 2]] = img_width - boxes[:, [2, 0]]
+    return boxes
+
+
+def _flip_vertical_image(image: np.ndarray) -> np.ndarray:
+    """
+    Vertically flips image
+    :param image: image to be flipped.
+    :return: flipped_image
+    """
+    return image[::-1, :]
+
+
+def _flip_vertical_boxes(boxes: np.ndarray, img_height: int) -> np.ndarray:
+    """
+    Vertically flips bboxes
+    :param boxes: bboxes to be flipped. (xyxy format)
+    :return: flipped_boxes
+    """
+    boxes[:, [1, 3]] = img_height - boxes[:, [3, 1]]
+    return boxes
 
 
 def augment_hsv(img: np.array, hgain: float, sgain: float, vgain: float, bgr_channels=(0, 1, 2)):
     hsv_augs = np.random.uniform(-1, 1, 3) * [hgain, sgain, vgain]  # random gains
     hsv_augs *= np.random.randint(0, 2, 3)  # random selection of h, s, v
     hsv_augs = hsv_augs.astype(np.int16)
     img_hsv = cv2.cvtColor(img[..., bgr_channels], cv2.COLOR_BGR2HSV).astype(np.int16)
@@ -1327,7 +1377,16 @@
 
     def __init__(self, max_val=255.0):
         super(Standardize, self).__init__()
         self.max_val = max_val
 
     def forward(self, img):
         return img / self.max_val
+
+
+def _max_targets_deprication(max_targets: Optional[int] = None):
+    if max_targets is not None:
+        warnings.warn(
+            "max_targets is deprecated and will be removed in the future, targets are not padded to the max length anymore. "
+            "If you are using collate_fn provided by SG, it is safe to simply drop this argument.",
+            DeprecationWarning,
+        )
```

## super_gradients/training/transforms/utils.py

```diff
@@ -15,36 +15,54 @@
     right: int
 
 
 def _rescale_image(image: np.ndarray, target_shape: Tuple[int, int]) -> np.ndarray:
     """Rescale image to target_shape, without preserving aspect ratio.
 
     :param image:           Image to rescale. (H, W, C) or (H, W).
-    :param target_shape:    Target shape to rescale to.
+    :param target_shape:    Target shape to rescale to (H, W).
     :return:                Rescaled image.
     """
     height, width = target_shape[:2]
-    return cv2.resize(image, dsize=(width, height), interpolation=cv2.INTER_LINEAR).astype(np.uint8)
+    return cv2.resize(image, dsize=(width, height), interpolation=cv2.INTER_LINEAR)
 
 
-def _rescale_bboxes(targets: np.array, scale_factors: Tuple[float, float]) -> np.array:
+def _rescale_bboxes(targets: np.ndarray, scale_factors: Tuple[float, float]) -> np.ndarray:
     """Rescale bboxes to given scale factors, without preserving aspect ratio.
 
     :param targets:         Targets to rescale (N, 4+), where target[:, :4] is the bounding box coordinates.
     :param scale_factors:   Tuple of (scale_factor_h, scale_factor_w) scale factors to rescale to.
     :return:                Rescaled targets.
     """
 
     targets = targets.astype(np.float32, copy=True)
 
     sy, sx = scale_factors
     targets[:, :4] *= np.array([[sx, sy, sx, sy]], dtype=targets.dtype)
     return targets
 
 
+def _rescale_keypoints(targets: np.ndarray, scale_factors: Tuple[float, float]) -> np.ndarray:
+    """Rescale keypoints to given scale factors, without preserving aspect ratio.
+
+    :param targets:         Array of keypoints to rescale. Can have arbitrary shape [N,2], [N,K,2], etc.
+                            Last dimension encodes XY coordinates: target[..., 0] is the X coordinates and
+                            targets[..., 1] is the Y coordinate.
+    :param scale_factors:   Tuple of (scale_factor_h, scale_factor_w) scale factors to rescale to.
+    :return:                Rescaled targets.
+    """
+
+    targets = targets.astype(np.float32, copy=True)
+
+    sy, sx = scale_factors
+    targets[..., 0] *= sx
+    targets[..., 1] *= sy
+    return targets
+
+
 def _get_center_padding_coordinates(input_shape: Tuple[int, int], output_shape: Tuple[int, int]) -> PaddingCoordinates:
     """Get parameters for padding an image to given output shape, in center mode.
 
     :param input_shape:  Shape of the input image.
     :param output_shape: Shape to resize to.
     :return:             Padding parameters.
     """
@@ -78,14 +96,15 @@
     :param pad_h:       Tuple of (padding_top, padding_bottom).
     :param pad_w:       Tuple of (padding_left, padding_right).
     :param pad_value:   Padding value
     :return:            Image shifted according to padding coordinates.
     """
     pad_h = (padding_coordinates.top, padding_coordinates.bottom)
     pad_w = (padding_coordinates.left, padding_coordinates.right)
+
     if len(image.shape) == 3:
         return np.pad(image, (pad_h, pad_w, (0, 0)), "constant", constant_values=pad_value)
     else:
         return np.pad(image, (pad_h, pad_w), "constant", constant_values=pad_value)
 
 
 def _shift_bboxes(targets: np.array, shift_w: float, shift_h: float) -> np.array:
@@ -98,14 +117,28 @@
     """
     boxes, labels = targets[:, :4], targets[:, 4:]
     boxes[:, [0, 2]] += shift_w
     boxes[:, [1, 3]] += shift_h
     return np.concatenate((boxes, labels), 1)
 
 
+def _shift_keypoints(targets: np.array, shift_w: float, shift_h: float) -> np.array:
+    """Shift keypoints with respect to padding values.
+
+    :param targets:  Keypoints to transform of shape (N, 2+), or (N, K, 2+), in format [x1, y1, ...]
+    :param shift_w:  shift width.
+    :param shift_h:  shift height.
+    :return:         Transformed keypoints of the same shape as input.
+    """
+    targets = targets.copy()
+    targets[..., 0] += shift_w
+    targets[..., 1] += shift_h
+    return targets
+
+
 def _rescale_xyxy_bboxes(targets: np.array, r: float) -> np.array:
     """Scale targets to given scale factors.
 
     :param targets:  Bboxes to transform of shape (N, 4+), in format [x1, y1, x2, y2, ...]
     :param r:        DetectionRescale coefficient that was applied to the image
     :return:         Rescaled Bboxes to transform of shape (N, 4+), in format [x1, y1, x2, y2, ...]
     """
```

## super_gradients/training/utils/__init__.py

```diff
@@ -1,11 +1,10 @@
 from super_gradients.training.utils.utils import (
     Timer,
     HpmStruct,
-    WrappedModel,
     convert_to_tensor,
     get_param,
     tensor_container_to_device,
     random_seed,
     make_divisible,
 )
 from super_gradients.training.utils.checkpoint_utils import adapt_state_dict_to_fit_model_layer_names, raise_informative_runtime_error
@@ -13,15 +12,14 @@
 from super_gradients.training.utils.config_utils import raise_if_unused_params, warn_if_unused_params
 from super_gradients.training.utils.early_stopping import EarlyStop
 from super_gradients.training.utils.pose_estimation import DEKRPoseEstimationDecodeCallback, DEKRVisualizationCallback
 
 __all__ = [
     "Timer",
     "HpmStruct",
-    "WrappedModel",
     "convert_to_tensor",
     "get_param",
     "tensor_container_to_device",
     "adapt_state_dict_to_fit_model_layer_names",
     "raise_informative_runtime_error",
     "random_seed",
     "torch_version_is_greater_or_equal",
```

## super_gradients/training/utils/checkpoint_utils.py

```diff
@@ -10,14 +10,15 @@
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.data_interface.adnn_model_repository_data_interface import ADNNModelRepositoryDataInterfaces
 from super_gradients.common.data_types import StrictLoad
 from super_gradients.common.decorators.explicit_params_validator import explicit_params_validation
 from super_gradients.module_interfaces import HasPredict
 from super_gradients.training.pretrained_models import MODEL_URLS
 from super_gradients.training.utils.distributed_training_utils import get_local_rank, wait_for_the_master
+from super_gradients.training.utils.utils import unwrap_model
 
 try:
     from torch.hub import download_url_to_file, load_state_dict_from_url
 except (ModuleNotFoundError, ImportError, NameError):
     from torch.hub import _download_url_to_file as download_url_to_file
 
 
@@ -43,21 +44,28 @@
             pass
 
 
 def adaptive_load_state_dict(net: torch.nn.Module, state_dict: dict, strict: Union[bool, StrictLoad], solver=None):
     """
     Adaptively loads state_dict to net, by adapting the state_dict to net's layer names first.
     :param net: (nn.Module) to load state_dict to
-    :param state_dict: (dict) Chekpoint state_dict
+    :param state_dict: (dict) Checkpoint state_dict
     :param strict: (StrictLoad) key matching strictness
     :param solver: callable with signature (ckpt_key, ckpt_val, model_key, model_val)
                      that returns a desired weight for ckpt_val.
     :return:
     """
     state_dict = state_dict["net"] if "net" in state_dict else state_dict
+
+    # This is a backward compatibility fix for checkpoints that were saved with DataParallel/DistributedDataParallel wrapper
+    # and contains "module." prefix in all keys
+    # If all keys start with "module.", then we remove it.
+    if all([key.startswith("module.") for key in state_dict.keys()]):
+        state_dict = collections.OrderedDict([(key[7:], value) for key, value in state_dict.items()])
+
     try:
         strict_bool = strict if isinstance(strict, bool) else strict != StrictLoad.OFF
         net.load_state_dict(state_dict, strict=strict_bool)
     except (RuntimeError, ValueError, KeyError) as ex:
         if strict == StrictLoad.NO_KEY_MATCHING:
             adapted_state_dict = adapt_state_dict_to_fit_model_layer_names(net.state_dict(), state_dict, solver=solver)
             net.load_state_dict(adapted_state_dict["net"], strict=True)
@@ -128,15 +136,15 @@
 
 
 def read_ckpt_state_dict(ckpt_path: str, device="cpu") -> Mapping[str, torch.Tensor]:
     """
     Reads a checkpoint state dict from a given path or url
 
     :param ckpt_path: Checkpoint path or url
-    :param device: Target devide where tensors should be loaded
+    :param device: Target device where tensors should be loaded
     :return: Checkpoint state dict object
     """
 
     if ckpt_path.startswith("https://"):
         with wait_for_the_master(get_local_rank()):
             state_dict = load_state_dict_from_url(ckpt_path, progress=False, map_location=device)
         return state_dict
@@ -213,14 +221,16 @@
     :param load_processing_params: Whether to call set_dataset_processing_params on "processing_params" entry inside the
      checkpoint file (default=False).
     :return:
     """
     if isinstance(strict, str):
         strict = StrictLoad(strict)
 
+    net = unwrap_model(net)
+
     if load_backbone and not hasattr(net, "backbone"):
         raise ValueError("No backbone attribute in net - Can't load backbone weights")
 
     # LOAD THE LOCAL CHECKPOINT PATH INTO A state_dict OBJECT
     checkpoint = read_ckpt_state_dict(ckpt_path=ckpt_local_path)
 
     if load_ema_as_net:
@@ -235,15 +245,15 @@
     else:
         adaptive_load_state_dict(net, checkpoint, strict)
 
     message_suffix = " checkpoint." if not load_ema_as_net else " EMA checkpoint."
     message_model = "model" if not load_backbone else "model's backbone"
     logger.info("Successfully loaded " + message_model + " weights from " + ckpt_local_path + message_suffix)
 
-    if (isinstance(net, HasPredict) or (hasattr(net, "module") and isinstance(net.module, HasPredict))) and load_processing_params:
+    if (isinstance(net, HasPredict)) and load_processing_params:
         if "processing_params" not in checkpoint.keys():
             raise ValueError("Can't load processing params - could not find any stored in checkpoint file.")
         try:
             net.set_dataset_processing_params(**checkpoint["processing_params"])
         except Exception as e:
             logger.warning(
                 f"Could not set preprocessing pipeline from the checkpoint dataset: {e}. Before calling"
@@ -271,15 +281,15 @@
 def _yolox_ckpt_solver(ckpt_key, ckpt_val, model_key, model_val):
     """
     Helper method for reshaping old pretrained checkpoint's focus weights to 6x6 conv weights.
     """
 
     if (
         ckpt_val.shape != model_val.shape
-        and ckpt_key == "module._backbone._modules_list.0.conv.conv.weight"
+        and (ckpt_key == "module._backbone._modules_list.0.conv.conv.weight" or ckpt_key == "_backbone._modules_list.0.conv.conv.weight")
         and model_key == "_backbone._modules_list.0.conv.weight"
     ):
         model_val.data[:, :, ::2, ::2] = ckpt_val.data[:, :3]
         model_val.data[:, :, 1::2, ::2] = ckpt_val.data[:, 3:6]
         model_val.data[:, :, ::2, 1::2] = ckpt_val.data[:, 6:9]
         model_val.data[:, :, 1::2, 1::2] = ckpt_val.data[:, 9:12]
         replacement = model_val
```

## super_gradients/training/utils/detection_utils.py

```diff
@@ -1,23 +1,22 @@
 import math
 import os
 import pathlib
 import random
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Callable, List, Union, Tuple, Optional, Dict
+from typing import Callable, List, Union, Tuple, Optional, Dict, Type
 
 import cv2
 
 import numpy as np
 import torch
 import torchvision
 from omegaconf import ListConfig
 from torch import nn
-from torch.utils.data.dataloader import default_collate
 
 from super_gradients.common.registry.registry import register_collate_function
 from super_gradients.training.utils.visualization.detection import draw_bbox
 from super_gradients.training.utils.visualization.utils import generate_color_mapping
 
 
 class DetectionTargetsFormat(Enum):
@@ -200,20 +199,30 @@
     MAP_05_TO_095 = (0.5, 0.95)
 
     def is_range(self):
         return self[0] != self[1]
 
     def to_tensor(self):
         if self.is_range():
-            n_iou_thresh = int(round((self[1] - self[0]) / 0.05)) + 1
-            return torch.linspace(self[0], self[1], n_iou_thresh)
+            return self.from_bounds(self[0], self[1], step=0.05)
         else:
-            n_iou_thresh = 1
             return torch.tensor([self[0]])
 
+    @classmethod
+    def from_bounds(cls, low: float, high: float, step: float = 0.05) -> torch.Tensor:
+        """
+        Create a tensor with values from low (including) to high (including) with a given step size.
+        :param low: Lower bound
+        :param high: Upper bound
+        :param step: Step size
+        :return: Tensor of [low, low + step, low + 2 * step, ..., high]
+        """
+        n_iou_thresh = int(round((high - low) / step)) + 1
+        return torch.linspace(low, high, n_iou_thresh)
+
 
 def box_iou(box1: torch.Tensor, box2: torch.Tensor) -> torch.Tensor:
     # https://github.com/pytorch/vision/blob/master/torchvision/ops/boxes.py
     """
     Return intersection-over-union (Jaccard index) of boxes.
     Both sets of boxes are expected to be in (x1, y1, x2, y2) format.
     :param box1: Tensor of shape [N, 4]
@@ -229,26 +238,34 @@
     area2 = box_area(box2.T)
 
     # inter(N,M) = (rb(N,M,2) - lt(N,M,2)).clamp(0).prod(2)
     inter = (torch.min(box1[:, None, 2:], box2[:, 2:]) - torch.max(box1[:, None, :2], box2[:, :2])).clamp(0).prod(2)
     return inter / (area1[:, None] + area2 - inter)  # iou = inter / (area1 + area2 - inter)
 
 
-def non_max_suppression(prediction, conf_thres=0.1, iou_thres=0.6, multi_label_per_box: bool = True, with_confidence: bool = False):
+def non_max_suppression(
+    prediction, conf_thres=0.1, iou_thres=0.6, multi_label_per_box: bool = True, with_confidence: bool = False, class_agnostic_nms: bool = False
+):
     """
     Performs Non-Maximum Suppression (NMS) on inference results
-        :param prediction: raw model prediction. Should be a list of Tensors of shape (cx, cy, w, h, confidence, cls0, cls1, ...)
-        :param conf_thres: below the confidence threshold - prediction are discarded
-        :param iou_thres: IoU threshold for the nms algorithm
-        :param multi_label_per_box: whether to use re-use each box with all possible labels
-                                    (instead of the maximum confidence all confidences above threshold
-                                    will be sent to NMS); by default is set to True
-        :param with_confidence: whether to multiply objectness score with class score.
-                                usually valid for Yolo models only.
-        :return: detections with shape nx6 (x1, y1, x2, y2, object_conf, class_conf, class)
+
+    :param prediction: raw model prediction. Should be a list of Tensors of shape (cx, cy, w, h, confidence, cls0, cls1, ...)
+    :param conf_thres: below the confidence threshold - prediction are discarded
+    :param iou_thres: IoU threshold for the nms algorithm
+    :param multi_label_per_box: controls whether to decode multiple labels per box.
+                                True - each anchor can produce multiple labels of different classes
+                                       that pass confidence threshold check (default).
+                                False - each anchor can produce only one label of the class with the highest score.
+    :param with_confidence: whether to multiply objectness score with class score.
+                            usually valid for Yolo models only.
+    :param class_agnostic_nms: indicates how boxes of different classes will be treated during NMS
+                               True - NMS will be performed on all classes together.
+                               False - NMS will be performed on each class separately (default).
+    :return: detections with shape nx6 (x1, y1, x2, y2, object_conf, class_conf, class)
+
     """
     candidates_above_thres = prediction[..., 4] > conf_thres  # filter by confidence
     output = [None] * prediction.shape[0]
 
     for image_idx, pred in enumerate(prediction):
 
         pred = pred[candidates_above_thres[image_idx]]  # confident
@@ -271,26 +288,25 @@
             pred = torch.cat((box, conf, j.float()), 1)[conf.view(-1) > conf_thres]
 
         if not pred.shape[0]:  # If none remain process next image
             continue
 
         # Apply torch batched NMS algorithm
         boxes, scores, cls_idx = pred[:, :4], pred[:, 4], pred[:, 5]
-        idx_to_keep = torchvision.ops.boxes.batched_nms(boxes, scores, cls_idx, iou_thres)
+        if class_agnostic_nms:
+            idx_to_keep = torchvision.ops.boxes.nms(boxes, scores, iou_thres)
+        else:
+            idx_to_keep = torchvision.ops.boxes.batched_nms(boxes, scores, cls_idx, iou_thres)
         output[image_idx] = pred[idx_to_keep]
 
     return output
 
 
 def matrix_non_max_suppression(
-    pred,
-    conf_thres: float = 0.1,
-    kernel: str = "gaussian",
-    sigma: float = 3.0,
-    max_num_of_detections: int = 500,
+    pred, conf_thres: float = 0.1, kernel: str = "gaussian", sigma: float = 3.0, max_num_of_detections: int = 500, class_agnostic_nms: bool = False
 ) -> List[torch.Tensor]:
     """Performs Matrix Non-Maximum Suppression (NMS) on inference results https://arxiv.org/pdf/1912.04488.pdf
 
     :param pred:        Raw model prediction (in test mode) - a Tensor of shape [batch, num_predictions, 85]
                         where each item format is (x, y, w, h, object_conf, class_conf, ... 80 classes score ...)
     :param conf_thres:  Threshold under which prediction are discarded
     :param kernel:      Type of kernel to use ['gaussian', 'linear']
@@ -313,19 +329,20 @@
     sort_ind = (-pred[:, :, 4]).argsort()
     pred = torch.stack([pred[i, sort_ind[i]] for i in range(pred.shape[0])])[:, 0:max_num_of_detections]
 
     ious = calc_bbox_iou_matrix(pred)
 
     ious = ious.triu(1)
 
-    # CREATE A LABELS MASK, WE WANT ONLY BOXES WITH THE SAME LABEL TO AFFECT EACH OTHER
-    labels = pred[:, :, 5:]
-    labeles_matrix = (labels == labels.transpose(2, 1)).float().triu(1)
+    if not class_agnostic_nms:
+        # CREATE A LABELS MASK, WE WANT ONLY BOXES WITH THE SAME LABEL TO AFFECT EACH OTHER
+        labels = pred[:, :, 5:]
+        labeles_matrix = (labels == labels.transpose(2, 1)).float().triu(1)
+        ious *= labeles_matrix
 
-    ious *= labeles_matrix
     ious_cmax, _ = ious.max(1)
     ious_cmax = ious_cmax.unsqueeze(2).repeat(1, 1, max_num_of_detections)
 
     if kernel == "gaussian":
         decay_matrix = torch.exp(-1 * sigma * (ious**2))
         compensate_matrix = torch.exp(-1 * sigma * (ious_cmax**2))
         decay, _ = (decay_matrix / compensate_matrix).min(dim=1)
@@ -653,80 +670,106 @@
     :return: modified bbox (np.array)
     """
     bbox[:, 0::2] = np.clip(bbox[:, 0::2] * scale_ratio + padw, 0, w_max)
     bbox[:, 1::2] = np.clip(bbox[:, 1::2] * scale_ratio + padh, 0, h_max)
     return bbox
 
 
+class DatasetItemsException(Exception):
+    def __init__(self, data_sample: Tuple, collate_type: Type, expected_item_names: Tuple):
+        """
+        :param data_sample: item(s) returned by a dataset
+        :param collate_type: type of the collate that caused the exception
+        :param expected_item_names: tuple of names of items that are expected by the collate to be returned from the dataset
+        """
+        collate_type_name = collate_type.__name__
+        num_sample_items = len(data_sample) if isinstance(data_sample, tuple) else 1
+        error_msg = f"`{collate_type_name}` only supports Datasets that return a tuple {expected_item_names}, but got a tuple of len={num_sample_items}"
+        super().__init__(error_msg)
+
+
 @register_collate_function()
 class DetectionCollateFN:
     """
     Collate function for Yolox training
     """
 
+    def __init__(self):
+        self.expected_item_names = ("image", "targets")
+
     def __call__(self, data) -> Tuple[torch.Tensor, torch.Tensor]:
-        batch = default_collate(data)
-        ims, targets = batch[0:2]
-        return ims, self._format_targets(targets)
-
-    def _format_targets(self, targets: torch.Tensor) -> torch.Tensor:
-        nlabel = (targets.sum(dim=2) > 0).sum(dim=1)  # number of label per image
-        targets_merged = []
-        for i in range(targets.shape[0]):
-            targets_im = targets[i, : nlabel[i]]
-            batch_column = targets.new_ones((targets_im.shape[0], 1)) * i
-            targets_merged.append(torch.cat((batch_column, targets_im), 1))
-        return torch.cat(targets_merged, 0)
+        try:
+            images_batch, labels_batch = list(zip(*data))
+        except (ValueError, TypeError):
+            raise DatasetItemsException(data_sample=data[0], collate_type=type(self), expected_item_names=self.expected_item_names)
+
+        return self._format_images(images_batch), self._format_targets(labels_batch)
+
+    def _format_images(self, images_batch: List[Union[torch.Tensor, np.array]]) -> torch.Tensor:
+        images_batch = [torch.tensor(img) for img in images_batch]
+        images_batch_stack = torch.stack(images_batch, 0)
+        if images_batch_stack.shape[3] == 3:
+            images_batch_stack = torch.moveaxis(images_batch_stack, -1, 1).float()
+        return images_batch_stack
+
+    def _format_targets(self, labels_batch: List[Union[torch.Tensor, np.array]]) -> torch.Tensor:
+        """
+        Stack a batch id column to targets and concatenate
+        :param labels_batch: a list of targets per image (each of arbitrary length)
+        :return: one tensor of targets of all imahes of shape [N, 6], where N is the total number of targets in a batch
+                 and the 1st column is batch item index
+        """
+        labels_batch = [torch.tensor(labels) for labels in labels_batch]
+        labels_batch_indexed = []
+        for i, labels in enumerate(labels_batch):
+            batch_column = labels.new_ones((labels.shape[0], 1)) * i
+            labels = torch.cat((batch_column, labels), dim=-1)
+            labels_batch_indexed.append(labels)
+        return torch.cat(labels_batch_indexed, 0)
 
 
-class PPYoloECollateFN:
+class PPYoloECollateFN(DetectionCollateFN):
     """
     Collate function for PPYoloE training
     """
 
     def __init__(self, random_resize_sizes: Union[List[int], None] = None, random_resize_modes: Union[List[int], None] = None):
         """
-
         :param random_resize_sizes: (rows, cols)
         """
+        super().__init__()
         self.random_resize_sizes = random_resize_sizes
         self.random_resize_modes = random_resize_modes
 
     def __repr__(self):
         return f"PPYoloECollateFN(random_resize_sizes={self.random_resize_sizes}, random_resize_modes={self.random_resize_modes})"
 
     def __str__(self):
         return self.__repr__()
 
     def __call__(self, data) -> Tuple[torch.Tensor, torch.Tensor]:
         if self.random_resize_sizes is not None:
             data = self.random_resize(data)
-
-        batch = default_collate(data)
-        ims, targets = batch
-        targets = self._format_targets(targets)
-        ims = torch.moveaxis(ims, -1, 1).float()
-
-        return ims, targets
+        return super().__call__(data)
 
     def random_resize(self, batch):
         target_size = random.choice(self.random_resize_sizes)
         interpolation = random.choice(self.random_resize_modes)
         batch = [self.random_resize_sample(sample, target_size, interpolation) for sample in batch]
         return batch
 
     def random_resize_sample(self, sample, target_size, interpolation):
         if len(sample) == 2:
             image, targets = sample  # TARGETS ARE IN LABEL_CXCYWH
             with_crowd = False
-        elif len(sample == 3):
+        elif len(sample) == 3:
             image, targets, crowd_targets = sample
             with_crowd = True
         else:
-            raise RuntimeError()
+            raise DatasetItemsException(data_sample=sample, collate_type=type(self), expected_item_names=self.expected_item_names)
 
         dsize = int(target_size), int(target_size)
         scale_factors = target_size / image.shape[0], target_size / image.shape[1]
 
         image = cv2.resize(
             image,
             dsize=dsize,
@@ -737,59 +780,54 @@
         targets[:, 1:5] *= np.array([[sx, sy, sx, sy]], dtype=targets.dtype)
         if with_crowd:
             crowd_targets[:, 1:5] *= np.array([[sx, sy, sx, sy]], dtype=targets.dtype)
             return image, targets, crowd_targets
 
         return image, targets
 
-    def _format_targets(self, targets: torch.Tensor) -> torch.Tensor:
-        """
-
-        :param targets:
-        :return: Tensor of shape [B, N, 6], where 6 elements are (index, c, cx, cy, w, h)
-        """
-        # Same collate as in YoloX. We convert to PPYoloTargets in the loss
-        nlabel = (targets.sum(dim=2) > 0).sum(dim=1)  # number of label per image
-        targets_merged = []
-        for i in range(targets.shape[0]):
-            targets_im = targets[i, : nlabel[i]]
-            batch_column = targets.new_ones((targets_im.shape[0], 1)) * i
-            targets_merged.append(torch.cat((batch_column, targets_im), 1))
-
-        return torch.cat(targets_merged, 0)
-
 
 class CrowdDetectionPPYoloECollateFN(PPYoloECollateFN):
     """
     Collate function for Yolox training with additional_batch_items that includes crowd targets
     """
 
+    def __init__(self, random_resize_sizes: Union[List[int], None] = None, random_resize_modes: Union[List[int], None] = None):
+        super().__init__(random_resize_sizes, random_resize_modes)
+        self.expected_item_names = ("image", "targets", "crowd_targets")
+
     def __call__(self, data) -> Tuple[torch.Tensor, torch.Tensor, Dict[str, torch.Tensor]]:
 
         if self.random_resize_sizes is not None:
             data = self.random_resize(data)
 
-        batch = default_collate(data)
-        ims, targets, crowd_targets = batch
-        if ims.shape[3] == 3:
-            ims = torch.moveaxis(ims, -1, 1).float()
+        try:
+            images_batch, labels_batch, crowd_labels_batch = list(zip(*data))
+        except (ValueError, TypeError):
+            raise DatasetItemsException(data_sample=data[0], collate_type=type(self), expected_item_names=self.expected_item_names)
 
-        return ims, self._format_targets(targets), {"crowd_targets": self._format_targets(crowd_targets)}
+        return self._format_images(images_batch), self._format_targets(labels_batch), {"crowd_targets": self._format_targets(crowd_labels_batch)}
 
 
 @register_collate_function()
 class CrowdDetectionCollateFN(DetectionCollateFN):
     """
     Collate function for Yolox training with additional_batch_items that includes crowd targets
     """
 
+    def __init__(self):
+        super().__init__()
+        self.expected_item_names = ("image", "targets", "crowd_targets")
+
     def __call__(self, data) -> Tuple[torch.Tensor, torch.Tensor, Dict[str, torch.Tensor]]:
-        batch = default_collate(data)
-        ims, targets, crowd_targets = batch[0:3]
-        return ims, self._format_targets(targets), {"crowd_targets": self._format_targets(crowd_targets)}
+        try:
+            images_batch, labels_batch, crowd_labels_batch = list(zip(*data))
+        except (ValueError, TypeError):
+            raise DatasetItemsException(data_sample=data[0], collate_type=type(self), expected_item_names=self.expected_item_names)
+
+        return self._format_images(images_batch), self._format_targets(labels_batch), {"crowd_targets": self._format_targets(crowd_labels_batch)}
 
 
 def compute_box_area(box: torch.Tensor) -> torch.Tensor:
     """
     Compute the area of one or many boxes.
     :param box: One or many boxes, shape = (4, ?), each box in format (x1, y1, x2, y2)
     :return: Area of every box, shape = (1, ?)
@@ -1054,14 +1092,15 @@
     preds_to_ignore: torch.Tensor,
     preds_scores: torch.Tensor,
     preds_cls: torch.Tensor,
     targets_cls: torch.Tensor,
     device: str,
     recall_thresholds: Optional[torch.Tensor] = None,
     score_threshold: Optional[float] = 0.1,
+    calc_best_score_thresholds: bool = False,
 ) -> Tuple:
     """
     Compute the list of precision, recall, MaP and f1 for every recall IoU threshold and for every class.
 
     :param preds_matched:      Tensor of shape (num_predictions, n_iou_thresholds)
                                     True when prediction (i) is matched with a target with respect to the (j)th IoU threshold
     :param preds_to_ignore     Tensor of shape (num_predictions, n_iou_thresholds)
@@ -1069,59 +1108,82 @@
     :param preds_scores:       Tensor of shape (num_predictions), confidence score for every prediction
     :param preds_cls:          Tensor of shape (num_predictions), predicted class for every prediction
     :param targets_cls:        Tensor of shape (num_targets), ground truth class for every target box to be detected
     :param recall_thresholds:   Recall thresholds used to compute MaP.
     :param score_threshold:    Minimum confidence score to consider a prediction for the computation of
                                     precision, recall and f1 (not MaP)
     :param device:             Device
-
+    :param calc_best_score_thresholds: If True, the best confidence score threshold is computed for each class
     :return:
         :ap, precision, recall, f1: Tensors of shape (n_class, nb_iou_thrs)
         :unique_classes:            Vector with all unique target classes
+        :best_score_threshold:      torch.float with the best overall score threshold if calc_best_score_thresholds
+                                    is True else None
+        :best_score_threshold_per_cls:     dict that stores the best score threshold for each class , if
+                                            calc_best_score_thresholds is True else None
+
     """
     preds_matched, preds_to_ignore = preds_matched.to(device), preds_to_ignore.to(device)
     preds_scores, preds_cls, targets_cls = preds_scores.to(device), preds_cls.to(device), targets_cls.to(device)
 
     recall_thresholds = torch.linspace(0, 1, 101, device=device) if recall_thresholds is None else recall_thresholds.to(device)
 
-    unique_classes = torch.unique(targets_cls)
+    unique_classes = torch.unique(targets_cls).long()
+
     n_class, nb_iou_thrs = len(unique_classes), preds_matched.shape[-1]
 
     ap = torch.zeros((n_class, nb_iou_thrs), device=device)
     precision = torch.zeros((n_class, nb_iou_thrs), device=device)
     recall = torch.zeros((n_class, nb_iou_thrs), device=device)
 
+    nb_score_thrs = 101
+    all_score_thresholds = torch.linspace(0, 1, nb_score_thrs, device=device)
+    f1_per_class_per_threshold = torch.zeros((n_class, nb_score_thrs), device=device) if calc_best_score_thresholds else None
+    best_score_threshold_per_cls = dict() if calc_best_score_thresholds else None
+
     for cls_i, cls in enumerate(unique_classes):
         cls_preds_idx, cls_targets_idx = (preds_cls == cls), (targets_cls == cls)
-        cls_ap, cls_precision, cls_recall = compute_detection_metrics_per_cls(
+        cls_ap, cls_precision, cls_recall, cls_f1_per_threshold, cls_best_score_threshold = compute_detection_metrics_per_cls(
             preds_matched=preds_matched[cls_preds_idx],
             preds_to_ignore=preds_to_ignore[cls_preds_idx],
             preds_scores=preds_scores[cls_preds_idx],
             n_targets=cls_targets_idx.sum(),
             recall_thresholds=recall_thresholds,
             score_threshold=score_threshold,
             device=device,
+            calc_best_score_thresholds=calc_best_score_thresholds,
+            nb_score_thrs=nb_score_thrs,
         )
         ap[cls_i, :] = cls_ap
         precision[cls_i, :] = cls_precision
         recall[cls_i, :] = cls_recall
+        if calc_best_score_thresholds:
+            f1_per_class_per_threshold[cls_i, :] = cls_f1_per_threshold
+            best_score_threshold_per_cls[f"Best_score_threshold_cls_{int(cls)}"] = cls_best_score_threshold
 
     f1 = 2 * precision * recall / (precision + recall + 1e-16)
+    if calc_best_score_thresholds:
+        mean_f1_across_classes = torch.mean(f1_per_class_per_threshold, dim=0)
+        best_score_threshold = all_score_thresholds[torch.argmax(mean_f1_across_classes)]
+    else:
+        best_score_threshold = None
 
-    return ap, precision, recall, f1, unique_classes
+    return ap, precision, recall, f1, unique_classes, best_score_threshold, best_score_threshold_per_cls
 
 
 def compute_detection_metrics_per_cls(
     preds_matched: torch.Tensor,
     preds_to_ignore: torch.Tensor,
     preds_scores: torch.Tensor,
     n_targets: int,
     recall_thresholds: torch.Tensor,
     score_threshold: float,
     device: str,
+    calc_best_score_thresholds: bool = False,
+    nb_score_thrs: int = 101,
 ):
     """
     Compute the list of precision, recall and MaP of a given class for every recall IoU threshold.
 
         :param preds_matched:      Tensor of shape (num_predictions, n_iou_thresholds)
                                         True when prediction (i) is matched with a target
                                         with respect to the(j)th IoU threshold
@@ -1130,24 +1192,38 @@
                                         with respect to the (j)th IoU threshold
         :param preds_scores:       Tensor of shape (num_predictions), confidence score for every prediction
         :param n_targets:          Number of target boxes of this class
         :param recall_thresholds:  Tensor of shape (max_n_rec_thresh) list of recall thresholds used to compute MaP
         :param score_threshold:    Minimum confidence score to consider a prediction for the computation of
                                         precision and recall (not MaP)
         :param device:             Device
+        :param calc_best_score_thresholds: If True, the best confidence score threshold is computed for this class
+        :param nb_score_thrs:       Number of score thresholds to consider when calc_best_score_thresholds is True
 
-        :return ap, precision, recall:  Tensors of shape (nb_iou_thrs)
+        :return:
+            :ap, precision, recall:     Tensors of shape (nb_iou_thrs)
+            :mean_f1_per_threshold:     Tensor of shape (nb_score_thresholds) if calc_best_score_thresholds is True else None
+            :best_score_threshold:      torch.float if calc_best_score_thresholds is True else None
     """
     nb_iou_thrs = preds_matched.shape[-1]
 
+    mean_f1_per_threshold = torch.zeros(nb_score_thrs, device=device) if calc_best_score_thresholds else None
+    best_score_threshold = torch.tensor(0.0, dtype=torch.float, device=device) if calc_best_score_thresholds else None
+
     tps = preds_matched
     fps = torch.logical_and(torch.logical_not(preds_matched), torch.logical_not(preds_to_ignore))
 
     if len(tps) == 0:
-        return torch.zeros(nb_iou_thrs, device=device), torch.zeros(nb_iou_thrs, device=device), torch.zeros(nb_iou_thrs, device=device)
+        return (
+            torch.zeros(nb_iou_thrs, device=device),
+            torch.zeros(nb_iou_thrs, device=device),
+            torch.zeros(nb_iou_thrs, device=device),
+            mean_f1_per_threshold,
+            best_score_threshold,
+        )
 
     # Sort by decreasing score
     dtype = torch.uint8 if preds_scores.is_cuda and preds_scores.dtype is torch.bool else preds_scores.dtype
     sort_ind = torch.argsort(preds_scores.to(dtype), descending=True)
     tps = tps[sort_ind, :]
     fps = fps[sort_ind, :]
     preds_scores = preds_scores[sort_ind].contiguous()
@@ -1163,24 +1239,47 @@
     rolling_precisions = rolling_precisions.flip(0).cummax(0).values.flip(0)
 
     # ==================
     # RECALL & PRECISION
 
     # We want the rolling precision/recall at index i so that: preds_scores[i-1] >= score_threshold > preds_scores[i]
     # Note: torch.searchsorted works on increasing sequence and preds_scores is decreasing, so we work with "-"
-    lowest_score_above_threshold = torch.searchsorted(-preds_scores, -score_threshold, right=False)
+    # Note2: right=True due to negation
+    lowest_score_above_threshold = torch.searchsorted(-preds_scores, -score_threshold, right=True)
 
     if lowest_score_above_threshold == 0:  # Here score_threshold > preds_scores[0], so no pred is above the threshold
         recall = torch.zeros(nb_iou_thrs, device=device)
         precision = torch.zeros(nb_iou_thrs, device=device)  # the precision is not really defined when no pred but we need to give it a value
     else:
         recall = rolling_recalls[lowest_score_above_threshold - 1]
         precision = rolling_precisions[lowest_score_above_threshold - 1]
 
     # ==================
+    # BEST CONFIDENCE SCORE THRESHOLD PER CLASS
+    if calc_best_score_thresholds:
+        all_score_thresholds = torch.linspace(0, 1, nb_score_thrs, device=device)
+
+        # We want the rolling precision/recall at index i so that: preds_scores[i-1] > score_threshold >= preds_scores[i]
+        # Note: torch.searchsorted works on increasing sequence and preds_scores is decreasing, so we work with "-"
+        lowest_scores_above_thresholds = torch.searchsorted(-preds_scores, -all_score_thresholds, right=True)
+
+        # When score_threshold > preds_scores[0], then no pred is above the threshold, so we pad with zeros
+        rolling_recalls_padded = torch.cat((torch.zeros(1, nb_iou_thrs, device=device), rolling_recalls), dim=0)
+        rolling_precisions_padded = torch.cat((torch.zeros(1, nb_iou_thrs, device=device), rolling_precisions), dim=0)
+
+        # shape = (n_score_thresholds, nb_iou_thrs)
+        recalls_per_threshold = torch.index_select(input=rolling_recalls_padded, dim=0, index=lowest_scores_above_thresholds)
+        precisions_per_threshold = torch.index_select(input=rolling_precisions_padded, dim=0, index=lowest_scores_above_thresholds)
+
+        # shape (n_score_thresholds, nb_iou_thrs)
+        f1_per_threshold = 2 * recalls_per_threshold * precisions_per_threshold / (recalls_per_threshold + precisions_per_threshold + 1e-16)
+        mean_f1_per_threshold = torch.mean(f1_per_threshold, dim=1)  # average over iou thresholds
+        best_score_threshold = all_score_thresholds[torch.argmax(mean_f1_per_threshold)]
+
+    # ==================
     # AVERAGE PRECISION
 
     # shape = (nb_iou_thrs, n_recall_thresholds)
     recall_thresholds = recall_thresholds.view(1, -1).repeat(nb_iou_thrs, 1)
 
     # We want the index i so that: rolling_recalls[i-1] < recall_thresholds[k] <= rolling_recalls[i]
     # Note:  when recall_thresholds[k] > max(rolling_recalls), i = len(rolling_recalls)
@@ -1192,8 +1291,8 @@
 
     # shape = (n_recall_thresholds, nb_iou_thrs)
     sampled_precision_points = torch.gather(input=rolling_precisions, index=recall_threshold_idx, dim=0)
 
     # Average over the recall_thresholds
     ap = sampled_precision_points.mean(0)
 
-    return ap, precision, recall
+    return ap, precision, recall, mean_f1_per_threshold, best_score_threshold
```

## super_gradients/training/utils/ema.py

```diff
@@ -1,17 +1,17 @@
 import warnings
 from copy import deepcopy
 from typing import Union
 
 import torch
+from super_gradients.training.utils.utils import unwrap_model
 from torch import nn
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.exceptions.factory_exceptions import UnknownTypeException
-from super_gradients.training import utils as core_utils
 from super_gradients.training.models import SgModule
 from super_gradients.training.models.kd_modules.kd_module import KDModule
 from super_gradients.training.utils.ema_decay_schedules import IDecayFunction, EMA_DECAY_FUNCTIONS
 
 logger = get_logger(__name__)
 
 
@@ -30,45 +30,46 @@
     This is intended to allow functionality like
     https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
     A smoothed version of the weights is necessary for some training schemes to perform well.
     This class is sensitive where it is initialized in the sequence of model init,
     GPU assignment and distributed training wrappers.
     """
 
-    def __init__(self, model, decay: float, decay_function: IDecayFunction):
+    def __init__(self, model: nn.Module, decay: float, decay_function: IDecayFunction):
         """
         Init the EMA
         :param model: Union[SgModule, nn.Module], the training model to construct the EMA model by
                     IMPORTANT: WHEN THE APPLICATION OF EMA ONLY ON A SUBSET OF ATTRIBUTES IS DESIRED, WRAP THE NN.MODULE
                     AS SgModule AND OVERWRITE get_include_attributes() AND get_exclude_attributes() AS DESIRED.
         :param decay: the maximum decay value. as the training process advances, the decay will climb towards this value
                       until the EMA_t+1 = EMA_t * decay + TRAINING_MODEL * (1- decay)
         :param beta: the exponent coefficient. The higher the beta, the sooner in the training the decay will saturate to
                      its final value. beta=15 is ~40% of the training process.
         """
         # Create EMA
+        model = unwrap_model(model)
         self.ema = deepcopy(model)
         self.ema.eval()
         self.decay = decay
         self.decay_function = decay_function
 
         """"
         we hold a list of model attributes (not wights and biases) which we would like to include in each
         attribute update or exclude from each update. a SgModule declare these attribute using
         get_include_attributes and get_exclude_attributes functions. for a nn.Module which is not a SgModule
         all non-private (not starting with '_') attributes will be updated (and only them).
         """
-        if isinstance(model.module, SgModule):
-            self.include_attributes = model.module.get_include_attributes()
-            self.exclude_attributes = model.module.get_exclude_attributes()
+        if isinstance(model, SgModule):
+            self.include_attributes = model.get_include_attributes()
+            self.exclude_attributes = model.get_exclude_attributes()
         else:
             warnings.warn("Warning: EMA should be used with SgModule instance. All attributes of the model will be " "included in EMA")
             self.include_attributes = []
             self.exclude_attributes = []
-        for p in self.ema.module.parameters():
+        for p in self.ema.parameters():
             p.requires_grad_(False)
 
     @classmethod
     def from_params(cls, model: nn.Module, decay_type: str = None, decay: float = None, **kwargs):
         if decay is None:
             logger.warning(
                 "Parameter `decay` is not specified for EMA params. Please specify `decay` parameter explicitly in your config:\n"
@@ -127,31 +128,32 @@
         Update the state of the EMA model.
 
         :param model: Current training model
         :param step: Current training step
         :param total_steps: Total training steps
         """
         # Update EMA parameters
+        model = unwrap_model(model)
         with torch.no_grad():
             decay = self.decay_function(self.decay, step, total_steps)
 
-            for ema_v, model_v in zip(self.ema.module.state_dict().values(), model.state_dict().values()):
+            for ema_v, model_v in zip(self.ema.state_dict().values(), model.state_dict().values()):
                 if ema_v.dtype.is_floating_point:
                     ema_v.copy_(ema_v * decay + (1.0 - decay) * model_v.detach())
 
     def update_attr(self, model):
         """
         This function updates model attributes (not weight and biases) from original model to the ema model.
         attributes of the original model, such as anchors and grids (of detection models), may be crucial to the
         model operation and need to be updated.
         If include_attributes and exclude_attributes lists were not defined, all non-private (not starting with '_')
         attributes will be updated (and only them).
         :param model: the source model
         """
-        copy_attr(self.ema.module, model.module, self.include_attributes, self.exclude_attributes)
+        copy_attr(self.ema, unwrap_model(model), self.include_attributes, self.exclude_attributes)
 
 
 class KDModelEMA(ModelEMA):
     """Model Exponential Moving Average from https://github.com/rwightman/pytorch-image-models
     Keep a moving average of everything in the model state_dict (parameters and buffers).
     This is intended to allow functionality like
     https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
@@ -168,19 +170,17 @@
                     AS SgModule AND OVERWRITE get_include_attributes() AND get_exclude_attributes() AS DESIRED.
         :param decay: the maximum decay value. as the training process advances, the decay will climb towards this value
                       until the EMA_t+1 = EMA_t * decay + TRAINING_MODEL * (1- decay)
         :param beta: the exponent coefficient. The higher the beta, the sooner in the training the decay will saturate to
                      its final value. beta=15 is ~40% of the training process.
         """
         # Only work on the student (we don't want to update and to have a duplicate of the teacher)
-        super().__init__(model=core_utils.WrappedModel(kd_model.module.student), decay=decay, decay_function=decay_function)
+        super().__init__(model=unwrap_model(kd_model).student, decay=decay, decay_function=decay_function)
 
         # Overwrite current ema attribute with combination of the student model EMA (current self.ema)
         # with already the instantiated teacher, to have the final KD EMA
-        self.ema = core_utils.WrappedModel(
-            KDModule(
-                arch_params=kd_model.module.arch_params,
-                student=self.ema.module,
-                teacher=kd_model.module.teacher,
-                run_teacher_on_eval=kd_model.module.run_teacher_on_eval,
-            )
+        self.ema = KDModule(
+            arch_params=unwrap_model(kd_model).arch_params,
+            student=self.ema,
+            teacher=unwrap_model(kd_model).teacher,
+            run_teacher_on_eval=unwrap_model(kd_model).run_teacher_on_eval,
         )
```

## super_gradients/training/utils/optimizer_utils.py

```diff
@@ -1,21 +1,22 @@
-import torch.optim as optim
 import torch.nn as nn
-from torch.nn.modules.batchnorm import _BatchNorm
-from torch.nn.modules.conv import _ConvNd
+import torch.optim as optim
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.factories.optimizers_type_factory import OptimizersTypeFactory
 from super_gradients.training.params import (
     DEFAULT_OPTIMIZER_PARAMS_SGD,
     DEFAULT_OPTIMIZER_PARAMS_ADAM,
     DEFAULT_OPTIMIZER_PARAMS_RMSPROP,
     DEFAULT_OPTIMIZER_PARAMS_RMSPROPTF,
 )
 from super_gradients.training.utils import get_param
 from super_gradients.training.utils.optimizers.rmsprop_tf import RMSpropTF
+from super_gradients.training.utils.utils import is_model_wrapped
+from torch.nn.modules.batchnorm import _BatchNorm
+from torch.nn.modules.conv import _ConvNd
 
 logger = get_logger(__name__)
 
 OPTIMIZERS_DEFAULT_PARAMS = {
     optim.SGD: DEFAULT_OPTIMIZER_PARAMS_SGD,
     optim.Adam: DEFAULT_OPTIMIZER_PARAMS_ADAM,
     optim.RMSprop: DEFAULT_OPTIMIZER_PARAMS_RMSPROP,
@@ -57,19 +58,19 @@
     # FIXME - replace usage of ids addresses to find batchnorm and biases params.
     #  Use other common way to identify torch parameters other than id or layer names
     """
     Iterate over module.modules() and returns params id addresses of batch-norm and biases params.
     NOTE - ALL MODULES WITH ATTRIBUTES NAMED BIAS AND ARE INSTANCE OF nn.Parameter WILL BE CONSIDERED A BIAS PARAM FOR
         ZERO WEIGHT DECAY.
     """
-    batchnorm_types = (_BatchNorm,)
+    norm_types = (_BatchNorm, nn.GroupNorm, nn.LayerNorm, nn.InstanceNorm1d, nn.InstanceNorm2d, nn.InstanceNorm3d)
     torch_weight_with_bias_types = (_ConvNd, nn.Linear)
     no_decay_ids = []
     for name, m in module.named_modules():
-        if isinstance(m, batchnorm_types):
+        if isinstance(m, norm_types):
             no_decay_ids.append(id(m.weight))
             no_decay_ids.append(id(m.bias))
         elif hasattr(m, "bias") and isinstance(m.bias, nn.Parameter):
             if not isinstance(m, torch_weight_with_bias_types):
                 logger.warning(
                     f"Module class: {m.__class__}, have a `bias` parameter attribute but is not instance of"
                     f" torch primitive modules, this bias parameter will be part of param group with zero"
@@ -82,32 +83,34 @@
 def build_optimizer(net: nn.Module, lr: float, training_params) -> optim.Optimizer:
     """
     Wrapper function for initializing the optimizer
         :param net: the nn_module to build the optimizer for
         :param lr: initial learning rate
         :param training_params: training_parameters
     """
+    if is_model_wrapped(net):
+        raise ValueError("Argument net for build_optimizer must be an unwrapped model. " "Please use build_optimizer(unwrap_model(net), ...).")
     if isinstance(training_params.optimizer, str):
         optimizer_cls = OptimizersTypeFactory().get(training_params.optimizer)
     else:
         optimizer_cls = training_params.optimizer
     optimizer_params = OPTIMIZERS_DEFAULT_PARAMS[optimizer_cls].copy() if optimizer_cls in OPTIMIZERS_DEFAULT_PARAMS.keys() else dict()
     optimizer_params.update(**training_params.optimizer_params)
     training_params.optimizer_params = optimizer_params
 
     weight_decay = get_param(training_params.optimizer_params, "weight_decay", 0.0)
     # OPTIMIZER PARAM GROUPS ARE SET USING DEFAULT OR MODEL SPECIFIC INIT
-    if hasattr(net.module, "initialize_param_groups"):
+    if hasattr(net, "initialize_param_groups"):
         # INITIALIZE_PARAM_GROUPS MUST RETURN A LIST OF DICTS WITH 'named_params' AND OPTIMIZER's ATTRIBUTES PER GROUP
-        net_named_params = net.module.initialize_param_groups(lr, training_params)
+        net_named_params = net.initialize_param_groups(lr, training_params)
     else:
         net_named_params = [{"named_params": net.named_parameters()}]
 
     if training_params.zero_weight_decay_on_bias_and_bn:
-        optimizer_training_params = separate_zero_wd_params_groups_for_optimizer(net.module, net_named_params, weight_decay)
+        optimizer_training_params = separate_zero_wd_params_groups_for_optimizer(net, net_named_params, weight_decay)
 
     else:
         # Overwrite groups to include params instead of named params
         for ind_group, param_group in enumerate(net_named_params):
             param_group["params"] = [param[1] for param in list(param_group["named_params"])]
             del param_group["named_params"]
             net_named_params[ind_group] = param_group
```

## super_gradients/training/utils/regularization_utils.py

```diff
@@ -1,26 +1,52 @@
-import torch
 from torch import nn
 
 
+def drop_path(x, drop_prob: float = 0.0, scale_by_keep: bool = True):
+    """
+    Drop paths (Stochastic Depth) per sample (when applied in main path of residual blocks).
+    """
+
+    keep_prob = 1 - drop_prob
+    shape = (x.shape[0],) + (1,) * (x.ndim - 1)  # work with diff dim tensors, not just 2D ConvNets
+    random_tensor = x.new_empty(shape).bernoulli_(keep_prob)
+    if keep_prob > 0.0 and scale_by_keep:
+        random_tensor.div_(keep_prob)
+    return x * random_tensor
+
+
 class DropPath(nn.Module):
     """
     Drop paths (Stochastic Depth) per sample  (when applied in main path of residual blocks).
 
+    Intended usage of this block is the following:
+
+    >>> class ResNetBlock(nn.Module):
+    >>>   def __init__(self, ..., drop_path_rate:float):
+    >>>     self.drop_path = DropPath(drop_path_rate)
+    >>>
+    >>>   def forward(self, x):
+    >>>     return x + self.drop_path(self.conv_bn_act(x))
+
     Code taken from TIMM (https://github.com/rwightman/pytorch-image-models)
     Apache License 2.0
     """
 
-    def __init__(self, drop_prob=None):
+    def __init__(self, drop_prob: float = 0.0, scale_by_keep: bool = True):
+        """
+
+        :param drop_prob: Probability of zeroing out individual vector (channel dimension) of each feature map
+        :param scale_by_keep: Whether to scale the output by the keep probability. Enable by default and helps to
+                              keep output mean & std in the same range as w/o drop path.
+        """
         super(DropPath, self).__init__()
         self.drop_prob = drop_prob
+        self.scale_by_keep = scale_by_keep
 
     def forward(self, x):
         if self.drop_prob == 0.0 or not self.training:
             return x
 
-        keep_prob = 1 - self.drop_prob
-        shape = (x.shape[0],) + (1,) * (x.ndim - 1)  # work with diff dim tensors, not just 2D ConvNets
-        random_tensor = keep_prob + torch.rand(shape, dtype=x.dtype, device=x.device)
-        random_tensor.floor_()  # binarize
-        output = x.div(keep_prob) * random_tensor
-        return output
+        return drop_path(x, self.drop_prob, self.scale_by_keep)
+
+    def extra_repr(self):
+        return f"drop_prob={round(self.drop_prob,3):0.3f}"
```

## super_gradients/training/utils/sg_trainer_utils.py

```diff
@@ -1,28 +1,28 @@
 import os
 import sys
 import socket
 import time
 from dataclasses import dataclass
 from multiprocessing import Process
 from pathlib import Path
-from typing import Tuple, Union, Dict, Sequence, Callable
+from typing import Tuple, Union, Dict, Sequence, Callable, Optional
 import random
 
 import inspect
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from treelib import Tree
 from termcolor import colored
 import torch
 
 from torch.utils.tensorboard import SummaryWriter
 
 from super_gradients.common.environment.device_utils import device_config
-from super_gradients.training.exceptions.dataset_exceptions import UnsupportedBatchItemsFormat
+from super_gradients.common.exceptions.dataset_exceptions import UnsupportedBatchItemsFormat
 from super_gradients.common.data_types.enum import MultiGPUMode
 
 
 from enum import Enum
 
 
 class IncreaseType(Enum):
@@ -93,20 +93,20 @@
     :param previous:                Value of the metric in previous iteration
     :param best:                    Value of the metric in best iteration (best according to greater_is_better)
     :param change_from_previous:    Change compared to previous iteration value
     :param change_from_best:        Change compared to best iteration value
     """
 
     name: str
-    greater_is_better: bool = None
-    current: float = None
-    previous: float = None
-    best: float = None
-    change_from_previous: float = None
-    change_from_best: float = None
+    greater_is_better: Optional[bool] = None
+    current: Optional[float] = None
+    previous: Optional[float] = None
+    best: Optional[float] = None
+    change_from_previous: Optional[float] = None
+    change_from_best: Optional[float] = None
 
     @property
     def has_increased_from_previous(self) -> IncreaseType:
         """Type of increase compared to previous value, i.e. if the value is greater, smaller or the same."""
         return self._get_increase_type(self.change_from_previous)
 
     @property
@@ -186,36 +186,34 @@
 def update_monitored_values_dict(monitored_values_dict: Dict[str, MonitoredValue], new_values_dict: Dict[str, float]) -> Dict[str, MonitoredValue]:
     """Update the given ValueToMonitor object (could be a loss or a metric) with the new value
 
     :param monitored_values_dict: Dict mapping value names to their stats throughout epochs.
     :param new_values_dict: Dict mapping value names to their new (i.e. current epoch) value.
     :return: Updated monitored_values_dict
     """
-    for monitored_value_name in monitored_values_dict.keys():
+    relevant_keys = set(new_values_dict.keys()).intersection(monitored_values_dict.keys())
+    for monitored_value_name in relevant_keys:
+        previous_value = monitored_values_dict[monitored_value_name]
         monitored_values_dict[monitored_value_name] = update_monitored_value(
             new_value=new_values_dict[monitored_value_name],
-            previous_monitored_value=monitored_values_dict[monitored_value_name],
+            previous_monitored_value=previous_value,
         )
     return monitored_values_dict
 
 
-def display_epoch_summary(
-    epoch: int, n_digits: int, train_monitored_values: Dict[str, MonitoredValue], valid_monitored_values: Dict[str, MonitoredValue]
-) -> None:
+def display_epoch_summary(epoch: int, n_digits: int, monitored_values_dict: Dict[str, Dict[str, MonitoredValue]]) -> None:
     """Display a summary of loss/metric of interest, for a given epoch.
 
     :param epoch: the number of epoch.
     :param n_digits: number of digits to display on screen for float values
-    :param train_monitored_values: mapping of loss/metric with their stats that will be displayed
-    :param valid_monitored_values: mapping of loss/metric with their stats that will be displayed
-    :return:
+    :param monitored_values_dict: Dict of Dict. The first one represents the splut, and the second one a loss/metric.
     """
 
-    def _format_to_str(val: float) -> str:
-        return str(round(val, n_digits))
+    def _format_to_str(val: Optional[float]) -> str:
+        return str(round(val, n_digits)) if val is not None else "None"
 
     def _generate_tree(value_name: str, monitored_value: MonitoredValue) -> Tree:
         """Generate a tree that represents the stats of a given loss/metric."""
 
         current = _format_to_str(monitored_value.current)
         root_id = str(hash(f"{value_name} = {current}")) + str(random.random())
 
@@ -236,29 +234,28 @@
                 text=f"{monitored_value.has_increased_from_best.to_symbol()} {change_from_best}", color=monitored_value.has_improved_from_best.to_color()
             )
 
             tree.create_node(tag=f"Epoch N-1      = {previous:6} ({diff_with_prev_colored:8})", identifier=f"0_previous_{root_id}", parent=root_id)
             tree.create_node(tag=f"Best until now = {best:6} ({diff_with_best_colored:8})", identifier=f"1_best_{root_id}", parent=root_id)
         return tree
 
-    train_tree = Tree()
-    train_tree.create_node("Training", "Training")
-    for name, value in train_monitored_values.items():
-        train_tree.paste("Training", new_tree=_generate_tree(name, monitored_value=value))
-
-    valid_tree = Tree()
-    valid_tree.create_node("Validation", "Validation")
-    for name, value in valid_monitored_values.items():
-        valid_tree.paste("Validation", new_tree=_generate_tree(name, monitored_value=value))
-
     summary_tree = Tree()
     summary_tree.create_node(f"SUMMARY OF EPOCH {epoch}", "Summary")
-    summary_tree.paste("Summary", train_tree)
-    summary_tree.paste("Summary", valid_tree)
-    summary_tree.show()
+
+    for split, monitored_values in monitored_values_dict.items():
+        if len(monitored_values):
+            split_tree = Tree()
+            split_tree.create_node(split, split)
+            for name, value in monitored_values.items():
+                split_tree.paste(split, new_tree=_generate_tree(name, monitored_value=value))
+            summary_tree.paste("Summary", split_tree)
+
+    print("===========================================================")
+    summary_tree.show(key=False)
+    print("===========================================================")
 
 
 def try_port(port):
     """
     try_port - Helper method for tensorboard port binding
     :param port:
     :return:
```

## super_gradients/training/utils/ssd_utils.py

```diff
@@ -117,17 +117,18 @@
         Predictions of SSD contain unnormalized probabilities for a background class,
         together with confidences for all the dataset classes. Background will be utilized and discarded,
         so this callback will return 0-based classes without background
         :param conf: confidence threshold
         :param iou: IoU threshold
         :param classes: (optional list) filter by class
         :param nms_type: the type of nms to use (iterative or matrix)
-        :param multi_label_per_box: whether to use re-use each box with all possible labels
-                                    (instead of the maximum confidence all confidences above threshold
-                                    will be sent to NMS)
+        :param multi_label_per_box: controls whether to decode multiple labels per box.
+                                    True - each anchor can produce multiple labels of different classes
+                                           that pass confidence threshold check (default).
+                                    False - each anchor can produce only one label of the class with the highest score.
         """
         super(SSDPostPredictCallback, self).__init__()
         self.conf = conf
         self.iou = iou
         self.nms_type = nms_type
         self.classes = classes
         self.max_predictions = max_predictions
```

## super_gradients/training/utils/utils.py

```diff
@@ -1,22 +1,24 @@
-import collections
 import math
 import os
 import random
 import re
 import tarfile
 import time
 import inspect
+import typing
+import warnings
 from functools import lru_cache, wraps
 from importlib import import_module
 from itertools import islice
 
 from pathlib import Path
 from typing import Mapping, Optional, Tuple, Union, List, Dict, Any, Iterable
 from zipfile import ZipFile
+from torch.nn.parallel import DistributedDataParallel
 
 import numpy as np
 import torch
 import torch.nn as nn
 from PIL import Image, ExifTags
 from jsonschema import validate
 
@@ -76,20 +78,44 @@
         else:
             validate(self.__dict__, self.schema)
 
 
 class WrappedModel(nn.Module):
     def __init__(self, module):
         super(WrappedModel, self).__init__()
+        warnings.warn(
+            "WrappedModel is deprecated and will be removed in next major release of SuperGradients. "
+            "You don't need to wrap your model anymore, simply remove it and everything will work as expected.",
+            DeprecationWarning,
+        )
+
         self.module = module  # that I actually define.
 
     def forward(self, x):
         return self.module(x)
 
 
+def is_model_wrapped(model: nn.Module) -> bool:
+    return isinstance(model, (nn.DataParallel, DistributedDataParallel, WrappedModel))
+
+
+def unwrap_model(model: Union[nn.Module, nn.DataParallel, DistributedDataParallel]) -> nn.Module:
+    """
+    Get the real model from a model wrapper (DataParallel, DistributedDataParallel)
+
+    :param model:
+    :return:
+    """
+    if is_model_wrapped(model):
+        return model.module
+    elif isinstance(model, nn.Module):
+        return model
+    raise ValueError(f"Unknown model type: {type(model)}")
+
+
 def arch_params_deprecated(func):
     """
     Since initialization of arch_params is deprecated and will be removed, this decorator will be used to wrap the _init_
     function of some models. It will unwrap the parameters of the function and will log a warning.
     """
 
     @wraps(func)
@@ -219,19 +245,19 @@
     :return: List[str], list of keys as discussed above.
     """
     return [fuzzy_str(s) for s in params.keys()]
 
 
 def fuzzy_str(s: str):
     """
-    Returns s removing leading and trailing white space, lower-casing and drops
+    Returns s removing leading and trailing white space, lower-casing and drops non word chars (except for '/')
     :param s: str, string to apply the manipulation discussed above.
     :return: str, s after the manipulation discussed above.
     """
-    return re.sub(r"[^\w]", "", s).replace("_", "").lower()
+    return re.sub(r"[^\w|\/]", "", s).replace("_", "").lower()
 
 
 def _get_fuzzy_attr_map(params):
     return {fuzzy_str(a): a for a in params.__dir__()}
 
 
 def _has_fuzzy_attr(params, name):
@@ -588,12 +614,12 @@
     Checks input and converts it to a tuple of length two. If input is None returns None.
     :param inputs: Input argument, either a number or a tuple of two numbers.
     :return: Tuple of two numbers if input is not None, otherwise - None.
     """
     if inputs is None:
         return None
 
-    if isinstance(inputs, collections.Iterable) and not isinstance(inputs, str):
+    if isinstance(inputs, typing.Iterable) and not isinstance(inputs, str):
         a, b = inputs
         return a, b
 
     return inputs, inputs
```

## super_gradients/training/utils/weight_averaging_utils.py

```diff
@@ -1,12 +1,12 @@
 import os
 import torch
 import numpy as np
 from super_gradients.training.utils.checkpoint_utils import read_ckpt_state_dict
-from super_gradients.training.utils.utils import move_state_dict_to_device
+from super_gradients.training.utils.utils import move_state_dict_to_device, unwrap_model
 
 
 class ModelWeightAveraging:
     """
     Utils class for managing the averaging of the best several snapshots into a single model.
     A snapshot dictionary file and the average model will be saved / updated at every epoch and evaluated only when
     training is completed. The snapshot file will only be deleted upon completing the training.
@@ -14,31 +14,28 @@
     """
 
     def __init__(
         self,
         ckpt_dir,
         greater_is_better,
         metric_to_watch="acc",
-        metric_idx=1,
         load_checkpoint=False,
         number_of_models_to_average=10,
     ):
         """
         Init the ModelWeightAveraging
         :param ckpt_dir: the directory where the checkpoints are saved
         :param metric_to_watch: monitoring loss or acc, will be identical to that which determines best_model
-        :param metric_idx:
         :param load_checkpoint: whether to load pre-existing snapshot dict.
         :param number_of_models_to_average: number of models to average
         """
 
         self.averaging_snapshots_file = os.path.join(ckpt_dir, "averaging_snapshots.pkl")
         self.number_of_models_to_average = number_of_models_to_average
         self.metric_to_watch = metric_to_watch
-        self.metric_idx = metric_idx
         self.greater_is_better = greater_is_better
 
         # if continuing training, copy previous snapshot dict if exist
         if load_checkpoint and ckpt_dir is not None and os.path.isfile(self.averaging_snapshots_file):
             averaging_snapshots_dict = read_ckpt_state_dict(self.averaging_snapshots_file)
 
         else:
@@ -47,45 +44,45 @@
             if self.greater_is_better:
                 averaging_snapshots_dict["snapshots_metric"] = -1 * np.inf * np.ones(self.number_of_models_to_average)
             else:
                 averaging_snapshots_dict["snapshots_metric"] = np.inf * np.ones(self.number_of_models_to_average)
 
             torch.save(averaging_snapshots_dict, self.averaging_snapshots_file)
 
-    def update_snapshots_dict(self, model, validation_results_tuple):
+    def update_snapshots_dict(self, model, validation_results_dict):
         """
         Update the snapshot dict and returns the updated average model for saving
         :param model: the latest model
-        :param validation_results_tuple: performance of the latest model
+        :param validation_results_dict: performance of the latest model
         """
         averaging_snapshots_dict = self._get_averaging_snapshots_dict()
 
         # IF CURRENT MODEL IS BETTER, TAKING HIS PLACE IN ACC LIST AND OVERWRITE THE NEW AVERAGE
-        require_update, update_ind = self._is_better(averaging_snapshots_dict, validation_results_tuple)
+        require_update, update_ind = self._is_better(averaging_snapshots_dict, validation_results_dict)
         if require_update:
             # moving state dict to cpu
-            new_sd = model.state_dict()
+            new_sd = unwrap_model(model).state_dict()
             new_sd = move_state_dict_to_device(new_sd, "cpu")
 
             averaging_snapshots_dict["snapshot" + str(update_ind)] = new_sd
-            averaging_snapshots_dict["snapshots_metric"][update_ind] = validation_results_tuple[self.metric_idx]
+            averaging_snapshots_dict["snapshots_metric"][update_ind] = validation_results_dict[self.metric_to_watch]
 
         return averaging_snapshots_dict
 
-    def get_average_model(self, model, validation_results_tuple=None):
+    def get_average_model(self, model, validation_results_dict=None):
         """
         Returns the averaged model
         :param model: will be used to determine arch
-        :param validation_results_tuple: if provided, will update the average model before returning
+        :param validation_results_dict: if provided, will update the average model before returning
         :param target_device: if provided, return sd on target device
 
         """
         # If validation tuple is provided, update the average model
-        if validation_results_tuple is not None:
-            averaging_snapshots_dict = self.update_snapshots_dict(model, validation_results_tuple)
+        if validation_results_dict is not None:
+            averaging_snapshots_dict = self.update_snapshots_dict(model, validation_results_dict)
         else:
             averaging_snapshots_dict = self._get_averaging_snapshots_dict()
 
         torch.save(averaging_snapshots_dict, self.averaging_snapshots_file)
         average_model_sd = averaging_snapshots_dict["snapshot0"]
         for n_model in range(1, self.number_of_models_to_average):
             if averaging_snapshots_dict["snapshot" + str(n_model)] is not None:
@@ -98,22 +95,22 @@
 
     def cleanup(self):
         """
         Delete snapshot file when reaching the last epoch
         """
         os.remove(self.averaging_snapshots_file)
 
-    def _is_better(self, averaging_snapshots_dict, validation_results_tuple):
+    def _is_better(self, averaging_snapshots_dict, validation_results_dict):
         """
         Determines if the new model is better according to the specified metrics
         :param averaging_snapshots_dict: snapshot dict
-        :param validation_results_tuple: latest model performance
+        :param validation_results_dict: latest model performance
         """
         snapshot_metric_array = averaging_snapshots_dict["snapshots_metric"]
-        val = validation_results_tuple[self.metric_idx]
+        val = validation_results_dict[self.metric_to_watch]
 
         if self.greater_is_better:
             update_ind = np.argmin(snapshot_metric_array)
         else:
             update_ind = np.argmax(snapshot_metric_array)
 
         if (self.greater_is_better and val > snapshot_metric_array[update_ind]) or (not self.greater_is_better and val < snapshot_metric_array[update_ind]):
```

## super_gradients/training/utils/callbacks/__init__.py

```diff
@@ -1,10 +1,9 @@
 from super_gradients.training.utils.callbacks.base_callbacks import CallbackHandler, PhaseCallback, Callback, PhaseContext, Phase
 from super_gradients.training.utils.callbacks.callbacks import (
-    ContextSgMethods,
     ModelConversionCheckCallback,
     DeciLabUploadCallback,
     LRCallbackBase,
     EpochStepWarmupLRCallback,
     BatchStepLinearWarmupLRCallback,
     StepLRCallback,
     ExponentialLRCallback,
@@ -17,29 +16,29 @@
     KDModelMetricsUpdateCallback,
     PhaseContextTestCallback,
     DetectionVisualizationCallback,
     BinarySegmentationVisualizationCallback,
     TrainingStageSwitchCallbackBase,
     YoloXTrainingStageSwitchCallback,
     TestLRCallback,
+    TimerCallback,
 )
 from super_gradients.training.utils.callbacks.ppyoloe_switch_callback import PPYoloETrainingStageSwitchCallback
 from super_gradients.common.object_names import Callbacks, LRSchedulers, LRWarmups
 from super_gradients.common.registry.registry import CALLBACKS, LR_SCHEDULERS_CLS_DICT, LR_WARMUP_CLS_DICT
 
 __all__ = [
     "Callback",
     "Callbacks",
     "CALLBACKS",
     "LRSchedulers",
     "LR_SCHEDULERS_CLS_DICT",
     "LRWarmups",
     "LR_WARMUP_CLS_DICT",
     "Phase",
-    "ContextSgMethods",
     "PhaseContext",
     "PhaseCallback",
     "ModelConversionCheckCallback",
     "DeciLabUploadCallback",
     "LRCallbackBase",
     "EpochStepWarmupLRCallback",
     "BatchStepLinearWarmupLRCallback",
@@ -56,8 +55,9 @@
     "DetectionVisualizationCallback",
     "BinarySegmentationVisualizationCallback",
     "TrainingStageSwitchCallbackBase",
     "YoloXTrainingStageSwitchCallback",
     "CallbackHandler",
     "TestLRCallback",
     "PPYoloETrainingStageSwitchCallback",
+    "TimerCallback",
 ]
```

## super_gradients/training/utils/callbacks/base_callbacks.py

```diff
@@ -46,18 +46,16 @@
         train_loader=None,
         valid_loader=None,
         training_params=None,
         ddp_silent_mode=None,
         checkpoint_params=None,
         architecture=None,
         arch_params=None,
-        metric_idx_in_results_tuple=None,
         metric_to_watch=None,
         valid_metrics=None,
-        context_methods=None,
         ema_model=None,
     ):
         self.epoch = epoch
         self.batch_idx = batch_idx
         self.optimizer = optimizer
         self.inputs = inputs
         self.preds = preds
@@ -79,15 +77,14 @@
         self.training_params = training_params
         self.ddp_silent_mode = ddp_silent_mode
         self.checkpoint_params = checkpoint_params
         self.architecture = architecture
         self.arch_params = arch_params
         self.metric_to_watch = metric_to_watch
         self.valid_metrics = valid_metrics
-        self.context_methods = context_methods
         self.ema_model = ema_model
 
     def update_context(self, **kwargs):
         for attr, attr_val in kwargs.items():
             setattr(self, attr, attr_val)
```

## super_gradients/training/utils/callbacks/callbacks.py

```diff
@@ -1,46 +1,39 @@
 import copy
 import math
 import os
 import signal
 import time
-from typing import List, Union, Optional, Sequence
+from typing import List, Union, Optional, Sequence, Mapping
 
 import csv
 import cv2
 import numpy as np
 import onnx
 import onnxruntime
 import torch
 from deprecated import deprecated
+from torch.utils.data import DataLoader
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
+from super_gradients.common.environment.ddp_utils import multi_process_safe
 from super_gradients.common.plugins.deci_client import DeciClient
-from super_gradients.common.registry.registry import register_lr_scheduler, register_lr_warmup, register_callback
+from super_gradients.common.registry.registry import register_lr_scheduler, register_lr_warmup, register_callback, LR_SCHEDULERS_CLS_DICT, TORCH_LR_SCHEDULERS
 from super_gradients.common.object_names import LRSchedulers, LRWarmups, Callbacks
+from super_gradients.common.sg_loggers.time_units import GlobalBatchStepNumber, EpochNumber
+from super_gradients.training.utils import get_param
 from super_gradients.training.utils.callbacks.base_callbacks import PhaseCallback, PhaseContext, Phase, Callback
 from super_gradients.training.utils.detection_utils import DetectionVisualization, DetectionPostPredictionCallback
 from super_gradients.training.utils.segmentation_utils import BinarySegmentationVisualization
-from super_gradients.common.environment.ddp_utils import multi_process_safe
 from super_gradients.common.environment.checkpoints_dir_utils import get_project_checkpoints_dir_path
-
+from super_gradients.training.utils.utils import unwrap_model
 
 logger = get_logger(__name__)
 
 
-class ContextSgMethods:
-    """
-    Class for delegating Trainer's methods, so that only the relevant ones are ("phase wise") are accessible.
-    """
-
-    def __init__(self, **methods):
-        for attr, attr_val in methods.items():
-            setattr(self, attr, attr_val)
-
-
 @register_callback(Callbacks.MODEL_CONVERSION_CHECK)
 class ModelConversionCheckCallback(PhaseCallback):
     """
     Pre-training callback that verifies model conversion to onnx given specified conversion parameters.
 
     The model is converted, then inference is applied with onnx runtime.
 
@@ -70,15 +63,15 @@
         self.output_names = kwargs.get("output_names") or ["output"]
         self.dynamic_axes = kwargs.get("dynamic_axes") or {"input": {0: "batch_size"}, "output": {0: "batch_size"}}
 
         self.rtol = kwargs.get("rtol", 1e-03)
         self.atol = kwargs.get("atol", 1e-05)
 
     def __call__(self, context: PhaseContext):
-        model = copy.deepcopy(context.net.module)
+        model = copy.deepcopy(unwrap_model(context.net))
         model = model.cpu()
         model.eval()  # Put model into eval mode
 
         if hasattr(model, "prep_model_for_conversion"):
             model.prep_model_for_conversion(input_size=self.input_dimensions)
 
         x = torch.randn(self.primary_batch_size, *self.input_dimensions, requires_grad=False)
@@ -199,20 +192,20 @@
     def __call__(self, context: PhaseContext) -> None:
         """
         This function will attempt to upload the trained model and schedule an optimization for it.
 
         :param context: Training phase context
         """
         try:
-            model = copy.deepcopy(context.net)
+            model = copy.deepcopy(unwrap_model(context.net))
             model_state_dict_path = os.path.join(context.ckpt_dir, self.ckpt_name)
             model_state_dict = torch.load(model_state_dict_path)["net"]
             model.load_state_dict(state_dict=model_state_dict)
 
-            model = model.module.cpu()
+            model = model.cpu()
             if hasattr(model, "prep_model_for_conversion"):
                 model.prep_model_for_conversion(input_size=self.input_dimensions)
 
             self.upload_model(model=model)
             model_name = self.model_name
             logger.info(f"Successfully added {model_name} to the model repository")
 
@@ -262,15 +255,17 @@
 
         :param context: PhaseContext: current phase's context.
         """
         raise NotImplementedError
 
     def update_lr(self, optimizer, epoch, batch_idx=None):
         if self.update_param_groups:
-            param_groups = self.net.module.update_param_groups(optimizer.param_groups, self.lr, epoch, batch_idx, self.training_params, self.train_loader_len)
+            param_groups = unwrap_model(self.net).update_param_groups(
+                optimizer.param_groups, self.lr, epoch, batch_idx, self.training_params, self.train_loader_len
+            )
             optimizer.param_groups = param_groups
         else:
             # UPDATE THE OPTIMIZERS PARAMETER
             for param_group in optimizer.param_groups:
                 param_group["lr"] = self.lr
 
 
@@ -368,15 +363,17 @@
         Same as in LRCallbackBase
         :param optimizer:
         :param epoch:
         :param batch_idx:
         :return:
         """
         if self.update_param_groups:
-            param_groups = self.net.module.update_param_groups(optimizer.param_groups, self.lr, epoch, batch_idx, self.training_params, self.train_loader_len)
+            param_groups = unwrap_model(self.net).update_param_groups(
+                optimizer.param_groups, self.lr, epoch, batch_idx, self.training_params, self.train_loader_len
+            )
             optimizer.param_groups = param_groups
         else:
             # UPDATE THE OPTIMIZERS PARAMETER
             for param_group in optimizer.param_groups:
                 param_group["lr"] = self.lr
 
 
@@ -734,15 +731,14 @@
         if self.output_path is None:
             raise ValueError("Output path must be specified")
 
         super(RoboflowResultCallback, self).__init__()
 
     @multi_process_safe
     def on_training_end(self, context: PhaseContext):
-
         with open(self.output_path, mode="a", newline="") as csv_file:
             writer = csv.writer(csv_file)
 
             mAP = context.metrics_dict["mAP@0.50:0.95"].item()
             writer.writerow([self.dataset_name, mAP])
 
 
@@ -755,7 +751,200 @@
 
     def __init__(self, lr_placeholder):
         super(TestLRCallback, self).__init__(Phase.VALIDATION_EPOCH_END)
         self.lr_placeholder = lr_placeholder
 
     def __call__(self, context: PhaseContext):
         self.lr_placeholder.append(context.optimizer.param_groups[0]["lr"])
+
+
+@register_callback(Callbacks.TIMER)
+class TimerCallback(Callback):
+    def __init__(self):
+        self.events = {}
+
+    @multi_process_safe
+    def on_train_loader_start(self, context: PhaseContext) -> None:
+        self.events["on_train_loader_start"] = cv2.getTickCount()
+
+    @multi_process_safe
+    def on_train_batch_start(self, context: PhaseContext) -> None:
+        self.events["on_train_batch_start"] = cv2.getTickCount()
+
+    @multi_process_safe
+    def on_train_batch_loss_end(self, context: PhaseContext) -> None:
+        self.events["on_train_batch_loss_end"] = cv2.getTickCount()
+        context.sg_logger.add_scalar(
+            tag="timer/train_batch_forward_with_loss_ms",
+            scalar_value=self._elapsed_time_between("on_train_batch_start", "on_train_batch_loss_end"),
+            global_step=GlobalBatchStepNumber(self._infer_global_step(context, is_train_loader=True)),
+        )
+
+    @multi_process_safe
+    def on_train_batch_gradient_step_start(self, context: PhaseContext) -> None:
+        self.events["on_train_batch_gradient_step_start"] = cv2.getTickCount()
+
+    @multi_process_safe
+    def on_train_batch_gradient_step_end(self, context: PhaseContext) -> None:
+        self.events["on_train_batch_gradient_step_end"] = cv2.getTickCount()
+        context.sg_logger.add_scalar(
+            tag="timer/train_batch_gradient_time",
+            scalar_value=self._elapsed_time_between("on_train_batch_gradient_step_start", "on_train_batch_gradient_step_end"),
+            global_step=GlobalBatchStepNumber(self._infer_global_step(context, is_train_loader=True)),
+        )
+
+    @multi_process_safe
+    def on_train_batch_end(self, context: PhaseContext) -> None:
+        self.events["on_train_batch_end"] = cv2.getTickCount()
+        context.sg_logger.add_scalar(
+            tag="timer/train_batch_total_time_ms",
+            scalar_value=self._elapsed_time_between("on_train_batch_start", "on_train_batch_end"),
+            global_step=GlobalBatchStepNumber(self._infer_global_step(context, is_train_loader=True)),
+        )
+
+    @multi_process_safe
+    def on_train_loader_end(self, context: PhaseContext) -> None:
+        self.events["on_train_loader_end"] = cv2.getTickCount()
+        context.sg_logger.add_scalar(
+            tag="timer/train_loader_total_time_ms",
+            scalar_value=self._elapsed_time_between("on_train_loader_start", "on_train_loader_end"),
+            global_step=EpochNumber(context.epoch),
+        )
+
+    @multi_process_safe
+    def on_validation_loader_start(self, context: PhaseContext) -> None:
+        self.events["on_validation_loader_start"] = cv2.getTickCount()
+
+    @multi_process_safe
+    def on_validation_batch_start(self, context: PhaseContext) -> None:
+        self.events["on_validation_batch_start"] = cv2.getTickCount()
+
+    @multi_process_safe
+    def on_validation_batch_end(self, context: PhaseContext) -> None:
+        self.events["on_validation_batch_end"] = cv2.getTickCount()
+        context.sg_logger.add_scalar(
+            tag="timer/validation_batch_total_time_ms",
+            scalar_value=self._elapsed_time_between("on_validation_batch_start", "on_validation_batch_end"),
+            global_step=GlobalBatchStepNumber(self._infer_global_step(context, is_train_loader=False)),
+        )
+
+    @multi_process_safe
+    def on_validation_loader_end(self, context: PhaseContext) -> None:
+        self.events["on_validation_loader_end"] = cv2.getTickCount()
+        context.sg_logger.add_scalar(
+            tag="timer/validation_loader_total_time_ms",
+            scalar_value=self._elapsed_time_between("on_validation_loader_start", "on_validation_loader_end"),
+            global_step=EpochNumber(context.epoch),
+        )
+
+        context.sg_logger.add_scalar(
+            tag="timer/epoch_total_time_sec",
+            scalar_value=self._elapsed_time_between("on_train_loader_start", "on_validation_loader_end") / 1000.0,
+            global_step=EpochNumber(context.epoch),
+        )
+
+    def _elapsed_time_between(self, start_event, end_event):
+        return 1000.0 * (self.events[end_event] - self.events[start_event]) / cv2.getTickFrequency()
+
+    def _infer_global_step(self, context: PhaseContext, is_train_loader: bool):
+        train_loader_length = len(context.train_loader) if context.train_loader is not None else 0
+        valid_loader_length = len(context.valid_loader) if context.valid_loader is not None else 0
+        total_steps_in_epoch = train_loader_length + valid_loader_length
+        total_steps_in_done = context.epoch * total_steps_in_epoch
+        if is_train_loader:
+            return total_steps_in_done + context.batch_idx
+        else:
+            return total_steps_in_done + train_loader_length + context.batch_idx
+
+
+def create_lr_scheduler_callback(
+    lr_mode: Union[str, Mapping],
+    train_loader: DataLoader,
+    net: torch.nn.Module,
+    training_params: Mapping,
+    update_param_groups: bool,
+    optimizer: torch.optim.Optimizer,
+) -> PhaseCallback:
+    """
+    Creates the phase callback in charge of LR scheduling, to be used by Trainer.
+
+    :param lr_mode: Union[str, Mapping],
+
+                    When str:
+
+                    Learning rate scheduling policy, one of ['step','poly','cosine','function'].
+
+                    'step' refers to constant updates at epoch numbers passed through `lr_updates`. Each update decays the learning rate by `lr_decay_factor`.
+
+                    'cosine' refers to the Cosine Anealing policy as mentioned in https://arxiv.org/abs/1608.03983.
+                      The final learning rate ratio is controlled by `cosine_final_lr_ratio` training parameter.
+
+                    'poly' refers to the polynomial decrease: in each epoch iteration `self.lr = self.initial_lr * pow((1.0 - (current_iter / max_iter)), 0.9)`
+
+                    'function' refers to a user-defined learning rate scheduling function, that is passed through `lr_schedule_function`.
+
+
+
+                    When Mapping, refers to a torch.optim.lr_scheduler._LRScheduler, following the below API:
+
+                        lr_mode = {LR_SCHEDULER_CLASS_NAME: {**LR_SCHEDULER_KWARGS, "phase": XXX, "metric_name": XXX)
+
+                        Where "phase" (of Phase type) controls when to call torch.optim.lr_scheduler._LRScheduler.step().
+
+                        For instance, in order to:
+                        - Update LR on each batch: Use phase: Phase.TRAIN_BATCH_END
+                        - Update LR after each epoch: Use phase: Phase.TRAIN_EPOCH_END
+
+                        The "metric_name" refers to the metric to watch (See docs for "metric_to_watch" in train(...)
+                         https://docs.deci.ai/super-gradients/docstring/training/sg_trainer.html) when using
+                          ReduceLROnPlateau. In any other case this kwarg is ignored.
+
+                        **LR_SCHEDULER_KWARGS are simply passed to the torch scheduler's __init__.
+
+
+
+
+    :param train_loader: DataLoader, the Trainer.train_loader used for training.
+
+    :param net: torch.nn.Module, the Trainer.net used for training.
+
+    :param training_params: Mapping, Trainer.training_params.
+
+    :param update_param_groups:bool,  Whether the Trainer.net has a specific way of updaitng its parameter group.
+
+    :param optimizer: The optimizer used for training. Will be passed to the LR callback's __init__
+     (or the torch scheduler's init, depending on the lr_mode value as described above).
+
+    :return: a PhaseCallback instance to be used by Trainer for LR scheduling.
+    """
+
+    if isinstance(lr_mode, str) and lr_mode in LR_SCHEDULERS_CLS_DICT:
+        sg_lr_callback_cls = LR_SCHEDULERS_CLS_DICT[lr_mode]
+        sg_lr_callback = sg_lr_callback_cls(
+            train_loader_len=len(train_loader),
+            net=net,
+            training_params=training_params,
+            update_param_groups=update_param_groups,
+            **training_params.to_dict(),
+        )
+    elif isinstance(lr_mode, Mapping) and list(lr_mode.keys())[0] in TORCH_LR_SCHEDULERS:
+        if update_param_groups:
+            logger.warning(
+                "The network's way of updataing (i.e update_param_groups) is not supported with native " "torch lr schedulers and will have no effect."
+            )
+        lr_scheduler_name = list(lr_mode.keys())[0]
+        torch_scheduler_params = {k: v for k, v in lr_mode[lr_scheduler_name].items() if k != "phase" and k != "metric_name"}
+        torch_scheduler_params["optimizer"] = optimizer
+        torch_scheduler = TORCH_LR_SCHEDULERS[lr_scheduler_name](**torch_scheduler_params)
+        if get_param(lr_mode[lr_scheduler_name], "phase") is None:
+            raise ValueError("Phase is required argument when working with torch schedulers.")
+
+        if lr_scheduler_name == "ReduceLROnPlateau" and get_param(lr_mode[lr_scheduler_name], "metric_name") is None:
+            raise ValueError("metric_name is required argument when working with ReduceLROnPlateau schedulers.")
+
+        sg_lr_callback = LRSchedulerCallback(
+            scheduler=torch_scheduler, phase=lr_mode[lr_scheduler_name]["phase"], metric_name=get_param(lr_mode[lr_scheduler_name], "metric_name")
+        )
+    else:
+        raise ValueError(f"Unknown lr_mode: {lr_mode}")
+
+    return sg_lr_callback
```

## super_gradients/training/utils/media/image.py

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 import torch
 import requests
 from urllib.parse import urlparse
 
 
-IMG_EXTENSIONS = ("bmp", "dng", "jpeg", "jpg", "mpo", "png", "tif", "tiff", "webp", "pfm")
+IMG_EXTENSIONS = ("bmp", "dng", "jpeg", "jpg", "mpo", "pfm", "pgm", "png", "ppm", "tif", "tiff", "webp")
 SingleImageSource = Union[str, np.ndarray, torch.Tensor, PIL.Image.Image]
 ImageSource = Union[SingleImageSource, List[SingleImageSource]]
 
 
 def load_images(images: Union[List[ImageSource], ImageSource]) -> List[np.ndarray]:
     """Load a single image or a list of images and return them as a list of numpy arrays.
```

## super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py

```diff
@@ -75,29 +75,29 @@
         maxm = pool2(heatmap[None, :, :, :])
     else:
         maxm = pool1(heatmap[None, :, :, :])
 
     return maxm
 
 
-def _get_maximum_from_heatmap(heatmap, max_num_people: int, keypoint_threshold: float):
+def _get_maximum_from_heatmap(heatmap, max_num_people: int, pose_center_score_threshold: float) -> Tuple[Tensor, Tensor]:
     """
 
     :param heatmap: [1, H, W] Single-channel heatmap
-    :param max_num_people: (int)
-    :param keypoint_threshold: (float)
-    :return:
+    :param max_num_people: (int) Maximum number of poses to return
+    :param pose_center_score_threshold: (float) A minimum score of a pose center keypoint for pose to be considered as a potential candidate
+    :return: Tuple of (indexes of poses, scores)
     """
     maxm = _hierarchical_pool(heatmap)
     maxm = torch.eq(maxm, heatmap).float()
     heatmap = heatmap * maxm
     scores = heatmap.view(-1)
     scores, pos_ind = scores.topk(max_num_people)
 
-    select_ind = (scores > (keypoint_threshold)).nonzero()
+    select_ind = (scores > pose_center_score_threshold).nonzero()
     scores = scores[select_ind][:, 0]
     pos_ind = pos_ind[select_ind][:, 0]
 
     return pos_ind, scores
 
 
 def _up_interpolate(x, size):
@@ -113,14 +113,25 @@
 def _cal_area_2_torch(v):
     w = torch.max(v[:, :, 0], -1)[0] - torch.min(v[:, :, 0], -1)[0]
     h = torch.max(v[:, :, 1], -1)[0] - torch.min(v[:, :, 1], -1)[0]
     return w * w + h * h
 
 
 def _nms_core(pose_coord, heat_score, nms_threshold: float, nms_num_threshold: int):
+    """
+    Non-maximum suppression for predicted poses.
+    Removes poses that has certain number of joints that are too close to each other.
+
+    :param pose_coord: Array of shape [num_people, num_joints, 2] with pose coordinates
+    :param heat_score: Scores of each joint
+    :param float nms_threshold: The maximum distance between two joints for them to be considered as belonging to the same pose.
+                          Given in terms of a percentage of a square root of the area of the pose bounding box.
+    :param int nms_num_threshold: Number of joints that must pass the NMS check for the pose to be considered as a valid one.
+    :return: Indexes of poses that should be kept
+    """
     num_people, num_joints, _ = pose_coord.shape
     pose_area = _cal_area_2_torch(pose_coord)[:, None].repeat(1, num_people * num_joints)
     pose_area = pose_area.reshape(num_people, num_people, num_joints)
 
     pose_diff = pose_coord[:, None, :, :] - pose_coord
     pose_diff.pow_(2)
     pose_dist = pose_diff.sum(3)
@@ -155,23 +166,27 @@
 
     y_b = torch.clamp(torch.floor(pose_coord[:, :, 1]), 0, h - 1).long()
     x_l = torch.clamp(torch.floor(pose_coord[:, :, 0]), 0, w - 1).long()
     heatval = torch.gather(heatmap_nocenter, 0, y_b * w + x_l).unsqueeze(-1)
     return heatval
 
 
-def pose_nms(heatmap_avg, poses, max_num_people: int, nms_threshold: float, nms_num_threshold: int) -> Tuple[np.ndarray, np.ndarray]:
+def pose_nms(
+    heatmap_avg, poses, max_num_people: int, nms_threshold: float, nms_num_threshold: int, pose_score_threshold: float
+) -> Tuple[np.ndarray, np.ndarray]:
     """
     NMS for the regressed poses results.
 
-    :param heatmap_avg (Tensor): Avg of the heatmaps at all scales (1, 1+num_joints, w, h)
-    :param poses (List): Gather of the pose proposals [(num_people, num_joints, 3)]
-    :param max_num_people (int): Maximum number of decoded poses
-    :param nms_threshold (float) Minimum confidence threshold for joint
-    :param nms_num_threshold (int): Minimum number of joints per pose above the nms_threshold for pose to be considered a valid candidate
+    :param Tensor heatmap_avg: Avg of the heatmaps at all scales (1, 1+num_joints, w, h)
+    :param List poses: Gather of the pose proposals [(num_people, num_joints, 3)]
+    :param int max_num_people: Maximum number of decoded poses
+    :param float nms_threshold: The maximum distance between two joints for them to be considered as belonging to the same pose.
+                          Given in terms of a percentage of a square root of the area of the pose bounding box.
+    :param int nms_num_threshold: Number of joints that must pass the NMS check for the pose to be considered as a valid one.
+    :param float pose_score_threshold: Minimum confidence threshold for pose. Pose with confidence lower than this threshold will be discarded.
 
     :return Tuple of (poses, scores)
     """
     assert len(poses) == 1
 
     pose_score = torch.cat([pose[:, :, 2:] for pose in poses], dim=0)
     pose_coord = torch.cat([pose[:, :, :2] for pose in poses], dim=0)
@@ -194,81 +209,99 @@
     if len(keep_pose_inds) > max_num_people:
         heat_score, topk_inds = torch.topk(heat_score, max_num_people)
         poses = poses[topk_inds]
 
     poses = poses.numpy()
     if len(poses):
         scores = poses[:, :, 2].mean(axis=1)
+
+        mask = scores >= pose_score_threshold
+        poses = poses[mask]
+        scores = scores[mask]
     else:
         return np.zeros((0, num_joints, 3), dtype=np.float32), np.zeros((0,), dtype=np.float32)
     return poses, scores
 
 
-def aggregate_results(heatmap: Tensor, posemap: Tensor, output_stride: int, keypoint_threshold: float, max_num_people: int) -> Tuple[Tensor, List[Tensor]]:
+def aggregate_results(
+    heatmap: Tensor, posemap: Tensor, output_stride: int, pose_center_score_threshold: float, max_num_people: int
+) -> Tuple[Tensor, List[Tensor]]:
     """
     Get initial pose proposals and aggregate the results of all scale.
     Not this implementation works only for batch size of 1.
 
     :param heatmap: Heatmap at this scale (B, 1+num_joints, w, h)
     :param posemap: Posemap at this scale (B, 2*num_joints, w, h)
     :param output_stride: Ratio of input size / predictions size
-    :param keypoint_threshold: (float)
+    :param pose_center_score_threshold: (float) A minimum score of a pose center keypoint for pose to be considered as a potential candidate
     :param max_num_people: (int)
 
     :return:
         - heatmap_sum: Sum of the heatmaps (1, 1+num_joints, w, h)
         - poses (List): Gather of the pose proposals [B, (num_people, num_joints, 3)]
     """
 
     poses = []
 
     h, w = heatmap[0].size(-1), heatmap[0].size(-2)
 
     heatmap_sum = _up_interpolate(heatmap, size=(int(output_stride * w), int(output_stride * h)))
     center_heatmap = heatmap[0, -1:]
-    pose_ind, ctr_score = _get_maximum_from_heatmap(center_heatmap, keypoint_threshold=keypoint_threshold, max_num_people=max_num_people)
+    pose_ind, ctr_score = _get_maximum_from_heatmap(center_heatmap, pose_center_score_threshold=pose_center_score_threshold, max_num_people=max_num_people)
     posemap = posemap[0].permute(1, 2, 0).view(h * w, -1, 2)
     pose = output_stride * posemap[pose_ind]
     ctr_score = ctr_score[:, None].expand(-1, pose.shape[-2])[:, :, None]
     poses.append(torch.cat([pose, ctr_score], dim=2))
 
     return heatmap_sum, poses
 
 
 class DEKRPoseEstimationDecodeCallback(nn.Module):
     """
     Class that implements decoding logic of DEKR's model predictions into poses.
     """
 
-    def __init__(self, output_stride: int, max_num_people: int, keypoint_threshold: float, nms_threshold: float, nms_num_threshold: int, apply_sigmoid: bool):
+    def __init__(
+        self,
+        output_stride: int,
+        max_num_people: int,
+        keypoint_threshold: float,
+        nms_threshold: float,
+        nms_num_threshold: int,
+        apply_sigmoid: bool,
+        min_confidence: float = 0.0,
+    ):
         """
 
-        :param output_stride:
-        :param max_num_people:
-        :param keypoint_threshold:
-        :param nms_threshold:
-        :param nms_num_threshold:
-        :param apply_sigmoid: If True, apply the sigmoid activation on heatmap. This is needed when heatmap is not
+        :param output_stride: Output stride of the model
+        :param int max_num_people: Maximum number of decoded poses
+        :param float keypoint_threshold: (float) A minimum score of a pose center keypoint for pose to be considered as a potential candidate
+        :param float nms_threshold: The maximum distance between two joints for them to be considered as belonging to the same pose.
+                              Given in terms of a percentage of a square root of the area of the pose bounding box.
+        :param int nms_num_threshold: Number of joints that must pass the NMS check for the pose to be considered as a valid one.
+        :param bool apply_sigmoid: If True, apply the sigmoid activation on heatmap. This is needed when heatmap is not
                               bound to [0..1] range and trained with logits (E.g focal loss)
+        :param float min_confidence: Minimum confidence threshold for pose
         """
         super().__init__()
         self.keypoint_threshold = keypoint_threshold
         self.max_num_people = max_num_people
         self.output_stride = output_stride
         self.nms_threshold = nms_threshold
         self.nms_num_threshold = nms_num_threshold
         self.apply_sigmoid = apply_sigmoid
+        self.min_confidence = min_confidence
 
     @torch.no_grad()
     def forward(self, predictions: Union[Tensor, Tuple[Tensor, Tensor]]) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """
 
-        :param predictions: Either tuple (heatmap, offset):
-            heatmap - [1, NumJoints+1,H,W]
-            offset - [1, NumJoints*2,H,W]
+        :param predictions: Tuple (heatmap, offset):
+            heatmap - [BatchSize, NumJoints+1,H,W]
+            offset - [BatchSize, NumJoints*2,H,W]
 
         :return: Tuple
         """
         all_poses = []
         all_scores = []
 
         heatmap, offset = predictions
@@ -288,20 +321,25 @@
 
         if self.apply_sigmoid:
             heatmap = heatmap.sigmoid()
 
         heatmap_sum, poses_sum = aggregate_results(
             heatmap,
             posemap,
-            keypoint_threshold=self.keypoint_threshold,
+            pose_center_score_threshold=self.keypoint_threshold,
             max_num_people=self.max_num_people,
             output_stride=self.output_stride,
         )
 
         poses, scores = pose_nms(
-            heatmap_sum, poses_sum, max_num_people=self.max_num_people, nms_threshold=self.nms_threshold, nms_num_threshold=self.nms_num_threshold
+            heatmap_sum,
+            poses_sum,
+            max_num_people=self.max_num_people,
+            nms_threshold=self.nms_threshold,
+            nms_num_threshold=self.nms_num_threshold,
+            pose_score_threshold=self.min_confidence,
         )
 
         if len(poses) != len(scores):
             raise RuntimeError("Decoding error detected. Returned mismatching number of poses/scores")
 
         return poses, scores
```

## Comparing `super_gradients/training/exceptions/dataset_exceptions.py` & `super_gradients/common/exceptions/dataset_exceptions.py`

 * *Files identical despite different names*

## Comparing `super_gradients/training/exceptions/kd_trainer_exceptions.py` & `super_gradients/common/exceptions/kd_trainer_exceptions.py`

 * *Files identical despite different names*

## Comparing `super_gradients/training/exceptions/loss_exceptions.py` & `super_gradients/common/exceptions/loss_exceptions.py`

 * *Files identical despite different names*

## Comparing `super_gradients/training/exceptions/sg_trainer_exceptions.py` & `super_gradients/common/exceptions/sg_trainer_exceptions.py`

 * *Files identical despite different names*

## Comparing `super_gradients/training/models/prediction_results.py` & `super_gradients/training/utils/predict/prediction_results.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 from abc import ABC, abstractmethod
-from typing import List, Optional, Tuple, Iterator
 from dataclasses import dataclass
+from typing import List, Optional, Tuple, Iterator
 
 import numpy as np
 
-from super_gradients.training.models.predictions import Prediction, DetectionPrediction
-from super_gradients.training.utils.media.video import show_video_from_frames, save_video
 from super_gradients.training.utils.media.image import show_image, save_image
-from super_gradients.training.utils.visualization.utils import generate_color_mapping
+from super_gradients.training.utils.media.video import show_video_from_frames, save_video
 from super_gradients.training.utils.visualization.detection import draw_bbox
+from super_gradients.training.utils.visualization.classification import draw_label
+
+from super_gradients.training.utils.visualization.utils import generate_color_mapping
+from .predictions import Prediction, DetectionPrediction, ClassificationPrediction
 
 
 @dataclass
 class ImagePrediction(ABC):
     """Object wrapping an image and a model's prediction.
 
     :attr image:        Input image
@@ -38,14 +40,62 @@
     @abstractmethod
     def save(self, *args, **kwargs) -> None:
         """Save the predictions on the image."""
         pass
 
 
 @dataclass
+class ImageClassificationPrediction(ImagePrediction):
+    """Object wrapping an image and a classification model's prediction.
+
+    :attr image:        Input image
+    :attr predictions:  Predictions of the model
+    :attr class_names:  List of the class names to predict
+    """
+
+    image: np.ndarray
+    prediction: ClassificationPrediction
+    class_names: List[str]
+
+    def draw(self, show_confidence: bool = True) -> np.ndarray:
+        """Draw the predicted label on the image.
+
+        :param show_confidence: Whether to show confidence scores on the image.
+        :return:                Image with predicted label.
+        """
+
+        image = self.image.copy()
+        return draw_label(
+            image=image, label=self.class_names[self.prediction.labels], confidence=str(self.prediction.confidence), image_shape=self.prediction.image_shape[1:]
+        )
+
+    def show(self, show_confidence: bool = True) -> None:
+        """Display the image with predicted label.
+
+        :param show_confidence: Whether to show confidence scores on the image.
+        """
+        # to do draw the prediction on the image
+        image = self.draw(show_confidence=show_confidence)
+        show_image(image)
+
+    def save(
+        self,
+        output_path: str,
+        show_confidence: bool = True,
+    ) -> None:
+        """Save the predicted label on the images.
+
+        :param output_path:     Path to the output video file.
+        :param show_confidence: Whether to show confidence scores on the image.
+        """
+        image = self.draw(show_confidence=show_confidence)
+        save_image(image=image, path=output_path)
+
+
+@dataclass
 class ImageDetectionPrediction(ImagePrediction):
     """Object wrapping an image and a detection model's prediction.
 
     :attr image:        Input image
     :attr predictions:  Predictions of the model
     :attr class_names:  List of the class names to predict
     """
@@ -63,15 +113,14 @@
                                 Default is None, which generates a default color mapping based on the number of class names.
         :return:                Image with predicted bboxes. Note that this does not modify the original image.
         """
         image = self.image.copy()
         color_mapping = color_mapping or generate_color_mapping(len(self.class_names))
 
         for pred_i in np.argsort(self.prediction.confidence):
-
             class_id = int(self.prediction.labels[pred_i])
             score = "" if not show_confidence else str(round(self.prediction.confidence[pred_i], 2))
 
             image = draw_bbox(
                 image=image,
                 title=f"{self.class_names[class_id]} {score}",
                 color=color_mapping[class_id],
@@ -156,14 +205,44 @@
     @abstractmethod
     def save(self, *args, **kwargs) -> None:
         """Save the predictions on the video."""
         pass
 
 
 @dataclass
+class ImagesClassificationPrediction(ImagesPredictions):
+    """Object wrapping the list of image classification predictions.
+
+    :attr _images_prediction_lst:  List of the predictions results
+    """
+
+    _images_prediction_lst: List[ImageClassificationPrediction]
+
+    def show(self, show_confidence: bool = True) -> None:
+        """Display the predicted labels on the images.
+        :param show_confidence: Whether to show confidence scores on the image.
+        """
+        for prediction in self._images_prediction_lst:
+            prediction.show(show_confidence=show_confidence)
+
+    def save(self, output_folder: str, show_confidence: bool = True) -> None:
+        """Save the predicted label on the images.
+
+        :param output_folder:     Folder path, where the images will be saved.
+        :param show_confidence: Whether to show confidence scores on the image.
+        """
+        if output_folder:
+            os.makedirs(output_folder, exist_ok=True)
+
+        for i, prediction in enumerate(self._images_prediction_lst):
+            image_output_path = os.path.join(output_folder, f"pred_{i}.jpg")
+            prediction.save(output_path=image_output_path, show_confidence=show_confidence)
+
+
+@dataclass
 class ImagesDetectionPrediction(ImagesPredictions):
     """Object wrapping the list of image detection predictions.
 
     :attr _images_prediction_lst:  List of the predictions results
     """
 
     _images_prediction_lst: List[ImageDetectionPrediction]
```

## Comparing `super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md` & `super_gradients-3.1.3.dist-info/LICENSE.YOLONAS.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.1.2.dist-info/LICENSE.md` & `super_gradients-3.1.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.1.2.dist-info/METADATA` & `super_gradients-3.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-gradients
-Version: 3.1.2
+Version: 3.1.3
 Summary: SuperGradients
 Home-page: https://docs.deci.ai/super-gradients/documentation/source/welcome.html
 Author: Deci AI
 Author-email: rnd@deci.ai
 Keywords: Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre Trained,Models
 Description-Content-Type: text/markdown
 License-File: LICENSE.YOLONAS.md
@@ -45,15 +45,15 @@
 Requires-Dist: rapidfuzz
 Requires-Dist: json-tricks (==3.16.1)
 Requires-Dist: onnx-simplifier (<1.0,>=0.3.6)
 Provides-Extra: pro
 Requires-Dist: deci-platform-client (>=5.0.0) ; extra == 'pro'
 
 <div align="center" markdown="1">
-  <img src="docs/assets/SG_img/SG - Horizontal Glow 2.png" width="600"/>
+  <img src="documentation/assets/SG_img/SG - Horizontal Glow 2.png" width="600"/>
  <br/><br/>
   
 **Build, train, and fine-tune production-ready deep learning  SOTA vision models**
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Easily%20train%20or%20fine-tune%20SOTA%20computer%20vision%20models%20from%20one%20training%20repository&url=https://github.com/Deci-AI/super-gradients&via=deci_ai&hashtags=AI,deeplearning,computervision,training,opensource)
 
 #### Version 3 is out! Notebooks have been updated!
 ______________________________________________________________________
@@ -83,17 +83,17 @@
 ______________________________________________________________________
 
 ## Build with SuperGradients
 __________________________________________________________________________________________________________
 
 ### Support various computer vision tasks
 <div align="center">
-<img src="https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Segmentation 1500x900 .png" width="250px">
-<img src="https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Object detection 1500X900.png" width="250px">
-<img src="https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Classification 1500x900.png" width="250px">
+<img src="https://github.com/Deci-AI/super-gradients/raw/master/documentation/assets/SG_img/Segmentation 1500x900 .png" width="250px">
+<img src="https://github.com/Deci-AI/super-gradients/raw/master/documentation/assets/SG_img/Object detection 1500X900.png" width="250px">
+<img src="https://github.com/Deci-AI/super-gradients/raw/master/documentation/assets/SG_img/Classification 1500x900.png" width="250px">
 </div>
 
 
 ### Ready to deploy pre-trained SOTA models
 
 YOLO-NAS architecture is out! The new YOLO-NAS delivers state-of-the-art performance with the unparalleled accuracy-speed performance, outperforming other models such as YOLOv5, YOLOv6, YOLOv7 and YOLOv8.
 Check it out here: [YOLO-NAS](YOLONAS.md).
@@ -109,25 +109,25 @@
 
 model = models.get(Models.YOLO_NAS_M, pretrained_weights="coco")
 ```
 #### All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
 
 #### Classification
 <div align="center">
-<img src="./docs/assets/SG_img/Classification@2xDark.png" width="800px">
+<img src="./documentation/assets/SG_img/Classification@2xDark.png" width="800px">
 </div>
 
 #### Semantic Segmentation
 <div align="center">
-<img src="./docs/assets/SG_img/Semantic Segmentation@2xDark.png" width="800px">
+<img src="./documentation/assets/SG_img/Semantic Segmentation@2xDark.png" width="800px">
 </div>
 
 #### Object Detection 
 <div align="center">
-<img src="./docs/assets/SG_img/Object Detection@2xDark.png" width="800px">
+<img src="./documentation/assets/SG_img/Object Detection@2xDark.png" width="800px">
 </div>
 
 
 ### Easy to train SOTA Models
 
 Easily load and fine-tune production-ready, pre-trained SOTA models that incorporate best practices and validated hyper-parameters for achieving best-in-class accuracy. 
 For more information on how to do it go to [Getting Started](#getting-started)
@@ -238,124 +238,124 @@
 
 ```   
 ###  Classification
 
 #### Transfer Learning 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">  
-  <a target="_blank" href="https://bit.ly/3xzIutb"><img src="./docs/assets/SG_img/colab_logo.png" /> Classification Transfer Learning</a>
+  <a target="_blank" href="https://bit.ly/3xzIutb"><img src="./documentation/assets/SG_img/colab_logo.png" /> Classification Transfer Learning</a>
   </td>
  <td width="200">    
- <a target="_blank" href="https://bit.ly/3xwYEn1"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
+ <a target="_blank" href="https://bit.ly/3xwYEn1"><img src="./documentation/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
  </td>
 </table>
  </br></br>
 
 
 ###  Semantic Segmentation
 
 ####  Quick Start 
 <table class="tfo-notebook-buttons" align="left">
  <td width="500">
-<a target="_blank" href="https://bit.ly/3qKx9m8"><img src="./docs/assets/SG_img/colab_logo.png" /> Segmentation Quick Start</a>
+<a target="_blank" href="https://bit.ly/3qKx9m8"><img src="./documentation/assets/SG_img/colab_logo.png" /> Segmentation Quick Start</a>
  </td>
 </table>
  </br></br>
 
 
  
  ####  Transfer Learning 
 <table class="tfo-notebook-buttons" align="left">
  <td width="500">
-<a target="_blank" href="https://bit.ly/3qKwMbe"><img src="./docs/assets/SG_img/colab_logo.png" /> Segmentation Transfer Learning</a>
+<a target="_blank" href="https://bit.ly/3qKwMbe"><img src="./documentation/assets/SG_img/colab_logo.png" /> Segmentation Transfer Learning</a>
  </td>
 </table>
  </br></br>
 
 
 
 ####  How to Connect Custom Dataset 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500"> 
-<a target="_blank" href="https://bit.ly/3QQBVJp"><img src="./docs/assets/SG_img/colab_logo.png" /> Segmentation How to Connect Custom Dataset</a>
+<a target="_blank" href="https://bit.ly/3QQBVJp"><img src="./documentation/assets/SG_img/colab_logo.png" /> Segmentation How to Connect Custom Dataset</a>
    </td>
 </table>
  </br></br>
 
 
 
 ###  Object Detection
 
 
 #### Transfer Learning
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
-<a target="_blank" href="https://bit.ly/3SkMohx"><img src="./docs/assets/SG_img/colab_logo.png" /> Detection Transfer Learning</a>
+<a target="_blank" href="https://bit.ly/3SkMohx"><img src="./documentation/assets/SG_img/colab_logo.png" /> Detection Transfer Learning</a>
    </td>
 </table>
  </br></br>
 
 #### How to Connect Custom Dataset 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">  
-  <a target="_blank" href="https://bit.ly/3dqDlg3"><img src="./docs/assets/SG_img/colab_logo.png" /> Detection How to Connect Custom Dataset</a>
+  <a target="_blank" href="https://bit.ly/3dqDlg3"><img src="./documentation/assets/SG_img/colab_logo.png" /> Detection How to Connect Custom Dataset</a>
   </td>
 </table>
  </br></br>
 
 
 
 ### How to Predict Using Pre-trained Model
 
 #### Segmentation, Detection and Classification Prediction 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">    
-<a target="_blank" href="https://bit.ly/3f4mssd"><img src="./docs/assets/SG_img/colab_logo.png" /> How to Predict Using Pre-trained Model</a>
+<a target="_blank" href="https://bit.ly/3f4mssd"><img src="./documentation/assets/SG_img/colab_logo.png" /> How to Predict Using Pre-trained Model</a>
   </td>
 </table>
  </br></br>
 
 
 ## Advanced Features
 __________________________________________________________________________________________________________
 ### Post Training Quantization and Quantization Aware Training
 Quantization involves representing weights and biases in lower precision, resulting in reduced memory and computational requirements, making it useful for deploying models on devices with limited resources. The process can be done during training, called Quantization aware training, or after training, called post-training quantization. A full tutorial can be found [here](http://bit.ly/41hC8uI).
   <table class=“tfo-notebook-buttons” align=“left”>
  <td width=“500”>
-   <a target="_blank" href="http://bit.ly/3KrN6an"><img src="./docs/assets/SG_img/colab_logo.png" /> Post Training Quantization and Quantization Aware Training</a>
+   <a target="_blank" href="http://bit.ly/3KrN6an"><img src="./documentation/assets/SG_img/colab_logo.png" /> Post Training Quantization and Quantization Aware Training</a>
   </td>
 </table>
 
 ### Quantization Aware Training YoloNAS on Custom Dataset
 This tutorial provides a comprehensive guide on how to fine-tune a YoloNAS model using a custom dataset. It also demonstrates how to utilize SG's QAT (Quantization-Aware Training) support. Additionally, it offers step-by-step instructions on deploying the model and performing benchmarking.
   <table class=“tfo-notebook-buttons” align=“left”>
  <td width=“500”>
-   <a target="_blank" href="https://bit.ly/3MIKdTy"><img src="./docs/assets/SG_img/colab_logo.png" /> Quantization Aware Training YoloNAS on Custom Dataset</a>
+   <a target="_blank" href="https://bit.ly/3MIKdTy"><img src="./documentation/assets/SG_img/colab_logo.png" /> Quantization Aware Training YoloNAS on Custom Dataset</a>
   </td>
 </table>
 
 ### Knowledge Distillation Training
 Knowledge Distillation is a training technique that uses a large model, teacher model, to improve the performance of a smaller model, the student model.
 Learn more about SuperGradients knowledge distillation training with our pre-trained BEiT base teacher model and Resnet18 student model on CIFAR10 example notebook on Google Colab for an easy to use tutorial using free GPU hardware
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
-   <a target="_blank" href="https://bit.ly/3BLA5oR"><img src="./docs/assets/SG_img/colab_logo.png" /> Knowledge Distillation Training</a>
+   <a target="_blank" href="https://bit.ly/3BLA5oR"><img src="./documentation/assets/SG_img/colab_logo.png" /> Knowledge Distillation Training</a>
   </td>
 </table>
  </br></br>
 
 ### Recipes
 To train a model, it is necessary to configure 4 main components. These components are aggregated into a single "main" recipe `.yaml` file that inherits the aforementioned dataset, architecture, raining and checkpoint params. It is also possible (and recomended for flexibility) to override default settings with custom ones.
 All recipes can be found [here](http://bit.ly/3gfLw07)
 </br>
 Recipes support out of the box every model, metric or loss that is implemented in SuperGradients, but you can easily extend this to any custom object that you need by "registering it". Check out [this](http://bit.ly/3TQ4iZB) tutorial for more information.
 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
-   <a target="_blank" href="https://bit.ly/3UiY5ab"><img src="./docs/assets/SG_img/colab_logo.png" /> How to Use Recipes</a>
+   <a target="_blank" href="https://bit.ly/3UiY5ab"><img src="./documentation/assets/SG_img/colab_logo.png" /> How to Use Recipes</a>
   </td>
 </table>
  </br></br>
 
  </br>
 <details markdown="1">
   <summary><h3>Using Distributed Data Parallel (DDP) </h3></summary>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: super-gradients Version: 3.1.2 Summary:
+Metadata-Version: 2.1 Name: super-gradients Version: 3.1.3 Summary:
 SuperGradients Home-page: https://docs.deci.ai/super-gradients/documentation/
 source/welcome.html Author: Deci AI Author-email: rnd@deci.ai Keywords:
 Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre
 Trained,Models Description-Content-Type: text/markdown License-File:
 LICENSE.YOLONAS.md License-File: LICENSE.md Requires-Dist: torch (>=1.9.0)
 Requires-Dist: tqdm (>=4.57.0) Requires-Dist: boto3 (>=1.17.15) Requires-Dist:
 jsonschema (>=3.2.0) Requires-Dist: Deprecated (>=1.2.11) Requires-Dist:
@@ -17,15 +17,15 @@
 Requires-Dist: einops (==0.3.2) Requires-Dist: pycocotools (==2.0.6) Requires-
 Dist: protobuf (==3.20.3) Requires-Dist: treelib (==1.6.1) Requires-Dist:
 termcolor (==1.1.0) Requires-Dist: packaging (>=20.4) Requires-Dist: wheel
 (>=0.38.0) Requires-Dist: pygments (>=2.7.4) Requires-Dist: stringcase
 (>=1.2.0) Requires-Dist: numpy (<=1.23) Requires-Dist: rapidfuzz Requires-Dist:
 json-tricks (==3.16.1) Requires-Dist: onnx-simplifier (<1.0,>=0.3.6) Provides-
 Extra: pro Requires-Dist: deci-platform-client (>=5.0.0) ; extra == 'pro'
-               [docs/assets/SG_img/SG - Horizontal Glow 2.png]
+           [documentation/assets/SG_img/SG - Horizontal Glow 2.png]
 
    **Build, train, and fine-tune production-ready deep learning SOTA vision
           models** [![Tweet](https://img.shields.io/twitter/url/http/
            shields.io.svg?style=social)](https://twitter.com/intent/
                     tweet?text=Easily%20train%20or%20fine-
 tune%20SOTA%20computer%20vision%20models%20from%20one%20training%20repository&url=https:
                           //github.com/Deci-AI/super-
@@ -41,34 +41,34 @@
       [https://img.shields.io/badge/slack-community-blueviolet]_[https://
 img.shields.io/badge/license-Apache%202.0-blue]_[https://img.shields.io/badge/
                            docs-mkdocs-brightgreen]
 ______________________________________________________________________ ## Build
 with SuperGradients
 __________________________________________________________________________________________________________
 ### Support various computer vision tasks
-  [https://github.com/Deci-AI/super-gradients/raw/master/docs/assets/SG_img/
- Segmentation 1500x900 .png] [https://github.com/Deci-AI/super-gradients/raw/
- master/docs/assets/SG_img/Object detection 1500X900.png] [https://github.com/
-     Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Classification
-                                 1500x900.png]
+ [https://github.com/Deci-AI/super-gradients/raw/master/documentation/assets/
+SG_img/Segmentation 1500x900 .png] [https://github.com/Deci-AI/super-gradients/
+raw/master/documentation/assets/SG_img/Object detection 1500X900.png] [https://
+  github.com/Deci-AI/super-gradients/raw/master/documentation/assets/SG_img/
+                         Classification 1500x900.png]
 ### Ready to deploy pre-trained SOTA models YOLO-NAS architecture is out! The
 new YOLO-NAS delivers state-of-the-art performance with the unparalleled
 accuracy-speed performance, outperforming other models such as YOLOv5, YOLOv6,
 YOLOv7 and YOLOv8. Check it out here: [YOLO-NAS](YOLONAS.md).
              [./documentation/source/images/yolo_nas_frontier.png]
 ```python # Load model with pretrained weights from super_gradients.training
 import models from super_gradients.common.object_names import Models model =
 models.get(Models.YOLO_NAS_M, pretrained_weights="coco") ``` #### All Computer
 Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://
 bit.ly/41dkt89) #### Classification
-               [./docs/assets/SG_img/Classification@2xDark.png]
+           [./documentation/assets/SG_img/Classification@2xDark.png]
 #### Semantic Segmentation
-            [./docs/assets/SG_img/Semantic Segmentation@2xDark.png]
+       [./documentation/assets/SG_img/Semantic Segmentation@2xDark.png]
 #### Object Detection
-              [./docs/assets/SG_img/Object Detection@2xDark.png]
+          [./documentation/assets/SG_img/Object Detection@2xDark.png]
 ### Easy to train SOTA Models Easily load and fine-tune production-ready, pre-
 trained SOTA models that incorporate best practices and validated hyper-
 parameters for achieving best-in-class accuracy. For more information on how to
 do it go to [Getting Started](#getting-started) #### Plug and play recipes
 ```bash python -m super_gradients.train_from_recipe architecture=regnetY800
 dataset_interface.data_dir= ckpt_root_dir= ``` More example on how and why to
 use recipes can be found in [Recipes](#recipes) ### Production readiness All
```

## Comparing `super_gradients-3.1.2.dist-info/RECORD` & `super_gradients-3.1.3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-super_gradients/__init__.py,sha256=0AjXNZu1bTNLAS1rBwo-NMblkVGnsF5M5fWofoSoqh8,916
+super_gradients/__init__.py,sha256=8YgRwLVQyb2zFOcJmrg1HouDT799BsefbGTlfwGXP4c,916
 super_gradients/evaluate_checkpoint.py,sha256=cAB8pjlpxrpyJ2RhDp9jtV90TRvih7Axl0D2HVbfFKA,1657
 super_gradients/evaluate_from_recipe.py,sha256=aEUFWz0ue8tI55ChEivtABxUe7lhLCqT9aOywoenYfM,1807
 super_gradients/qat_from_recipe.py,sha256=AL7V8rS14iBwY3hH-BPXCwpa-Y1U1M3tCOy8o1yZnbY,639
 super_gradients/requirements.pro.txt,sha256=aYAzKlErZArFhx1DFYdxhMz3onw7QFKCy87VSfuEAT0,28
 super_gradients/requirements.txt,sha256=mvNAxH_Y4kSVvluGB_HaI7RFl_BvuH0mBbspC-DnQwI,729
 super_gradients/resume_experiment.py,sha256=VSmGBGaFOdz6hOTRkHm7un0MHolUk4_CvXfu2jtjGZM,537
 super_gradients/train_from_kd_recipe.py,sha256=OpRZsmleqXWQyFeaLzcnIooa_YEYEHFhkHr63Cs_QU8,693
 super_gradients/train_from_recipe.py,sha256=ZdCUpUlLPiCejcKff2FTfg33_TjZF0CwvZ-eaQlVyrA,650
 super_gradients/common/__init__.py,sha256=1F7pRDWoGs7wMWpbBw3iaTPWpeegxOroNPqUO3nzEMw,1098
-super_gradients/common/object_names.py,sha256=l6PvK87ZrPzyeAv9-kZY0dE0VIO8NOETcllT7or9-XY,15566
+super_gradients/common/object_names.py,sha256=X-V2uMpO4VCmfd54yX8O1xNbeaGdN0pURFcqYNcCOVM,15892
 super_gradients/common/abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/abstractions/abstract_logger.py,sha256=MpEjg7PihMZb_qLBKC-R58wWFqNJdPJMlOkxEU25hCU,879
-super_gradients/common/abstractions/mute_processes.py,sha256=JxC3ofVySoiL7U7x9QYhzWLVYArkgqKQB2Kp3HyPOyE,3129
+super_gradients/common/abstractions/mute_processes.py,sha256=Ve5n9L5fFK5qQbSiuN4rV0f0poZW-ndKJgPimvXs53c,3147
 super_gradients/common/auto_logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/auto_logging/auto_logger.py,sha256=WtlKaj5p8Ayx3gJ9XcRkuIG7oVicTs3K_X_gVeEfZOI,4846
 super_gradients/common/auto_logging/console_logging.py,sha256=PEPSfHQ8incS13dkM9gzlWBeRdwbodo9qVqRSk32s_E,6625
 super_gradients/common/aws_connection/__init__.py,sha256=cZCFSeQHk8E6TTZHTjnAhezGATF5iSKiFR2dBof8vqg,142
 super_gradients/common/aws_connection/aws_connector.py,sha256=2wHpTZubxc54tAqE5FaNIbC0LwtLFMkDS_rmx9x3XXg,4182
 super_gradients/common/aws_connection/aws_secrets_manager_connector.py,sha256=RUyDEx96sC4pGI3lH_z_Eo0dwP5QxZ0Qpy-ZFxQ6mz4,7198
 super_gradients/common/crash_handler/__init__.py,sha256=BWse71cn7bDfvpw52Rhpr0WtQyoxN9KmzEWX3w__ElE,119
@@ -43,15 +43,15 @@
 super_gradients/common/decorators/deci_logger.py,sha256=vyvodC1QCdLp_S05ELnBDnK1vCHBjtbvCsLRVnIdYHc,3663
 super_gradients/common/decorators/explicit_params_validator.py,sha256=EtW4ebI18tgPCBsA6v0Go3RY87iiqEEiQUQrujOb-y0,2921
 super_gradients/common/decorators/factory_decorator.py,sha256=PPHORVS_3fHGMqy7jbfTRwrHhDtXtHwWjR6hQe4J41s,1315
 super_gradients/common/decorators/singleton.py,sha256=6lVKPFSidDVRMOLeQ2YK-c7FRcxQEhrWU_AbuC7JXSc,1132
 super_gradients/common/environment/__init__.py,sha256=ljbYwQPDh8G0dCHjA6EGPSX5guFcsj-tUB6Ks0mHR-A,202
 super_gradients/common/environment/argparse_utils.py,sha256=c-XT11eDEZ42bWu2eKr4e6i30SF-OlM0a8xxgD08ob4,993
 super_gradients/common/environment/cfg_utils.py,sha256=_jUmcZ6HG7NK2R0H7edjNM62rDNzCTeRXBdAH2FFbq4,9170
-super_gradients/common/environment/checkpoints_dir_utils.py,sha256=0tYx8KMDRFINdpzEM7YZgXjJSzz8GzevGay3xD513sY,4383
+super_gradients/common/environment/checkpoints_dir_utils.py,sha256=xS7xQT8xJxHr8dbUuQFCotHLSD75pG3Ab_rhOtUZZX8,4398
 super_gradients/common/environment/ddp_utils.py,sha256=JMEzTKSrQ5pG9MGLd0xaIGIlg4Rlexh4soXhi0r6nzY,2682
 super_gradients/common/environment/device_utils.py,sha256=wV1pK5rjB4IShktrVdo9vx5mg_tF4XHIrRFssl2ftZA,752
 super_gradients/common/environment/env_variables.py,sha256=BHuwlhzAOxMxLvgWj616eOwEhnFvbliEdyrrDiYUA2Y,927
 super_gradients/common/environment/omegaconf_utils.py,sha256=ycjvwGWxhhnBUwWXljqcSw-IJ8UH1BW1E3AznUSNN60,4047
 super_gradients/common/environment/path_utils.py,sha256=p6fBTLBdxdpsALaD0lanM2jEtZcbSdthuEXSoOmgT5Q,459
 super_gradients/common/environment/monitoring/__init__.py,sha256=QmJWRpVWwHOK0qjNPV6PlA5ZzKjgumxNbSoYDnhUzzo,112
 super_gradients/common/environment/monitoring/cpu.py,sha256=eGHnEDbci_jku-RTzgROxt_kPy9bUdydk_bUMin3Kxc,153
@@ -61,15 +61,19 @@
 super_gradients/common/environment/monitoring/network.py,sha256=kfse7NZsOErzvkYmHKRbCP4g5hVW0ZNyZ0GbRTjtrw4,948
 super_gradients/common/environment/monitoring/utils.py,sha256=rqwSgOUjo6Ocxmh_u22pkQk3ol_CjUEX_eeqOcuyh3o,629
 super_gradients/common/environment/monitoring/virtual_memory.py,sha256=Pa2dh1okRqhQMWtQI9zkqWaE1JmMkAFJVw9RTa4KpFE,145
 super_gradients/common/environment/monitoring/gpu/__init__.py,sha256=rrflJdcOmbF5M-RFxjPROh_M9sAPICJ4UATkPXFafz8,681
 super_gradients/common/environment/monitoring/gpu/gpu.py,sha256=xFj5xTZrfBzmOKGrH7-dn62XqYyHHUotT2iA1hA14fE,2270
 super_gradients/common/environment/monitoring/gpu/pynvml.py,sha256=eoscxzudf5E8VE0VgiRB0l2i-Qxem60N17IvNFPQEFc,121647
 super_gradients/common/exceptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/common/exceptions/dataset_exceptions.py,sha256=csxJGdEunAi7XZAryqelr0NiZN5d4MxPFbZXklPyoDU,1761
 super_gradients/common/exceptions/factory_exceptions.py,sha256=67YRcabENWx_ZU9JounpU3_hZZyk_llaxEtASMTT62I,926
+super_gradients/common/exceptions/kd_trainer_exceptions.py,sha256=KD3rgit7YCxwoQPK7aamFVpOLEHhbLaQI8NsqIoVSFQ,2826
+super_gradients/common/exceptions/loss_exceptions.py,sha256=IOw4_QUfupjz1JkJXLQ_gGfzE60f5v7KInbAGw_IeA8,946
+super_gradients/common/exceptions/sg_trainer_exceptions.py,sha256=cGdofjAzqQmqH5QKpQP4-25JAIbakgQ9jv8uHTFS5bo,1268
 super_gradients/common/factories/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/factories/activations_type_factory.py,sha256=tDjG9H6tX2vT-qm4LdUMhhYMCxtJgbn5T3BcWhq9Oa0,1715
 super_gradients/common/factories/base_factory.py,sha256=sS8FMGsY2cQX2-irX8BUvcVEmOkfFcnXho7txNdUYdg,2881
 super_gradients/common/factories/bbox_format_factory.py,sha256=5IeX3wQ3WG3Jzr9iJXOhB7QCvuEGdMLKR6juDDeM14o,258
 super_gradients/common/factories/callbacks_factory.py,sha256=gbSYB4XX_672ujDF8swkGP-nTvaLWDxFu3CtaC7PiG4,232
 super_gradients/common/factories/collate_functions_factory.py,sha256=TtbwCeqTy1rY3u94Jg0zDk1bbFyMSkZU_V8ZDwRUatM,263
 super_gradients/common/factories/context_modules_factory.py,sha256=p3l8GWgmg6kTstZdS2y12YdqcJvoy4dsCPCnDdclu3Y,292
@@ -80,31 +84,33 @@
 super_gradients/common/factories/losses_factory.py,sha256=X0wM4QzKOszDVSUGLOgC01MALnREZFy12EKh3Jqc_yw,223
 super_gradients/common/factories/metrics_factory.py,sha256=yV5D5iHgcj2Q-a632zymQF7NnCwvOiYMVJnlbPQBslo,226
 super_gradients/common/factories/optimizers_type_factory.py,sha256=tIad1d-uYmT1glByXT-JXTkZpEygyk2zdb4ihiP7qVk,467
 super_gradients/common/factories/pre_launch_callbacks_factory.py,sha256=qjd2jvcn95jRNcmJRBa0IWnGSkxNPJf-Xn66j-4H6MY,271
 super_gradients/common/factories/processing_factory.py,sha256=t-IEuzn6SxR7gDLQQ_WMp8-zPiq7UCjlDuONTnplWpk,623
 super_gradients/common/factories/samplers_factory.py,sha256=pdsa9My_0aF63vBgHLQtzobw8-ykz-dFbDemMizJrdI,229
 super_gradients/common/factories/target_generator_factory.py,sha256=LZXQUxMI-jz_QPj0Bfi9FccLgX3Ky2MjU1llqxHFvOE,263
+super_gradients/common/factories/torch_schedulers_factory.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/factories/transforms_factory.py,sha256=TrwGexN9y33eAw0wQRFDgM5a26FKhCOzQvyC-fp2kfM,1873
 super_gradients/common/factories/type_factory.py,sha256=HwIiWskEfoHZiEkN8batqIxATs_20TJqq8qR9W0_Has,2377
 super_gradients/common/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/plugins/deci_client.py,sha256=88QA4_kEGwLwQkvPJa3N2R7WbVqRcoHHN6mywf_V7HI,12245
 super_gradients/common/plugins/wandb/__init__.py,sha256=J6rwLbKUtKgQIwYVJayBaXx0Tb77I7ZDE_5pEkQvFi4,143
-super_gradients/common/plugins/wandb/log_predictions.py,sha256=YiUKIYGsWfJxFaBLiZYITS0lYYEM_X3LXeawWD1EZvE,2329
+super_gradients/common/plugins/wandb/log_predictions.py,sha256=fkFP6AG_sQxFcqoovSAFcBdrSA7BPyemuSwzwVpyH-c,2317
 super_gradients/common/registry/__init__.py,sha256=gYkyLBFQN2kIgt0YFzGJl7lXKyOHBHE67B-1_C_JS8I,271
 super_gradients/common/registry/albumentation.py,sha256=MU7ZkXX-qSM5A_2l2apl6njJECwuUn4U1bo22yovOIY,1231
-super_gradients/common/registry/registry.py,sha256=XNgmvUY3kV3oF7i-yz4aZqyoM42EG4cV_mwS1EIyNFw,6006
+super_gradients/common/registry/registry.py,sha256=MS4WyQv3O5VOY0Z_pGeM-mSYJRxTqv9TCMSvqI71tUc,6634
 super_gradients/common/registry/registry_utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/common/sg_loggers/__init__.py,sha256=MJ9Gte7Zs_gGGge3zH7Tqv8iMm6Pic03YBHtrNqZUfc,508
-super_gradients/common/sg_loggers/abstract_sg_logger.py,sha256=t76j41J_a4Lt1ab7UyNkt_gsEJOuxaudnShKgDoPyyI,7460
-super_gradients/common/sg_loggers/base_sg_logger.py,sha256=ae331wSsQzJ4VTA97YqKa_C6lP5qzgTZL3dkMJ3UhcM,15095
-super_gradients/common/sg_loggers/clearml_sg_logger.py,sha256=BWAJzubNT974xgcsOVckRsU8KLsYW2NLJ5x65tCeQ6w,10055
-super_gradients/common/sg_loggers/dagshub_sg_logger.py,sha256=H0DJKzKQoL3ooXWvvx3fnidRTkuhTcL7tzQ5-mW9TaI,10103
+super_gradients/common/sg_loggers/__init__.py,sha256=B96-bFeweiNSHdyhS3xzBf7fwKvOKcVZEg8ZWqrWwMk,662
+super_gradients/common/sg_loggers/abstract_sg_logger.py,sha256=WAACGQrQT4o0UxmkkemvA21PW-Iu8ePdr3ctLuV0NFA,7544
+super_gradients/common/sg_loggers/base_sg_logger.py,sha256=wM1uUdl23FH8oZG26kB72-T1Wcp2_FXwVn87zasEWVs,15274
+super_gradients/common/sg_loggers/clearml_sg_logger.py,sha256=3garIr4_kdVPJcVseFVtMP9n2hnXNPKtF04UjfA2Tcw,10234
+super_gradients/common/sg_loggers/dagshub_sg_logger.py,sha256=3Gcz37OFyGQUOtz7Cq1_bO71OBC4ro9LAot87auXP8I,10277
 super_gradients/common/sg_loggers/deci_platform_sg_logger.py,sha256=XLanzH_CwW4Nw6Mx-m4tS6rFkDH3xZ9P8rCIyYIxoGs,6618
-super_gradients/common/sg_loggers/wandb_sg_logger.py,sha256=GHdZMjsM2FeZ72XQoE6DSb_9CPXNnMTUvE4s2wtMIOc,15000
+super_gradients/common/sg_loggers/time_units.py,sha256=DYYkVyZuLbBQZ_8ejzqtcglgegRaki8rMApqKDzbaAc,1104
+super_gradients/common/sg_loggers/wandb_sg_logger.py,sha256=2E4d27Ax8RMwPLa5UUPWZxIUwf6fhQo3koKO7zGdHTo,15242
 super_gradients/examples/SG_Walkthrough.ipynb,sha256=bhJ62ERSAchiroY49KiQiycgyDjlgPgHeXLwcZdUuNY,85509
 super_gradients/examples/SG_quickstart_classification.ipynb,sha256=aMGQCqFss-flEKvUaVj5WiKStr0S8TRKUsHwoyFcuko,69618
 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb,sha256=M9YZY9VpKJNFHxBz-IGSRvdAACQJ1n-wTQgWSpZVW78,54966
 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb,sha256=Gyx6LjKAwHwUdJsGiSiBn-AdbcgTdpD2DvRWB7IaGYk,65090
 super_gradients/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/cifar10_training_torch_objects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py,sha256=1tKhBpRwHWi4foJVVW1Ol3IlaJdJ2O3AGT3NKVsJr9k,2526
@@ -202,15 +208,15 @@
 super_gradients/recipes/imagenet_resnet50_kd.yaml,sha256=JuVQSpPYHuKfggQpdXXBEEKZhFMwBQf3W0ima5TO414,2722
 super_gradients/recipes/imagenet_vit_base.yaml,sha256=dnvr4h7-d1XHhF09Q9dZWoNLGZvdCZZys32siTH1Ta8,1136
 super_gradients/recipes/imagenet_vit_large.yaml,sha256=QuI6OVc5XAUcIUsOfnFpcO76jZ79HMhhwnk8Aq_azaU,1010
 super_gradients/recipes/roboflow_ppyoloe.yaml,sha256=ukl-e8Qze0hZ-ENcD93PTql5xaNHtcVIItzDJF3yGWI,2007
 super_gradients/recipes/roboflow_yolo_nas_m.yaml,sha256=qpOIQmV3mwelxK5Xn8RXPFhE6Cb2dlIPm42WlvP-eok,2347
 super_gradients/recipes/roboflow_yolo_nas_s.yaml,sha256=Gj1L8Ky92PcX8pQ5wKKgc353HGzJYun4xuoQkMgGfpk,2347
 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml,sha256=-zTGn37Y59d_9_z4HSsNfcEZ7eNr8j4Zi-VAv3-l3so,473
-super_gradients/recipes/roboflow_yolox.yaml,sha256=d6Y-nv_7p9SX63d8kJ1oiPS-U6Znu6DLye5IvIP9ypk,1915
+super_gradients/recipes/roboflow_yolox.yaml,sha256=nJ2Pq3m3R-DYGkgAFniAiAh0Od5xxa7YGQdPSlTg_hc,1917
 super_gradients/recipes/script_generate_rescoring_data_dekr_coco2017.yaml,sha256=D6OvC2Qz14mqHe3hfNHk4V8cfhG4f1h4u28eE5TwXkc,1344
 super_gradients/recipes/supervisely_unet.yaml,sha256=L1bl1QsgThj9iv5dEZSSGMBYFR1SmW9Mgr7cddaXOoE,1246
 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml,sha256=XR86Cg1sGjgoT8RHjdpnhJA01tFXYTz3QqiLYmLO46E,1672
 super_gradients/recipes/user_recipe_mnist_example.yaml,sha256=JtzZebnnTPGQUgsqu6i73zb5uF0l6_LPNnuh2q3UYD4,2133
 super_gradients/recipes/variable_setup.yaml,sha256=189UzdcCcHLw37-W1XF0W-j1k80IGMcMd8JkHwBXI9E,2000
 super_gradients/recipes/anchors/ssd_anchors.yaml,sha256=iRsfDXt3bWyCvmZtOQK-Y2maAJEgfgXVWF5sos6r7RU,2222
 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml,sha256=dEn_jgEn_NA80xaugB6lY1mdRRjVcOTwnckMlVmdbXE,563
@@ -224,15 +230,15 @@
 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml,sha256=QtyQb5EY_dUZydU94t39111d82vV5mAp4Wbq2JZlrKI,103
 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml,sha256=ALS6kf1BY3eBeFHTvoMVgp9ZVZ1vPXNgzTVn3scZEAo,103
 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml,sha256=AKCehy-NKiRXMCjmHs8u9-F4QtQGH7NxjTLtuvGybNU,103
 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml,sha256=aV7XQ9mFxZwsf2DHPuy3gJp2ScA2Z9wPHti4al341Co,194
 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml,sha256=NJe2vbIFbe9__tf1LuEMykNkHxF_5ofWNWMi4rsXSig,156
 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml,sha256=ky9f9lsQLJAcF0sUN-tYiZbMRpVIZAtwQTlrjPrpYpc,409
 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml,sha256=tAx0Wqeg0e0-rRjKPZyqB4Jvehe29u_ubJNX0cA3y6c,356
-super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml,sha256=0Ypq4caGTdodre32LZQz3970M-V_Wu06nmnABrKc8Uk,324
+super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml,sha256=fFIXV3JLBMu2ShXmAVY97XlLD0pu_X3Uee93Gsu5-Qw,323
 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml,sha256=PXIq_uMnPqfTa4IxfvhTFxYmaZEigFpFUAKBTxs0zqA,1113
 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml,sha256=qn1K7oUioAXHtNlg8gWqhkRWlXdF357eWSO8BhafJPY,985
 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml,sha256=l2jwsHzlQgb6mGMspWRMk2G0WA7VXVjSsioAVB_6rHU,1112
 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml,sha256=FzRo92_R5fXhHIbKYjKt_gcN97fl4sk4T-2SH6SVnaI,196
 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml,sha256=hTogCyoRf0tHU71NAxxW_lY1_6cK5dKBNra0pwnAlHM,198
 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml,sha256=KSbtJ6yeajB_PIvkGyCR6UFwXJB6VzH1NQbJa4m1EOM,198
 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml,sha256=wSVUpGaOQy74g9HqzHRqO0zOZIe4KkjzK-m9ocQcoM0,198
@@ -274,72 +280,74 @@
 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml,sha256=1NjXHAMg_znj2v-UHR57daxXpzLPvN3ZIMLKwsH5Zso,615
 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml,sha256=HUr8IaV0IIfuxK-fibY42yKUHe04kUCBFnYAE5E3rGI,525
 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml,sha256=CKSennwvRG1a-swVvL1he18vdtNRnCStH3LFhruGSnQ,706
 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml,sha256=dtbvoxt9IR9cBaslNOWCcsX7s_gjHRnWK5Ayl1ElzmI,644
 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml,sha256=i7l9LXea216Y2RB8e3FxhlGNBR_a1tLJKCg2Ix8JsTI,721
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml,sha256=WK7UH73r-nuHMKepBVyykR0tf306s-P5NgQNGI-dZWk,709
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml,sha256=wBHhYk6Q6kdmLDk9tTi0vpREr0fhTz4r1Zh0ybrRPGw,708
-super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml,sha256=x8wk7EC6eKGlxSyaBTxKGJidss5BbgX1MTG9KLCnU0M,3946
-super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml,sha256=GeCdBxnGf5WqQ165WIVCg4jz4vmjqT2LzofdvXB6bAs,4202
-super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml,sha256=PqQ6fBINO3sHHAAGx4rHKz4PAURkd67qPrVLWu1WM5Y,3590
-super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml,sha256=kbFd4bvfi8bhpX1qALfyjLZ3At9eHdC0J80w-a3OUkM,5568
-super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml,sha256=Nex5fWsHcmS5KJSkb32HNFaiXHVdovNKJMliXnLzg3U,3684
-super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml,sha256=T7GkJR2HFNeJYZzkHvAINP7ubHtN5xdhVNekPh4oZ84,2700
+super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml,sha256=nuwGWGB5WBpLuraALdBnwW9LRuzHMqBQl01ryGFRA04,3899
+super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml,sha256=rAtCkf_QT1a36XuUuA6wGiasN9a6iu4GBJvvwBJpkgM,4152
+super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml,sha256=VHkXaOymhV3QQgIFt9cBoKFlq_TjFBc4zaxuEaS8OMY,3517
+super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml,sha256=sgEDGTetpwQKy-GuAJpk2NMTcIVvl8H8vapxMkjv7iE,5521
+super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml,sha256=9ozbeoQueGfXCJRFZrBq5vKcsV4jCCkoNegb5TmcF0Q,3610
+super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml,sha256=sRYkQ9gIuqZxCviZQUfaFd_RgIx6Ikg85nwg2fBoADg,4073
 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml,sha256=q8s65W76DEu9XWRY_gR9fyr5Xp5HH1vLh8eG9ZvR7fA,405
-super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml,sha256=FOP_E-fLf3stEg8TNpDRfwLbWq_NvvVTXge6GcNyTeo,842
+super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml,sha256=eXdmcZA7fwXtNWLo194JI9piwD7I121T6AUCspKfvYQ,841
 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml,sha256=SC_nc2CyZqQ7R-z4pcqoTyZlBZB7JlmT_5hzgMjHCRc,1466
 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml,sha256=9JnbyZjCkZ3ZdMHj0CwVkQdzi7QBevwmoK1KQlxlymU,931
 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml,sha256=CILfhTGk4ne0wk0L7gbD95EjBTKGGTR8UjCaTW79Joc,732
 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml,sha256=lp64i0smov-lT6Xko9-fzVsxWO0UWdimXQnwrx0D3sY,794
 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml,sha256=YH7UxRgDjcR3qWs0yifxlgHsckHRqEYWx-kYRwNhPVo,142
 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml,sha256=Hf9BHIs4N2oRWpph7xr7x5AOZtBbV5eEaMOlShORjQg,734
 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml,sha256=SiPRDxzkwoOMDtKqzM7p0c5M658dQNEMQRvFH24K3aA,1059
 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml,sha256=C5-HGDjjDbnDWy43zM5byBmZicVqey-YQdoTkqKA7nw,1093
 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml,sha256=YvXeTTMlK8hEOu6HoedazdFtkk81icNHBg81yNGKmSw,845
 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml,sha256=mgexC2b4s-uabJsT2v51GdifhDg67WZfnexTMo-_NTY,1762
 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml,sha256=KzOrZe-NRkZ3XGkixGkUTA6Pd9aO2fTtnIhpaQOdIvU,149
-super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml,sha256=exEzH6LsS7KdvC975vG7TiA5byADG4YSfLUpCss58uI,1571
+super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml,sha256=9HVxBWFJlvljsHvcy25mpHL9H79ZVY4qIl_r_5NqEzY,1523
 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml,sha256=eIHwt4ZsVYKtpQbNSk1ZbsdneEZ6twlZkpxVG9LLt84,1414
-super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml,sha256=k9D4xbYMsuJv88r6m7MOeB3vQ37sUSnD94BQMMMExSM,4112
+super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml,sha256=zF1C1WOPYIufVkfCTH7uNdg7Cii1imt4Ey8-kWlmZn4,4016
 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml,sha256=GshRG6Jqdb1S9uoBjWbckkSajIPo6Avuf46WXFMcC5w,961
 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml,sha256=4_4HkNjzZDKFHpgSV1-S0s9rRrZJUj5S-7zUk1wOFaY,559
 super_gradients/recipes/quantization_params/default_quantization_params.yaml,sha256=OVewy7FMpSUpheoL7_eAzbJVpcfy5O2eIwpEri0tUc8,1155
 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml,sha256=jZV1VVe3Lda96Mq-hb8zHfR3EATHt0kSGLOpcdxssFg,591
 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml,sha256=NUOLRusDJ9H6Nxp-NGVsie7tPuRXKE493jwzI_U8rqE,700
 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml,sha256=JkLfCz7y-H0jOXzXvxHuqS--uFHfAj7ENwKLixblpmA,2063
 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml,sha256=Ah9iuCKngV2Bri_R0PPB-p5SB0oPpVYGs38yG83X-kU,1302
 super_gradients/recipes/training_hyperparams/coco2017_rescoring_train_params.yaml,sha256=EwmB6KWcfozUG885htJHZxlr9tbF5N_nBelFBESVQ0o,771
 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml,sha256=vuTXdVTzwM52w1n44mGBB-kJKluXtmxymgmbdLg85Jw,723
 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml,sha256=wjpqncCxlCxTg2zH30OoqqdctXYcoWz8nDOkD7DPTyM,1121
-super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml,sha256=hMDTZejrlTXQxuSJPXyW6jdxTrd5De5IoilzpP-Fmis,956
+super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml,sha256=nZfiQBBnPzECNJqbySE-K_G0HOdC05BpjbWqv8Otyw0,957
 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml,sha256=4k8cytIVPZH37ALyCqhziIA9i8HDrSwyvK1nrk1et8w,461
-super_gradients/recipes/training_hyperparams/default_train_params.yaml,sha256=iZclyubNwwIUwHeEeadZjvyZztDD1yCqqQEcrdm1ZdM,6081
+super_gradients/recipes/training_hyperparams/default_train_params.yaml,sha256=SOAsxf6clC0y6vLCKFqeQXfoQwRfq4WwPb7jk1G2Tas,7133
 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml,sha256=ueqNFnlvkCj78yA70mPDPp0n6AcikQkfCl35XLLE12c,794
 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml,sha256=xrCPTtKoJ85TjCART4sOLWMc7b5p2X2ZARt41WYScj0,742
 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml,sha256=xLXjLxQUyh6RJzBEtvrBPhKRAZre7OuVSZyAvErk3XA,549
 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml,sha256=A5j4hUflhQHwIPR8awxs64GuEH3AAFJbWT-Wo3g_nAs,795
 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml,sha256=XH-fzy5kx9HmMW6pA-0nmnWMxpcpdrIcTQ-Imyy8tsM,476
 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml,sha256=ebSVisdQvy4Shvzh95tKkXMD6VQkkrPLhBKuR-jOBVw,484
 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml,sha256=DO5N9jxrfn-jEoJS74JMghZB5ZN_nvLA3llRLe7NTLY,522
 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml,sha256=_-n1iLYFwhEDBxCnO8L5OTa8A5gKvVgTPC19g5wVx9A,602
 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml,sha256=NoLNnoAVy7-P7IJAymyPY7sjhiNuy973WHttv_Hh8eI,519
 super_gradients/sanity_check/__init__.py,sha256=IrTB1Lxw15cKFjxV8bGraUxj5d_pmEqYk7FHa01nuvk,107
 super_gradients/sanity_check/env_sanity_check.py,sha256=bq20O4wh04bPeRo1xv9-xDFaeU6_EOtXCd-PP7Fb9tc,5267
+super_gradients/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/scripts/find_detection_score_threshold.py,sha256=9e0N3doyjH9xpsCBNYdi1YvguEQVobZ-6PwiKSd5UIs,2310
 super_gradients/training/__init__.py,sha256=dBnpzi4Z1qNEMKpPhupeACBpSh6bXWoTwXyWn8cOC8I,775
-super_gradients/training/params.py,sha256=33QsbQo384OfUmKzA6x04Wf0cNJHiu-5yFcfG_rXzxQ,4715
+super_gradients/training/params.py,sha256=BIRare1whgmZArPsFXMVhtJmKE5EpLoxrJSRzBvYUsk,5513
 super_gradients/training/pretrained_models.py,sha256=GXfv3BW9msTEU_KZetZHDjHyxs3tQTtWXORG8TngBh8,4518
 super_gradients/training/dataloaders/__init__.py,sha256=AeUX5aLgSkFmOUGdwBe-JnBYoNc3dqT9h4ofK9dHvuw,3344
 super_gradients/training/dataloaders/dataloaders.py,sha256=Lgb6GmFyoRIJIHdDPtHfwNRFshUXXq3ySXDNbniD1NM,36154
 super_gradients/training/datasets/__init__.py,sha256=_8d9MmxGw3IFxOtZlbf7-ZYnlmyxpmZiTl9cbMyUNt0,1867
 super_gradients/training/datasets/auto_augment.py,sha256=VHw-Wq4ecHSKcqe9l63RUGpNa6JygUP3N7B6hbnTPxg,14162
 super_gradients/training/datasets/data_augmentation.py,sha256=TJOIT7j6ZWaNW6E4VvkJ-ARIWBY7Y4210NqrZbzKJJ8,3705
-super_gradients/training/datasets/datasets_conf.py,sha256=U2FTTYwCFp3cFZkzliWSGCHuCUUrns57AX7uS5Wn5NY,3484
+super_gradients/training/datasets/datasets_conf.py,sha256=_iavYqcoIfYQSzWkNE0djYtBNKCP-3_IHyBC5ogcq98,32184
 super_gradients/training/datasets/datasets_utils.py,sha256=FXaIOEoYEJ-eeWoh63kZRNwc6XdBs94JMAkDkCd9tns,29577
-super_gradients/training/datasets/mixup.py,sha256=WDHoqTFbq-PGemKxE0eZ10Q03mpH8GIj-vFBNIZEg1U,14663
-super_gradients/training/datasets/sg_dataset.py,sha256=xVqf-7vvGk96TkshGHIcqiQfIVXdOCs12U1fcJjWrX0,11746
+super_gradients/training/datasets/mixup.py,sha256=dvfQ86Coc3njWMx97fq2BHtO5vDQvWHEq0F9s5a28P0,14661
+super_gradients/training/datasets/sg_dataset.py,sha256=VshN3ZLxQEI_pbpPTtZUS5j4y8EAF91W_CwVixD5Xuk,11723
 super_gradients/training/datasets/classification_datasets/__init__.py,sha256=LcdaPeIQxwDM_qRb-sEwVswsjSveuZcdndpZKusGGsQ,252
 super_gradients/training/datasets/classification_datasets/cifar.py,sha256=lH_iBhC2igE_KQEJb_Lc1FpKvs4QsnuCxzOTIE0qNUw,3096
 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py,sha256=idY9fSwXxrgqJt9lJOaLFsQS0hz5qX6BIbXHBW_TIrU,1706
 super_gradients/training/datasets/data_formats/__init__.py,sha256=V2Sioujv6egladjkcsgceQ-goRUpja2Ey0ma-DDihWc,862
 super_gradients/training/datasets/data_formats/default_formats.py,sha256=GbP2UWXISbkfKtP7rjV2Qag3Q5BrlwU_RDzdM8DJuDk,3927
 super_gradients/training/datasets/data_formats/format_converter.py,sha256=yMJj-9REVJ_T-JkPB34IJsQzpxWOhhnlxxRNRhMUSqU,3071
 super_gradients/training/datasets/data_formats/formats.py,sha256=Aa3odNETBnS5_ZC3TcKOevqr89gw_qWZKZpS9Gb_wPo,7928
@@ -352,45 +360,40 @@
 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py,sha256=VhtZmqnW1cxeo1azP-zPNcMYMPCzc4ZBBokkFWioqPw,2948
 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py,sha256=nCCohobPvCOtQ_SF2BAyyVyuSV68ZjjxrUurGfwNXMs,575
 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py,sha256=LChhVCXQ9-d9Zp3sa_PzAOrUBa15f_QKtxHdW51ocwg,1792
 super_gradients/training/datasets/data_formats/output_adapters/__init__.py,sha256=n7aH5WQzk_awjpei_GY-yOktBTw7LtzekY-gHJ8_AKE,92
 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py,sha256=qH0LPewt8hvKE5jVaZl0HunzONd7UHErbBcCuK_rjZk,8373
 super_gradients/training/datasets/detection_datasets/__init__.py,sha256=g86eRhqJoDs-9snO7QR6zejTmqhF2Amq71O-ZZQLPZc,683
 super_gradients/training/datasets/detection_datasets/coco_detection.py,sha256=EUTVRS0igoBFeUDhXg_tqxJSDhGUEU45jdL8YYko2ng,2505
-super_gradients/training/datasets/detection_datasets/coco_format_detection.py,sha256=OJ0JEQLClxRgdMZlUpuVEH0jxRqwfTbhOZnHK4rzjuY,9258
-super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=9BG__DvgmOmHSR_vgF1A9uKoFMwcgpzZFTBi_svZiK8,26566
+super_gradients/training/datasets/detection_datasets/coco_format_detection.py,sha256=QGdvCdJkkg7FFBLahhW1DgkFQN-QJJck6Ob59zh5VVA,9258
+super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=XqeSlmAL4URto4JBWiKY8u-sBZW7oHawZossHopcJXE,26564
 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py,sha256=pAtuVBRVO_Y0Q-diaHQz3tWyjW7U3xR04ohzPx-vkbo,11353
-super_gradients/training/datasets/detection_datasets/yolo_format_detection.py,sha256=ZP8zw0vvQ5CK-RkZ7EOGaLyLCAAzjuEev34SJQYVxag,11120
+super_gradients/training/datasets/detection_datasets/yolo_format_detection.py,sha256=T97ZYyX_kTtZuoBYgc8hqD1_PIe2dW_QyTLszvWiOXU,11117
 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py,sha256=Kw_KF41iHBr9tHrg6I6T6gdy8fgKLlG0NLCtXOyNpEs,328
 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py,sha256=Ccxl7kt5F3E58oU4qJftnxIRaOc2iRyfCiyz_X4_lBc,18882
 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py,sha256=PkQ5CJdQ_jd9gYy4HcZTiODGbhH_IibXcNp_1k4cnAA,3503
 super_gradients/training/datasets/detection_datasets/roboflow/utils.py,sha256=_7mtuGnTHUVqfUqWlC9zpKGutBdaYJCGGj9pSbItfxI,1997
 super_gradients/training/datasets/pose_estimation_datasets/__init__.py,sha256=BeCVpXLn0FV9Oo_8iWtHz9n1GxdhXqTzymGT97_bdCA,502
-super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=6xNszBrqqOOdIKgM2ZFOZ4Crwssfh096_AcLZL5R1q4,4910
-super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=WK7FD6fV_iDZSjvH4REc-8ZJkSBtOQq2_Fwgw35nWlw,9088
+super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=iCM4E07i2xoEjQZDTk1UM4JxPnaqGv_0YTGBx2On_NY,6314
+super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=gT2pIJ7Hd5VBGIhB7N51QKOMZVw0KrIB_LqvGUgIBoc,10545
 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py,sha256=uMq0vV22npZqz21L_preyhbyKSHiBqS14Mp2UuEb-_4,5929
 super_gradients/training/datasets/pose_estimation_datasets/rescoring_dataset.py,sha256=uDZYe4yuDANJNN7IseXKAunYwqL7d73wvOhB9TBuxMk,3736
 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py,sha256=D7r0pXrv95zy_BFf9X-u26zsCaGuGcMQcVVPlus-eWM,10281
 super_gradients/training/datasets/samplers/__init__.py,sha256=bsLNxxZ61qQx2DbmGzsfd_6jDo4UYPkYNswoTOQtjrE,385
 super_gradients/training/datasets/samplers/infinite_sampler.py,sha256=ihUYmPJPKF0Z3lLdnQbGdlsB0jBmBxJvyySlXDbjyko,738
 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py,sha256=dnYh_2wWCFPlWVwnEhUEwhAaRpJGIGtoIbNiXSRAfq4,4809
 super_gradients/training/datasets/segmentation_datasets/__init__.py,sha256=JBkaU-0CwYInI7sdF_lbbFR8PPUFczMqF3Ose8wFaDo,1093
 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py,sha256=3hDw12hReFgaQelft0mXIhw70ccpnb-w1s4hMBSH9ho,8304
 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py,sha256=MqWN9UVMBcodqXm7LuC21MOazCsbBtL4ue7GXZgN80k,7757
 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py,sha256=DcRz59FNdX3koBCth09AT1EEHn77xXoxBX-yaWa-fmo,5518
 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py,sha256=uQJyztsrnSHbxvzitYqixVeNeXN52UYZ66L__Pkcgbc,11146
 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py,sha256=_nYIvWd9g0tyCg29t7UgN1LQvbpRj0VuOQcN0qQsg-g,8572
 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py,sha256=rG5w5hu0hqjzhhMutygfF9zegTM4nbUU-89St1F6Rh0,3062
-super_gradients/training/exceptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/exceptions/dataset_exceptions.py,sha256=csxJGdEunAi7XZAryqelr0NiZN5d4MxPFbZXklPyoDU,1761
-super_gradients/training/exceptions/kd_trainer_exceptions.py,sha256=KD3rgit7YCxwoQPK7aamFVpOLEHhbLaQI8NsqIoVSFQ,2826
-super_gradients/training/exceptions/loss_exceptions.py,sha256=IOw4_QUfupjz1JkJXLQ_gGfzE60f5v7KInbAGw_IeA8,946
-super_gradients/training/exceptions/sg_trainer_exceptions.py,sha256=cGdofjAzqQmqH5QKpQP4-25JAIbakgQ9jv8uHTFS5bo,1268
 super_gradients/training/kd_trainer/__init__.py,sha256=Ah4RhtFt2KzmN41c815uedwo7CyfBlX1zusR1w2LTEU,132
-super_gradients/training/kd_trainer/kd_trainer.py,sha256=DiobuDsXfaX4wY1Lj91H8opxlCFVDbgzsRgXfwnUu0Q,16582
+super_gradients/training/kd_trainer/kd_trainer.py,sha256=atsAD_koolw_5KeDygwBu-HpLKTy8I3ri0-CWlDA3sM,16599
 super_gradients/training/legacy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/legacy/utils.py,sha256=30Kcx8FOBARF_9y4K9Tue8aLUsv7HS0OrnIHL9-TV0Y,4198
 super_gradients/training/losses/__init__.py,sha256=ZH-dcE3zjpnMBj3_MOFx4DlYFmP_EEcLcPois6Krxiw,1570
 super_gradients/training/losses/all_losses.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/losses/bce_dice_loss.py,sha256=uBqTiQDgBCzd62lcZN_fLEmPOyuCbh9r6BYLlFiCPns,1219
 super_gradients/training/losses/bce_loss.py,sha256=F7oXzO08RJVjVfglKszaJ3j3CaqO2T6tVaSBdCgUFpw,419
 super_gradients/training/losses/cwd_loss.py,sha256=1jO8qdoGd9NKdZbWvc-2hAuN5Cn9U8Vk-3rIQt2bGj4,2374
@@ -400,85 +403,84 @@
 super_gradients/training/losses/dice_loss.py,sha256=hcVfl6Jrf0SKTDUf8dEWD15np99XU_I9yv9rR7G142I,5208
 super_gradients/training/losses/focal_loss.py,sha256=-mrmypTdwa5XcSCas-4Hk2wsc_oIaJjvhqY6FHyJ0Go,1214
 super_gradients/training/losses/iou_loss.py,sha256=ON_fJAatqVH4_XVNCrSd9gLNkYlPLEhizUPaJ9jwvT8,5051
 super_gradients/training/losses/kd_losses.py,sha256=-CGP7dWa1B-Ni2MnCQQLARRWxg5ajIUay81xQag-ZUI,2176
 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py,sha256=74uR2HNtiC7h59ywLCjb1NL_3DPtLuNHx3fcxHXGLcs,4177
 super_gradients/training/losses/loss_utils.py,sha256=E23MWbrXOsyF-DexK-tnCB2XyMajI0LHhtPXX9t1FT0,550
 super_gradients/training/losses/mask_loss.py,sha256=w7kxBZGHAXp3y-EB5FE6RKE1slxnYSvfIWpNJOQP1lg,4004
-super_gradients/training/losses/ohem_ce_loss.py,sha256=g-6Sltb2N_RBLyuWLBfFOWAQWeq7wrsMydoh9zOZX5w,4129
+super_gradients/training/losses/ohem_ce_loss.py,sha256=rg_yKWKitfuJQ3oUQVTLThFvCX3EcXPpS_meV5kYfTY,4127
 super_gradients/training/losses/ppyolo_loss.py,sha256=ZryjBfWsxxUPhmflYFfCh_Eq_DW68h0aD8hiR68ZGdA,41319
 super_gradients/training/losses/r_squared_loss.py,sha256=O1YCoeAwHTNNU2-qTLXlqE-hS2rro0DYaXkgtoDPmRA,1010
 super_gradients/training/losses/rescoring_loss.py,sha256=tmm3kNdBFRoEITEugq2wCW7EddXxBTQluTZqpr-SKqE,665
 super_gradients/training/losses/seg_kd_loss.py,sha256=IDUfzdaBpaOyhQFRSa4OZdmg_KYF2Mf1Xb65P6Qogjk,3453
 super_gradients/training/losses/shelfnet_ohem_loss.py,sha256=Qvova3DBVFpVjpho6Er79OSR61Jf_15yB0rU6L4ttM8,1650
 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py,sha256=o9kw_HPv8QZltQrVOJLdo4Q2G57lmxKsPGZySj5M7SA,1949
 super_gradients/training/losses/ssd_loss.py,sha256=Cou0Bqg0CzPq-d2zLocW7BkhKNB6xOq4FBJjk7cGlsc,8794
 super_gradients/training/losses/stdc_loss.py,sha256=l0TGotIYU3Ka4YnEl0xY1xtWOpZ5PC_8hOlvFUqjCyo,9721
 super_gradients/training/losses/structure_loss.py,sha256=w42pFyv69m7zrbnymPHFgOMvA30esbvn5FrGjWMG9F0,5771
 super_gradients/training/losses/yolox_loss.py,sha256=YvVIYTN6nl1PW5rH72u11O3gYVl8OMFbdeoFkk_mM2M,50149
 super_gradients/training/metrics/__init__.py,sha256=_EHNYpE89jPWTWQsODGYnzQEIlefbh5cvfdOIbWsGpU,1052
 super_gradients/training/metrics/all_metrics.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/metrics/classification_metrics.py,sha256=Zopby8WBumdoJxZLJv5YgL7W_ZQODN4hKs55UJKO_H0,3262
-super_gradients/training/metrics/detection_metrics.py,sha256=XXneeuIzFCMwQfiGQcZZCN9cWhD6v3Cj_25HJTZ93nE,10741
+super_gradients/training/metrics/detection_metrics.py,sha256=qYXkTktbDegRdn6zzvSOocGHKMs6X_wNS-_QgoPBl-U,16709
 super_gradients/training/metrics/metric_utils.py,sha256=WT1TmuARbVKDLhw4Z1rJt38JM6jnSLAqO6gJa8rKWWY,3973
-super_gradients/training/metrics/pose_estimation_metrics.py,sha256=SVsug8LaLfrDg7lX04MJnwqNe0Ym3z0V8QhHoDe1roQ,15404
+super_gradients/training/metrics/pose_estimation_metrics.py,sha256=xkMW6sb8GVL56HYA2SG287PGZHXbw-9qAnNwBCx4Pm4,15813
 super_gradients/training/metrics/pose_estimation_utils.py,sha256=GZnpT--sJUmdwmPPtS_JVslNp4mEx-G0p71N00OpiR0,11536
-super_gradients/training/metrics/segmentation_metrics.py,sha256=B24ivTj53cF2COHeyDutxGohDLYcFT_eiKEqXpjDMXk,11935
-super_gradients/training/models/__init__.py,sha256=ikB1pTl2acFGlntQk8AoTluVEQlZl4B5oOARA6htfn0,11245
+super_gradients/training/metrics/segmentation_metrics.py,sha256=9QzpDX3FQDKuyv2Ctb14B5WtNRQL8Cc7w2HNXUkE85I,19665
+super_gradients/training/models/__init__.py,sha256=DuATaoaRniuFtwmXgD9i0OrUmWsyd8CktNemAPJ3mSs,11309
 super_gradients/training/models/arch_params_factory.py,sha256=ufy6mCMPUm1b9s3wm-AVMIbX2irytPoZpeXELgtCROs,1226
 super_gradients/training/models/conversion.py,sha256=p5b6ioRN749Z5GlJE8azAjzlUMMv-Uc72VKRYgDGo44,12587
-super_gradients/training/models/model_factory.py,sha256=BJzz9K4rhFrmU7O0roix_0_VLbGuX3aQRqfrfqdgd48,11887
-super_gradients/training/models/prediction_results.py,sha256=TDsTihNB5pJgk0bTbvOo4cWNc4tkprtc_jwTr3SdK9Y,10997
-super_gradients/training/models/predictions.py,sha256=-i4fUfLThPPTpSPiyFj-3TS_MRQWwXwQm5QZG1GD754,2054
-super_gradients/training/models/results.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/training/models/model_factory.py,sha256=LxnG_WE8ztd_p89cwKV1KgP5c5pE1VSbj6ZtmAaYZ7U,12758
+super_gradients/training/models/predictions.py,sha256=I7o0G7OAAUHcDervYHQUFHL2ELE29NQ6IQFOeqto_fQ,366
 super_gradients/training/models/sg_module.py,sha256=JalNA0oIrW5IqV6Fl-SkAaq1qmcdLcAS8jx9QC84zMk,2998
 super_gradients/training/models/classification_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/training/models/classification_models/base_classifer.py,sha256=QP7KbkTHR692q20MpgD4hp3sdK5qYT4Ow8rTNjac5h4,3080
 super_gradients/training/models/classification_models/beit.py,sha256=kAq50cBeBteSF3uE3SW4TwYqfVn6edxPNXQEvOXc1Xg,20025
 super_gradients/training/models/classification_models/densenet.py,sha256=kDFzSB95Zk9OES501IiAyZmUlOnT03M3BEDaxlFONjM,7472
 super_gradients/training/models/classification_models/dpn.py,sha256=B5wPjPhPGp2PhTRxbC3w4VheCqVVs_8s9swqtwWnNKQ,3707
 super_gradients/training/models/classification_models/efficientnet.py,sha256=t9Rc9DveDC99iin-Xsv6UQ_Oy43SMOx3WjykTziqRgA,36745
 super_gradients/training/models/classification_models/googlenet.py,sha256=H57hvNMY7fqOV4v7Ezre-QVvawD1U9wuyAKUmpC1A4o,8862
 super_gradients/training/models/classification_models/lenet.py,sha256=uCaZPPVyfwyLfmD1KfoXiw05PvH-Ue4oa9Zczb_dHmg,798
 super_gradients/training/models/classification_models/mobilenet.py,sha256=JuABaCD_b6_Sh1EzigrBKqOniTTnI9RQ-a1V_YGaS6g,2407
 super_gradients/training/models/classification_models/mobilenetv2.py,sha256=V8FF_9Ibrn9LCf_4ybvQVKr5wVs1LEhpbXOff_XE0pY,9472
 super_gradients/training/models/classification_models/mobilenetv3.py,sha256=2aVzTJOufcdqthtSbjVHE7ViT3iaZcvvwTE9l-GiiKA,8696
 super_gradients/training/models/classification_models/pnasnet.py,sha256=DAo76uXefiCtOUTJ8uiuwAKSDN0nasSSOsCHg-sCkP0,4339
 super_gradients/training/models/classification_models/preact_resnet.py,sha256=24X4Zz00jj3Tj_l3BlLZOl-Z-dLJQ17mf7WKcpYcMtw,4209
-super_gradients/training/models/classification_models/regnet.py,sha256=TqBLs0lkE8yot9CEwtus16KPRHwn5X-HToqF9UGfU3A,13599
+super_gradients/training/models/classification_models/regnet.py,sha256=JZbzXs8j7soFBzO6WuW61JoYzJLRNBHWV5Z6DWwiWlg,13603
 super_gradients/training/models/classification_models/repvgg.py,sha256=gh9vB8y6ZUF8t-dUzxjy5_vpL8RMy6NbzYAYppL4ZoA,7924
-super_gradients/training/models/classification_models/resnet.py,sha256=nT1IgjRKRPibtIvyJSePYRWLd9esf-cPmP1HuYvIIGU,15067
+super_gradients/training/models/classification_models/resnet.py,sha256=mXV7LzcWldThm9wBNk09ZaVGq3AtMf_S9qLwUtLyKg0,15077
 super_gradients/training/models/classification_models/resnext.py,sha256=oK78roHfDVm0dZA88ZaLgx8ml9tQkvwU95kRGtfsyGI,6294
 super_gradients/training/models/classification_models/senet.py,sha256=QypzG-XPOvY7HzannhLaT2wtyDeLhT5PZReopJRqgAA,4134
 super_gradients/training/models/classification_models/shufflenet.py,sha256=-57ZOa75ul4eEUMi3fnNbEff2AJGCXJaXQ9npLzETa4,3660
 super_gradients/training/models/classification_models/shufflenetv2.py,sha256=hHMYew6ET-QV8bYhwyCfCoXwIGn1uAJjSyQ9F6EJ9Kw,9768
 super_gradients/training/models/classification_models/vgg.py,sha256=byU29VjwL79efNtIC_ETLXhBLSe8qn_4Wm2RJ4BQYlo,1538
 super_gradients/training/models/classification_models/vit.py,sha256=NwtBiuhcO8dFTXwRb7h66phGDyrQuztdAM_nO5--1UA,9210
 super_gradients/training/models/detection_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/detection_models/csp_darknet53.py,sha256=4EIj_ptbYiRu1hNYDPut9cQcUwetuVplpilj4sQHkpk,9130
-super_gradients/training/models/detection_models/csp_resnet.py,sha256=OVL-DXEWj7e5B873jujeKxYvhs7Nhy6ViXOcLDHr49E,9814
-super_gradients/training/models/detection_models/customizable_detector.py,sha256=MaE05_09QYoCGFJjitsqqxkSTrIxidAHgk2eqgCkc9o,9986
+super_gradients/training/models/detection_models/csp_resnet.py,sha256=223oBvq4jIQs8EYnRnXUe2RiByUStFB2C_jvgKZBd5U,9821
+super_gradients/training/models/detection_models/customizable_detector.py,sha256=KnO6rCLJM5bm-0AfozBtYWbcJpzjrXa94oBBvi0nPzo,10173
 super_gradients/training/models/detection_models/darknet53.py,sha256=FBFqJjU01A1l94HW7u7gCBmnRhSUvRVjlXZCsqyR4X8,4746
 super_gradients/training/models/detection_models/ssd.py,sha256=wvl6t3ltL6y5tjwqiFzBl8KmkwBOyUh07VS_7yVDfjs,2315
-super_gradients/training/models/detection_models/yolo_base.py,sha256=Uy0RPUc-8sQBRXdL4SANIJEkKu08awHLr8SWRRH-laQ,30262
+super_gradients/training/models/detection_models/yolo_base.py,sha256=FWxau6d9-OcMuOazKWh9_wXyTJUanMfXlN7Hs_FMPHs,32774
 super_gradients/training/models/detection_models/yolox.py,sha256=Wjz2H7NwX3j_YkUzLWMSmcDbnEqee59dCXLrd4jRJ-Q,2459
 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py,sha256=kdGGMgi8qmk8vjKKGVk5Ap46e1yjdNmtdQFALb8eiFo,251
 super_gradients/training/models/detection_models/pp_yolo_e/pan.py,sha256=zndJicizLwqjLdAtfWsKd2GnuPv2IoTf4YZW3wcjV1U,7000
-super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py,sha256=D4V9FAX5_VoxoPcwbuvYDtxaTfPRxFfvM5Ds0frO6js,3487
-super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=qr__SoXa4QNtBpX0x40byPmKzvTcygdFPI0pYMqpuD8,9023
-super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py,sha256=lSKZgvbXW2sD0Kd6ImzeOLN7d-kEiBjlB8dDsWc4cKM,12397
+super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py,sha256=U08C_CnWvpJFREYPqO2KjoDFTxZd6Z4SUgpbRliuROk,3889
+super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=A6kbFQyppEjNPf1EFiGTZv-Ezv7nI0mI0VnEjVCzoJw,9210
+super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py,sha256=eK_-CKn4h66x7usKyhvnc0UMPxpZzhlWIGgh3RLGp00,12404
 super_gradients/training/models/detection_models/yolo_nas/__init__.py,sha256=TJ9gQeZO8gmsZm0K-hyGxXyIZA8fwYuEaDheRMbXLUk,756
-super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py,sha256=P0TqYiqLgpQpJcaMeGIkT_A9jZrikQ6pVwxzzP_iTlI,12084
+super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py,sha256=7ryDl1xr6A2GTME7potrS-AwKPP_dM4M7uiJ-RLr5ic,12692
 super_gradients/training/models/detection_models/yolo_nas/panneck.py,sha256=qt0ChEAfmYU7Yc5Om7qQW4JMpRVQhMYW9hb-bLWsx2Q,2646
 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py,sha256=ZiIarpR5IavXvR7DgrFwzRD1bwx3U_qX7yvq5SB_RPs,4166
-super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py,sha256=yEPlfJoqCAHtFhKebaj89vIt2DMjM5VHg5zqaiX6-bo,13329
+super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py,sha256=WIZ9OJkniJDEPNPQfmfxTfrApE7bLrGHHT_DoH_kFEA,15510
 super_gradients/training/models/kd_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/kd_modules/kd_module.py,sha256=urOyHbsubq615UiGJo4-CAFpKvdKxHLrTFMzp1TlM5c,3553
 super_gradients/training/models/pose_estimation_models/__init__.py,sha256=MI9kzASiHp7WNv9_5JT_TdnHWzuYjHYzNlstf4QOv9M,179
-super_gradients/training/models/pose_estimation_models/dekr_hrnet.py,sha256=pNuaQHLz-bR90el2KscdrvOIc1B0DeUsUAA04ivVaso,23096
-super_gradients/training/models/pose_estimation_models/rescoring_net.py,sha256=KcAtuW4AWVNkXme_KYyZrtdM0u4tz63kGcW9R_3Rsxg,4298
+super_gradients/training/models/pose_estimation_models/dekr_hrnet.py,sha256=UwxZNdzIJCtwkh0n7klDgLzA_YgOERVcytuprlMZBFM,29151
+super_gradients/training/models/pose_estimation_models/rescoring_net.py,sha256=h9uIEzT0blJdk3XcufOgS5V2Vx-M3Tsmu0ZaNQ9hb3A,4286
 super_gradients/training/models/segmentation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/segmentation_models/common.py,sha256=58mVuAE3Hds_5f_5hr3a-ovHzYoGMslKBlwQRhl_5dY,964
 super_gradients/training/models/segmentation_models/context_modules.py,sha256=CcUiqpDPW2iyBuzzcpFGEYu50slxXenRrKdPVJ-zhTo,5139
 super_gradients/training/models/segmentation_models/ddrnet.py,sha256=3pSTLluvZnR2DMslt4t2GKRnbf2V1uihvdu27Ta-r_g,28514
 super_gradients/training/models/segmentation_models/ddrnet_backbones.py,sha256=tLHTnh590-QIg_Jyw87uLgGPt_yM2djx9pqilaAG7hk,2439
 super_gradients/training/models/segmentation_models/laddernet.py,sha256=aQAwG7h_AinfT6r-LvYqdzkWDzcKV0YqzQMNbRcOMmU,21760
 super_gradients/training/models/segmentation_models/ppliteseg.py,sha256=tuwPCaE8CyDU4OX0SqZyJ4B8JD377rOBC7Tgr8F20Qk,15648
@@ -489,79 +491,85 @@
 super_gradients/training/models/segmentation_models/stdc.py,sha256=rph_dQY3M-dvgPPkc7tpVIRC9w0RDZhLv6abDzggPRQ,29091
 super_gradients/training/models/segmentation_models/unet/__init__.py,sha256=WZp8BByl8QZpdPlnLwvW7QF5qfODj_-yo4UbtoScPng,260
 super_gradients/training/models/segmentation_models/unet/unet.py,sha256=x5Zu2Z7rw6i4LXyxcyxfL2uOzt3DuofWo7uKX_utTCw,12324
 super_gradients/training/models/segmentation_models/unet/unet_decoder.py,sha256=nqwXOlJkAddqNHBQOgaBIJQdPExMwNWZQrlEqUMP8ME,10718
 super_gradients/training/models/segmentation_models/unet/unet_encoder.py,sha256=auTtUn6jkKWUOdW_wKvOyKC9DpVSi7Y-LjoZY1POA3g,13292
 super_gradients/training/models/user_models/__init__.py,sha256=WNfXGheDVebPB3XmC9ce-wkyh0qXHRlINW43JIdnY6E,119
 super_gradients/training/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/pipelines/pipelines.py,sha256=_X3NBJ2xtklz3Wiyjl-rHWNww8Q6vOeMS-n1i0zLG2I,15639
+super_gradients/training/pipelines/pipelines.py,sha256=WEgrOxhEIkeygvDwztINeCKDlFLkJk7CmGfmN56D9To,23544
 super_gradients/training/pre_launch_callbacks/__init__.py,sha256=xL5z1cJdr_uGuNyBt8PHiQ8g7lwY3mZyYWwtnspQ-C0,445
-super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=vKkUAaRwsATmFc_B021a_ik3Lf4QO03rd8dphubI0iE,21020
+super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=0cZ3tiXu1RXCfCQmaW7wAON3BGs56hyvHUmIMDMr21w,21083
 super_gradients/training/processing/__init__.py,sha256=L_S3KapcujiBTXjHcMZxQz5aCwJM9Xxurbhs08oy0_o,517
-super_gradients/training/processing/processing.py,sha256=xx6q2nO2VXC-FGX4rYVp9Otbipbv43gToYepKe0jQyk,13177
+super_gradients/training/processing/processing.py,sha256=iaTsNOqmkijQV1vMjfg1D9pYkPnph-_N3cyFdhGBaJQ,20260
 super_gradients/training/qat_trainer/__init__.py,sha256=GZRdCf6P1Ximp-eoVw8kHv5Zb4AjBqxV0E2NwO1OmNo,98
 super_gradients/training/qat_trainer/qat_trainer.py,sha256=MoWilDaeWBj6CRQsmObIaB5K4QHIDA2uyWNgdnfGmW8,608
 super_gradients/training/sg_trainer/__init__.py,sha256=dug-p1erLN2SzYFQytJzPWDLOCmfvE94kFtcFLOTqj0,184
-super_gradients/training/sg_trainer/sg_trainer.py,sha256=4rMNageVk4D3zP67Irl6IUmvBwHDQ7PlaB-qoChwGDM,116430
+super_gradients/training/sg_trainer/sg_trainer.py,sha256=VRZrz3KF_xb4Dx6E9524zMeJzdMKNjMGxuTCySWK4LY,123049
 super_gradients/training/training_hyperparams/__init__.py,sha256=R5pvZNSQgDNxRp23qAlAAhGdPT7u_e78QiztqQDqosc,1685
 super_gradients/training/training_hyperparams/training_hyperparams.py,sha256=pZIOz9L6vf-tgCMUbvf2WLch1zCCfDevhfYPnL3QR7A,3774
 super_gradients/training/transforms/__init__.py,sha256=SMLfPEp8zqooiV6mB4byOzk5SprUUo77LIUNgTTB7A8,1024
 super_gradients/training/transforms/all_transforms.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/transforms/keypoint_transforms.py,sha256=-lTR8tHtWGmK6THZvyI52OpH5yhWXDGJeUJM_FwcZhE,16193
+super_gradients/training/transforms/keypoint_transforms.py,sha256=F0KNprt2sbCDKgHpQadm4fjqxNTodHauMb94lEL49tg,20123
 super_gradients/training/transforms/pipeline_adaptors.py,sha256=ukVHjcx-XaCEGZ3I_afIb9Uj73vwYtkmgrLJw9jr7oU,1134
-super_gradients/training/transforms/transforms.py,sha256=nqOwUZzuWhFVLO43e_eBk5m46IFxZHNVshtmhCCpbkM,55587
-super_gradients/training/transforms/utils.py,sha256=WkgT9-2hZm7IBS_HZzy1kOE0EOb-k0t8gypuPhpC5Z4,6048
-super_gradients/training/utils/__init__.py,sha256=ygVj0ne8ck50XC4PvBrSANZB4QwBBRV6OtNVC_ppsMQ,1179
+super_gradients/training/transforms/transforms.py,sha256=XgsITQEj7l63lawIPMYPMpfYWTErRe5pawx9CKGCUFk,57393
+super_gradients/training/transforms/utils.py,sha256=NqTKooEMKt-6ikiqFLQKlLdvFx0PYhWBsqQ23ELKvsU,7307
+super_gradients/training/utils/__init__.py,sha256=PRAfje4nXrlMLV9MtyaHVF5CS8FpxTM4F4CdkdUM8fw,1141
 super_gradients/training/utils/activations_utils.py,sha256=LNgR7SUWOehjBbvtHvU8PtgazsbxX9ztvIUNAQ4nB64,1673
 super_gradients/training/utils/bbox_utils.py,sha256=tvDIJ5TkShshteJAzXVtQZaZFMtIHrYS98U5bpcc0sU,1111
-super_gradients/training/utils/checkpoint_utils.py,sha256=J4N5jXb37w-JCTGoEYNkx79ZWi5r45KMjHaGYpRrk3U,15712
+super_gradients/training/utils/checkpoint_utils.py,sha256=5vzz765siYTXyPWLcQa-udQDIz7xRa5YxZ_6A8sNeY4,16205
 super_gradients/training/utils/config_utils.py,sha256=jDS_SaRfIEvAXzPB5ZerzVtKaDxD8mgKesUI4M2ERdo,9794
 super_gradients/training/utils/deprecated_utils.py,sha256=YtKScFu62sn2IDBtzC2cPmdSFQ_UfeQZ3CrPDuOZpO4,1132
-super_gradients/training/utils/detection_utils.py,sha256=cAsBoQ5fsCN1hZMBgxs4rG-axC5lp47xdrnoC1PiaJA,53289
+super_gradients/training/utils/detection_utils.py,sha256=sidj0J_2m0SwPYiAFA9F5cmn11RnOFG15m-UaxO7K-4,60150
 super_gradients/training/utils/distributed_training_utils.py,sha256=1hUkc_OE3CCvBtcWlUsGbB8kmgjAUWtgXFJs9QORX-I,16195
 super_gradients/training/utils/early_stopping.py,sha256=FGv-bFT6N1WrtEmZ2Q0xmmijmOI_IKoTvxQcua0LK9g,6352
-super_gradients/training/utils/ema.py,sha256=xPjihYYtpKqrOth0KoRyTeFarCTEH-AVnh0J9M767PM,9322
+super_gradients/training/utils/ema.py,sha256=sMgbv48xoyGIl-aFc_3FR3BQBoN6iff3T7mpfTkb0Qk,9304
 super_gradients/training/utils/ema_decay_schedules.py,sha256=lV9zLoVvfPPWJajPpNBnkn8d5ahLJIAjHtv3rZsDU1E,2610
 super_gradients/training/utils/export_utils.py,sha256=Ci9yz8OiK0oVEBHaG74-YuPqBANciWpFf17w-IVYvRc,1072
 super_gradients/training/utils/get_model_stats.py,sha256=nMKVdVxsLPSKDXD7qnTWk60f0B3F1-Ct-XdZchFbsJM,7508
 super_gradients/training/utils/kd_trainer_utils.py,sha256=j-RWPU7_0rKX-4Cf9RiyGk3GuH6j7_cGeBLKYhuXYOk,771
 super_gradients/training/utils/load_image.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/utils/optimizer_utils.py,sha256=tB-M7Iv9SqRMyzTpk_5tL1gNTk7tpeVPRyEhI_5tqY0,5827
-super_gradients/training/utils/regularization_utils.py,sha256=apNkV4g-9-mA0m6aSGVz6M5Y6MisplfmcdkYwDnFIyA,839
+super_gradients/training/utils/optimizer_utils.py,sha256=YdkzmvGRcnuomZXvzgpNYZ5mKMnnw_8XC81Q5HSL11I,6120
+super_gradients/training/utils/regularization_utils.py,sha256=SJAArT-MNDhAlV98DxUA9kDjHmpDCuEGTETXYPCpZqA,1833
 super_gradients/training/utils/segmentation_utils.py,sha256=otlxMRGq63cNsSj39lTQtNLyDvM9UrU7LVPlHHYxbRI,10388
-super_gradients/training/utils/sg_trainer_utils.py,sha256=wnH6njXa_0eENF9QpznsYi81lfUrOLzbBqaOVAbSd50,19625
-super_gradients/training/utils/ssd_utils.py,sha256=n31g0sdpHM96PWJGrJlXK5EGMb0t1nRgAE5sI17XXM4,6272
-super_gradients/training/utils/utils.py,sha256=LLQ_W5d3sNaUY01q92-C368SUPBMwvv_CARpCSjile8,20438
+super_gradients/training/utils/sg_trainer_utils.py,sha256=2LW2ATLqO29cFYkKhg7HUE-IfVE0BfPL_ujHdVJMeYA,19713
+super_gradients/training/utils/ssd_utils.py,sha256=e0gB7OEEtQP3RZX61jCNsb9rAwI5WhggQPFatHoI1CQ,6423
+super_gradients/training/utils/utils.py,sha256=XZzPy-SOb2fJ6WJK8ZOgmfjLVe2w75lmfhGx8ZzdDlw,21363
 super_gradients/training/utils/version_utils.py,sha256=lzIg-vB-ok6tF2HfzFNkIEpq1XB3_cVqoaaNikGR1PE,303
-super_gradients/training/utils/weight_averaging_utils.py,sha256=3e5RpP8vasmEiY1ZJP5stbSFEbq97wbRJj89rwB4dfE,5687
-super_gradients/training/utils/callbacks/__init__.py,sha256=IW4hEmiLvmSqcvYMQn6D0e8qcI-avUnHUcMI8Mv9gvg,2030
+super_gradients/training/utils/weight_averaging_utils.py,sha256=jB_IlDXQMDBOoHOoWe5PmIOmc5tNWnjPeixy2PoT84Q,5628
+super_gradients/training/utils/callbacks/__init__.py,sha256=7ofGR4uuZAEbrwA6P_dY1x2WkI2I86_iHkOXeUROF3k,2024
 super_gradients/training/utils/callbacks/all_callbacks.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/utils/callbacks/base_callbacks.py,sha256=pCMNK9iUQm8jqSAm5elZrG9Oy3AYD62L-_qj8e9du8U,20126
-super_gradients/training/utils/callbacks/callbacks.py,sha256=0jrto6bqX5yMxb92mhHWsAplhtjXGRiJRgkRVkYK-zc,33409
+super_gradients/training/utils/callbacks/base_callbacks.py,sha256=i-MIQ-UmsHAfTJg81nbfiWK0a-_VlKSfPP8G0xp1Myc,20007
+super_gradients/training/utils/callbacks/callbacks.py,sha256=U1aS51bLqg8jPHlvhrbVk4k8icsjkmN6UpK0qa_00CU,42787
 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py,sha256=7-EaXO3ipczQw9H6NIGqZ-3cR3n-ZN6oAEcnCsv-VtE,1169
 super_gradients/training/utils/media/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/utils/media/image.py,sha256=CZ6_K-yifXXNqGe3grp1e5hl-Ug_0lFUGH5CIm_1Glo,5880
+super_gradients/training/utils/media/image.py,sha256=i8eb4yqioFzAHjeXLDOcwjDiU-9Vj9n_GEd09gwvrfM,5894
 super_gradients/training/utils/media/stream.py,sha256=wgVafnzRXnZvSxaiquNXUC6PqSMlLI4A6YS6_b4A04Y,4046
 super_gradients/training/utils/media/video.py,sha256=DC9xdQX5g2JCWalBeHAGh3VWtvBRvxOs3dIgIuqURtw,6926
 super_gradients/training/utils/optimizers/__init__.py,sha256=Z-kZTiqwHe-KFYP0BTFsX0TNms8-CfRrc6iKEfewopM,396
 super_gradients/training/utils/optimizers/all_optimizers.py,sha256=9oPneh_UFmDWb-NWBKWa3X7EaYTVN8KYxc_LE7D2n94,422
 super_gradients/training/utils/optimizers/lamb.py,sha256=zdvmfKHGen7_rwMohoEs6DOSDEH95ELFCKezD1fN1v0,9760
 super_gradients/training/utils/optimizers/lion.py,sha256=ivMkwLg0vpOyfD4h226wScYXYDwTdCh0o_zkOeyrdcs,3008
 super_gradients/training/utils/optimizers/rmsprop_tf.py,sha256=5gzx0uy3x4c8G8UgfDnOTLjASwT1enBAcfUkgzrOOJU,6834
 super_gradients/training/utils/pose_estimation/__init__.py,sha256=-gXj3fMnEXjfmj_3NCeMtEsddOMSSxVzXWA72Slh5tw,324
-super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py,sha256=6p4vxEx1mqP_ziGUR22foG1Bb5_9H0P9yFJV97iCLFo,11309
+super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py,sha256=pnahdzQSZbriaMl7GTxOcCVESQD-F1B393pPkoHNr2M,13624
 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py,sha256=HEdNaksgnzoXh1RWRvB5rd_tniZWkk6Ro-6D2-Abv1Q,7140
 super_gradients/training/utils/pose_estimation/rescoring_callback.py,sha256=kwWbyJ6C6hY8G072gSYqUh0uGB7K3bM-heIDwIU0KyA,920
+super_gradients/training/utils/predict/__init__.py,sha256=HUW02effjP3DSNgguKHRpkD_jba7LP7UdR8nQ_dh9jk,1012
+super_gradients/training/utils/predict/prediction_pose_estimation_results.py,sha256=eDDKHHiUuU0fcxM0Z_SxPJ5DCEq6S-JFg8kGHsTsrb4,14550
+super_gradients/training/utils/predict/prediction_results.py,sha256=kzwcpA4E_vjk5NyPGvj592LoZPrDZ9rtDygeYQ65fzg,13944
+super_gradients/training/utils/predict/predictions.py,sha256=FAr5ZpyGrj00oajB62HYBz5XRMH8s0PUqHXAI64-OYg,5263
 super_gradients/training/utils/quantization/__init__.py,sha256=FsLDGZR4MT_1tTIcnyOhIqUTfCf178tU7Y72och-Fws,387
 super_gradients/training/utils/quantization/calibrator.py,sha256=vfXnyPxLdHjk5e5CF3-lBwofRDjX-ZCyDaRreuu6_h4,6271
 super_gradients/training/utils/quantization/core.py,sha256=CYykLasziH9YT0h_utxWj6WZ6tXi4KUSKaiBf1N2YZM,8417
 super_gradients/training/utils/quantization/export.py,sha256=EpP1RQ--B2YnleMv54cpGURpv_MpbOx-CKPjfspSVF0,2504
 super_gradients/training/utils/quantization/selective_quantization_utils.py,sha256=hQ8uZliyAK21pguj0aSybxINffXrj0R2YCHCWIRV7Z4,17062
 super_gradients/training/utils/visualization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/training/utils/visualization/classification.py,sha256=zOfC5dmLDmdpTTYIk5W1uQ8bEoXC1ZnrDcEvJk-iW5o,1647
 super_gradients/training/utils/visualization/detection.py,sha256=348rm6aggC_RLn9Zsnr9FC0AJu5zieHVhTzQGJs6sfk,1698
+super_gradients/training/utils/visualization/pose_estimation.py,sha256=uZMmRpmtnwoCOlfHPyGGg3Iwb2g5qCTiJ8QYEiqpJ1Y,2684
 super_gradients/training/utils/visualization/utils.py,sha256=LXh2fmdauApUJEn62a0yEXwKQ6G1ySlWvqkK9Ap8ybU,2847
-super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
-super_gradients-3.1.2.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
-super_gradients-3.1.2.dist-info/METADATA,sha256=1E7tnIGPTD38zi6t2ghWa6xHwXZ9_oUWEjvtANEILkQ,35552
-super_gradients-3.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-super_gradients-3.1.2.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
-super_gradients-3.1.2.dist-info/RECORD,,
+super_gradients-3.1.3.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
+super_gradients-3.1.3.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
+super_gradients-3.1.3.dist-info/METADATA,sha256=w40sZN_jzIHk7a2pVzdq2vSR8P4RNXiUhTZ21kL7Low,35723
+super_gradients-3.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+super_gradients-3.1.3.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
+super_gradients-3.1.3.dist-info/RECORD,,
```

