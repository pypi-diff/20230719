# Comparing `tmp/autogluon.core-0.8.3b20230717.tar.gz` & `tmp/autogluon.core-0.8.3b20230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.8.3b20230717.tar", last modified: Mon Jul 17 09:03:59 2023, max compression
+gzip compressed data, was "autogluon.core-0.8.3b20230718.tar", last modified: Tue Jul 18 09:04:02 2023, max compression
```

## Comparing `autogluon.core-0.8.3b20230717.tar` & `autogluon.core-0.8.3b20230718.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.539021 autogluon.core-0.8.3b20230717/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-17 09:03:59.539021 autogluon.core-0.8.3b20230717/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:03:59.539021 autogluon.core-0.8.3b20230717/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.527021 autogluon.core-0.8.3b20230717/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.527021 autogluon.core-0.8.3b20230717/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.527021 autogluon.core-0.8.3b20230717/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29443 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17849 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    93732 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.531021 autogluon.core-0.8.3b20230717/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59573 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    39284 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   176270 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36043 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.535021 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49501 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-17 09:03:42.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:59.527021 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:03:59.000000 autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.853440 autogluon.core-0.8.3b20230718/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-18 09:04:02.853440 autogluon.core-0.8.3b20230718/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:04:02.853440 autogluon.core-0.8.3b20230718/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.841442 autogluon.core-0.8.3b20230718/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.841442 autogluon.core-0.8.3b20230718/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29419 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21155 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17849 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93732 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.845441 autogluon.core-0.8.3b20230718/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59573 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39284 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176270 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36043 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.849440 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49501 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-18 09:03:47.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:02.841442 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:04:02.000000 autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.8.3b20230717/PKG-INFO` & `autogluon.core-0.8.3b20230718/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.8.3b20230717
+Version: 0.8.3b20230718
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.8.3b20230717/setup.py` & `autogluon.core-0.8.3b20230718/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 }
 
 tests_require = [
     "pytest",
     "types-requests",
     "types-setuptools",
     "pytest-mypy",
-    # TODO(Re-enable ray_lightning once it released 0.3.0) 'ray_lightning>=0.2.0,<0.3.0'
 ]
 
 all_requires = []
 
 for extra_package in ["ray", "raytune"]:
     all_requires += extras_require[extra_package]
 tests_require = list(set(tests_require))
```

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/__init__.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/constants.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/dataset.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
         minimum_gpu_per_trial: float
             Minimum number of gpu required to perform a trial. You are allowed to provide fractional gpu with a float.
             If not needed, provide 0
         adapter_type: str
             Type of adapter used by ray hpo experiment.
             Adapters are used to provide custom info or behavior that's module specific to the ray hpo experiment.
             For more info, please refer to `autogluon/core/hpo/ray_hpo`
-            Valid values are ['tabular', 'timeseries', 'automm', 'automm_ray_lightning']
+            Valid values are ['tabular', 'timeseries', 'automm']
         trainable_is_parallel
             Whether the trainable itself will use ray to run parallel job or not.
         tune_config_kwargs
             Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.tune.tune_config.TuneConfig
         run_config_kwargs
             Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.air.config.RunConfig
         """
```

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 14% similar despite different names*

```diff
@@ -453,59 +453,14 @@
     def trainable_args_update_method(self, trainable_args: dict) -> dict:
         trainable_args["hyperparameters"]["env.num_gpus"] = self.gpu_per_job
         trainable_args["hyperparameters"]["env.num_workers"] = self.cpu_per_job
 
         return trainable_args
 
 
-class AutommRayTuneLightningAdapter(RayTuneAdapter):
-
-    supported_searchers = ["random", "bayes"]
-    supported_schedulers = ["FIFO", "ASHA"]
-
-    def __init__(self):
-        super().__init__()
-        self.num_workers = None
-        self.cpu_per_worker = None
-
-    @property
-    def adapter_type(self):
-        return "automm_ray_lightning"
-
-    def check_user_provided_resources_per_trial(self, resources_per_trial: Optional[dict] = None):
-        if resources_per_trial is not None:
-            # Ray Lightning provides a way to get the resources_per_trial because of the complexity of head process and worker process.
-            # It's non-trivial to let the user to specify it. Hence we disable such option
-            logger.warning("AutoMM does not support customized resources_per_trial. We will calculate it for you instead.")
-
-    def get_resource_calculator(self, num_gpus):
-        return ResourceCalculatorFactory.get_resource_calculator(calculator_type="ray_lightning_cpu" if num_gpus == 0 else "ray_lightning_gpu")
-
-    def update_resource_info(self, resources_info: dict):
-        self.num_parallel_jobs = resources_info.get("num_parallel_jobs", None)
-        self.cpu_per_job = resources_info.get("cpu_per_job", None)
-        self.gpu_per_job = resources_info.get("gpu_per_job", None)
-        self.num_workers = resources_info.get("num_workers", None)
-        self.cpu_per_worker = resources_info.get("cpu_per_worker", None)
-        self.resources_per_trial = resources_info.get("resources_per_job", None)
-
-    def trainable_args_update_method(self, trainable_args: dict) -> dict:
-        from ray_lightning import RayPlugin
-
-        trainable_args["hyperparameters"]["env.num_gpus"] = self.gpu_per_job
-        trainable_args["hyperparameters"]["env.num_workers"] = self.cpu_per_job
-        trainable_args["hyperparameters"]["env.num_nodes"] = 1  # num_nodes is not needed by ray lightning. Setting it to default, which is 1
-        trainable_args["_ray_lightning_plugin"] = RayPlugin(
-            num_workers=self.num_workers,
-            num_cpus_per_worker=self.cpu_per_worker,
-            use_gpu=self.gpu_per_job is not None,
-        )
-        return trainable_args
-
-
 class TimeSeriesRayTuneAdapter(TabularRayTuneAdapter):
 
     supported_searchers = ["random", "bayes"]
     supported_schedulers = ["FIFO"]
 
     @property
     def adapter_type(self):
@@ -514,15 +469,14 @@
 
 class RayTuneAdapterFactory:
 
     __supported_adapters = [
         TabularRayTuneAdapter,
         TimeSeriesRayTuneAdapter,
         AutommRayTuneAdapter,
-        AutommRayTuneLightningAdapter,
     ]
 
     __type_to_adapter = {cls().adapter_type: cls for cls in __supported_adapters}
 
     @staticmethod
     def get_adapter(adapter_type: str) -> RayTuneAdapter:
         """Return the executor"""
```

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/_utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/problem_type.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/ray/resources_calculator.py`

 * *Files 16% similar despite different names*

```diff
@@ -191,118 +191,20 @@
             gpu_per_job=gpu_per_job,
         )
         logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
 
         return resources_info
 
 
-class RayLightningCpuResourceCalculator(ResourceCalculator):
-    @property
-    def calc_type(self):
-        return "ray_lightning_cpu"
-
-    def get_resources_per_job(
-        self,
-        total_num_cpus,
-        num_jobs,
-        minimum_cpu_per_job,
-        model_estimate_memory_usage=None,
-        **kwargs,
-    ):
-        from ray_lightning.tune import get_tune_resources
-
-        # TODO: for cpu case, is it better to have more workers or more cpus per worker?
-        cpu_per_job = max(minimum_cpu_per_job, total_num_cpus // num_jobs)
-        max_jobs_in_parallel_memory = num_jobs
-        if model_estimate_memory_usage is not None:
-            mem_available = ResourceManager.get_available_virtual_mem()
-            # calculate how many jobs can run in parallel given memory available
-            max_jobs_in_parallel_memory = max(1, int(mem_available // model_estimate_memory_usage))
-        num_parallel_jobs = min(num_jobs, total_num_cpus // cpu_per_job, max_jobs_in_parallel_memory)
-        if num_parallel_jobs == 0:
-            error_msg = "Cannot train model with provided resources! " f"num_cpus=={total_num_cpus} | " f"min_cpus=={minimum_cpu_per_job}"
-            if model_estimate_memory_usage is not None:
-                error_msg += f" | mem_available=={mem_available} | " f"model_estimate_memory_usage=={model_estimate_memory_usage}"
-            raise AssertionError(error_msg)
-        num_workers = max(minimum_cpu_per_job, cpu_per_job - 1)  # 1 cpu for master process
-        cpu_per_worker = 1
-        resources_per_job = get_tune_resources(num_workers=num_workers, num_cpus_per_worker=cpu_per_worker, use_gpu=False)
-        batches = math.ceil(num_jobs / num_parallel_jobs)
-
-        resources_info = dict(
-            resources_per_job=resources_per_job,
-            num_parallel_jobs=num_parallel_jobs,
-            batches=batches,
-            cpu_per_job=cpu_per_job,
-            num_workers=num_workers,
-        )
-        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
-
-        return resources_info
-
-
-class RayLightningGpuResourceCalculator(ResourceCalculator):
-    @property
-    def calc_type(self):
-        return "ray_lightning_gpu"
-
-    def get_resources_per_job(
-        self,
-        total_num_cpus,
-        total_num_gpus,
-        num_jobs,
-        minimum_cpu_per_job,
-        minimum_gpu_per_job,
-        **kwargs,
-    ):
-        from ray_lightning.tune import get_tune_resources
-
-        # Ray Tune requires 1 additional CPU per trial to use for the Trainable driver.
-        # So the actual number of cpu resources each trial requires is num_workers * num_cpus_per_worker + 1
-        # Each ray worker will reserve 1 gpu
-        # The num_workers in ray stands for worker process to train the model
-        # The num_workers in AutoMM stands for worker process to load data
-        gpu_per_job = max(int(minimum_gpu_per_job), total_num_gpus // num_jobs)
-        num_workers = gpu_per_job  # each worker uses 1 gpu
-        num_parallel_jobs = min(num_jobs, total_num_gpus // gpu_per_job)
-        if num_parallel_jobs == 0:
-            raise AssertionError(
-                "Cannot train model with provided resources! "
-                f"(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | "
-                f"(min_cpus, min_gpus)==({minimum_cpu_per_job}, {minimum_gpu_per_job})"
-            )
-        num_cpus = total_num_cpus - num_parallel_jobs  # reserve cpus for the master process
-        assert num_cpus > 0
-        cpu_per_job = max(minimum_cpu_per_job, num_cpus // num_parallel_jobs)
-        cpu_per_worker = max(1, cpu_per_job // num_workers)
-        resources_per_job = get_tune_resources(num_workers=num_workers, num_cpus_per_worker=cpu_per_worker, use_gpu=True)
-        batches = math.ceil(num_jobs / num_parallel_jobs)
-
-        resources_info = dict(
-            resources_per_job=resources_per_job,
-            num_parallel_jobs=num_parallel_jobs,
-            batches=batches,
-            cpu_per_job=cpu_per_job,
-            gpu_per_job=gpu_per_job,
-            num_workers=num_workers,
-            cpu_per_worker=cpu_per_worker,
-        )
-        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
-
-        return resources_info
-
-
 class ResourceCalculatorFactory:
 
     __supported_calculators = [
         CpuResourceCalculator,
         GpuResourceCalculator,
         NonParallelGpuResourceCalculator,
-        RayLightningCpuResourceCalculator,
-        RayLightningGpuResourceCalculator,
     ]
     __type_to_calculator = {cls().calc_type: cls for cls in __supported_calculators}
 
     @staticmethod
     def get_resource_calculator(calculator_type: str) -> ResourceCalculator:
         """Return the resource calculator"""
         assert calculator_type in ResourceCalculatorFactory.__type_to_calculator, f"{calculator_type} not supported"
```

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/space.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/files.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/plots.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/time.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.8.3b20230718/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.8.3b20230717
+Version: 0.8.3b20230718
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.8.3b20230717/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.8.3b20230718/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

