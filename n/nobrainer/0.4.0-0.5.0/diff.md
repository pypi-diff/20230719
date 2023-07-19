# Comparing `tmp/nobrainer-0.4.0.tar.gz` & `tmp/nobrainer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nobrainer/nobrainer/dist/tmp58tw1_65/nobrainer-0.4.0.tar", last modified: Tue Oct 18 19:21:11 2022, max compression
+gzip compressed data, was "nobrainer-0.5.0.tar", last modified: Wed Jul 19 05:21:26 2023, max compression
```

## Comparing `nobrainer-0.4.0.tar` & `nobrainer-0.5.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    16907 2022-10-18 19:20:53.000000 nobrainer-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-10-18 19:20:53.000000 nobrainer-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-18 19:20:53.000000 nobrainer-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    16415 2022-10-18 19:21:11.000000 nobrainer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-10-18 19:20:53.000000 nobrainer-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11488 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/bayesian_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16648 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7540 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/cli/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16414 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/distrubuted_learning/
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/distrubuted_learning/dwc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9410 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/intensity_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6774 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/layers/
--rw-r--r--   0 runner    (1001) docker     (121)    26347 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/Conv_v.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/InstanceNorm.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8584 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (121)     8828 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/max_pool4d.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/padding.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/layers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43487 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/tests/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/layers/tests/layers_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9065 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     5157 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/bayesian_meshnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8984 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/bayesian_vnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8026 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/bayesian_vnet_semi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/brainsiam.py
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/dcgan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/meshnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    11070 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/progressiveae.py
--rw-r--r--   0 runner    (1001) docker     (121)    11508 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/progressivegan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/models/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7120 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (121)    10191 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/unet_lstm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/vnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/models/vox2vox.py
--rw-r--r--   0 runner    (1001) docker     (121)    22632 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/processing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7076 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/processing/generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/processing/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7854 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/spatial_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/io_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6184 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/losses_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/prediction_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/test_intensity_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     5525 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/test_spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5451 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/tfrecord_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5334 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tests/volume_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    14491 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (121)    15016 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/training.py
--rw-r--r--   0 runner    (1001) docker     (121)    12599 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     6523 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6594 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)    10769 2022-10-18 19:20:53.000000 nobrainer-0.4.0/nobrainer/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16415 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-18 19:21:11.000000 nobrainer-0.4.0/nobrainer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-18 19:20:53.000000 nobrainer-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-10-18 19:21:11.000000 nobrainer-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-10-18 19:20:53.000000 nobrainer-0.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80049 2022-10-18 19:20:53.000000 nobrainer-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.117359 nobrainer-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    19229 2023-07-19 05:21:12.000000 nobrainer-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-19 05:21:12.000000 nobrainer-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 05:21:12.000000 nobrainer-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-19 05:21:26.117359 nobrainer-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-19 05:21:12.000000 nobrainer-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.117359 nobrainer-0.5.0/nobrainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-19 05:21:26.117359 nobrainer-0.5.0/nobrainer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/bayesian_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.105358 nobrainer-0.5.0/nobrainer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.105358 nobrainer-0.5.0/nobrainer/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/cli/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.105358 nobrainer-0.5.0/nobrainer/distrubuted_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/distrubuted_learning/dwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/intensity_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.109359 nobrainer-0.5.0/nobrainer/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)    26347 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/Conv_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/InstanceNorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/max_pool4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/padding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.109359 nobrainer-0.5.0/nobrainer/layers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43487 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/tests/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/layers/tests/layers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.113359 nobrainer-0.5.0/nobrainer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/bayesian_meshnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/bayesian_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/bayesian_vnet_semi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/brainsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/dcgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/meshnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/progressiveae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/progressivegan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.113359 nobrainer-0.5.0/nobrainer/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/unet_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/models/vox2vox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.113359 nobrainer-0.5.0/nobrainer/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/processing/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/processing/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/spatial_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.117359 nobrainer-0.5.0/nobrainer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/losses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/prediction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/test_intensity_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/test_spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/tfrecord_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tests/volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-19 05:21:12.000000 nobrainer-0.5.0/nobrainer/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:21:26.105358 nobrainer-0.5.0/nobrainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-19 05:21:26.000000 nobrainer-0.5.0/nobrainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-19 05:21:26.000000 nobrainer-0.5.0/nobrainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:21:26.000000 nobrainer-0.5.0/nobrainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 05:21:26.000000 nobrainer-0.5.0/nobrainer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:21:25.000000 nobrainer-0.5.0/nobrainer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-19 05:21:26.000000 nobrainer-0.5.0/nobrainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 05:21:26.000000 nobrainer-0.5.0/nobrainer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-19 05:21:12.000000 nobrainer-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-19 05:21:26.117359 nobrainer-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-19 05:21:12.000000 nobrainer-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-19 05:21:12.000000 nobrainer-0.5.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nobrainer-0.4.0/CHANGELOG.md` & `nobrainer-0.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+# 0.5.0 (Wed Jul 19 2023)
+
+#### 🚀 Enhancement
+
+- Remove guide [#243](https://github.com/neuronets/nobrainer/pull/243) ([@ohinds](https://github.com/ohinds) [@satra](https://github.com/satra))
+
+#### 🐛 Bug Fix
+
+- [pre-commit.ci] pre-commit autoupdate [#247](https://github.com/neuronets/nobrainer/pull/247) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]) [@satra](https://github.com/satra))
+- Fix #246: Transforms now return labels if passed [#250](https://github.com/neuronets/nobrainer/pull/250) ([@ohinds](https://github.com/ohinds) [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+- Check out the master branch of the book repo on CI [#249](https://github.com/neuronets/nobrainer/pull/249) ([@ohinds](https://github.com/ohinds))
+- Nobrainer book guide examples run on AWS EC2 as a form of regression testing [#248](https://github.com/neuronets/nobrainer/pull/248) ([@ohinds](https://github.com/ohinds))
+- [pre-commit.ci] pre-commit autoupdate [#236](https://github.com/neuronets/nobrainer/pull/236) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]) [@satra](https://github.com/satra))
+- Multi-GPU support [#242](https://github.com/neuronets/nobrainer/pull/242) ([@ohinds](https://github.com/ohinds) [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+- [pre-commit.ci] pre-commit autoupdate [#234](https://github.com/neuronets/nobrainer/pull/234) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+- [pre-commit.ci] pre-commit autoupdate [#232](https://github.com/neuronets/nobrainer/pull/232) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+- [pre-commit.ci] pre-commit autoupdate [#231](https://github.com/neuronets/nobrainer/pull/231) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+
+#### ⚠️ Pushed to `master`
+
+- Update setup.cfg ([@satra](https://github.com/satra))
+- Update ci.yml ([@satra](https://github.com/satra))
+- update python and tensorflow versions ([@satra](https://github.com/satra))
+- [CI] update python and auto versions ([@satra](https://github.com/satra))
+- replace special branch ([@satra](https://github.com/satra))
+
+#### Authors: 3
+
+- [@ohinds](https://github.com/ohinds)
+- [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot])
+- Satrajit Ghosh ([@satra](https://github.com/satra))
+
+---
+
 # 0.4.0 (Tue Oct 18 2022)
 
 #### 🚀 Enhancement
 
 - update actions [#230](https://github.com/neuronets/nobrainer/pull/230) ([@satra](https://github.com/satra))
 - [pre-commit.ci] pre-commit autoupdate [#229](https://github.com/neuronets/nobrainer/pull/229) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
```

### Comparing `nobrainer-0.4.0/LICENSE` & `nobrainer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/PKG-INFO` & `nobrainer-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobrainer
-Version: 0.4.0
+Version: 0.5.0
 Summary: A framework for developing neural network models for 3D image processing.
 Home-page: https://neuronets.github.io
 Author: Nobrainer Developers
 Author-email: jakub.kaczmarzyk@gmail.com
 License: Apache License, 2.0
 Project-URL: Source Code, https://github.com/neuronets/nobrainer
 Classifier: Development Status :: 3 - Alpha
@@ -13,22 +13,21 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 License-File: LICENSE
 
 # Nobrainer
 
 ![Build status](https://github.com/neuronets/nobrainer/actions/workflows/ci.yml/badge.svg)
@@ -101,18 +100,18 @@
 
 #### Intensity Transforms
 [Add gaussian noise](), [Min-Max intensity scaling](), [Costom intensity scaling](), [Intensity masking](), [Contrast adjustment]()
 
 #### Affine Transform
 Afifine transformation including rotation, translation, reflection.
 
-## Guide Jupyter Notebooks [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuronets/nobrainer)
+## Guide Jupyter Notebooks [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuronets/nobrainer-book/blob/master/)
 
-Please refer to the Jupyter notebooks in the [guide](/guide) directory to get
-started with _Nobrainer_. [Try them out](https://colab.research.google.com/github/neuronets/nobrainer) in Google Colaboratory!
+Please refer to the Jupyter notebooks in the [guide](https://github.com/neuronets/nobrainer-book/blob/master/docs/nobrainer-guides/notebooks/) directory to get
+started with _Nobrainer_. [Try them out](https://colab.research.google.com/github/neuronets/nobrainer-book/blob/master/) in Google Colaboratory!
 
 ## Installation
 
 ### Container
 
 We recommend using the official _Nobrainer_ Docker container, which includes all
 of the dependencies necessary to use the framework. Please see the available images
```

### Comparing `nobrainer-0.4.0/README.md` & `nobrainer-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,18 @@
 
 #### Intensity Transforms
 [Add gaussian noise](), [Min-Max intensity scaling](), [Costom intensity scaling](), [Intensity masking](), [Contrast adjustment]()
 
 #### Affine Transform
 Afifine transformation including rotation, translation, reflection.
 
-## Guide Jupyter Notebooks [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuronets/nobrainer)
+## Guide Jupyter Notebooks [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuronets/nobrainer-book/blob/master/)
 
-Please refer to the Jupyter notebooks in the [guide](/guide) directory to get
-started with _Nobrainer_. [Try them out](https://colab.research.google.com/github/neuronets/nobrainer) in Google Colaboratory!
+Please refer to the Jupyter notebooks in the [guide](https://github.com/neuronets/nobrainer-book/blob/master/docs/nobrainer-guides/notebooks/) directory to get
+started with _Nobrainer_. [Try them out](https://colab.research.google.com/github/neuronets/nobrainer-book/blob/master/) in Google Colaboratory!
 
 ## Installation
 
 ### Container
 
 We recommend using the official _Nobrainer_ Docker container, which includes all
 of the dependencies necessary to use the framework. Please see the available images
```

### Comparing `nobrainer-0.4.0/nobrainer/bayesian_utils.py` & `nobrainer-0.5.0/nobrainer/bayesian_utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/cli/main.py` & `nobrainer-0.5.0/nobrainer/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,15 +508,17 @@
                 img = generate(latents)["generated"]
                 img = np.squeeze(img)
                 images.append(img)
                 resolutions.append(os.path.splitext(model_path)[0].split("_")[-1])
 
         else:
             output_resolution = int(output_shape[0])
-            model = os.path.join(model, "generator_res_{}".format(output_resolution))
+            model = os.path.join(
+                model, "generator_res_{}".format(output_resolution), "weights"
+            )
             generator = tf.saved_model.load(model)
             generate = generator.signatures["serving_default"]
             img = generate(latents)["generated"]
             img = np.squeeze(img)
 
     except Exception:
         click.echo(click.style("ERROR: generation failed. See error trace.", fg="red"))
```

### Comparing `nobrainer-0.4.0/nobrainer/cli/tests/main_test.py` & `nobrainer-0.5.0/nobrainer/cli/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/dataset.py` & `nobrainer-0.5.0/nobrainer/dataset.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/distrubuted_learning/dwc.py` & `nobrainer-0.5.0/nobrainer/distrubuted_learning/dwc.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/intensity_transforms.py` & `nobrainer-0.5.0/nobrainer/intensity_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,17 @@
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         if len(y.shape) != 3:
             raise ValueError("`LabelMap` must be equal or higher than rank 2")
 
         y = tf.cast(y, tf.float32)
         return tf.math.add(x, noise), tf.math.add(y, noise)
-    else:
+    if y is None:
         return tf.math.add(x, noise)
+    return tf.math.add(x, noise), y
 
 
 def minmaxIntensityScaling(x, y=None, trans_xy=False):
     """Apply intensity scaling [0-1] to input and label.
 
     Usage:
     ```python
@@ -86,14 +87,16 @@
             raise ValueError("`LabelMap` must be equal or higher than rank 2")
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         y = tf.cast(y, tf.float32)
         ymin = tf.cast(tf.reduce_min(y), tf.float32)
         ymax = tf.cast(tf.reduce_max(y), tf.float32)
         y = tf.divide(tf.subtract(y, ymin), tf.add(tf.subtract(ymax, ymin), ep))
+    if y is None:
+        return x
     return x, y
 
 
 def customIntensityScaling(x, y=None, trans_xy=False, scale_x=[0.0, 1.0], scale_y=None):
     """Apply custom intensity scaling to input and label.
 
     Usage:
@@ -147,17 +150,17 @@
         )
         maxy = tf.cast(
             tf.convert_to_tensor(scale_y[1] * np.ones(y_norm.shape).astype(np.float32)),
             tf.float32,
         )
         diff_y = tf.subtract(maxy, miny)
         y = tf.add(tf.multiply(y_norm, diff_y), miny)
-        return x, y
-    else:
+    if y is None:
         return x
+    return x, y
 
 
 def intensityMasking(x, mask_x, y=None, trans_xy=False, mask_y=None):
     """Masking the intensity values in input and label.
 
     Usage:
     ```python
@@ -202,16 +205,17 @@
             y = tf.convert_to_tensor(y)
             mask_y = tf.convert_to_tensor(mask_y)
         y = tf.cast(y, tf.float32)
         mask_x = tf.cast(mask_x, tf.float32)
         if mask_y.shape[0] != y.shape[0] and mask_x.shape[1] != x.shape[1]:
             raise ValueError("Label Masks shape should be same as Label")
         return x, tf.multiply(y, mask_y)
-    else:
+    if y is None:
         return x
+    return x, y
 
 
 def contrastAdjust(x, y=None, trans_xy=False, gamma=1.0):
     """Apply contrast adjustment to input and label.
 
     Usage:
     ```python
@@ -261,9 +265,10 @@
         y = tf.cast(y, tf.float32)
         ymin = tf.cast(tf.reduce_min(y), tf.float32)
         ymax = tf.cast(tf.reduce_max(y), tf.float32)
         y_range = tf.subtract(ymax, ymin)
         y = tf.pow(tf.divide(tf.subtract(y, ymin), tf.add(y_range, ep)), gamma)
         y = tf.add(tf.multiply(y, y_range), ymin)
         return x, y
-    else:
+    if y is None:
         return x
+    return x, y
```

### Comparing `nobrainer-0.4.0/nobrainer/io.py` & `nobrainer-0.5.0/nobrainer/io.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/Conv_v.py` & `nobrainer-0.5.0/nobrainer/layers/Conv_v.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/InstanceNorm.py` & `nobrainer-0.5.0/nobrainer/layers/InstanceNorm.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/dropout.py` & `nobrainer-0.5.0/nobrainer/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/groupnorm.py` & `nobrainer-0.5.0/nobrainer/layers/groupnorm.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/max_pool4d.py` & `nobrainer-0.5.0/nobrainer/layers/max_pool4d.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/padding.py` & `nobrainer-0.5.0/nobrainer/layers/padding.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/tests/dropout_test.py` & `nobrainer-0.5.0/nobrainer/layers/tests/dropout_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/layers/tests/layers_test.py` & `nobrainer-0.5.0/nobrainer/layers/tests/layers_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/losses.py` & `nobrainer-0.5.0/nobrainer/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
     """
 
     def __init__(self, reduction=ReductionV2.AUTO, name="wasserstein"):
         super().__init__(wasserstein, reduction=reduction, name=name)
 
 
 def gradient_penalty(gradients, real_pred, gp_weight=10, epsilon_weight=0.001):
-
     gradients_squared = tf.square(gradients)
     gradients_sqr_sum = tf.reduce_sum(
         gradients_squared, axis=tf.range(1, tf.rank(gradients_squared))
     )
     gradient_l2_norm = tf.sqrt(gradients_sqr_sum)
 
     gradient_penalty = gp_weight * tf.square(1 - gradient_l2_norm)
```

### Comparing `nobrainer-0.4.0/nobrainer/metrics.py` & `nobrainer-0.5.0/nobrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/__init__.py` & `nobrainer-0.5.0/nobrainer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/autoencoder.py` & `nobrainer-0.5.0/nobrainer/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/bayesian_meshnet.py` & `nobrainer-0.5.0/nobrainer/models/bayesian_meshnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/bayesian_vnet.py` & `nobrainer-0.5.0/nobrainer/models/bayesian_vnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/bayesian_vnet_semi.py` & `nobrainer-0.5.0/nobrainer/models/bayesian_vnet_semi.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/brainsiam.py` & `nobrainer-0.5.0/nobrainer/models/brainsiam.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/dcgan.py` & `nobrainer-0.5.0/nobrainer/models/dcgan.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/highresnet.py` & `nobrainer-0.5.0/nobrainer/models/highresnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/meshnet.py` & `nobrainer-0.5.0/nobrainer/models/meshnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/progressiveae.py` & `nobrainer-0.5.0/nobrainer/models/progressiveae.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
             + (self.num_channels,)
         )
         alpha_shape = (1,)
 
         self.build([images_shape, alpha_shape])
 
     def call(self, inputs):
-
         images, alpha = inputs
 
         x = self.Head_Conv(images)
         y = self.highest_resolution_block(x)
         x = self.make_Ebase(images, y, alpha)
 
         for e_block in self.resolution_blocks[::-1]:
@@ -257,15 +256,14 @@
         self.Base_Dense = tf.keras.layers.Dense(
             units=self._nf(1) * 2**self.dimensionality
         )
 
         self.build([(None, latent_size), (1,)])
 
     def update_res(self):
-
         self.current_resolution += 1
         self.current_width = 2**self.current_resolution
 
     def _pixel_norm(self, epsilon=1e-08):
         """
         Pixelwise normalization
         """
@@ -359,15 +357,14 @@
 
         self.Head_Conv1 = self.Conv(filters=(self.num_channels), kernel_size=1)
         self.Head_Conv2 = self.Conv(filters=(self.num_channels), kernel_size=1)
 
         self.build([(None, self.latent_size), (1,)])
 
     def call(self, inputs):
-
         latents, alpha = inputs
 
         x = self.make_Dbase(latents)
 
         for d_block in self.resolution_blocks:
             x = d_block(x)
```

### Comparing `nobrainer-0.4.0/nobrainer/models/progressivegan.py` & `nobrainer-0.5.0/nobrainer/models/progressivegan.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,27 +155,25 @@
         )
         block_layers.append(layers.Activation(tf.nn.leaky_relu))
         block_layers.append(self._pixel_norm())
 
         return models.Sequential(block_layers, name=name)
 
     def generator_head(self, x, y, alpha):
-
         x = self.Upsampling()(x)
         x = self.HeadConv1(x)
 
         y = self.HeadConv2(y)
 
         output = self._weighted_sum()([x, y, alpha])
         output = layers.Activation("tanh")(output)
 
         return output
 
     def add_resolution(self):
-
         self.current_resolution += 1
         self.resolution_blocks.append(self.highest_resolution_block)
         self.highest_resolution_block = self._make_generator_block(
             self._nf(self.current_resolution),
             name="g_block_{}".format(self.current_resolution),
         )
 
@@ -277,15 +275,14 @@
     def _nf(self, stage):
         """
         Computes number of filters for a conv layer
         """
         return min(int(self.fmap_base / (2.0 ** (stage))), self.fmap_max)
 
     def discriminator_base(self, x, y, alpha):
-
         x = self.AveragePooling()(x)
         x = self.BaseConv(x)
 
         lerp_input = self._weighted_sum()([x, y, alpha])
 
         return lerp_input
 
@@ -353,15 +350,14 @@
             + (self.num_channels,)
         )
         alpha_shape = (1,)
 
         self.build([images_shape, alpha_shape])
 
     def call(self, inputs):
-
         images, alpha = inputs
 
         # To bring to the right number of filters
         x = self.FadeConv(images)
         y = self.highest_resolution_block(x)
         x = self.discriminator_base(images, y, alpha)
```

### Comparing `nobrainer-0.4.0/nobrainer/models/tests/models_test.py` & `nobrainer-0.5.0/nobrainer/models/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/unet.py` & `nobrainer-0.5.0/nobrainer/models/unet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/unet_lstm.py` & `nobrainer-0.5.0/nobrainer/models/unet_lstm.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/vnet.py` & `nobrainer-0.5.0/nobrainer/models/vnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/models/vox2vox.py` & `nobrainer-0.5.0/nobrainer/models/vox2vox.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/prediction.py` & `nobrainer-0.5.0/nobrainer/prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,14 @@
         # Bayesian prediction based on sampling from distributions
         means = np.zeros_like(features.squeeze(-1))
         variances = np.zeros_like(features.squeeze(-1))
         entropies = np.zeros_like(features.squeeze(-1))
         progbar = tf.keras.utils.Progbar(n_batches)
         progbar.update(0)
         for j in range(0, n_blocks, batch_size):
-
             this_x = features[j : j + batch_size]
             s = StreamingStats()
             for n in range(n_samples):
                 # TODO: has better performance but output should change to numpy array
                 # new_prediction = model(this_x).numpy()
                 new_prediction = model.predict(this_x, batch_size=1, verbose=0)
                 s.update(new_prediction)
```

### Comparing `nobrainer-0.4.0/nobrainer/processing/base.py` & `nobrainer-0.5.0/nobrainer/processing/base.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/processing/generation.py` & `nobrainer-0.5.0/nobrainer/processing/generation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# import importlib
 import os
 from pathlib import Path
 
 import tensorflow as tf
 
 from .base import BaseEstimator
 from .. import losses
@@ -39,16 +38,16 @@
         checkpoint_dir=Path(os.getcwd()) / "temp",
         normalizer=None,
         # TODO: figure out whether optimizer args should be flattened
         g_optimizer=None,
         g_opt_args=None,
         d_optimizer=None,
         d_opt_args=None,
-        g_loss=losses.wasserstein,
-        d_loss=losses.wasserstein,
+        g_loss=losses.Wasserstein,
+        d_loss=losses.Wasserstein,
         warm_start=False,
         multi_gpu=False,
         num_parallel_calls=None,
         save_freq=500,
     ):
         """Train a progressive gan model"""
         # TODO: check validity of datasets
@@ -79,36 +78,64 @@
             d_optimizer = tf.keras.optimizers.Adam
         d_opt_args_tmp = dict(
             learning_rate=1e-04, beta_1=0.0, beta_2=0.99, epsilon=1e-8
         )
         d_opt_args_tmp.update(**d_opt_args)
         d_opt_args = d_opt_args_tmp
 
+        # for multi gpu training
+        if multi_gpu:
+            strategy = tf.distribute.MirroredStrategy()
+        else:
+            strategy = tf.distribute.get_strategy()
+
         if warm_start:
             if self.model_ is None:
                 raise ValueError("warm_start requested, but model is undefined")
         else:
             from ..models.progressivegan import progressivegan
             from ..training import ProgressiveGANTrainer
 
             # Instantiate the generator and discriminator
-            generator, discriminator = progressivegan(
-                latent_size=self.latent_size,
-                g_fmap_base=self.g_fmap_base,
-                d_fmap_base=self.d_fmap_base,
-                num_channels=self.num_channels,
-                dimensionality=self.dimensionality,
-            )
-            self.model_ = ProgressiveGANTrainer(
-                generator=generator,
-                discriminator=discriminator,
-                gradient_penalty=True,
-            )
+            with strategy.scope():
+                generator, discriminator = progressivegan(
+                    latent_size=self.latent_size,
+                    g_fmap_base=self.g_fmap_base,
+                    d_fmap_base=self.d_fmap_base,
+                    num_channels=self.num_channels,
+                    dimensionality=self.dimensionality,
+                )
+                self.model_ = ProgressiveGANTrainer(
+                    generator=generator,
+                    discriminator=discriminator,
+                    gradient_penalty=True,
+                )
             self.current_resolution_ = 0
 
+        # wrap the losses to work on multiple GPUs
+        with strategy.scope():
+            d_loss_object = d_loss(reduction=tf.keras.losses.Reduction.NONE)
+
+            def compute_d_loss(labels, predictions):
+                per_example_loss = d_loss_object(labels, predictions)
+                return tf.nn.compute_average_loss(
+                    per_example_loss, global_batch_size=batch_size
+                )
+
+            g_loss_object = g_loss(reduction=tf.keras.losses.Reduction.NONE)
+
+            def compute_g_loss(labels, predictions):
+                per_example_loss = g_loss_object(labels, predictions)
+                return tf.nn.compute_average_loss(
+                    per_example_loss, global_batch_size=batch_size
+                )
+
+            d_loss = compute_d_loss
+            g_loss = compute_g_loss
+
         # instantiate a progressive training helper and compile with loss and optimizer
         def _compile():
             self.model_.compile(
                 g_optimizer=g_optimizer(**g_opt_args),
                 d_optimizer=d_optimizer(**d_opt_args),
                 g_loss_fn=g_loss,
                 d_loss_fn=d_loss,
@@ -117,45 +144,47 @@
         print(self.model_.generator.summary())
         print(self.model_.discriminator.summary())
 
         for resolution, info in dataset_train.items():
             if resolution < self.current_resolution_:
                 continue
             # create a train dataset with features for resolution
+            batch_size = info.get("batch_size")
+            if batch_size % strategy.num_replicas_in_sync:
+                raise ValueError("batch size must be a multiple of the number of GPUs")
+
             dataset = get_dataset(
                 file_pattern=info.get("file_pattern"),
-                batch_size=info.get("batch_size"),
+                batch_size=batch_size,
                 num_parallel_calls=num_parallel_calls,
                 volume_shape=(resolution, resolution, resolution),
                 n_classes=1,
                 scalar_label=True,
                 normalizer=info.get("normalizer") or normalizer,
             )
 
-            # grow the networks by one (2^x) resolution
-            if resolution > self.current_resolution_:
-                self.model_.generator.add_resolution()
-                self.model_.discriminator.add_resolution()
-
-            if multi_gpu:
-                strategy = tf.distribute.MirroredStrategy()
-                with strategy.scope():
-                    _compile()
-            else:
+            with strategy.scope():
+                # grow the networks by one (2^x) resolution
+                if resolution > self.current_resolution_:
+                    self.model_.generator.add_resolution()
+                    self.model_.discriminator.add_resolution()
                 _compile()
 
-            steps_per_epoch = (info.get("epochs") or epochs) // info.get("batch_size")
-            # save_best_only is set to False as it is an adversarial loss
-            model_checkpoint_callback = tf.keras.callbacks.ModelCheckpoint(
-                str(model_dir),
-                save_weights_only=True,
-                save_best_only=False,
-                save_freq=save_freq,
-                verbose=False,
-            )
+                steps_per_epoch = (info.get("epochs") or epochs) // info.get(
+                    "batch_size"
+                )
+
+                # save_best_only is set to False as it is an adversarial loss
+                model_checkpoint_callback = tf.keras.callbacks.ModelCheckpoint(
+                    str(model_dir),
+                    save_weights_only=True,
+                    save_best_only=False,
+                    save_freq=save_freq,
+                    verbose=False,
+                )
 
             # Train at resolution
             print("Resolution : {}".format(resolution))
 
             print("Transition phase")
             self.model_.fit(
                 dataset,
```

### Comparing `nobrainer-0.4.0/nobrainer/processing/segmentation.py` & `nobrainer-0.5.0/nobrainer/processing/segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,19 @@
             else:
                 _compile()
         else:
             mod = importlib.import_module("..models", "nobrainer.processing")
             base_model = getattr(mod, self.base_model)
             if multi_gpu:
                 strategy = tf.distribute.MirroredStrategy()
+                if batch_size % strategy.num_replicas_in_sync:
+                    raise ValueError(
+                        "batch size must be a multiple of the number of GPUs"
+                    )
+
                 with strategy.scope():
                     _create(base_model)
                     _compile()
             else:
                 _create(base_model)
                 _compile()
         print(self.model_.summary())
```

### Comparing `nobrainer-0.4.0/nobrainer/spatial_transforms.py` & `nobrainer-0.5.0/nobrainer/spatial_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
             raise ValueError("`LabelMap' should be assigned")
         if len(y.shape) != 3:
             raise ValueError("`LabelMap` must be equal or higher than rank 2")
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         y = tf.cast(y, tf.float32)
         y = y[y1 : y1 + th, x1 : x1 + tw, :]
-        return x, y
-    else:
+    if y is None:
         return x
+    return x, y
 
 
 def spatialConstantPadding(x, y=None, trans_xy=False, padding_zyx=[1, 1, 1]):
     """Add constant padding to input and label.
 
     Usage:
     ```python
@@ -94,17 +94,17 @@
             raise ValueError("`LabelMap' should be assigned")
         if len(y.shape) != 3:
             raise ValueError("`LabelMap` must be equal or higher than rank 2")
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         y = tf.cast(y, tf.float32)
         y = tf.pad(y, padding, "CONSTANT")
-        return x, y
-    else:
+    if y is None:
         return x
+    return x, y
 
 
 def randomCrop(x, y=None, trans_xy=False, cropsize=16):
     """Apply random crops to input and label.
 
     Usage:
     ```python
@@ -138,16 +138,17 @@
             raise ValueError("`LabelMap` must be equal or higher than rank 2")
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         y = tf.cast(y, tf.float32)
         stacked = tf.stack([x, y], axis=0)
         cropped = tf.image.random_crop(stacked, [2, cropsize, cropsize, x.shape[2]])
         return cropped[0], cropped[1]
-    else:
+    if y is None:
         return tf.image.random_crop(x, [cropsize, cropsize, x.shape[2]])
+    return tf.image.random_crop(x, [cropsize, cropsize, x.shape[2]]), y
 
 
 def resize(x, y=None, trans_xy=False, size=[32, 32], mode="bicubic"):
     """Resize the input and label.
 
     Usage:
     ```python
@@ -185,17 +186,17 @@
             raise ValueError("`LabelMap' should be assigned")
         if len(y.shape) != 3:
             raise ValueError("`LabelMap` must be equal or higher than rank 2")
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         y = tf.cast(y, tf.float32)
         y = tf.image.resize(y, size, method=mode)
-        return x, y
-    else:
+    if y is None:
         return x
+    return x, y
 
 
 def randomflip_leftright(x, y=None, trans_xy=False):
     """Randomly flips the input and label.
 
     Usage:
     ```python
@@ -230,9 +231,10 @@
         if ~tf.is_tensor(y):
             y = tf.convert_to_tensor(y)
         y = tf.cast(y, tf.float32)
         c = tf.concat([x, y], axis=0)
         c = tf.image.random_flip_left_right(c, seed=None)
         split_channel = int(c.shape[0] / 2)
         return c[0:split_channel, :, :], c[split_channel : c.shape[0], :, :]
-    else:
+    if y is None:
         return tf.image.random_flip_left_right(x, seed=None)
+    return tf.image.random_flip_left_right(x, seed=None), y
```

### Comparing `nobrainer-0.4.0/nobrainer/tests/dataset_test.py` & `nobrainer-0.5.0/nobrainer/tests/dataset_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/io_test.py` & `nobrainer-0.5.0/nobrainer/tests/io_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/losses_test.py` & `nobrainer-0.5.0/nobrainer/tests/losses_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/metrics_test.py` & `nobrainer-0.5.0/nobrainer/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/prediction_test.py` & `nobrainer-0.5.0/nobrainer/tests/prediction_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from .. import prediction
 from ..models.bayesian_meshnet import variational_meshnet
 from ..models.meshnet import meshnet
 
 
 def test_predict(tmp_path):
-
     x = np.ones((4, 4, 4))
     img = nib.Nifti1Image(x, affine=np.eye(4))
     path = str(tmp_path / "features.nii.gz")
     img.to_filename(path)
 
     x2 = x * -50
     img2 = nib.Nifti1Image(x2, affine=np.eye(4))
```

### Comparing `nobrainer-0.4.0/nobrainer/tests/test_utils.py` & `nobrainer-0.5.0/nobrainer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/tfrecord_test.py` & `nobrainer-0.5.0/nobrainer/tests/tfrecord_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/transform_test.py` & `nobrainer-0.5.0/nobrainer/tests/transform_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/utils.py` & `nobrainer-0.5.0/nobrainer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tests/volume_test.py` & `nobrainer-0.5.0/nobrainer/tests/volume_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/tfrecord.py` & `nobrainer-0.5.0/nobrainer/tfrecord.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/training.py` & `nobrainer-0.5.0/nobrainer/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
     def compile(self, optimizer, loss_fn):
         super(ProgressiveAETrainer, self).compile()
 
         self.optimizer = optimizer
         self.loss_fn = compile_utils.LossesContainer(loss_fn)
 
     def train_step(self, images):
-
         if isinstance(images, tuple):
             images = images[0]
 
         self.train_step_counter.assign_add(1.0)
 
         alpha = tf.cond(
             tf.math.equal(self.phase, "transition"),
```

### Comparing `nobrainer-0.4.0/nobrainer/transform.py` & `nobrainer-0.5.0/nobrainer/transform.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/utils.py` & `nobrainer-0.5.0/nobrainer/utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer/validation.py` & `nobrainer-0.5.0/nobrainer/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         batch_size: int, number of sub-volumes per batch for prediction.
         dtype: str or dtype object, dtype of features.
 
     Returns:
         None
     """
     for filepath in filepaths:
-
         outputs, dice = validate_from_filepath(
             filepath=filepath,
             predictor=predictor,
             n_classes=n_classes,
             mapping_y=mapping_y,
             block_shape=block_shape,
             return_variance=return_variance,
```

### Comparing `nobrainer-0.4.0/nobrainer/volume.py` & `nobrainer-0.5.0/nobrainer/volume.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/nobrainer.egg-info/PKG-INFO` & `nobrainer-0.5.0/nobrainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobrainer
-Version: 0.4.0
+Version: 0.5.0
 Summary: A framework for developing neural network models for 3D image processing.
 Home-page: https://neuronets.github.io
 Author: Nobrainer Developers
 Author-email: jakub.kaczmarzyk@gmail.com
 License: Apache License, 2.0
 Project-URL: Source Code, https://github.com/neuronets/nobrainer
 Classifier: Development Status :: 3 - Alpha
@@ -13,22 +13,21 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 License-File: LICENSE
 
 # Nobrainer
 
 ![Build status](https://github.com/neuronets/nobrainer/actions/workflows/ci.yml/badge.svg)
@@ -101,18 +100,18 @@
 
 #### Intensity Transforms
 [Add gaussian noise](), [Min-Max intensity scaling](), [Costom intensity scaling](), [Intensity masking](), [Contrast adjustment]()
 
 #### Affine Transform
 Afifine transformation including rotation, translation, reflection.
 
-## Guide Jupyter Notebooks [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuronets/nobrainer)
+## Guide Jupyter Notebooks [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuronets/nobrainer-book/blob/master/)
 
-Please refer to the Jupyter notebooks in the [guide](/guide) directory to get
-started with _Nobrainer_. [Try them out](https://colab.research.google.com/github/neuronets/nobrainer) in Google Colaboratory!
+Please refer to the Jupyter notebooks in the [guide](https://github.com/neuronets/nobrainer-book/blob/master/docs/nobrainer-guides/notebooks/) directory to get
+started with _Nobrainer_. [Try them out](https://colab.research.google.com/github/neuronets/nobrainer-book/blob/master/) in Google Colaboratory!
 
 ## Installation
 
 ### Container
 
 We recommend using the official _Nobrainer_ Docker container, which includes all
 of the dependencies necessary to use the framework. Please see the available images
```

### Comparing `nobrainer-0.4.0/nobrainer.egg-info/SOURCES.txt` & `nobrainer-0.5.0/nobrainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/setup.cfg` & `nobrainer-0.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -15,35 +15,34 @@
 	Intended Audience :: Education
 	Intended Audience :: Healthcare Industry
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Software Development
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
 	Source Code = https://github.com/neuronets/nobrainer
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.8
 install_requires = 
 	click
 	fsspec
 	joblib
 	nibabel
 	numpy
 	scikit-image
 	tensorflow-probability >= 0.11.0
-	tensorflow >= 2.7.0
+	tensorflow >= 2.10.0
 	tensorflow-addons >= 0.12.0
 	psutil
 zip_safe = False
 packages = find:
 include_package_data = True
 
 [options.entry_points]
```

### Comparing `nobrainer-0.4.0/setup.py` & `nobrainer-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `nobrainer-0.4.0/versioneer.py` & `nobrainer-0.5.0/versioneer.py`

 * *Files identical despite different names*

