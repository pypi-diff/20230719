# Comparing `tmp/syne_tune-0.9.0.tar.gz` & `tmp/syne_tune-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syne_tune-0.9.0.tar", last modified: Tue Jul  4 10:02:50 2023, max compression
+gzip compressed data, was "syne_tune-0.9.1.tar", last modified: Wed Jul 19 13:22:38 2023, max compression
```

## Comparing `syne_tune-0.9.0.tar` & `syne_tune-0.9.1.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.236537 syne_tune-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-04 10:02:41.000000 syne_tune-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 10:02:41.000000 syne_tune-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 10:02:41.000000 syne_tune-0.9.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-04 10:02:50.236537 syne_tune-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-07-04 10:02:41.000000 syne_tune-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 10:02:50.236537 syne_tune-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-04 10:02:41.000000 syne_tune-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/local_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/python_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/python_backend/python_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/python_backend/python_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/custom_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/backend/simulator_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/simulator_backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/trial_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/backend/trial_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/blackbox_repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/blackbox_repository/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/callbacks/tensorboard_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/config_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/baselines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/nas201.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/yahpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/default_baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/experiment_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/launchers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/experiments/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/aggregate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/multiobjective.py
--rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/plot_per_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    36795 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/experiments/visualization/results_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/num_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.216537 syne_tune-0.9.0/syne_tune/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45677 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_rush.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/random_seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/ray_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.220537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.224537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.228537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    42228 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31125 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.232537 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.236537 syne_tune-0.9.0/syne_tune/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/remote_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/remote_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/remote_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/remote/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/results_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/tuner_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/tuning_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.236537 syne_tune-0.9.0/syne_tune/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/config_as_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/utils/parse_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 10:02:41.000000 syne_tune-0.9.0/syne_tune/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:02:50.212537 syne_tune-0.9.0/syne_tune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 10:02:50.000000 syne_tune-0.9.0/syne_tune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.958582 syne_tune-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-19 13:22:25.000000 syne_tune-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 13:22:25.000000 syne_tune-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 13:22:25.000000 syne_tune-0.9.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-19 13:22:38.958582 syne_tune-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22427 2023-07-19 13:22:25.000000 syne_tune-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 13:22:38.958582 syne_tune-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-19 13:22:25.000000 syne_tune-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.930580 syne_tune-0.9.1/syne_tune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.930580 syne_tune-0.9.1/syne_tune/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/local_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.930580 syne_tune-0.9.1/syne_tune/backend/python_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/python_backend/python_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/python_backend/python_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.930580 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/custom_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.930580 syne_tune-0.9.1/syne_tune/backend/simulator_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/simulator_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/simulator_backend/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/simulator_backend/simulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/simulator_backend/simulator_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/simulator_backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/trial_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/backend/trial_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/blackbox_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/simulated_tabular_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/blackbox_repository/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/callbacks/remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/callbacks/tensorboard_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/config_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/baselines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/nas201.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/yahpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/default_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/experiment_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.934580 syne_tune-0.9.1/syne_tune/experiments/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/launchers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.938580 syne_tune-0.9.1/syne_tune/experiments/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/visualization/aggregate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/visualization/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/visualization/plot_per_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36795 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/visualization/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/experiments/visualization/results_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/num_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.938580 syne_tune-0.9.1/syne_tune/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45677 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.938580 syne_tune-0.9.1/syne_tune/optimizer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_pasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/median_stopping_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.938580 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/moasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.942581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/random_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/ray_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/remove_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/scheduler_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.942581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.942581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.942581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.946581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.946581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.946581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.946581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.946581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/constrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.950581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42228 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31125 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/dehb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.954581 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.958582 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.958582 syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/simple_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.958582 syne_tune-0.9.1/syne_tune/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/remote_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/remote_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/remote_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/remote/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/results_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/tuner_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/tuning_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.958582 syne_tune-0.9.1/syne_tune/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/utils/config_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/utils/parse_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 13:22:25.000000 syne_tune-0.9.1/syne_tune/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:22:38.930580 syne_tune-0.9.1/syne_tune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-19 13:22:38.000000 syne_tune-0.9.1/syne_tune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-07-19 13:22:38.000000 syne_tune-0.9.1/syne_tune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:22:38.000000 syne_tune-0.9.1/syne_tune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-19 13:22:38.000000 syne_tune-0.9.1/syne_tune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 13:22:38.000000 syne_tune-0.9.1/syne_tune.egg-info/top_level.txt
```

### Comparing `syne_tune-0.9.0/LICENSE` & `syne_tune-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/PKG-INFO` & `syne_tune-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne_tune
-Version: 0.9.0
+Version: 0.9.1
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,14 +20,15 @@
 Provides-Extra: blackbox-repository
 Provides-Extra: benchmarks
 Provides-Extra: yahpo
 Provides-Extra: raytune
 Provides-Extra: botorch
 Provides-Extra: bore
 Provides-Extra: extra
+Provides-Extra: basic
 License-File: LICENSE
 License-File: NOTICE
 
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -37,39 +38,49 @@
 [![codecov.io](https://codecov.io/github/awslabs/syne-tune/branch/main/graphs/badge.svg)](https://app.codecov.io/gh/awslabs/syne-tune)
 
 ![Syne Tune](docs/source/synetune.gif)
 
 **[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)** | **[Tutorials](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)** | **[API Reference](https://syne-tune.readthedocs.io/en/latest/_apidoc/modules.html#)** | **[PyPI](https://pypi.org/project/syne-tune)** | **[Latest Blog Post](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/)**
 
 Syne Tune provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
+* **Lightweight and platform-agnostic**: Syne Tune is designed to work with
+  different execution backends, so you are not locked into a particular
+  distributed system architecture. Syne Tune runs with minimal dependencies.
+* **Wide coverage of different HPO methods**: Syne Tune supports more than 20 different optimization methods across [multi-fidelity HPO](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html), [constrained HPO](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/basics_outlook.html#further-topics), [multi-objective HPO](https://syne-tune.readthedocs.io/en/latest/getting_started.html#supported-multi-objective-optimization-methods), [transfer learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html), [cost-aware HPO](https://syne-tune.readthedocs.io/en/latest/_apidoc/syne_tune.optimizer.schedulers.searchers.cost_aware.html), and [population-based training](https://syne-tune.readthedocs.io/en/latest/_apidoc/syne_tune.optimizer.schedulers.pbt.html).
+* **Simple, modular design**: Rather than wrapping other HPO
+  frameworks, Syne Tune provides simple APIs and scheduler templates, which can
+  easily be [extended to your specific needs](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html).
+  Studying the code will allow you to understand what the different algorithms
+  are doing, and how they differ from each other.
+* **Industry-strength Bayesian optimization**: Syne Tune has comprehensive support
+  for [Gaussian Process-based Bayesian optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/basics_bayesopt.html).
+  The same code powers modalities such as multi-fidelity HPO, constrained HPO, and
+  cost-aware HPO, and has been tried and tested in production for several years.
+* **Support for distributed workloads**: Syne Tune lets you move fast, thanks to the parallel compute resources AWS SageMaker offers. Syne Tune allows ML/AI practitioners to easily set up and run studies with many [experiments running in parallel](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html). Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
+* **Out-of-the-box tabulated benchmarks:** Tabulated benchmarks let you simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
+
+
+Syne Tune is developed in collaboration with the team behind the [Automatic Model Tuning](https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning.html) service.
 
-* Wide coverage (>20) of different HPO methods, including:
-  * Asynchronous and distributed tuning (i.e., with multiple workers);
-  * Multi-fidelity methods supporting model-based decisions (BOHB and MOBSTER);
-  * Transfer learning to speed up (repeated) tuning jobs;
-  * Multi-objective optimizers that can tune multiple objectives simultaneously (such as accuracy and latency).
-* Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
-* Out-of-the-box tabulated benchmarks allow you to simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
 
 ## Installing
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
 ```
 
-or to install the latest version from source (necessary to run the scripts in the [examples/](https://github.com/awslabs/syne-tune/tree/main/examples) folder): 
+or to install the latest version from source: 
 
 ```bash
 git clone https://github.com/awslabs/syne-tune.git
 cd syne-tune
 python3 -m venv st_venv
 . st_venv/bin/activate
-pip install wheel
 pip install --upgrade pip
 pip install -e '.[extra]'
 ```
 
 This installs everything in a virtual environment `st_venv`. Remember to activate
 this environment before working with Syne Tune. We also recommend building the
 virtual environment from scratch now and then, in particular when you pull a new
@@ -165,26 +176,30 @@
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
 HyperTune | Li, et al. (2022) | model-based | yes | yes | no
-DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
+DyHPO<sup>*</sup> | Wistuba, et al. (2022) | model-based | yes | yes | no
 ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no
 ASHACQR | Salinas, et al. (2023) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
 RUSH | Zappella, et al. (2021)| random | yes | yes | yes 
 BoundingBox | Perrone, et al. (2019) | any | yes | yes | yes
 
+<sup>*</sup>: We implement the model-based scheduling logic of DyHPO, but use
+the same Gaussian process surrogate models as MOBSTER and HyperTune. The original
+source code for the paper is [here](https://github.com/releaunifreiburg/DyHPO/tree/main).
+
 The searchers fall into four broad categories, **deterministic**, **random**, **evolutionary** and **model-based**. The random searchers sample candidate hyperparameter configurations uniformly at random, while the model-based searchers sample them non-uniformly at random, according to a model (e.g., Gaussian process, density ration estimator, etc.) and an acquisition function. The evolutionary searchers make use of an evolutionary algorithm.
 
 Syne Tune also supports [BoTorch](https://github.com/awslabs/syne-tune/blob/main/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py) searchers.
 
 ## Supported multi-objective optimization methods
 
 Method |          Reference          |   Searcher   | Asynchronous? | Multi-fidelity? | Transfer?
@@ -239,15 +254,15 @@
   launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
   scheduler
 
 ## Examples for Experimentation and Benchmarking
 
 You will find many examples for experimentation and benchmarking in
 [benchmarking/examples/](benchmarking/examples/) and in
-benchmarking/nusery/](benchmarking/nursery/).
+[benchmarking/nusery/](benchmarking/nursery/).
 
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
@@ -294,17 +309,21 @@
 * [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
 * [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
 * [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
 * [Distributed Hyperparameter Tuning: Finding the Right Model can be Fast and Fun](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html)
 
 ## Blog Posts
 
-- [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
-- [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
-- [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
+* [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
+* [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
+* [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
+
+## Videos
+
+* [Martin Wistuba: Hyperparameter Optimization for the Impatient (PyData 2023)](https://www.youtube.com/watch?v=onX6fXzp9Yk)
 
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## Citing Syne Tune
```

### Comparing `syne_tune-0.9.0/README.md` & `syne_tune-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,39 +8,49 @@
 [![codecov.io](https://codecov.io/github/awslabs/syne-tune/branch/main/graphs/badge.svg)](https://app.codecov.io/gh/awslabs/syne-tune)
 
 ![Syne Tune](docs/source/synetune.gif)
 
 **[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)** | **[Tutorials](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)** | **[API Reference](https://syne-tune.readthedocs.io/en/latest/_apidoc/modules.html#)** | **[PyPI](https://pypi.org/project/syne-tune)** | **[Latest Blog Post](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/)**
 
 Syne Tune provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
+* **Lightweight and platform-agnostic**: Syne Tune is designed to work with
+  different execution backends, so you are not locked into a particular
+  distributed system architecture. Syne Tune runs with minimal dependencies.
+* **Wide coverage of different HPO methods**: Syne Tune supports more than 20 different optimization methods across [multi-fidelity HPO](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html), [constrained HPO](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/basics_outlook.html#further-topics), [multi-objective HPO](https://syne-tune.readthedocs.io/en/latest/getting_started.html#supported-multi-objective-optimization-methods), [transfer learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html), [cost-aware HPO](https://syne-tune.readthedocs.io/en/latest/_apidoc/syne_tune.optimizer.schedulers.searchers.cost_aware.html), and [population-based training](https://syne-tune.readthedocs.io/en/latest/_apidoc/syne_tune.optimizer.schedulers.pbt.html).
+* **Simple, modular design**: Rather than wrapping other HPO
+  frameworks, Syne Tune provides simple APIs and scheduler templates, which can
+  easily be [extended to your specific needs](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html).
+  Studying the code will allow you to understand what the different algorithms
+  are doing, and how they differ from each other.
+* **Industry-strength Bayesian optimization**: Syne Tune has comprehensive support
+  for [Gaussian Process-based Bayesian optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/basics_bayesopt.html).
+  The same code powers modalities such as multi-fidelity HPO, constrained HPO, and
+  cost-aware HPO, and has been tried and tested in production for several years.
+* **Support for distributed workloads**: Syne Tune lets you move fast, thanks to the parallel compute resources AWS SageMaker offers. Syne Tune allows ML/AI practitioners to easily set up and run studies with many [experiments running in parallel](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html). Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
+* **Out-of-the-box tabulated benchmarks:** Tabulated benchmarks let you simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
+
+
+Syne Tune is developed in collaboration with the team behind the [Automatic Model Tuning](https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning.html) service.
 
-* Wide coverage (>20) of different HPO methods, including:
-  * Asynchronous and distributed tuning (i.e., with multiple workers);
-  * Multi-fidelity methods supporting model-based decisions (BOHB and MOBSTER);
-  * Transfer learning to speed up (repeated) tuning jobs;
-  * Multi-objective optimizers that can tune multiple objectives simultaneously (such as accuracy and latency).
-* Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
-* Out-of-the-box tabulated benchmarks allow you to simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
 
 ## Installing
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
 ```
 
-or to install the latest version from source (necessary to run the scripts in the [examples/](https://github.com/awslabs/syne-tune/tree/main/examples) folder): 
+or to install the latest version from source: 
 
 ```bash
 git clone https://github.com/awslabs/syne-tune.git
 cd syne-tune
 python3 -m venv st_venv
 . st_venv/bin/activate
-pip install wheel
 pip install --upgrade pip
 pip install -e '.[extra]'
 ```
 
 This installs everything in a virtual environment `st_venv`. Remember to activate
 this environment before working with Syne Tune. We also recommend building the
 virtual environment from scratch now and then, in particular when you pull a new
@@ -136,26 +146,30 @@
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
 HyperTune | Li, et al. (2022) | model-based | yes | yes | no
-DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
+DyHPO<sup>*</sup> | Wistuba, et al. (2022) | model-based | yes | yes | no
 ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no
 ASHACQR | Salinas, et al. (2023) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
 RUSH | Zappella, et al. (2021)| random | yes | yes | yes 
 BoundingBox | Perrone, et al. (2019) | any | yes | yes | yes
 
+<sup>*</sup>: We implement the model-based scheduling logic of DyHPO, but use
+the same Gaussian process surrogate models as MOBSTER and HyperTune. The original
+source code for the paper is [here](https://github.com/releaunifreiburg/DyHPO/tree/main).
+
 The searchers fall into four broad categories, **deterministic**, **random**, **evolutionary** and **model-based**. The random searchers sample candidate hyperparameter configurations uniformly at random, while the model-based searchers sample them non-uniformly at random, according to a model (e.g., Gaussian process, density ration estimator, etc.) and an acquisition function. The evolutionary searchers make use of an evolutionary algorithm.
 
 Syne Tune also supports [BoTorch](https://github.com/awslabs/syne-tune/blob/main/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py) searchers.
 
 ## Supported multi-objective optimization methods
 
 Method |          Reference          |   Searcher   | Asynchronous? | Multi-fidelity? | Transfer?
@@ -210,15 +224,15 @@
   launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
   scheduler
 
 ## Examples for Experimentation and Benchmarking
 
 You will find many examples for experimentation and benchmarking in
 [benchmarking/examples/](benchmarking/examples/) and in
-benchmarking/nusery/](benchmarking/nursery/).
+[benchmarking/nusery/](benchmarking/nursery/).
 
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
@@ -265,17 +279,21 @@
 * [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
 * [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
 * [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
 * [Distributed Hyperparameter Tuning: Finding the Right Model can be Fast and Fun](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html)
 
 ## Blog Posts
 
-- [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
-- [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
-- [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
+* [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
+* [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
+* [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
+
+## Videos
+
+* [Martin Wistuba: Hyperparameter Optimization for the Impatient (PyData 2023)](https://www.youtube.com/watch?v=onX6fXzp9Yk)
 
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## Citing Syne Tune
```

### Comparing `syne_tune-0.9.0/setup.py` & `syne_tune-0.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # gluon-ts is not added as the git dependency does not work with setup.py
     k = "git+https://github.com/awslabs/gluon-ts.git"
     if k in res:
         res.remove(k)
     return list(res)
 
 
+long_description = (Path(__file__).parent / "README.md").read_text()
+
 required_core = load_requirements("requirements.txt")
 required_ray = load_requirements("requirements-ray.txt")
 required_gpsearchers = load_requirements("requirements-gpsearchers.txt")
 required_bore = load_requirements("requirements-bore.txt")
 required_botorch = load_requirements("requirements-botorch.txt")
 required_kde = load_requirements("requirements-kde.txt")
 required_blackbox_repository = load_requirements(
@@ -38,15 +40,14 @@
 required_benchmarks = load_benchmark_requirements()
 required_dev = load_requirements("requirements-dev.txt")
 required_aws = load_requirements("requirements-aws.txt")
 required_moo = load_requirements("requirements-moo.txt")
 required_visual = load_requirements("requirements-visual.txt")
 required_sklearn = load_requirements("requirements-sklearn.txt")
 
-long_description = (Path(__file__).parent / "README.md").read_text()
 required_extra = (
     required_gpsearchers
     + required_kde
     + required_dev
     + required_aws
     + required_moo
     + required_visual
@@ -57,14 +58,18 @@
     + required_ray
 )
 
 # Botorch only supports python version >= 3.8
 if sys.version_info >= (3, 8):
     required_extra += required_botorch
 
+required_basic = (
+    required_gpsearchers + required_kde + required_aws + required_moo + required_sklearn
+)
+
 setup(
     name="syne_tune",
     version=read_version(),
     description="Distributed Hyperparameter Optimization on SageMaker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="AWS",
@@ -85,14 +90,15 @@
         "blackbox-repository": required_blackbox_repository,
         "benchmarks": required_benchmarks,
         "yahpo": required_yahpo,
         "raytune": required_ray,
         "botorch": required_botorch,
         "bore": required_bore,
         "extra": required_extra,
+        "basic": required_basic,
     },
     install_requires=required_core,
     include_package_data=True,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `syne_tune-0.9.0/syne_tune/__init__.py` & `syne_tune-0.9.1/syne_tune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/__init__.py` & `syne_tune-0.9.1/syne_tune/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/local_backend.py` & `syne_tune-0.9.1/syne_tune/backend/local_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/python_backend/__init__.py` & `syne_tune-0.9.1/syne_tune/backend/python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/python_backend/python_backend.py` & `syne_tune-0.9.1/syne_tune/backend/python_backend/python_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/python_backend/python_entrypoint.py` & `syne_tune-0.9.1/syne_tune/backend/python_backend/python_entrypoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/__init__.py` & `syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/custom_framework.py` & `syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/custom_framework.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv` & `syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/instance-types-cost.csv`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/instance_info.py` & `syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/instance_info.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py` & `syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py` & `syne_tune-0.9.1/syne_tune/backend/sagemaker_backend/sagemaker_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/simulator_backend/__init__.py` & `syne_tune-0.9.1/syne_tune/backend/simulator_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/simulator_backend/events.py` & `syne_tune-0.9.1/syne_tune/backend/simulator_backend/events.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_backend.py` & `syne_tune-0.9.1/syne_tune/backend/simulator_backend/simulator_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/simulator_backend/simulator_callback.py` & `syne_tune-0.9.1/syne_tune/backend/simulator_backend/simulator_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/simulator_backend/time_keeper.py` & `syne_tune-0.9.1/syne_tune/backend/simulator_backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/time_keeper.py` & `syne_tune-0.9.1/syne_tune/backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/trial_backend.py` & `syne_tune-0.9.1/syne_tune/backend/trial_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/backend/trial_status.py` & `syne_tune-0.9.1/syne_tune/backend/trial_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/__init__.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_offline.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox_offline.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_surrogate.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox_surrogate.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/blackbox_tabular.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/blackbox_tabular.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/recipes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/conversion_scripts/utils.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/conversion_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/repository.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/repository.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/serialize.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/serialize.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/simulated_tabular_backend.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/simulated_tabular_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/blackbox_repository/utils.py` & `syne_tune-0.9.1/syne_tune/blackbox_repository/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/callbacks/__init__.py` & `syne_tune-0.9.1/syne_tune/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py` & `syne_tune-0.9.1/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py` & `syne_tune-0.9.1/syne_tune/callbacks/hyperband_remove_checkpoints_score.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/callbacks/remove_checkpoints_callback.py` & `syne_tune-0.9.1/syne_tune/callbacks/remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/callbacks/tensorboard_callback.py` & `syne_tune-0.9.1/syne_tune/callbacks/tensorboard_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/config_space.py` & `syne_tune-0.9.1/syne_tune/config_space.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/constants.py` & `syne_tune-0.9.1/syne_tune/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/__init__.py` & `syne_tune-0.9.1/syne_tune/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/baselines.py` & `syne_tune-0.9.1/syne_tune/experiments/baselines.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/__init__.py` & `syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/common.py` & `syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/fcnet.py` & `syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/fcnet.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/lcbench.py` & `syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/nas201.py` & `syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/nas201.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/benchmark_definitions/yahpo.py` & `syne_tune-0.9.1/syne_tune/experiments/benchmark_definitions/yahpo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/default_baselines.py` & `syne_tune-0.9.1/syne_tune/experiments/default_baselines.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/experiment_result.py` & `syne_tune-0.9.1/syne_tune/experiments/experiment_result.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/__init__.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_common.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_local.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_local.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_sagemaker.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_sagemaker.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/hpo_main_simulator.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/hpo_main_simulator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_common.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_local.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_local.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_sagemaker.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_sagemaker.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/launch_remote_simulator.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/launch_remote_simulator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/launchers/utils.py` & `syne_tune-0.9.1/syne_tune/experiments/launchers/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/visualization/__init__.py` & `syne_tune-0.9.1/syne_tune/experiments/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/visualization/aggregate_results.py` & `syne_tune-0.9.1/syne_tune/experiments/visualization/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/visualization/multiobjective.py` & `syne_tune-0.9.1/syne_tune/experiments/visualization/multiobjective.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/visualization/plot_per_trial.py` & `syne_tune-0.9.1/syne_tune/experiments/visualization/plot_per_trial.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/visualization/plotting.py` & `syne_tune-0.9.1/syne_tune/experiments/visualization/plotting.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/experiments/visualization/results_utils.py` & `syne_tune-0.9.1/syne_tune/experiments/visualization/results_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/num_gpu.py` & `syne_tune-0.9.1/syne_tune/num_gpu.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/baselines.py` & `syne_tune-0.9.1/syne_tune/optimizer/baselines.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/scheduler.py` & `syne_tune-0.9.1/syne_tune/optimizer/scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/fifo.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/fifo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_pasha.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_pasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_promotion.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_rush.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/hyperband_stopping.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/median_stopping_rule.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/median_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multi_fidelity.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/moasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/multiobjective/utils.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/multiobjective/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/networks.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/networks.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/neuralband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/pbt.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/pbt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/random_seeds.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/random_seeds.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/ray_scheduler.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/ray_scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/remove_checkpoints.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/remove_checkpoints.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/scheduler_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/scheduler_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/de.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/de.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/common.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/dehb.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/__init__.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/simple_profiler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/optimizer/schedulers/utils/successive_halving.py` & `syne_tune-0.9.1/syne_tune/optimizer/schedulers/utils/successive_halving.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/__init__.py` & `syne_tune-0.9.1/syne_tune/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/constants.py` & `syne_tune-0.9.1/syne_tune/remote/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/estimators.py` & `syne_tune-0.9.1/syne_tune/remote/estimators.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/remote_launcher.py` & `syne_tune-0.9.1/syne_tune/remote/remote_launcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/remote_main.py` & `syne_tune-0.9.1/syne_tune/remote/remote_main.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/remote_metrics_callback.py` & `syne_tune-0.9.1/syne_tune/remote/remote_metrics_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/remote/scheduling.py` & `syne_tune-0.9.1/syne_tune/remote/scheduling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/report.py` & `syne_tune-0.9.1/syne_tune/report.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/results_callback.py` & `syne_tune-0.9.1/syne_tune/results_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/stopping_criterion.py` & `syne_tune-0.9.1/syne_tune/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/try_import.py` & `syne_tune-0.9.1/syne_tune/try_import.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,64 +21,75 @@
 
 def try_import_kde_message() -> str:
     return _try_import_message("KDE searchers are not imported", tag="kde")
 
 
 def try_import_bore_message() -> str:
     return _try_import_message(
-        "BORE searchers are not imported (not contained in extra)", tag="bore"
+        "BORE searchers are not imported (not contained in extra)",
+        tag="bore",
+        recommend_extra=True,
     )
 
 
 def try_import_raytune_message() -> str:
     return _try_import_message(
-        "Ray Tune schedulers and searchers are not imported", tag="raytune"
+        "Ray Tune schedulers and searchers are not imported",
+        tag="raytune",
+        recommend_extra=True,
     )
 
 
 def try_import_benchmarks_message() -> str:
     return _try_import_message(
-        "Dependencies for benchmarks are not imported", tag="benchmarks"
+        "Dependencies for benchmarks are not imported",
+        tag="benchmarks",
+        recommend_extra=True,
     )
 
 
 def try_import_aws_message() -> str:
     return _try_import_message("AWS dependencies are not imported", tag="aws")
 
 
 def try_import_botorch_message() -> str:
     return _try_import_message(
         "BoTorch dependencies are not imported (needs Python 3.8 or later)",
         tag="botorch",
+        recommend_extra=True,
     )
 
 
 def try_import_blackbox_repository_message() -> str:
     return _try_import_message(
         "Dependencies of blackbox repository are not imported",
         tag="blackbox-repository",
+        recommend_extra=True,
     )
 
 
 def try_import_yahpo_message() -> str:
     return _try_import_message(
         "Dependencies of YAHPO are not imported",
         tag="yahpo",
+        recommend_extra=True,
     )
 
 
 def try_import_moo_message() -> str:
     return _try_import_message(
         "Multi Objective Optimization dependencies are not imported", tag="moo"
     )
 
 
 def try_import_visual_message() -> str:
     return _try_import_message(
-        "Dependencies for visualization are not imported", tag="visual"
+        "Dependencies for visualization are not imported",
+        tag="visual",
+        recommend_extra=True,
     )
 
 
 def try_import_sklearn_message() -> str:
     return _try_import_message(
         "Dependencies for scikit-learn are not imported", tag="sklearn"
     )
@@ -86,19 +97,27 @@
 
 def try_import_backends_message() -> str:
     return _try_import_message(
         "LocalBackend / PythonBackend are not imported", tag=None
     )
 
 
-def _try_import_message(message_text: str, tag: Optional[str]) -> str:
+def _try_import_message(
+    message_text: str, tag: Optional[str], recommend_extra: bool = False
+) -> str:
     if tag is None:
         insert = ""
     else:
         insert = "[" + tag + "]"
+    if recommend_extra:
+        full_tag = "extra"
+        before_everything = ""
+    else:
+        full_tag = "basic"
+        before_everything = "almost "
     return (
         message_text
         + " since dependencies are missing. You can install them with\n"
         + f"   pip install 'syne-tune{insert}'\n"
-        + "or (for everything)\n"
-        + "   pip install 'syne-tune[extra]'"
+        + f"or (for {before_everything}everything)\n"
+        + f"   pip install 'syne-tune[{full_tag}]'"
     )
```

### Comparing `syne_tune-0.9.0/syne_tune/tuner.py` & `syne_tune-0.9.1/syne_tune/tuner.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/tuner_callback.py` & `syne_tune-0.9.1/syne_tune/tuner_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/tuning_status.py` & `syne_tune-0.9.1/syne_tune/tuning_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/util.py` & `syne_tune-0.9.1/syne_tune/util.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/utils/__init__.py` & `syne_tune-0.9.1/syne_tune/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/utils/checkpoint.py` & `syne_tune-0.9.1/syne_tune/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/utils/config_as_json.py` & `syne_tune-0.9.1/syne_tune/utils/config_as_json.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune/utils/parse_bool.py` & `syne_tune-0.9.1/syne_tune/utils/parse_bool.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune.egg-info/PKG-INFO` & `syne_tune-0.9.1/syne_tune.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne-tune
-Version: 0.9.0
+Version: 0.9.1
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,14 +20,15 @@
 Provides-Extra: blackbox-repository
 Provides-Extra: benchmarks
 Provides-Extra: yahpo
 Provides-Extra: raytune
 Provides-Extra: botorch
 Provides-Extra: bore
 Provides-Extra: extra
+Provides-Extra: basic
 License-File: LICENSE
 License-File: NOTICE
 
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -37,39 +38,49 @@
 [![codecov.io](https://codecov.io/github/awslabs/syne-tune/branch/main/graphs/badge.svg)](https://app.codecov.io/gh/awslabs/syne-tune)
 
 ![Syne Tune](docs/source/synetune.gif)
 
 **[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)** | **[Tutorials](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)** | **[API Reference](https://syne-tune.readthedocs.io/en/latest/_apidoc/modules.html#)** | **[PyPI](https://pypi.org/project/syne-tune)** | **[Latest Blog Post](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/)**
 
 Syne Tune provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
+* **Lightweight and platform-agnostic**: Syne Tune is designed to work with
+  different execution backends, so you are not locked into a particular
+  distributed system architecture. Syne Tune runs with minimal dependencies.
+* **Wide coverage of different HPO methods**: Syne Tune supports more than 20 different optimization methods across [multi-fidelity HPO](https://syne-tune.readthedocs.io/en/latest/tutorials/multifidelity/README.html), [constrained HPO](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/basics_outlook.html#further-topics), [multi-objective HPO](https://syne-tune.readthedocs.io/en/latest/getting_started.html#supported-multi-objective-optimization-methods), [transfer learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html), [cost-aware HPO](https://syne-tune.readthedocs.io/en/latest/_apidoc/syne_tune.optimizer.schedulers.searchers.cost_aware.html), and [population-based training](https://syne-tune.readthedocs.io/en/latest/_apidoc/syne_tune.optimizer.schedulers.pbt.html).
+* **Simple, modular design**: Rather than wrapping other HPO
+  frameworks, Syne Tune provides simple APIs and scheduler templates, which can
+  easily be [extended to your specific needs](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html).
+  Studying the code will allow you to understand what the different algorithms
+  are doing, and how they differ from each other.
+* **Industry-strength Bayesian optimization**: Syne Tune has comprehensive support
+  for [Gaussian Process-based Bayesian optimization](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/basics_bayesopt.html).
+  The same code powers modalities such as multi-fidelity HPO, constrained HPO, and
+  cost-aware HPO, and has been tried and tested in production for several years.
+* **Support for distributed workloads**: Syne Tune lets you move fast, thanks to the parallel compute resources AWS SageMaker offers. Syne Tune allows ML/AI practitioners to easily set up and run studies with many [experiments running in parallel](https://syne-tune.readthedocs.io/en/latest/tutorials/experimentation/README.html). Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
+* **Out-of-the-box tabulated benchmarks:** Tabulated benchmarks let you simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
+
+
+Syne Tune is developed in collaboration with the team behind the [Automatic Model Tuning](https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning.html) service.
 
-* Wide coverage (>20) of different HPO methods, including:
-  * Asynchronous and distributed tuning (i.e., with multiple workers);
-  * Multi-fidelity methods supporting model-based decisions (BOHB and MOBSTER);
-  * Transfer learning to speed up (repeated) tuning jobs;
-  * Multi-objective optimizers that can tune multiple objectives simultaneously (such as accuracy and latency).
-* Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
-* Out-of-the-box tabulated benchmarks allow you to simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
 
 ## Installing
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
 ```
 
-or to install the latest version from source (necessary to run the scripts in the [examples/](https://github.com/awslabs/syne-tune/tree/main/examples) folder): 
+or to install the latest version from source: 
 
 ```bash
 git clone https://github.com/awslabs/syne-tune.git
 cd syne-tune
 python3 -m venv st_venv
 . st_venv/bin/activate
-pip install wheel
 pip install --upgrade pip
 pip install -e '.[extra]'
 ```
 
 This installs everything in a virtual environment `st_venv`. Remember to activate
 this environment before working with Syne Tune. We also recommend building the
 virtual environment from scratch now and then, in particular when you pull a new
@@ -165,26 +176,30 @@
 SyncBOHB | Falkner, et al. (2018) | model-based | no | yes | no 
 SyncMOBSTER | Klein, et al. (2020) | model-based | no | yes | no 
 ASHA | Li, et al. (2019) | random | yes | yes | no 
 BOHB | Falkner, et al. (2018) | model-based | yes | yes | no 
 MOBSTER | Klein, et al. (2020) | model-based | yes | yes | no 
 DEHB | Awad, et al. (2021) | evolutionary | no | yes | no 
 HyperTune | Li, et al. (2022) | model-based | yes | yes | no
-DyHPO | Wistuba, et al. (2022) | model-based | yes | yes | no
+DyHPO<sup>*</sup> | Wistuba, et al. (2022) | model-based | yes | yes | no
 ASHABORE | Tiao, et al. (2021) | model-based | yes | yes | no
 ASHACQR | Salinas, et al. (2023) | model-based | yes | yes | no 
 PASHA | Bohdal, et al. (2022)| random or model-based | yes | yes | no 
 REA | Real, et al. (2019) | evolutionary | yes | no | no 
 KDE | Falkner, et al. (2018) | model-based | yes | no | no 
 PBT | Jaderberg, et al. (2017) | evolutionary | no | yes | no 
 ZeroShotTransfer | Wistuba, et al. (2015) | deterministic | yes | no | yes 
 ASHA-CTS | Salinas, et al. (2021)| random | yes | yes | yes 
 RUSH | Zappella, et al. (2021)| random | yes | yes | yes 
 BoundingBox | Perrone, et al. (2019) | any | yes | yes | yes
 
+<sup>*</sup>: We implement the model-based scheduling logic of DyHPO, but use
+the same Gaussian process surrogate models as MOBSTER and HyperTune. The original
+source code for the paper is [here](https://github.com/releaunifreiburg/DyHPO/tree/main).
+
 The searchers fall into four broad categories, **deterministic**, **random**, **evolutionary** and **model-based**. The random searchers sample candidate hyperparameter configurations uniformly at random, while the model-based searchers sample them non-uniformly at random, according to a model (e.g., Gaussian process, density ration estimator, etc.) and an acquisition function. The evolutionary searchers make use of an evolutionary algorithm.
 
 Syne Tune also supports [BoTorch](https://github.com/awslabs/syne-tune/blob/main/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py) searchers.
 
 ## Supported multi-objective optimization methods
 
 Method |          Reference          |   Searcher   | Asynchronous? | Multi-fidelity? | Transfer?
@@ -239,15 +254,15 @@
   launches HPO locally with [Ray Tune](https://docs.ray.io/en/master/tune/index.html)
   scheduler
 
 ## Examples for Experimentation and Benchmarking
 
 You will find many examples for experimentation and benchmarking in
 [benchmarking/examples/](benchmarking/examples/) and in
-benchmarking/nusery/](benchmarking/nursery/).
+[benchmarking/nusery/](benchmarking/nursery/).
 
 ## FAQ and Tutorials
 
 You can check our [FAQ](https://syne-tune.readthedocs.io/en/latest/faq.html), to
 learn more about Syne Tune functionalities.
 
 * [Why should I use Syne Tune?](https://syne-tune.readthedocs.io/en/latest/faq.html#why-should-i-use-syne-tune)
@@ -294,17 +309,21 @@
 * [How to Contribute a New Scheduler](https://syne-tune.readthedocs.io/en/latest/tutorials/developer/README.html)
 * [PASHA: Efficient HPO and NAS with Progressive Resource Allocation](https://syne-tune.readthedocs.io/en/latest/tutorials/pasha/pasha.html)
 * [Using Syne Tune for Transfer Learning](https://syne-tune.readthedocs.io/en/latest/tutorials/transfer_learning/transfer_learning.html)
 * [Distributed Hyperparameter Tuning: Finding the Right Model can be Fast and Fun](https://syne-tune.readthedocs.io/en/latest/tutorials/odsc_tutorial/README.html)
 
 ## Blog Posts
 
-- [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
-- [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
-- [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
+* [Run distributed hyperparameter and neural architecture tuning jobs with Syne Tune](https://aws.amazon.com/blogs/machine-learning/run-distributed-hyperparameter-and-neural-architecture-tuning-jobs-with-syne-tune/)
+* [Hyperparameter optimization for fine-tuning pre-trained transformer models from Hugging Face](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/) [(notebook)](https://github.com/awslabs/syne-tune/blob/hf_blog_post/hf_blog_post/example_syne_tune_for_hf.ipynb)
+* [Learn Amazon Simple Storage Service transfer configuration with Syne Tune](https://aws.amazon.com/blogs/opensource/learn-amazon-simple-storage-service-transfer-configuration-with-syne-tune/) [(code)](https://github.com/aws-samples/syne-tune-s3-transfer)
+
+## Videos
+
+* [Martin Wistuba: Hyperparameter Optimization for the Impatient (PyData 2023)](https://www.youtube.com/watch?v=onX6fXzp9Yk)
 
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## Citing Syne Tune
```

### Comparing `syne_tune-0.9.0/syne_tune.egg-info/SOURCES.txt` & `syne_tune-0.9.1/syne_tune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syne_tune-0.9.0/syne_tune.egg-info/requires.txt` & `syne_tune-0.9.1/syne_tune.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,33 @@
 [aws]
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 
+[basic]
+scipy>=1.3.3
+autograd>=1.3
+statsmodels
+boto3
+sagemaker>=2.112.0
+PyYaml
+ujson
+s3fs
+pymoo>=0.6.0
+scikit-learn
+
 [benchmarks]
 tqdm
 torch
+transformers
 torchvision
 filelock
 datasets==1.8.0
-transformers
 
 [blackbox-repository]
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
 s3fs
 scikit-learn
@@ -46,14 +58,15 @@
 sphinx<7.0.0
 sphinx-rtd-theme
 sphinx-autodoc-typehints
 myst-parser
 sphinx_copybutton
 sphinxcontrib-bibtex
 sphinxcontrib.jquery
+wheel
 
 [extra]
 scipy>=1.3.3
 autograd>=1.3
 statsmodels
 pytest
 pytest-cov~=4.1.0
@@ -63,14 +76,15 @@
 sphinx<7.0.0
 sphinx-rtd-theme
 sphinx-autodoc-typehints
 myst-parser
 sphinx_copybutton
 sphinxcontrib-bibtex
 sphinxcontrib.jquery
+wheel
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 pymoo>=0.6.0
 matplotlib
@@ -78,18 +92,18 @@
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
 xgboost
 h5py
 tqdm
 torch
+transformers
 torchvision
 filelock
 datasets==1.8.0
-transformers
 onnxruntime>=1.10.0
 configspace<=0.6.1
 yahpo-gym
 ray[tune]>=2.0.0
 scikit-optimize
 botorch>=0.7.2
```

