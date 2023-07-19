# Comparing `tmp/TSInterpret-0.3.1.tar.gz` & `tmp/TSInterpret-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.3.1.tar", last modified: Thu Jun 15 09:18:08 2023, max compression
+gzip compressed data, was "TSInterpret-0.3.2.tar", last modified: Wed Jul 19 13:06:00 2023, max compression
```

## Comparing `TSInterpret-0.3.1.tar` & `TSInterpret-0.3.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.312834 TSInterpret-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.304834 TSInterpret-0.3.1/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-15 09:18:08.312834 TSInterpret-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.304834 TSInterpret-0.3.1/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.308834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.312834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.312834 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.312834 TSInterpret-0.3.1/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:18:08.304834 TSInterpret-0.3.1/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-15 09:18:08.000000 TSInterpret-0.3.1/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-15 09:18:08.000000 TSInterpret-0.3.1/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:18:08.000000 TSInterpret-0.3.1/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-15 09:18:08.000000 TSInterpret-0.3.1/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 09:18:08.000000 TSInterpret-0.3.1/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:18:08.312834 TSInterpret-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-15 09:17:57.000000 TSInterpret-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/setup.py
```

### Comparing `TSInterpret-0.3.1/ClassificationModels/CNN.py` & `TSInterpret-0.3.2/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/ClassificationModels/CNN_T.py` & `TSInterpret-0.3.2/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/ClassificationModels/DecisionTree.py` & `TSInterpret-0.3.2/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/ClassificationModels/LSTM.py` & `TSInterpret-0.3.2/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/ClassificationModels/LSTM_T.py` & `TSInterpret-0.3.2/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/ClassificationModels/ResNet.py` & `TSInterpret-0.3.2/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/ClassificationModels/utils.py` & `TSInterpret-0.3.2/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/LICENSE` & `TSInterpret-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/PKG-INFO` & `TSInterpret-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.3.1
+Version: 0.3.2
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.1 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.2 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.3.1/README.md` & `TSInterpret-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,24 @@
             model [torch.nn.Module, tf.keras.Model]: model to be explained
             NumTimeSteps int : Number of Time Step
             NumFeatures int : Number Features
             method str: Saliency Methode to be used
             mode str: Second dimension 'time'->`(1,time,feat)`  or 'feat'->`(1,feat,time)`
         """
         if isinstance(model, torch.nn.Module):
-
             return Saliency_PTY(
                 model,
                 NumTimeSteps,
                 NumFeatures,
                 method=method,
                 mode=mode,
                 device=device,
             )
 
         elif isinstance(model, tensorflow.keras.Model):
-
             return Saliency_TF(
                 model, NumTimeSteps, NumFeatures, method=method, mode=mode
             )
         else:
             raise NotImplementedError(
                 "Please use a TF or PYT Classification model! \
                 If the current model is a TF or PYT Model, \
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         self.per_class_node_indices = {c: [] for c in np.unique(self.labels)}
 
         input_ = self.timeseries.reshape(-1, self.channels, self.window_size)
 
         preds = np.argmax(self.clf(input_), axis=1)
         true_positive_node_ids = {c: [] for c in np.unique(self.labels)}
         for pred, (idx, row) in zip(preds, self.labels.iterrows()):
-
             if row["label"] == pred:
                 true_positive_node_ids[pred].append(idx)
         for c in np.unique(self.labels):
             dataset = []
             for node_id in true_positive_node_ids[c]:
                 dataset.append(self.timeseries[[node_id], :, :].T.flatten())
                 self.per_class_node_indices[c].append(node_id)
@@ -357,15 +356,14 @@
         self.window_size = x_test.shape[-1]
         self.channels = x_test.shape[-2]
 
     def __call__(self, feature_matrix):
         return self.evaluate(feature_matrix)
 
     def evaluate(self, feature_matrix):
-
         new_case = self.x_test.copy()
         assert len(self.cols_swap) == len(feature_matrix)
 
         for col_replace, a in zip(self.cols_swap, feature_matrix):
             if a == 1:
                 new_case[0][col_replace] = self.distractor[0][col_replace]
 
@@ -402,15 +400,14 @@
         super().__init__(clf, timeseries, labels, **kwargs)
         self.discrete_state = False
         self.backup = BruteForceSearch(clf, timeseries, labels, **kwargs)
         self.max_attemps = max_attempts
         self.maxiter = maxiter
 
     def opt_Discrete(self, to_maximize, x_test, dist, columns, init, num_features=None):
-
         fitness_fn = LossDiscreteState(
             to_maximize,
             self.clf,
             x_test,
             dist,
             columns,
             reg=0.8,
@@ -460,15 +457,14 @@
             else:
                 short_explanation.add(best_col)
         return short_explanation
 
     def explain(
         self, x_test, num_features=None, to_maximize=None
     ) -> Tuple[np.array, int]:
-
         input_ = x_test.reshape(1, -1, self.window_size)
         orig_preds = self.clf(input_)
 
         orig_label = np.argmax(orig_preds)
 
         if to_maximize is None:
             to_maximize = np.argsort(orig_preds)[0][-2:-1][0]
@@ -599,15 +595,14 @@
             self.ts_length = shape[-2]
             test_x = test_x.reshape(test_x.shape[0], test_x.shape[2], test_x.shape[1])
         elif mode == "feat":
             change = False
             self.ts_length = shape[-1]
 
         if backend == "PYT":
-
             self.predict = PyTorchModel(model, change).predict
         elif backend == "TF":
             self.predict = TensorFlowModel(model, change).predict
 
         elif backend == "SK":
             self.predict = SklearnModel(model, change).predict
         self.referenceset = (test_x, test_y)
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,14 @@
         individual = np.array(nun.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
         return nun, np.argmax(out)
 
     def _findSubarray(
         self, a, k
     ):  # used to find the maximum contigious subarray of length k in the explanation weight vector
-
         n = len(a)
 
         vec = []
 
         # Iterate to find all the sub-arrays
         for i in range(n - k + 1):
             temp = []
@@ -203,14 +202,17 @@
             )  # grad_cam(self.model, instance.reshape(1,-1,1))#self.cam_extractor.explain(data, self.model,class_index=label)#instance
         # Classify Original
         individual = np.array(instance.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
 
         most_influencial_array = self._findSubarray((training_weights), subarray_length)
 
+        if np.any(np.isnan(most_influencial_array)):
+            return np.full(individual.shape, None), None
+
         starting_point = np.where(training_weights == most_influencial_array[0])[0][0]
 
         X_example = instance.copy().reshape(1, -1)
 
         nun = nun.reshape(1, -1)
         X_example[0, starting_point : subarray_length + starting_point] = nun[
             0, starting_point : subarray_length + starting_point
@@ -221,15 +223,14 @@
         # )
         out = self.predict(individual)
         prob_target = out[0][
             label
         ]  # torch.nn.functional.softmax(model(torch.from_numpy(test_x))).detach().numpy()[0][y_pred[instance]]
         counter = 0
         while prob_target > 0.5 and counter < max_iter:
-
             subarray_length += 1
             most_influencial_array = self._findSubarray(
                 (training_weights), subarray_length
             )
             starting_point = np.where(training_weights == most_influencial_array[0])[0][
                 0
             ]
@@ -247,15 +248,14 @@
             if counter == max_iter or subarray_length == self.ts_length:
                 print("No Counterfactual found")
                 return None, None
 
         return X_example, np.argmax(out, axis=1)[0]
 
     def _instance_based_cf(self, query, label, target, distance="dtw", max_iter=500):
-
         d, nan = self._native_guide_retrieval(query, label, distance, 1)
         beta = 0
         insample_cf = nan.reshape(1, 1, -1)
 
         individual = np.array(query.tolist())  # , dtype=np.float64)
 
         output = self.predict(individual)
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,16 @@
         )
         # self.observation=observation_x
 
     def run(self):
         """
         Runs the optimization
         Returns:
-            [deap.Individual, deap.logbook]: Return the Best Individual and Logbook Info."""
+            [deap.Individual, deap.logbook]: Return the Best Individual and Logbook Info.
+        """
 
         pop = self.toolbox.population(n=self.MU)
         window = []
         mutation = []
         for ind in pop:
             ind.window = np.random.randint(1, 0.5 * np.array(ind).shape[1])
             ind.mutation = random.choice(MUT_TYPES)
@@ -173,15 +174,14 @@
 
         mstats = create_mstats()
         logbook = create_logbook()
 
         record = mstats.compile(pop)
         logbook.record(gen=0, evals=len(pop), **record)
         while gen < self.NGEN:
-
             offspring = tools.selTournamentDCD(pop, len(pop))
             offspring = algorithms.varAnd(
                 offspring, self.toolbox, cxpb=self.CXPB, mutpb=self.MUTPB
             )
 
             offspring = evaluate_pop(offspring, self.toolbox)
             # NSGA
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,15 @@
     if window_size1 == 1:
         ind1, ind2 = tools.cxUniform(
             np.array(ind1).reshape(num_channels, shape),
             np.array(ind2).reshape(num_channels, shape),
             indpb=0.1,
         )
     else:
-
         if (shape / window_size1).is_integer():
-
             ind1 = windowed_view(
                 np.array(ind1).reshape(num_channels, shape),
                 window_size1,
                 window_step=window_size1,
             )
 
             ind2 = windowed_view(
@@ -91,27 +89,25 @@
 
         if num_channels == 1:
             ind1[0], ind2[0] = tools.cxUniform(
                 np.array(ind1[0]).tolist(), np.array(ind2[0]).tolist(), indpb=0.1
             )
 
         else:
-
             items = np.where(channel1 == 1)
             if len(items[0]) != 0:
                 for item in items[0]:
                     ind1[item], ind2[item] = tools.cxUniform(
                         np.array(ind1[item]).tolist(),
                         np.array(ind2[item]).tolist(),
                         indpb=0.1,
                     )
 
     shape_new = np.array(ind1).reshape(1, -1).shape[1]
     if shape_new > shape:
-
         diff = shape_new - shape
         ind1 = np.array(ind1).reshape(num_channels, -1)[:, 0 : shape_new - diff]
         ind2 = np.array(ind2).reshape(num_channels, -1)[:, 0 : shape_new - diff]
     ind1 = creator.Individual(np.array(ind1).reshape(num_channels, -1).tolist())
     ind2 = creator.Individual(np.array(ind2).reshape(num_channels, -1).tolist())
     ind1.window = window_size1
     ind2.window = window_size2
@@ -132,15 +128,14 @@
     items = np.where(channels == 1)
 
     if len(items[0]) != 0:
         channel = random.choice(items[0])
         means = means[channel]
         sigmas = sigmas[channel]
         for i, m, s in zip(range(len(individual[int(channel)])), means, sigmas):
-
             if random.random() < indpb:
                 individual[channel][i] = random.gauss(m, s)
 
     window, channels = mutate_hyperperameter(
         individual, window, channels, len(channels)
     )
     ind = creator.Individual(individual)
@@ -198,15 +193,14 @@
         Boolean indicating whether the two individuals are equal on
         the Pareto front
     """
     return np.all(ind1.fitness.values == ind2.fitness.values)
 
 
 def authentic_opposing_information(ind1, reference_set):
-
     window = ind1.window
     # window=10
     num_channels = len(ind1.channels)
     channels = ind1.channels
     shape = np.array(ind1).shape[-1]
     sample_series = random.choice(reference_set)
     if (shape / window).is_integer():
@@ -214,15 +208,14 @@
             np.array(ind1).reshape(num_channels, shape), window, window_step=window
         )  # [0]
         sample_series = windowed_view(
             sample_series.reshape(num_channels, shape), window, window_step=window
         )  # [0]
 
     else:
-
         shape_new = window * (int(shape / window) + 1)
         padded = np.zeros((num_channels, shape_new))
         sample_padded = np.zeros((num_channels, shape_new))
         padded[:, :shape] = np.array(ind1).reshape(num_channels, shape)
         sample_padded[:, :shape] = sample_series.reshape(num_channels, shape)
         ind1 = windowed_view(
             np.array(padded).reshape(num_channels, shape_new),
@@ -235,15 +228,14 @@
     if len(items[0]) != 0:
         channel = random.choice(items[0])
         index = random.randint(0, len(ind1[0]) - 1)
         ind1[channel, index] = sample_series[channel, index]
 
     new_shape = ind1.reshape(num_channels, -1).shape[1]
     if new_shape > shape:
-
         diff = shape_new - shape
         ind1 = np.array(ind1).reshape(num_channels, -1)[:, 0 : shape_new - diff]
 
     ind1 = ind1.reshape(num_channels, -1)
 
     ind1 = creator.Individual(np.array(ind1).reshape(num_channels, -1).tolist())
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
         reference_set,
         neighborhood,
         window,
         backend="torch",
         channels=1,
         mode="feat",
     ):
-
         super().__init__(n_var=channels, n_obj=3, n_constr=0, evaluation_of="auto")
 
         self.model = model
         self.mode = mode
         self.window = window
         self.observation = observation
-        print(self.observation.shape)
         self.target = target
         self.original_y = original_y
-        if len(original_y) > 1:
+        if type(original_y) is int:
+            self.original_label = original_y
+        elif len(original_y) > 1:
             self.original_label = np.argmax(original_y, axis=1)[0]
         else:
             self.original_label = original_y
 
         self.reference_set = reference_set
         # self.max= max(reference_set)
         self.neighborhood = neighborhood
@@ -67,15 +67,14 @@
                 self.predict = self.get_prediction_torch
             if self.backend == "TF":
                 self.predict = self.get_prediction_tensorflow
             self.output_distance = self.output_distance_target
         self.label, self.output = self.predict(observation, full=True)
 
     def _evaluate(self, explanation, out, *args, **kwargs):
-
         label, output = self.predict(explanation)
 
         output_distance = self.output_distance(output, label)
 
         x_distance = self.mean_delta(self.observation, explanation)
 
         num_changed_features = np.count_nonzero(self.observation - explanation) / (
@@ -155,30 +154,26 @@
         output = self.model.predict(individual.reshape(1, self.window, -1), verbose=0)
         idx = output.argmax()
         if full:
             return idx, output[0]
         return idx, output[0][idx]
 
     def output_distance_binary(self, output, label):
-
         output_distance = 1 - output
 
         if label == self.original_label:
-
             output_distance = 1.0  # output
 
         return output_distance
 
     def output_distance_multi(self, output, label):
-
         output_distance = output - self.output[label]
 
         if label == self.original_label:
             output_distance = 1.0  # output
         return output_distance
 
     def output_distance_target(self, output, label):
-
         output_distance = output - self.output[self.target]
         if label != self.target:
             output_distance = 1.0  # output
         return output_distance
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         self.backend = backend
         self.verbose = verbose
         self.transformer = transformer
         self.epochs = epochs
         if type(data) == tuple:
             self.x, self.y = data
             # print('Len Reference Set ', len(self.x.shape))
-            print(type(self.y[0]))
             if not type(self.y[0]) == int and not type(self.y[0]) == np.int64:
                 print("y was one Hot Encoded")
                 self.y = np.argmax(self.y, axis=1)
             if len(self.x.shape) == 2:
                 print("Reshape Reference Set")
                 self.x.reshape(-1, 1, self.x.shape[-1])
             # print('Reference Set Constructor',self.x.shape)
@@ -88,14 +87,16 @@
         neighborhood = []
         if target_y is not None:
             if not type(target_y) == int:
                 target_y = np.argmax(original_y, axis=1)[0]
             reference_set = self.x[np.where(self.y == target_y)]
         elif len(original_y) > 1:
             reference_set = self.x[np.where(self.y != np.argmax(original_y, axis=1)[0])]
+        elif type(original_y) is int:
+            reference_set = self.x[np.where(self.y != original_y)]
         else:
             reference_set = self.x[np.where(self.y != original_y)]
 
         reference_set = reference_set.reshape(
             -1, original_x.shape[1], original_x.shape[2]
         )
         if len(reference_set.shape) == 2:
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         nsubsets = self._compute_nb_subset(nb_features, subset_size)
 
         # check if we can completely fill the subset size with the remaining neighbors
         while (subset_size < self.num_subset_sizes + 1) and (
             self.num_samples_left * remaining_weight_vector[subset_size - 1] / nsubsets
             >= 1.0 - 1e-8
         ):
-
             # update the counter of full subset and the remaining neighbors to draw
             self.num_full_subsets += 1
             self.num_samples_left -= nsubsets
 
             # rescale what's left of the remaining weight vector to sum to 1
             if remaining_weight_vector[subset_size - 1] < 1.0:
                 remaining_weight_vector /= 1 - remaining_weight_vector[subset_size - 1]
@@ -174,15 +173,14 @@
                 self.neighbors.kernel_weights[used_masks[mask_tuple]] += 1.0
 
             # add the compliment sample
             if (
                 self.num_samples_left > 0
                 and subset_size <= self.num_paired_subset_sizes
             ):
-
                 neighbor_mask[:] = np.abs(neighbor_mask - 1)
                 # only add the sample if we have not seen it before, otherwise just
                 # increment a previous sample's weight
                 if new_sample:
                     self.num_samples_left -= 1
                     self._add_sample(self.nsamplesAdded, neighbor_mask, 1.0)
                 else:
```

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.3.2/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.3.2/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.3.2/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret/Models/base_model.py` & `TSInterpret-0.3.2/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.3.2/TSInterpret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.3.1
+Version: 0.3.2
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.1 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.2 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.3.1/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.3.2/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.1/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.3.2/TSInterpret.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-scikit-learn==1.0.2
+scikit-learn==1.3.0
 torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
-tqdm~=4.61.2
+tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
 tensorflow<3.0,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
-mlrose<2.0,>=1.3.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
 opencv-python==4.6.0.66
 captum<1.0,>=0.5.0
 pyts<1.0,>=0.12.0
 deprecated==1.2.13
 pymop
 deap
 wheel
 
 [:python_version == '3.8']
 dataclasses
 
 [all]
-scikit-learn==1.0.2
+scikit-learn==1.3.0
 torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
-tqdm~=4.61.2
+tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
 tensorflow<3.0,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
-mlrose<2.0,>=1.3.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
 opencv-python==4.6.0.66
 captum<1.0,>=0.5.0
 pyts<1.0,>=0.12.0
 deprecated==1.2.13
 pymop
@@ -81,33 +79,32 @@
 mkdocs-bibtex==2.8.1
 nbconvert==6.4.2
 numpydoc==1.2
 spacy==3.2.2
 jinja2==3.0.3
 
 [dev]
-scikit-learn==1.0.2
+scikit-learn==1.3.0
 torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
-tqdm~=4.61.2
+tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
 tensorflow<3.0,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
-mlrose<2.0,>=1.3.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
 opencv-python==4.6.0.66
 captum<1.0,>=0.5.0
 pyts<1.0,>=0.12.0
 deprecated==1.2.13
 pymop
@@ -137,33 +134,32 @@
 mkdocs-bibtex==2.8.1
 nbconvert==6.4.2
 numpydoc==1.2
 spacy==3.2.2
 jinja2==3.0.3
 
 [test]
-scikit-learn==1.0.2
+scikit-learn==1.3.0
 torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
-tqdm~=4.61.2
+tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
 tensorflow<3.0,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
-mlrose<2.0,>=1.3.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
 opencv-python==4.6.0.66
 captum<1.0,>=0.5.0
 pyts<1.0,>=0.12.0
 deprecated==1.2.13
 pymop
```

### Comparing `TSInterpret-0.3.1/setup.py` & `TSInterpret-0.3.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,35 +19,37 @@
 URL = "https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries"
 EMAIL = "hoellig@fzi.de"
 AUTHOR = "Jacqueline Hoellig"
 REQUIRES_PYTHON = ">=3.6.0"
 
 # Package requirements.
 base_packages = [
-    "scikit-learn==1.0.2",
+    #"mlrose @ https://github.com/gkhayes/mlrose/archive/refs/heads/master.zip",
+    #"mlrose>=1.3.0,< 2.0",
+    "scikit-learn==1.3.0",
     # "scikit-surprise==1.1.1",
     "torch>=1.13.0,<2.0",
     "pandas~=1.3.2",
     "numpy>=1.21.6,< 2.0",
-    "tqdm~=4.61.2",
+    "tqdm>=4.61.2, < 4.66.0",
     "h5py==3.7.0", # todo add version
     "joblib>=1.0.1,< 2.0",
     #"lime==0.2.0.1",
     "Markdown==3.3.4,< 4.0",
     "matplotlib>=3.3.4,< 4.0",
     "partd==1.2.0",
     "pytz>=2021.3",
     "shap>=0.39.0,< 1.0",
     "tensorflow>=2.9.1,< 3.0",
     "keras>=2.9.0,< 3.0",
     "tsfresh>=0.18.0,< 1.0",
     "tslearn>= 0.5.2,< 1.0",
     "seaborn>=0.11.2,< 1.0",
     "scikit_optimize>=0.9.0,< 1.0",
-    "mlrose>=1.3.0,< 2.0",
+    
     "torchcam>=0.3.1,< 1.0",
     "tf_explain>=0.3.1,< 1.0",
     "opencv-python==4.6.0.66",
     "captum>= 0.5.0,< 1.0",
     "pyts>=0.12.0,< 1.0",
     "deprecated==1.2.13",
     "pymop",
@@ -58,15 +60,16 @@
 dev_packages = base_packages + [
     "flake8>=5.0.4,< 6.0",
     "isort==5.9.3",
     "mypy>=0.761,< 1.0",
     "pre-commit>=2.9.2,< 3.0",
     "pytest>=4.5.0,< 5.0",
     "pytest-cov>=2.6.1,< 3.0",
-    "pyupgrade>=3.2.0,< 4.0"
+    "pyupgrade>=3.2.0,< 4.0",
+    #"mlrose @ https://github.com/gkhayes/mlrose/archive/refs/heads/master.zip"
 ]
 
 docs_packages = [
     "flask>=2.0.2,< 3.0",
     "ipykernel>=6.9.0,< 7.0",
     "mike>=0.5.3,< 1.0",
     "mkdocs>=1.2.3,< 2.0",
```

