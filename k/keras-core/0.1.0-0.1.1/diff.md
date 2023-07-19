# Comparing `tmp/keras-core-0.1.0.tar.gz` & `tmp/keras-core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-core-0.1.0.tar", last modified: Mon Jul 10 18:13:33 2023, max compression
+gzip compressed data, was "keras-core-0.1.1.tar", last modified: Wed Jul 19 04:17:52 2023, max compression
```

## Comparing `keras-core-0.1.0.tar` & `keras-core-0.1.1.tar`

### file list

```diff
@@ -1,464 +1,486 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.195251 keras-core-0.1.0/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3794 2023-07-10 18:13:33.195078 keras-core-0.1.0/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2944 2023-07-10 18:13:26.000000 keras-core-0.1.0/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.134671 keras-core-0.1.0/keras_core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1578 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.135562 keras-core-0.1.0/keras_core/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.135708 keras-core-0.1.0/keras_core/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3513 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.135848 keras-core-0.1.0/keras_core/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      571 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.135980 keras-core-0.1.0/keras_core/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136119 keras-core-0.1.0/keras_core/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136264 keras-core-0.1.0/keras_core/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      779 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136417 keras-core-0.1.0/keras_core/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      269 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136565 keras-core-0.1.0/keras_core/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      357 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136712 keras-core-0.1.0/keras_core/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136852 keras-core-0.1.0/keras_core/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      319 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.136993 keras-core-0.1.0/keras_core/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.137141 keras-core-0.1.0/keras_core/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      265 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.137293 keras-core-0.1.0/keras_core/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      372 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.137449 keras-core-0.1.0/keras_core/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.137612 keras-core-0.1.0/keras_core/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      309 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.137778 keras-core-0.1.0/keras_core/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      444 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.137934 keras-core-0.1.0/keras_core/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.138088 keras-core-0.1.0/keras_core/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.138249 keras-core-0.1.0/keras_core/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.138387 keras-core-0.1.0/keras_core/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      672 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.138554 keras-core-0.1.0/keras_core/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      978 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.138766 keras-core-0.1.0/keras_core/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1030 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.138933 keras-core-0.1.0/keras_core/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      807 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.139090 keras-core-0.1.0/keras_core/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      412 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.139247 keras-core-0.1.0/keras_core/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      249 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.139388 keras-core-0.1.0/keras_core/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.139551 keras-core-0.1.0/keras_core/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.139708 keras-core-0.1.0/keras_core/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.139866 keras-core-0.1.0/keras_core/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      230 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140018 keras-core-0.1.0/keras_core/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      175 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140157 keras-core-0.1.0/keras_core/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      296 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140288 keras-core-0.1.0/keras_core/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1498 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140435 keras-core-0.1.0/keras_core/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10052 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140571 keras-core-0.1.0/keras_core/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140701 keras-core-0.1.0/keras_core/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140844 keras-core-0.1.0/keras_core/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      427 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.140972 keras-core-0.1.0/keras_core/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      447 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141117 keras-core-0.1.0/keras_core/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7624 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141260 keras-core-0.1.0/keras_core/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      167 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141385 keras-core-0.1.0/keras_core/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1287 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141522 keras-core-0.1.0/keras_core/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5671 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141676 keras-core-0.1.0/keras_core/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      881 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141820 keras-core-0.1.0/keras_core/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      910 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.141958 keras-core-0.1.0/keras_core/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.142096 keras-core-0.1.0/keras_core/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      347 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.142250 keras-core-0.1.0/keras_core/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      185 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.142401 keras-core-0.1.0/keras_core/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      492 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.142531 keras-core-0.1.0/keras_core/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      804 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.142678 keras-core-0.1.0/keras_core/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      859 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.142996 keras-core-0.1.0/keras_core/src/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      673 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.143314 keras-core-0.1.0/keras_core/src/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3483 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11945 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/activations/activations.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/api_export.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.146333 keras-core-0.1.0/keras_core/src/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24827 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/convnext.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16707 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/densenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25491 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/efficientnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40609 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/efficientnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16018 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/imagenet_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14635 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/inception_resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15629 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/inception_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17281 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/mobilenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18043 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/mobilenet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23560 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/mobilenet_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30680 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/nasnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19144 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/resnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6454 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9225 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/vgg16.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9548 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/vgg19.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12812 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/applications/xception.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.146903 keras-core-0.1.0/keras_core/src/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2001 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.147723 keras-core-0.1.0/keras_core/src/backend/common/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      573 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/common/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4777 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/common/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3114 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/common/global_state.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7541 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/common/keras_tensor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2525 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/common/stateless_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15831 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/common/variables.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6793 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/config.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/device_placement.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      495 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/exports.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.149066 keras-core-0.1.0/keras_core/src/backend/jax/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1137 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7805 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1303 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      119 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12413 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10178 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2408 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7298 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26044 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/jax/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.150736 keras-core-0.1.0/keras_core/src/backend/tensorflow/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1349 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4421 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1411 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1762 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1049 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19646 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11071 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4920 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2554 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34633 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31970 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.152495 keras-core-0.1.0/keras_core/src/backend/torch/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1913 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10959 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2268 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      837 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2691 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19148 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23001 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4627 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13621 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/torch_module_wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19119 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/backend/torch/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.154950 keras-core-0.1.0/keras_core/src/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      856 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9866 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5293 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/callback_list.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3256 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/csv_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7605 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/early_stopping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/history.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3467 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/lambda_callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2972 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17342 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/model_checkpoint.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3140 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/progbar_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5373 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2756 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/remote_monitor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26810 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      700 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.155315 keras-core-0.1.0/keras_core/src/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1836 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/constraints/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7462 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/constraints/constraints.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.157177 keras-core-0.1.0/keras_core/src/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      424 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      472 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/boston_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3314 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/california_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/cifar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3122 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/cifar10.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2950 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/cifar100.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2955 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/fashion_mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7130 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/imdb.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2419 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7255 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/datasets/reuters.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.157898 keras-core-0.1.0/keras_core/src/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4024 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/initializers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3159 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/initializers/constant_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2587 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/initializers/initializer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22960 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/initializers/random_initializers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.158434 keras-core-0.1.0/keras_core/src/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8973 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.159482 keras-core-0.1.0/keras_core/src/layers/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      298 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1287 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/activation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      838 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/elu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/leaky_relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3504 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/prelu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2299 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/activations/softmax.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.160103 keras-core-0.1.0/keras_core/src/layers/attention/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/attention/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4359 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/attention/additive_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11501 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/attention/attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26275 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.162744 keras-core-0.1.0/keras_core/src/layers/convolutional/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11882 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/base_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10751 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11658 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12685 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5617 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5697 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5721 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5920 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/conv3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5927 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6024 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6084 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6481 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6533 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.164202 keras-core-0.1.0/keras_core/src/layers/core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5516 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13204 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/einsum_dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4750 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/embedding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      512 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/identity.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4354 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/input_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9086 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/lambda_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2680 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/masking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1566 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/core/wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9867 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/input_spec.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    54600 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.165780 keras-core-0.1.0/keras_core/src/layers/merging/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2242 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/add.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2306 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/average.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8910 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/base_merge.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5755 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/concatenate.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12921 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/dot.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2345 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/maximum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2343 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/minimum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2298 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/multiply.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2771 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/merging/subtract.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.166793 keras-core-0.1.0/keras_core/src/layers/normalization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/normalization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11595 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8915 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/normalization/group_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9266 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4266 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.169137 keras-core-0.1.0/keras_core/src/layers/pooling/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3396 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4213 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3293 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1533 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2456 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/base_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3177 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2510 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2398 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2492 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2626 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3395 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4177 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3272 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.172585 keras-core-0.1.0/keras_core/src/layers/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5520 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5234 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8573 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/discretization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28590 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5301 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7695 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/hashing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21332 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14026 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6448 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3803 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3392 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2908 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4939 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4711 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5556 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4643 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/resizing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20831 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18727 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2166 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.173638 keras-core-0.1.0/keras_core/src/layers/regularization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1229 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2999 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3010 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2010 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2056 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7361 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.175696 keras-core-0.1.0/keras_core/src/layers/reshaping/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2802 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8710 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11123 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2442 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/flatten.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1853 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/permute.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1381 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/reshape.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5694 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4968 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2153 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4698 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5112 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.177595 keras-core-0.1.0/keras_core/src/layers/rnn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13012 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/bidirectional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27301 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8320 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8405 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8313 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26171 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/gru.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25054 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17397 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17630 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4926 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4852 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.178042 keras-core-0.1.0/keras_core/src/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5787 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/losses/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5930 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/losses/loss.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    60698 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/losses/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.180157 keras-core-0.1.0/keras_core/src/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7381 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14673 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/accuracy_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61800 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/confusion_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11725 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/f_score_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3084 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/hinge_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26961 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/iou_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7419 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/metric.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26220 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/metrics_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10449 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6647 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/reduction_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19266 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/metrics/regression_metrics.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.180502 keras-core-0.1.0/keras_core/src/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      769 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/mixed_precision/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6532 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/mixed_precision/dtype_policy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.181375 keras-core-0.1.0/keras_core/src/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      159 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/models/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10808 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/models/cloning.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25586 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/models/functional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21833 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/models/model.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10947 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/models/sequential.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.183107 keras-core-0.1.0/keras_core/src/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      666 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10419 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14295 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/function.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2104 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4866 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35150 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5591 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/node.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   104604 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9521 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/operation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8324 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/operation_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1729 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.185187 keras-core-0.1.0/keras_core/src/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2905 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4262 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7231 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/adafactor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3637 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5504 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4684 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6217 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26136 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/base_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8554 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/ftrl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      625 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5422 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/rmsprop.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.185500 keras-core-0.1.0/keras_core/src/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      577 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/schedules/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34551 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4057 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/optimizers/sgd.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.186184 keras-core-0.1.0/keras_core/src/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/random/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8706 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/random/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2622 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/random/seed_generator.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.186617 keras-core-0.1.0/keras_core/src/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1851 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/regularizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11821 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/regularizers/regularizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.187682 keras-core-0.1.0/keras_core/src/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      660 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.188156 keras-core-0.1.0/keras_core/src/saving/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/legacy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11181 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/legacy/legacy_h5_format.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7429 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/object_registration.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6218 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/saving_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21011 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/saving_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27103 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/saving/serialization_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.188707 keras-core-0.1.0/keras_core/src/testing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/testing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15442 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/testing/test_case.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1196 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/testing/test_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.189460 keras-core-0.1.0/keras_core/src/trainers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25420 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/compile_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.191051 keras-core-0.1.0/keras_core/src/trainers/data_adapters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12171 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6868 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1887 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19256 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3159 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2486 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/data_adapters/torch_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8644 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/epoch_iterator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34645 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/trainers/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.194639 keras-core-0.1.0/keras_core/src/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1507 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2282 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/argument_validation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1311 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/code_stats.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23609 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1246 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/dtype_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13673 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/file_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16035 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/image_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2727 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/io_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15136 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/model_visualization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1802 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/naming.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3383 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/numerical_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10306 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/progbar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3823 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/python_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1409 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/rng_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4760 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/sequence_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      722 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/shape_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13578 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/summary_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8892 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/traceback_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4906 2023-07-10 18:13:26.000000 keras-core-0.1.0/keras_core/src/utils/tracking.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.194820 keras-core-0.1.0/keras_core/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2443 2023-07-10 18:13:30.000000 keras-core-0.1.0/keras_core/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-10 18:13:33.135407 keras-core-0.1.0/keras_core.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3794 2023-07-10 18:13:33.000000 keras-core-0.1.0/keras_core.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15635 2023-07-10 18:13:33.000000 keras-core-0.1.0/keras_core.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-10 18:13:33.000000 keras-core-0.1.0/keras_core.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       41 2023-07-10 18:13:33.000000 keras-core-0.1.0/keras_core.egg-info/requires.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       11 2023-07-10 18:13:33.000000 keras-core-0.1.0/keras_core.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-07-10 18:13:33.195296 keras-core-0.1.0/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1813 2023-07-10 18:13:26.000000 keras-core-0.1.0/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.063420 keras-core-0.1.1/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3794 2023-07-19 04:17:52.063228 keras-core-0.1.1/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2944 2023-07-19 04:17:46.000000 keras-core-0.1.1/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.966875 keras-core-0.1.1/keras_core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1578 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.968330 keras-core-0.1.1/keras_core/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.968696 keras-core-0.1.1/keras_core/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3513 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.969000 keras-core-0.1.1/keras_core/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      571 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.969241 keras-core-0.1.1/keras_core/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.969434 keras-core-0.1.1/keras_core/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.969641 keras-core-0.1.1/keras_core/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      779 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.969837 keras-core-0.1.1/keras_core/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      269 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.970217 keras-core-0.1.1/keras_core/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      357 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.970496 keras-core-0.1.1/keras_core/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.970736 keras-core-0.1.1/keras_core/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      319 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.970949 keras-core-0.1.1/keras_core/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      330 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.971155 keras-core-0.1.1/keras_core/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      265 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.971471 keras-core-0.1.1/keras_core/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      372 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.971693 keras-core-0.1.1/keras_core/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.971922 keras-core-0.1.1/keras_core/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      309 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.972151 keras-core-0.1.1/keras_core/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      444 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.972387 keras-core-0.1.1/keras_core/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.972609 keras-core-0.1.1/keras_core/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.972829 keras-core-0.1.1/keras_core/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.973052 keras-core-0.1.1/keras_core/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      672 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.973251 keras-core-0.1.1/keras_core/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      978 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.973447 keras-core-0.1.1/keras_core/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1030 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.973641 keras-core-0.1.1/keras_core/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      807 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.973885 keras-core-0.1.1/keras_core/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      412 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.974148 keras-core-0.1.1/keras_core/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      249 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.974389 keras-core-0.1.1/keras_core/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.974634 keras-core-0.1.1/keras_core/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.974828 keras-core-0.1.1/keras_core/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.975091 keras-core-0.1.1/keras_core/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      230 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.975329 keras-core-0.1.1/keras_core/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      175 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.975581 keras-core-0.1.1/keras_core/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      296 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.975847 keras-core-0.1.1/keras_core/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1498 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.976089 keras-core-0.1.1/keras_core/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9976 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.976327 keras-core-0.1.1/keras_core/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.976582 keras-core-0.1.1/keras_core/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.976812 keras-core-0.1.1/keras_core/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      505 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.977094 keras-core-0.1.1/keras_core/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      447 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.977357 keras-core-0.1.1/keras_core/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7624 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.977630 keras-core-0.1.1/keras_core/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      167 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.977854 keras-core-0.1.1/keras_core/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1287 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.978116 keras-core-0.1.1/keras_core/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5671 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.978312 keras-core-0.1.1/keras_core/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      881 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.978520 keras-core-0.1.1/keras_core/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      910 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.978978 keras-core-0.1.1/keras_core/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      440 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.979213 keras-core-0.1.1/keras_core/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      347 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.979479 keras-core-0.1.1/keras_core/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      185 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.979770 keras-core-0.1.1/keras_core/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      492 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.980014 keras-core-0.1.1/keras_core/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      804 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.980239 keras-core-0.1.1/keras_core/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      859 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.980971 keras-core-0.1.1/keras_core/src/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      697 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.981392 keras-core-0.1.1/keras_core/src/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3483 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11945 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/activations/activations.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/api_export.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.988037 keras-core-0.1.1/keras_core/src/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24800 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/convnext.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16679 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/densenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25463 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/efficientnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40581 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/efficientnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16018 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/imagenet_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14607 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15601 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/inception_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17253 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/mobilenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18015 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/mobilenet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23532 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/mobilenet_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30652 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/nasnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19116 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/resnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6454 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9197 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/vgg16.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9520 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/vgg19.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12784 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/applications/xception.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.989112 keras-core-0.1.1/keras_core/src/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2274 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.990390 keras-core-0.1.1/keras_core/src/backend/common/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      573 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/common/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4777 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/common/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3153 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/common/global_state.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7525 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/common/keras_tensor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2525 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/common/stateless_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15831 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/common/variables.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7075 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/config.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/device_placement.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      495 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/exports.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.992482 keras-core-0.1.1/keras_core/src/backend/jax/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1137 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7839 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1303 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      119 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12413 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10178 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2408 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7327 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25929 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/jax/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.994511 keras-core-0.1.1/keras_core/src/backend/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1067 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5875 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1346 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       59 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2578 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14063 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10580 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3088 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7633 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      663 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/numpy/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.997227 keras-core-0.1.1/keras_core/src/backend/tensorflow/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1349 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4421 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1411 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2539 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1049 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19646 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11071 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4920 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2554 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34502 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31950 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.000371 keras-core-0.1.1/keras_core/src/backend/torch/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1913 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11027 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2268 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      837 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2691 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19115 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23001 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/numpy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.002373 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       84 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1688 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1905 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      161 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1302 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      428 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2069 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1186 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4627 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13577 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/torch_module_wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18941 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/backend/torch/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.005510 keras-core-0.1.1/keras_core/src/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      856 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9866 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5277 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/callback_list.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3237 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/csv_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7605 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/early_stopping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1327 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/history.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3467 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/lambda_callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2972 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17330 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3140 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/progbar_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5373 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2756 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/remote_monitor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27243 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      700 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.006260 keras-core-0.1.1/keras_core/src/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1836 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/constraints/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7462 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/constraints/constraints.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.008916 keras-core-0.1.1/keras_core/src/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      424 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      472 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/boston_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3314 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/california_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/cifar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3122 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/cifar10.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2950 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/cifar100.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2955 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/fashion_mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7130 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/imdb.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2419 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7255 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/datasets/reuters.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.009678 keras-core-0.1.1/keras_core/src/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4024 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/initializers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3200 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/initializers/constant_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2587 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/initializers/initializer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22960 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/initializers/random_initializers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.010338 keras-core-0.1.1/keras_core/src/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8973 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.011690 keras-core-0.1.1/keras_core/src/layers/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      298 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1287 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/activation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      838 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/elu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3504 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/prelu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2299 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/activations/softmax.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.012409 keras-core-0.1.1/keras_core/src/layers/attention/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/attention/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4359 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/attention/additive_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11501 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/attention/attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26275 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.015984 keras-core-0.1.1/keras_core/src/layers/convolutional/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11882 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10751 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11658 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12685 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5617 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5697 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5721 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5920 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5927 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6024 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6084 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6481 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6533 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.018017 keras-core-0.1.1/keras_core/src/layers/core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5516 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13204 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/einsum_dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4750 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/embedding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      512 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/identity.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4354 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/input_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9070 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/lambda_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2680 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/masking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1566 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/core/wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9851 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/input_spec.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    56763 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.020306 keras-core-0.1.1/keras_core/src/layers/merging/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2242 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/add.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2306 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/average.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8910 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/base_merge.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5755 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/concatenate.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12921 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/dot.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2345 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/maximum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2343 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/minimum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2298 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/multiply.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2771 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/merging/subtract.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.021849 keras-core-0.1.1/keras_core/src/layers/normalization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/normalization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11595 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8915 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9266 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4266 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.025538 keras-core-0.1.1/keras_core/src/layers/pooling/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3396 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4213 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3293 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1533 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2456 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3177 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2510 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2398 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2492 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2626 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3395 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4177 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3272 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.030609 keras-core-0.1.1/keras_core/src/layers/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5755 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5234 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8807 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28583 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5534 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7922 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21565 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14065 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6448 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3803 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3622 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3138 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5173 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4948 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5786 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1870 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4643 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21063 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18964 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2163 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.032228 keras-core-0.1.1/keras_core/src/layers/regularization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/regularization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1229 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3010 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/regularization/dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2010 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2056 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7361 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.036909 keras-core-0.1.1/keras_core/src/layers/reshaping/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2802 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8710 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11123 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2442 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/flatten.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1853 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/permute.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1381 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/reshape.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5694 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4968 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2153 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4698 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5112 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.039711 keras-core-0.1.1/keras_core/src/layers/rnn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13012 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27285 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8320 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8405 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8313 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26407 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/gru.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25290 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17381 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17630 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4910 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4852 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.040222 keras-core-0.1.1/keras_core/src/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5787 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/losses/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5914 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/losses/loss.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    60698 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/losses/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.042419 keras-core-0.1.1/keras_core/src/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7381 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14709 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61800 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/confusion_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11725 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/f_score_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3084 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/hinge_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26961 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/iou_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7419 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/metric.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26220 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/metrics_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10449 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6647 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/reduction_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19266 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/metrics/regression_metrics.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.043035 keras-core-0.1.1/keras_core/src/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      769 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/mixed_precision/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6600 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/mixed_precision/dtype_policy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.044154 keras-core-0.1.1/keras_core/src/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      159 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/models/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10792 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/models/cloning.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25593 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/models/functional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21945 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/models/model.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10931 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/models/sequential.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.046903 keras-core-0.1.1/keras_core/src/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      666 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12035 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14329 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/function.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3649 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8685 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40797 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5575 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/node.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   104868 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9505 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/operation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8308 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/operation_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1686 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.050901 keras-core-0.1.1/keras_core/src/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2905 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4262 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7231 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/adafactor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3637 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5448 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4684 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3582 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26886 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/base_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8554 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/ftrl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      753 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5422 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/rmsprop.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.051380 keras-core-0.1.1/keras_core/src/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      577 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34551 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4057 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/optimizers/sgd.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.052333 keras-core-0.1.1/keras_core/src/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/random/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8706 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/random/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2695 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/random/seed_generator.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.052879 keras-core-0.1.1/keras_core/src/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1851 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/regularizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11821 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/regularizers/regularizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.054079 keras-core-0.1.1/keras_core/src/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      660 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.054624 keras-core-0.1.1/keras_core/src/saving/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/legacy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11181 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/legacy/legacy_h5_format.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7429 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/object_registration.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6239 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/saving_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20986 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/saving_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27208 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/saving/serialization_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.055331 keras-core-0.1.1/keras_core/src/testing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/testing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15426 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/testing/test_case.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1196 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/testing/test_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.056437 keras-core-0.1.1/keras_core/src/trainers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25404 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/compile_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.058230 keras-core-0.1.1/keras_core/src/trainers/data_adapters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12464 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2690 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7028 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2292 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19550 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3278 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2612 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/data_adapters/torch_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8838 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/epoch_iterator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34716 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/trainers/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.062538 keras-core-0.1.1/keras_core/src/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1507 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2282 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/argument_validation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1750 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/code_stats.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23647 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1246 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/dtype_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15848 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/file_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16035 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/image_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3545 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/io_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15136 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/model_visualization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1024 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/module_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1802 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/naming.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3656 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/nest.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3442 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/numerical_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10306 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/progbar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3823 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/python_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1634 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/rng_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4760 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/sequence_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      722 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/shape_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13813 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/summary_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9093 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/traceback_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4906 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/utils/tracking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       72 2023-07-19 04:17:46.000000 keras-core-0.1.1/keras_core/src/version.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:52.062720 keras-core-0.1.1/keras_core/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2443 2023-07-19 04:17:49.000000 keras-core-0.1.1/keras_core/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2023-07-19 04:17:51.968040 keras-core-0.1.1/keras_core.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3794 2023-07-19 04:17:51.000000 keras-core-0.1.1/keras_core.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16508 2023-07-19 04:17:51.000000 keras-core-0.1.1/keras_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2023-07-19 04:17:51.000000 keras-core-0.1.1/keras_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-07-19 04:17:51.000000 keras-core-0.1.1/keras_core.egg-info/requires.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       11 2023-07-19 04:17:51.000000 keras-core-0.1.1/keras_core.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2023-07-19 04:17:52.063491 keras-core-0.1.1/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1915 2023-07-19 04:17:46.000000 keras-core-0.1.1/setup.py
```

### Comparing `keras-core-0.1.0/PKG-INFO` & `keras-core-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras-core
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 
 ## Backwards compatibility
 
 Keras Core is intended to work as a drop-in replacement for `tf.keras` (when using the TensorFlow backend). Just take your
 existing `tf.keras` code, change the `keras` imports to `keras_core`, make sure that your calls to `model.save()` are using
 the up-to-date `.keras` format, and you're done.
 
-If your `tf.keras` model does not include custom compoments, you can start running it on top of JAX or PyTorch immediately.
+If your `tf.keras` model does not include custom components, you can start running it on top of JAX or PyTorch immediately.
 
 If it does include custom components (e.g. custom layers or a custom `train_step()`), it is usually possible to convert it
 to a backend-agnostic implementation in just a few minutes.
 
 In addition, Keras models can consume datasets in any format, regardless of the backend you're using:
 you can train your models with your existing `tf.data.Dataset` pipelines or PyTorch `DataLoaders`.
```

### Comparing `keras-core-0.1.0/README.md` & `keras-core-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 ## Backwards compatibility
 
 Keras Core is intended to work as a drop-in replacement for `tf.keras` (when using the TensorFlow backend). Just take your
 existing `tf.keras` code, change the `keras` imports to `keras_core`, make sure that your calls to `model.save()` are using
 the up-to-date `.keras` format, and you're done.
 
-If your `tf.keras` model does not include custom compoments, you can start running it on top of JAX or PyTorch immediately.
+If your `tf.keras` model does not include custom components, you can start running it on top of JAX or PyTorch immediately.
 
 If it does include custom components (e.g. custom layers or a custom `train_step()`), it is usually possible to convert it
 to a backend-agnostic implementation in just a few minutes.
 
 In addition, Keras models can consume datasets in any format, regardless of the backend you're using:
 you can train your models with your existing `tf.data.Dataset` pipelines or PyTorch `DataLoaders`.
```

### Comparing `keras-core-0.1.0/keras_core/__init__.py` & `keras-core-0.1.1/keras_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 from keras_core.src.models.sequential import Sequential
 from keras_core.src.ops.function import Function
 from keras_core.src.ops.operation import Operation
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.regularizers.regularizers import Regularizer
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `keras-core-0.1.0/keras_core/activations/__init__.py` & `keras-core-0.1.1/keras_core/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/applications/__init__.py` & `keras-core-0.1.1/keras_core/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/applications/convnext/__init__.py` & `keras-core-0.1.1/keras_core/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/applications/efficientnet/__init__.py` & `keras-core-0.1.1/keras_core/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/applications/efficientnet_v2/__init__.py` & `keras-core-0.1.1/keras_core/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/backend/__init__.py` & `keras-core-0.1.1/keras_core/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/callbacks/__init__.py` & `keras-core-0.1.1/keras_core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/config/__init__.py` & `keras-core-0.1.1/keras_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/constraints/__init__.py` & `keras-core-0.1.1/keras_core/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/initializers/__init__.py` & `keras-core-0.1.1/keras_core/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/layers/__init__.py` & `keras-core-0.1.1/keras_core/layers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 from keras_core.src.layers.preprocessing.random_translation import RandomTranslation
 from keras_core.src.layers.preprocessing.random_zoom import RandomZoom
 from keras_core.src.layers.preprocessing.rescaling import Rescaling
 from keras_core.src.layers.preprocessing.resizing import Resizing
 from keras_core.src.layers.preprocessing.string_lookup import StringLookup
 from keras_core.src.layers.preprocessing.text_vectorization import TextVectorization
 from keras_core.src.layers.regularization.activity_regularization import ActivityRegularization
-from keras_core.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras_core.src.layers.regularization.dropout import Dropout
 from keras_core.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras_core.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras_core.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras_core.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras_core.src.layers.regularization.spatial_dropout import SpatialDropout3D
 from keras_core.src.layers.reshaping.cropping1d import Cropping1D
```

### Comparing `keras-core-0.1.0/keras_core/losses/__init__.py` & `keras-core-0.1.1/keras_core/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/metrics/__init__.py` & `keras-core-0.1.1/keras_core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/ops/__init__.py` & `keras-core-0.1.1/keras_core/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/ops/nn/__init__.py` & `keras-core-0.1.1/keras_core/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/ops/numpy/__init__.py` & `keras-core-0.1.1/keras_core/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/optimizers/__init__.py` & `keras-core-0.1.1/keras_core/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/optimizers/schedules/__init__.py` & `keras-core-0.1.1/keras_core/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/regularizers/__init__.py` & `keras-core-0.1.1/keras_core/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/saving/__init__.py` & `keras-core-0.1.1/keras_core/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/__init__.py` & `keras-core-0.1.1/keras_core/src/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,10 +11,9 @@
 from keras_core.src import regularizers
 from keras_core.src import utils
 from keras_core.src.layers import Input
 from keras_core.src.layers import Layer
 from keras_core.src.models import Functional
 from keras_core.src.models import Model
 from keras_core.src.models import Sequential
-
-__version__ = "0.1.0"
+from keras_core.src.version import __version__
```

### Comparing `keras-core-0.1.0/keras_core/src/activations/__init__.py` & `keras-core-0.1.1/keras_core/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/activations/activations.py` & `keras-core-0.1.1/keras_core/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/api_export.py` & `keras-core-0.1.1/keras_core/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/applications/convnext.py` & `keras-core-0.1.1/keras_core/src/applications/convnext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from tensorflow.io import gfile
 
 from keras_core.src import backend
 from keras_core.src import initializers
 from keras_core.src import layers
 from keras_core.src import ops
 from keras_core.src import random
 from keras_core.src.api_export import keras_core_export
@@ -386,15 +385,15 @@
             on the "top" layer. Ignored unless `include_top=True`.
             Set `classifier_activation=None` to return the logits
             of the "top" layer.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/densenet.py` & `keras-core-0.1.1/keras_core/src/applications/densenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -178,15 +176,15 @@
             `classifier_activation=None` to return the logits of the "top"
             layer. When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/efficientnet.py` & `keras-core-0.1.1/keras_core/src/applications/efficientnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import copy
 import math
 
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -267,15 +265,15 @@
 
     Returns:
         A model instance.
     """
     if blocks_args == "default":
         blocks_args = DEFAULT_BLOCKS_ARGS
 
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/efficientnet_v2.py` & `keras-core-0.1.1/keras_core/src/applications/efficientnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import copy
 import math
 
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import initializers
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
@@ -888,15 +886,15 @@
     Returns:
         A model instance.
     """
 
     if blocks_args == "default":
         blocks_args = DEFAULT_BLOCKS_ARGS[model_name]
 
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
             f"Received: weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/imagenet_utils.py` & `keras-core-0.1.1/keras_core/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/applications/inception_resnet_v2.py` & `keras-core-0.1.1/keras_core/src/applications/inception_resnet_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.layers.layer import Layer
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
@@ -90,15 +88,15 @@
             Set `classifier_activation=None` to return the logits
             of the "top" layer. When loading pretrained weights,
             `classifier_activation` can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/inception_v3.py` & `keras-core-0.1.1/keras_core/src/applications/inception_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -93,15 +91,15 @@
             Set `classifier_activation=None` to return the logits of the "top"
             layer. When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded; "
             f"Received: weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/mobilenet.py` & `keras-core-0.1.1/keras_core/src/applications/mobilenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import warnings
 
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -103,15 +101,15 @@
             Set `classifier_activation=None` to return the logits of the "top"
             layer. When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), 'imagenet' "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded. "
             f"Received weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/mobilenet_v2.py` & `keras-core-0.1.1/keras_core/src/applications/mobilenet_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import warnings
 
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -105,15 +103,15 @@
             Set `classifier_activation=None` to return the logits of the "top"
             layer. When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded.  "
             f"Received `weights={weights}`"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/mobilenet_v3.py` & `keras-core-0.1.1/keras_core/src/applications/mobilenet_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import warnings
 
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -161,15 +159,15 @@
     input_tensor=None,
     classes=1000,
     pooling=None,
     dropout_rate=0.2,
     classifier_activation="softmax",
     include_preprocessing=True,
 ):
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded.  "
             f"Received weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/nasnet.py` & `keras-core-0.1.1/keras_core/src/applications/nasnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import warnings
 
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -107,15 +105,15 @@
             Set `classifier_activation=None` to return the logits
             of the "top" layer. When loading pretrained weights,
             `classifier_activation` can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/resnet.py` & `keras-core-0.1.1/keras_core/src/applications/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -103,15 +101,15 @@
             pretrained weights, `classifier_activation` can only be
             `None` or `"softmax"`.
 
     Returns:
         A Model instance.
     """
 
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), 'imagenet' "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded.  Received: "
             f"weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/resnet_v2.py` & `keras-core-0.1.1/keras_core/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/applications/vgg16.py` & `keras-core-0.1.1/keras_core/src/applications/vgg16.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -90,15 +88,15 @@
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), 'imagenet' "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded.  Received: "
             f"weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/vgg19.py` & `keras-core-0.1.1/keras_core/src/applications/vgg19.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -90,15 +88,15 @@
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation` can
             only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), 'imagenet' "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded.  Received: "
             f"weights={weights}"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/applications/xception.py` & `keras-core-0.1.1/keras_core/src/applications/xception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tensorflow.io import gfile
-
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.applications import imagenet_utils
 from keras_core.src.models import Functional
 from keras_core.src.ops import operation_utils
 from keras_core.src.utils import file_utils
@@ -88,15 +86,15 @@
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation` can
             only be `None` or `"softmax"`.
 
     Returns:
         A model instance.
     """
-    if not (weights in {"imagenet", None} or gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), 'imagenet' "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/__init__.py` & `keras-core-0.1.1/keras_core/src/backend/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,10 +33,17 @@
     from keras_core.src.backend.tensorflow import *  # noqa: F403
 elif backend() == "jax":
     print_msg("Using JAX backend.")
     from keras_core.src.backend.jax import *  # noqa: F403
 elif backend() == "torch":
     print_msg("Using PyTorch backend.")
     from keras_core.src.backend.torch import *  # noqa: F403
+elif backend() == "numpy":
+    print_msg(
+        "Using NumPy backend.\nThe NumPy backend does not support "
+        "training. It should only be used for inference, evaluation, "
+        "and debugging."
+    )
+    from keras_core.src.backend.numpy import *  # noqa: F403
 else:
     raise ValueError(f"Unable to import backend : {backend()}")
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/common/__init__.py` & `keras-core-0.1.1/keras_core/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/common/backend_utils.py` & `keras-core-0.1.1/keras_core/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/common/global_state.py` & `keras-core-0.1.1/keras_core/src/backend/common/global_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     global GLOBAL_STATE_TRACKER
     global GLOBAL_SETTINGS_TRACKER
 
     GLOBAL_STATE_TRACKER = threading.local()
     GLOBAL_SETTINGS_TRACKER = threading.local()
 
     if backend.backend() == "tensorflow":
-        import tensorflow as tf
+        from keras_core.src.utils.module_utils import tensorflow as tf
 
         tf.compat.v1.reset_default_graph()
         if tf.executing_eagerly():
             # Clear pending nodes in eager executors, kernel caches and
             # step_containers.
             from tensorflow.python.eager import context
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/common/keras_tensor.py` & `keras-core-0.1.1/keras_core/src/backend/common/keras_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.utils.naming import auto_name
 
 
 @keras_core_export("keras_core.KerasTensor")
 class KerasTensor:
@@ -228,15 +228,15 @@
     #   "astype"
     #   a few more NumPy ones...
 
 
 def any_symbolic_tensors(args=None, kwargs=None):
     args = args or ()
     kwargs = kwargs or {}
-    for x in nest.flatten((args, kwargs)):
+    for x in tree.flatten((args, kwargs)):
         if isinstance(x, KerasTensor):
             return True
     return False
 
 
 @keras_core_export("keras_core.utils.is_keras_tensor")
 def is_keras_tensor(x):
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/common/stateless_scope.py` & `keras-core-0.1.1/keras_core/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/common/variables.py` & `keras-core-0.1.1/keras_core/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/config.py` & `keras-core-0.1.1/keras_core/src/backend/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,21 @@
 # Set backend based on KERAS_BACKEND flag, if applicable.
 if "KERAS_BACKEND" in os.environ:
     _backend = os.environ["KERAS_BACKEND"]
     if _backend:
         _BACKEND = _backend
 
 
+if _BACKEND != "tensorflow":
+    # If we are not running on the tensorflow backend, we should stop tensorflow
+    # from using all available GPU memory. See
+    # https://www.tensorflow.org/guide/gpu#limiting_gpu_memory_growth
+    os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "true"
+
+
 @keras_core_export(
     [
         "keras_core.config.backend",
         "keras_core.backend.backend",
     ]
 )
 def backend():
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/__init__.py` & `keras-core-0.1.1/keras_core/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/core.py` & `keras-core-0.1.1/keras_core/src/backend/jax/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
-from tensorflow import nest
+import tree
 
 from keras_core.src.backend.common import KerasVariable
 from keras_core.src.backend.common import standardize_dtype
 from keras_core.src.backend.common.keras_tensor import KerasTensor
 from keras_core.src.backend.common.stateless_scope import StatelessScope
+from keras_core.src.utils.nest import pack_sequence_as
 
 DYNAMIC_SHAPES_OK = True
 
 
 class Variable(KerasVariable):
     def _initialize(self, value):
         self._value = jnp.array(value, dtype=self._dtype)
@@ -85,15 +86,15 @@
         # Second, identify all ktensors
         def index_all_ktensors(x):
             if isinstance(x, KerasTensor):
                 all_input_ktensors.append(x)
             return x
 
         # Third, find out if there are dynamic shapes
-        maybe_symbolic_args, maybe_symbolic_kwargs = nest.map_structure(
+        maybe_symbolic_args, maybe_symbolic_kwargs = tree.map_structure(
             index_all_ktensors, (maybe_symbolic_args, maybe_symbolic_kwargs)
         )
         none_count = 0
         for x in all_input_ktensors:
             for d in x.shape:
                 if d is None:
                     none_count += 1
@@ -111,32 +112,32 @@
 
         def wrapped_fn(*args, **kwargs):
             return fn(*args, *static_args, **kwargs, **static_kwargs)
 
         jax_out = None
         if none_count:
             try:
-                ms_args_1, ms_kwargs_1 = nest.map_structure(
+                ms_args_1, ms_kwargs_1 = tree.map_structure(
                     lambda x: convert_keras_tensor_to_jax(x, fill_value=83),
                     (maybe_symbolic_args, maybe_symbolic_kwargs),
                 )
                 _, jax_out_1 = jax.make_jaxpr(wrapped_fn, return_shape=True)(
                     *ms_args_1, **ms_kwargs_1
                 )
 
-                ms_args_2, ms_kwargs_2 = nest.map_structure(
+                ms_args_2, ms_kwargs_2 = tree.map_structure(
                     lambda x: convert_keras_tensor_to_jax(x, fill_value=89),
                     (maybe_symbolic_args, maybe_symbolic_kwargs),
                 )
                 _, jax_out_2 = jax.make_jaxpr(wrapped_fn, return_shape=True)(
                     *ms_args_2, **ms_kwargs_2
                 )
 
-                flat_out_1 = nest.flatten(jax_out_1)
-                flat_out_2 = nest.flatten(jax_out_2)
+                flat_out_1 = tree.flatten(jax_out_1)
+                flat_out_2 = tree.flatten(jax_out_2)
 
                 flat_out = []
                 for x1, x2 in zip(flat_out_1, flat_out_2):
                     if isinstance(x1, jax.ShapeDtypeStruct):
                         if not isinstance(x2, jax.ShapeDtypeStruct):
                             raise ValueError("Indeterministic output ordering.")
                         shape = list(x1.shape)
@@ -144,42 +145,42 @@
                             if e != shape[i]:
                                 shape[i] = None
                         flat_out.append(
                             jax.ShapeDtypeStruct(shape, dtype=x1.dtype)
                         )
                     else:
                         flat_out.append(x1)
-                jax_out = nest.pack_sequence_as(jax_out_1, flat_out)
+                jax_out = pack_sequence_as(jax_out_1, flat_out)
             except:
                 # Errors can happen when the filled dimensions
                 # are not compatible with the function
                 # (or when the function contains a bug).
                 # In such cases we don't want to confuse users
                 # with random filled dimensions and the like,
                 # so we rerun a pass on the dynamic shapes,
                 # which will likely error out when JAX tries to
                 # validate shapes as fully static.
                 # The error message will be much easier to understand.
                 pass
 
         if jax_out is None:
-            maybe_symbolic_args, maybe_symbolic_kwargs = nest.map_structure(
+            maybe_symbolic_args, maybe_symbolic_kwargs = tree.map_structure(
                 convert_keras_tensor_to_jax,
                 (maybe_symbolic_args, maybe_symbolic_kwargs),
             )
             _, jax_out = jax.make_jaxpr(wrapped_fn, return_shape=True)(
                 *maybe_symbolic_args, **maybe_symbolic_kwargs
             )
 
         def convert_jax_spec_to_keras_tensor(x):
             if isinstance(x, jax.ShapeDtypeStruct):
                 return KerasTensor(x.shape, x.dtype)
             return x
 
-        output_shape = nest.map_structure(
+        output_shape = tree.map_structure(
             convert_jax_spec_to_keras_tensor, jax_out
         )
     return output_shape
 
 
 def cond(pred, true_fn, false_fn):
     return jax.lax.cond(pred, true_fun=true_fn, false_fun=false_fn)
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/image.py` & `keras-core-0.1.1/keras_core/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/math.py` & `keras-core-0.1.1/keras_core/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/nn.py` & `keras-core-0.1.1/keras_core/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/numpy.py` & `keras-core-0.1.1/keras_core/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/random.py` & `keras-core-0.1.1/keras_core/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/rnn.py` & `keras-core-0.1.1/keras_core/src/backend/jax/rnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import tree
 from jax import lax
 from jax import numpy as jnp
-from tensorflow import nest
 
 from keras_core.src.backend.common.stateless_scope import StatelessScope
+from keras_core.src.utils.nest import pack_sequence_as
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -21,36 +22,36 @@
     def swap_batch_timestep(input_t):
         # Swap the batch and timestep dim for the incoming tensor.
         axes = list(range(len(input_t.shape)))
         axes[0], axes[1] = 1, 0
         return jnp.transpose(input_t, axes)
 
     if not time_major:
-        inputs = nest.map_structure(swap_batch_timestep, inputs)
+        inputs = tree.map_structure(swap_batch_timestep, inputs)
 
-    flattened_inputs = nest.flatten(inputs)
+    flattened_inputs = tree.flatten(inputs)
     time_steps = flattened_inputs[0].shape[0]
 
     if mask is not None:
         if mask.dtype != "bool":
             mask = mask.astype("bool")
         if len(mask.shape) == 2:
             mask = jnp.expand_dims(mask, axis=-1)
         if not time_major:
             mask = swap_batch_timestep(mask)
 
     if constants is None:
         constants = []
 
     def _expand_mask(mask_t, input_t, fixed_dim=1):
-        if nest.is_nested(mask_t):
+        if tree.is_nested(mask_t):
             raise ValueError(
                 f"mask_t is expected to be tensor, but got {mask_t}"
             )
-        if nest.is_nested(input_t):
+        if tree.is_nested(input_t):
             raise ValueError(
                 f"input_t is expected to be tensor, but got {input_t}"
             )
         rank_diff = len(input_t.shape) - len(mask_t.shape)
         for _ in range(rank_diff):
             mask_t = jnp.expand_dims(mask_t, -1)
         multiples = [1] * fixed_dim + list(input_t.shape[fixed_dim:])
@@ -70,24 +71,24 @@
         # the item in tuple is list of the tensor with shape (batch, feature)
         def _process_single_input_t(input_t):
             input_t = unstack(input_t)  # unstack for time_step dim
             if go_backwards:
                 input_t.reverse()
             return input_t
 
-        if nest.is_nested(inputs):
-            processed_input = nest.map_structure(
+        if tree.is_nested(inputs):
+            processed_input = tree.map_structure(
                 _process_single_input_t, inputs
             )
         else:
             processed_input = (_process_single_input_t(inputs),)
 
         def _get_input_tensor(time):
             inp = [t_[time] for t_ in processed_input]
-            return nest.pack_sequence_as(inputs, inp)
+            return pack_sequence_as(inputs, inp)
 
         if mask is not None:
             mask_list = unstack(mask)
             if go_backwards:
                 mask_list.reverse()
 
             for i in range(time_steps):
@@ -101,26 +102,26 @@
                 if not successive_outputs:
                     prev_output = jnp.zeros_like(output)
                 else:
                     prev_output = successive_outputs[-1]
 
                 output = jnp.where(tiled_mask_t, output, prev_output)
 
-                flat_states = nest.flatten(states)
-                flat_new_states = nest.flatten(new_states)
+                flat_states = tree.flatten(states)
+                flat_new_states = tree.flatten(new_states)
                 tiled_mask_t = tuple(
                     _expand_mask(mask_t, s) for s in flat_states
                 )
                 flat_final_states = tuple(
                     jnp.where(m, s, ps)
                     for m, s, ps in zip(
                         tiled_mask_t, flat_new_states, flat_states
                     )
                 )
-                states = nest.pack_sequence_as(states, flat_final_states)
+                states = pack_sequence_as(states, flat_final_states)
 
                 if return_all_outputs:
                     successive_outputs.append(output)
                     successive_states.append(states)
                 else:
                     successive_outputs = [output]
                     successive_states = [states]
@@ -191,15 +192,15 @@
                 reverse=go_backwards,
             )
         if go_backwards:
             outputs = jnp.flip(outputs, axis=0)
         last_output = outputs[-1]
 
     if not time_major:
-        outputs = nest.map_structure(swap_batch_timestep, outputs)
+        outputs = tree.map_structure(swap_batch_timestep, outputs)
 
     return last_output, outputs, new_states
 
 
 def lstm(*args, **kwargs):
     raise NotImplementedError
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/jax/trainer.py` & `keras-core-0.1.1/keras_core/src/backend/jax/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import jax
 import numpy as np
-import tensorflow as tf  # for nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import callbacks as callbacks_module
 from keras_core.src import ops
 from keras_core.src import optimizers as optimizers_module
 from keras_core.src.trainers import trainer as base_trainer
 from keras_core.src.trainers.data_adapters import data_adapter_utils
@@ -246,15 +246,15 @@
             outputs, state = one_predict_step(state, data[:1])
 
             for single_step_data in data[1:]:
                 step_outputs, state = one_predict_step(
                     state,
                     [single_step_data],
                 )
-                outputs = tf.nest.map_structure(
+                outputs = tree.map_structure(
                     lambda t1, t2: jax.numpy.concatenate([t1, t2]),
                     outputs,
                     step_outputs,
                 )
             return outputs, state
 
         if self.steps_per_execution > 1:
@@ -579,20 +579,20 @@
             )
 
         self.make_predict_function()
         callbacks.on_predict_begin()
 
         def append_to_outputs(batch_outputs, outputs):
             if outputs is None:
-                outputs = tf.nest.map_structure(
+                outputs = tree.map_structure(
                     lambda batch_output: [batch_output],
                     batch_outputs,
                 )
             else:
-                tf.__internal__.nest.map_structure_up_to(
+                tree.map_structure_up_to(
                     batch_outputs,
                     lambda output, batch_output: output.append(batch_output),
                     outputs,
                     batch_outputs,
                 )
             return outputs
 
@@ -602,17 +602,15 @@
         outputs = None
         for step, x in epoch_iterator.enumerate_epoch(return_type="np"):
             callbacks.on_predict_batch_begin(step)
             batch_outputs, state = self.predict_function(state, x)
             outputs = append_to_outputs(batch_outputs, outputs)
             callbacks.on_predict_batch_end(step, {"outputs": batch_outputs})
         callbacks.on_predict_end()
-        return tf.__internal__.nest.map_structure_up_to(
-            batch_outputs, np.concatenate, outputs
-        )
+        return tree.map_structure_up_to(batch_outputs, np.concatenate, outputs)
 
     def train_on_batch(
         self,
         x,
         y=None,
         sample_weight=None,
         class_weight=None,
@@ -661,15 +659,15 @@
             "non_trainable_variables": non_trainable_variables,
             "optimizer_variables": optimizer_variables,
             "metrics_variables": metrics_variables,
         }
         self.jax_state_sync()
 
         # Format return values
-        logs = tf.nest.map_structure(lambda x: np.array(x), logs)
+        logs = tree.map_structure(lambda x: np.array(x), logs)
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     def test_on_batch(
         self,
         x,
@@ -700,15 +698,15 @@
         self._jax_state = {
             "non_trainable_variables": non_trainable_variables,
             "metrics_variables": metrics_variables,
         }
         self.jax_state_sync()
 
         # Format return values.
-        logs = tf.nest.map_structure(lambda x: np.array(x), logs)
+        logs = tree.map_structure(lambda x: np.array(x), logs)
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     def predict_on_batch(self, x):
         if not all(layer.built for layer in self._flatten_layers()):
             # Build model
@@ -716,17 +714,15 @@
                 self(x)
 
         self.make_predict_function()
         trainable_variables = self.trainable_variables
         non_trainable_variables = self.non_trainable_variables
         state = (trainable_variables, non_trainable_variables)
         batch_outputs, state = self.predict_function(state, [x])
-        batch_outputs = tf.nest.map_structure(
-            lambda x: np.array(x), batch_outputs
-        )
+        batch_outputs = tree.map_structure(lambda x: np.array(x), batch_outputs)
         return batch_outputs
 
     def jax_state_sync(self):
         if not getattr(self, "_jax_state", None):
             return
 
         trainable_variables = self._jax_state.get("trainable_variables", None)
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/__init__.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/core.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/image.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/math.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/nn.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/numpy.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/optimizer.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/random.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/rnn.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import tensorflow as tf
+import tree
+
+from keras_core.src.utils.nest import pack_sequence_as
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -79,17 +82,17 @@
     def swap_batch_timestep(input_t):
         # Swap the batch and timestep dim for the incoming tensor.
         axes = list(range(len(input_t.shape)))
         axes[0], axes[1] = 1, 0
         return tf.transpose(input_t, axes)
 
     if not time_major:
-        inputs = tf.nest.map_structure(swap_batch_timestep, inputs)
+        inputs = tree.map_structure(swap_batch_timestep, inputs)
 
-    flattened_inputs = tf.nest.flatten(inputs)
+    flattened_inputs = tree.flatten(inputs)
     time_steps = flattened_inputs[0].shape[0]
     time_steps_t = tf.shape(flattened_inputs[0])[0]
 
     for input_ in flattened_inputs:
         input_.shape.with_rank_at_least(3)
 
     if mask is not None:
@@ -106,19 +109,19 @@
     # tf.where needs its condition tensor to be the same shape as its two
     # result tensors, but in our case the condition (mask) tensor is
     # (nsamples, 1), and inputs are (nsamples, ndimensions) or even more.
     # So we need to broadcast the mask to match the shape of inputs.
     # That's what the tile call does, it just repeats the mask along its
     # second dimension n times.
     def _expand_mask(mask_t, input_t, fixed_dim=1):
-        if tf.nest.is_nested(mask_t):
+        if tree.is_nested(mask_t):
             raise ValueError(
                 f"mask_t is expected to be tensor, but got {mask_t}"
             )
-        if tf.nest.is_nested(input_t):
+        if tree.is_nested(input_t):
             raise ValueError(
                 f"input_t is expected to be tensor, but got {input_t}"
             )
         rank_diff = len(input_t.shape) - len(mask_t.shape)
         for _ in range(rank_diff):
             mask_t = tf.expand_dims(mask_t, -1)
         multiples = [1] * fixed_dim + input_t.shape.as_list()[fixed_dim:]
@@ -138,24 +141,24 @@
         # the item in tuple is list of the tensor with shape (batch, feature)
         def _process_single_input_t(input_t):
             input_t = tf.unstack(input_t)  # unstack for time_step dim
             if go_backwards:
                 input_t.reverse()
             return input_t
 
-        if tf.nest.is_nested(inputs):
-            processed_input = tf.nest.map_structure(
+        if tree.is_nested(inputs):
+            processed_input = tree.map_structure(
                 _process_single_input_t, inputs
             )
         else:
             processed_input = (_process_single_input_t(inputs),)
 
         def _get_input_tensor(time):
             inp = [t_[time] for t_ in processed_input]
-            return tf.nest.pack_sequence_as(inputs, inp)
+            return pack_sequence_as(inputs, inp)
 
         if mask is not None:
             mask_list = tf.unstack(mask)
             if go_backwards:
                 mask_list.reverse()
 
             for i in range(time_steps):
@@ -169,26 +172,26 @@
                 if not successive_outputs:
                     prev_output = tf.zeros_like(output)
                 else:
                     prev_output = successive_outputs[-1]
 
                 output = tf.where(tiled_mask_t, output, prev_output)
 
-                flat_states = tf.nest.flatten(states)
-                flat_new_states = tf.nest.flatten(new_states)
+                flat_states = tree.flatten(states)
+                flat_new_states = tree.flatten(new_states)
                 tiled_mask_t = tuple(
                     _expand_mask(mask_t, s) for s in flat_states
                 )
                 flat_final_states = tuple(
                     tf.where(m, s, ps)
                     for m, s, ps in zip(
                         tiled_mask_t, flat_new_states, flat_states
                     )
                 )
-                states = tf.nest.pack_sequence_as(states, flat_final_states)
+                states = pack_sequence_as(states, flat_final_states)
 
                 if return_all_outputs:
                     successive_outputs.append(output)
                     successive_states.append(states)
                 else:
                     successive_outputs = [output]
                     successive_states = [states]
@@ -244,15 +247,15 @@
             else ta.unstack(tf.reverse(input_, [0]))
             for ta, input_ in zip(input_ta, flattened_inputs)
         )
 
         # Get the time(0) input and compute the output for that, the output will
         # be used to determine the dtype of output tensor array. Don't read from
         # input_ta due to TensorArray clear_after_read default to True.
-        input_time_zero = tf.nest.pack_sequence_as(
+        input_time_zero = pack_sequence_as(
             inputs, [inp[0] for inp in flattened_inputs]
         )
         # output_time_zero is used to determine the cell output shape and its
         # dtype.  the value is discarded.
         output_time_zero, _ = step_function(
             input_time_zero, tuple(initial_states) + tuple(constants)
         )
@@ -261,15 +264,15 @@
         output_ta = tuple(
             tf.TensorArray(
                 dtype=out.dtype,
                 size=output_ta_size,
                 element_shape=out.shape,
                 tensor_array_name=f"output_ta_{i}",
             )
-            for i, out in enumerate(tf.nest.flatten(output_time_zero))
+            for i, out in enumerate(tree.flatten(output_time_zero))
         )
 
         time = tf.constant(0, dtype="int32", name="time")
 
         if input_length is None:
             max_iterations = time_steps_t
         else:
@@ -325,15 +328,15 @@
         else:
             masking_fn = None
 
         if masking_fn is not None:
             # Mask for the T output will be base on the output of T - 1. In the
             # case T = 0, a zero filled tensor will be used.
             flat_zero_output = tuple(
-                tf.zeros_like(o) for o in tf.nest.flatten(output_time_zero)
+                tf.zeros_like(o) for o in tree.flatten(output_time_zero)
             )
 
             def _step(time, output_ta_t, prev_output, *states):
                 """RNN step function.
 
                 Args:
                     time: Current timestep value.
@@ -342,39 +345,37 @@
                     *states: List of states.
 
                 Returns:
                     Tuple: `(time + 1, output_ta_t, output) + tuple(new_states)`
                 """
                 current_input = tuple(ta.read(time) for ta in input_ta)
                 # maybe set shape.
-                current_input = tf.nest.pack_sequence_as(inputs, current_input)
+                current_input = pack_sequence_as(inputs, current_input)
                 mask_t = masking_fn(time)
                 output, new_states = step_function(
                     current_input, tuple(states) + tuple(constants)
                 )
                 # mask output
-                flat_output = tf.nest.flatten(output)
+                flat_output = tree.flatten(output)
                 flat_mask_output = (
                     flat_zero_output
                     if zero_output_for_mask
-                    else tf.nest.flatten(prev_output)
+                    else tree.flatten(prev_output)
                 )
                 flat_new_output = compute_masked_output(
                     mask_t, flat_output, flat_mask_output
                 )
 
                 # mask states
-                flat_state = tf.nest.flatten(states)
-                flat_new_state = tf.nest.flatten(new_states)
+                flat_state = tree.flatten(states)
+                flat_new_state = tree.flatten(new_states)
                 flat_final_state = compute_masked_output(
                     mask_t, flat_new_state, flat_state
                 )
-                new_states = tf.nest.pack_sequence_as(
-                    new_states, flat_final_state
-                )
+                new_states = pack_sequence_as(new_states, flat_final_state)
 
                 ta_index_to_write = time if return_all_outputs else 0
                 output_ta_t = tuple(
                     ta.write(ta_index_to_write, out)
                     for ta, out in zip(output_ta_t, flat_new_output)
                 )
 
@@ -399,49 +400,47 @@
                     output_ta_t: TensorArray.
                     *states: List of states.
 
                 Returns:
                     Tuple: `(time + 1,output_ta_t) + tuple(new_states)`
                 """
                 current_input = tuple(ta.read(time) for ta in input_ta)
-                current_input = tf.nest.pack_sequence_as(inputs, current_input)
+                current_input = pack_sequence_as(inputs, current_input)
                 output, new_states = step_function(
                     current_input, tuple(states) + tuple(constants)
                 )
-                flat_new_state = tf.nest.flatten(new_states)
+                flat_new_state = tree.flatten(new_states)
 
-                flat_output = tf.nest.flatten(output)
+                flat_output = tree.flatten(output)
                 ta_index_to_write = time if return_all_outputs else 0
                 output_ta_t = tuple(
                     ta.write(ta_index_to_write, out)
                     for ta, out in zip(output_ta_t, flat_output)
                 )
 
-                new_states = tf.nest.pack_sequence_as(
-                    initial_states, flat_new_state
-                )
+                new_states = pack_sequence_as(initial_states, flat_new_state)
                 return (time + 1, output_ta_t) + tuple(new_states)
 
             final_outputs = tf.while_loop(
                 body=_step,
                 loop_vars=(time, output_ta) + states,
                 **while_loop_kwargs,
             )
             new_states = final_outputs[2:]
 
         output_ta = final_outputs[1]
 
         outputs = tuple(o.stack() for o in output_ta)
         last_output = tuple(o[-1] for o in outputs)
 
-        outputs = tf.nest.pack_sequence_as(output_time_zero, outputs)
-        last_output = tf.nest.pack_sequence_as(output_time_zero, last_output)
+        outputs = pack_sequence_as(output_time_zero, outputs)
+        last_output = pack_sequence_as(output_time_zero, last_output)
 
     if not time_major:
-        outputs = tf.nest.map_structure(swap_batch_timestep, outputs)
+        outputs = tree.map_structure(swap_batch_timestep, outputs)
 
     return last_output, outputs, new_states
 
 
 def gru(
     inputs,
     initial_state,
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/tensorflow/trainer.py` & `keras-core-0.1.1/keras_core/src/backend/tensorflow/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import warnings
 
 import numpy as np
 import tensorflow as tf
+import tree
 from tensorflow.python.eager import context as tf_context
 
 from keras_core.src import callbacks as callbacks_module
 from keras_core.src import metrics as metrics_module
 from keras_core.src import optimizers as optimizers_module
 from keras_core.src.trainers import trainer as base_trainer
 from keras_core.src.trainers.data_adapters import data_adapter_utils
@@ -445,15 +446,15 @@
         def append_to_outputs(batch_outputs, outputs):
             if outputs is None:
                 outputs = tf.nest.map_structure(
                     lambda batch_output: [batch_output],
                     batch_outputs,
                 )
             else:
-                tf.__internal__.nest.map_structure_up_to(
+                tree.map_structure_up_to(
                     batch_outputs,
                     lambda output, batch_output: output.append(batch_output),
                     outputs,
                     batch_outputs,
                 )
             return outputs
 
@@ -482,15 +483,15 @@
             for step, iterator in epoch_iterator.enumerate_epoch():
                 callbacks.on_predict_batch_begin(step)
                 data = get_data(iterator)
                 batch_outputs = self.predict_function(data)
                 outputs = append_to_outputs(batch_outputs, outputs)
                 callbacks.on_predict_batch_end(step, {"outputs": batch_outputs})
         callbacks.on_predict_end()
-        outputs = tf.__internal__.nest.map_structure_up_to(
+        outputs = tree.map_structure_up_to(
             batch_outputs, potentially_ragged_concat, outputs
         )
         return tf.nest.map_structure(convert_to_np_if_not_ragged, outputs)
 
     def train_on_batch(
         self,
         x,
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/__init__.py` & `keras-core-0.1.1/keras_core/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/core.py` & `keras-core-0.1.1/keras_core/src/backend/torch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import contextlib
 
 import numpy as np
 import torch
-from tensorflow import nest
+import tree
 
 from keras_core.src.backend.common import KerasVariable
 from keras_core.src.backend.common import global_state
 from keras_core.src.backend.common import standardize_dtype
 from keras_core.src.backend.common.keras_tensor import KerasTensor
 from keras_core.src.backend.common.stateless_scope import StatelessScope
+from keras_core.src.utils.nest import pack_sequence_as
 
 DYNAMIC_SHAPES_OK = True
-
+DEFAULT_DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 
 TORCH_DTYPES = {
     "float16": torch.float16,
     "float32": torch.float32,
     "float64": torch.float64,
     "uint8": torch.uint8,
     "uint16": torch.int32,  # TODO: Torch doesn't have `uint16` dtype.
@@ -35,28 +36,22 @@
     global_state.set_global_attribute("torch_device", device)
     try:
         yield
     finally:
         global_state.set_global_attribute("torch_device", previous_device)
 
 
-def get_default_device():
-    return "cuda" if torch.cuda.is_available() else "cpu"
-
-
 def get_device():
     device = global_state.get_global_attribute("torch_device", None)
     if device is None:
-        return get_default_device()
+        return DEFAULT_DEVICE
     return device
 
 
 def to_torch_dtype(dtype):
-    if dtype in [value for key, value in TORCH_DTYPES.items()]:
-        return dtype
     dtype = standardize_dtype(dtype)
     dtype = TORCH_DTYPES.get(dtype, None)
     if dtype is None:
         raise ValueError(f"Unsupported dtype for PyTorch: {dtype}")
     return dtype
 
 
@@ -110,40 +105,40 @@
         try:
             return super().__eq__(other)
         except Exception:
             return False
 
 
 def convert_to_tensor(x, dtype=None):
-    dtype = to_torch_dtype(dtype or getattr(x, "dtype", None))
-    device = get_device()
-    if isinstance(x, int):
-        dtype = torch.int32
-    if isinstance(x, float):
-        dtype = torch.float32
+    if is_tensor(x):
+        if dtype is None:
+            return x
+        return x.to(to_torch_dtype(dtype))
     if isinstance(x, Variable):
         # TorchDynamo has bugs supporting nn.Parameter type check.
         # Return it directly instead of pass it to the rest of the logic in the
         # function.
         return x.value
-    if is_tensor(x):
-        if dtype and dtype != x.dtype:
-            x = x.to(dtype)
-        return x.to(device)
-
+    if isinstance(x, int):
+        return torch.as_tensor(x, dtype=torch.int32, device=get_device())
+    if isinstance(x, float):
+        return torch.as_tensor(x, dtype=torch.float32, device=get_device())
     # Convert to np in case of any array-like that is not list or tuple.
     if not isinstance(x, (list, tuple)):
         x = np.array(x)
     elif len(x) > 0 and any(isinstance(x1, torch.Tensor) for x1 in x):
         # Handle list or tuple of torch tensors
         return torch.stack([convert_to_tensor(x1) for x1 in x])
-    if isinstance(x, np.ndarray) and x.dtype == np.uint32:
-        # Torch backend does not support uint32.
-        x = x.astype(np.int64)
-    return torch.as_tensor(x, dtype=dtype, device=device)
+    if isinstance(x, np.ndarray):
+        if x.dtype == np.uint32:
+            # Torch backend does not support uint32.
+            x = x.astype(np.int64)
+        dtype = dtype or x.dtype
+    dtype = to_torch_dtype(dtype)
+    return torch.as_tensor(x, dtype=dtype, device=get_device())
 
 
 def convert_to_numpy(x):
     def transform(x):
         if is_tensor(x):
             if x.requires_grad:
                 x = x.detach()
@@ -166,15 +161,18 @@
 
 
 def cast(x, dtype):
     dtype = to_torch_dtype(dtype)
     if isinstance(x, KerasVariable):
         x = x.value
     if is_tensor(x):
-        return x.to(dtype)
+        if x.dtype == dtype:
+            return x
+        else:
+            return x.to(dtype)
     return convert_to_tensor(x, dtype)
 
 
 def name_scope(name):
     return contextlib.nullcontext()
 
 
@@ -210,51 +208,51 @@
     def symbolic_call(fn, args, kwargs, fill_value):
         """Call `fn` to infer output shape and dtype."""
         try:
             # First try instantiating all tensors on the `"meta"` device,
             # which  should give a "zero flop" way to trace shape, but does
             # not have universal support with torch operations.
             with device_scope("meta"):
-                meta_args, meta_kwargs = nest.map_structure(
+                meta_args, meta_kwargs = tree.map_structure(
                     lambda x: convert_keras_tensor_to_torch(x, fill_value),
                     (args, kwargs),
                 )
                 return fn(*meta_args, **meta_kwargs)
         except:
-            with device_scope(get_default_device()):
+            with device_scope(DEFAULT_DEVICE):
                 # If the `"meta"` device placement fails, fall back to tracing
                 # eagerly with tensors on the default device. This will be
                 # more robust, but more expensive.
-                eager_args, eager_kwargs = nest.map_structure(
+                eager_args, eager_kwargs = tree.map_structure(
                     lambda x: convert_keras_tensor_to_torch(x, fill_value),
                     (args, kwargs),
                 )
                 return fn(*eager_args, **eager_kwargs)
 
     with StatelessScope():
         outputs = symbolic_call(fn, args, kwargs, fill_value=83)
 
-        none_in_shape = any(map(has_none_shape, nest.flatten((args, kwargs))))
+        none_in_shape = any(map(has_none_shape, tree.flatten((args, kwargs))))
         if none_in_shape:
             outputs_1 = outputs
             outputs_2 = symbolic_call(fn, args, kwargs, fill_value=89)
 
-            flat_out_1 = nest.flatten(outputs_1)
-            flat_out_2 = nest.flatten(outputs_2)
+            flat_out_1 = tree.flatten(outputs_1)
+            flat_out_2 = tree.flatten(outputs_2)
 
             flat_out = []
             for x1, x2 in zip(flat_out_1, flat_out_2):
                 shape = list(x1.shape)
                 for i, e in enumerate(x2.shape):
                     if e != shape[i]:
                         shape[i] = None
                 flat_out.append(KerasTensor(shape, standardize_dtype(x1.dtype)))
-            outputs = nest.pack_sequence_as(outputs_1, flat_out)
+            outputs = pack_sequence_as(outputs_1, flat_out)
 
-        output_spec = nest.map_structure(convert_torch_to_keras_tensor, outputs)
+        output_spec = tree.map_structure(convert_torch_to_keras_tensor, outputs)
     return output_spec
 
 
 def cond(pred, true_fn, false_fn):
     # When symbolic execution, take pred as true.
     if get_device() == "meta":
         return true_fn()
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/image.py` & `keras-core-0.1.1/keras_core/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/layer.py` & `keras-core-0.1.1/keras_core/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/math.py` & `keras-core-0.1.1/keras_core/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/nn.py` & `keras-core-0.1.1/keras_core/src/backend/torch/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,23 +463,21 @@
     kernel = _transpose_conv_kernel(kernel)
     kernel_spatial_shape = kernel.shape[2:]
     padding_arg = []
     output_padding_arg = []
     if isinstance(dilation_rate, int):
         dilation_rate = [dilation_rate] * len(kernel_spatial_shape)
     for i, value in enumerate(padding_values):
-        total_padding = value[0] + value[1]
+        both_side_padding = value[0]
+        longer_side_padding = value[1] - value[0]
         padding_arg.append(
             dilation_rate[i] * (kernel_spatial_shape[i] - 1)
-            - total_padding // 2
+            - both_side_padding,
         )
-        if total_padding % 2 == 0:
-            output_padding_arg.append(0)
-        else:
-            output_padding_arg.append(1)
+        output_padding_arg.append(longer_side_padding)
 
     if num_spatial_dims == 1:
         outputs = tnn.conv_transpose1d(
             inputs,
             kernel,
             stride=strides,
             padding=padding_arg,
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/numpy.py` & `keras-core-0.1.1/keras_core/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/random.py` & `keras-core-0.1.1/keras_core/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/rnn.py` & `keras-core-0.1.1/keras_core/src/backend/torch/rnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
-from tensorflow import nest
+import tree
 
 from keras_core.src.backend.torch.core import convert_to_tensor
+from keras_core.src.utils.nest import pack_sequence_as
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -22,17 +23,17 @@
     def swap_batch_timestep(input_t):
         # Swap the batch and timestep dim for the incoming tensor.
         axes = list(range(len(input_t.shape)))
         axes[0], axes[1] = 1, 0
         return torch.permute(input_t, axes)
 
     if not time_major:
-        inputs = nest.map_structure(swap_batch_timestep, inputs)
+        inputs = tree.map_structure(swap_batch_timestep, inputs)
 
-    flattened_inputs = nest.flatten(inputs)
+    flattened_inputs = tree.flatten(inputs)
     time_steps = flattened_inputs[0].shape[0]
     time_steps_t = time_steps
 
     if mask is not None:
         if mask.dtype != torch.bool:
             mask = mask.type(torch.bool)
         if len(mask.shape) == 2:
@@ -40,19 +41,19 @@
         if not time_major:
             mask = swap_batch_timestep(mask)
 
     if constants is None:
         constants = []
 
     def _expand_mask(mask_t, input_t, fixed_dim=1):
-        if nest.is_nested(mask_t):
+        if tree.is_nested(mask_t):
             raise ValueError(
                 f"mask_t is expected to be tensor, but got {mask_t}"
             )
-        if nest.is_nested(input_t):
+        if tree.is_nested(input_t):
             raise ValueError(
                 f"input_t is expected to be tensor, but got {input_t}"
             )
         rank_diff = len(input_t.shape) - len(mask_t.shape)
         for _ in range(rank_diff):
             mask_t = torch.unsqueeze(mask_t, -1)
         multiples = [1] * fixed_dim + list(input_t.shape[fixed_dim:])
@@ -72,24 +73,24 @@
         # the item in tuple is list of the tensor with shape (batch, feature)
         def _process_single_input_t(input_t):
             input_t = torch.unbind(input_t)  # unstack for time_step dim
             if go_backwards:
                 input_t = input_t[::-1]
             return input_t
 
-        if nest.is_nested(inputs):
-            processed_input = nest.map_structure(
+        if tree.is_nested(inputs):
+            processed_input = tree.map_structure(
                 _process_single_input_t, inputs
             )
         else:
             processed_input = (_process_single_input_t(inputs),)
 
         def _get_input_tensor(time):
             inp = [t_[time] for t_ in processed_input]
-            return nest.pack_sequence_as(inputs, inp)
+            return pack_sequence_as(inputs, inp)
 
         if mask is not None:
             mask_list = torch.unbind(mask)
             if go_backwards:
                 mask_list = torch.flip(mask_list, dims=mask_list.shape)
 
             for i in range(time_steps):
@@ -103,26 +104,26 @@
                 if not successive_outputs:
                     prev_output = torch.zeros_like(output)
                 else:
                     prev_output = successive_outputs[-1]
 
                 output = torch.where(tiled_mask_t, output, prev_output)
 
-                flat_states = nest.flatten(states)
-                flat_new_states = nest.flatten(new_states)
+                flat_states = tree.flatten(states)
+                flat_new_states = tree.flatten(new_states)
                 tiled_mask_t = tuple(
                     _expand_mask(mask_t, s) for s in flat_states
                 )
                 flat_final_states = tuple(
                     torch.where(m, s, ps)
                     for m, s, ps in zip(
                         tiled_mask_t, flat_new_states, flat_states
                     )
                 )
-                states = nest.pack_sequence_as(states, flat_final_states)
+                states = pack_sequence_as(states, flat_final_states)
 
                 if return_all_outputs:
                     successive_outputs.append(output)
                     successive_states.append(states)
                 else:
                     successive_outputs = [output]
                     successive_states = [states]
@@ -169,25 +170,25 @@
             list(torch.unbind(input_))
             if not go_backwards
             else list(torch.unbind(torch.flip(input_, [0])))
             for input_ in flattened_inputs
         )
 
         # Get the time(0) input and compute the output for that.
-        input_time_zero = nest.pack_sequence_as(
+        input_time_zero = pack_sequence_as(
             inputs, [inp[0] for inp in flattened_inputs]
         )
         # output_time_zero is used to determine the cell output shape.
         output_time_zero, _ = step_function(
             input_time_zero, tuple(initial_states) + tuple(constants)
         )
 
         output_ta_size = time_steps_t if return_all_outputs else 1
         output_ta = []
-        for out in nest.flatten(output_time_zero):
+        for out in tree.flatten(output_time_zero):
             out_list = list(out)
             if len(out) < output_ta_size:
                 out_list.extend([[]] * (output_ta_size - len(out)))
             output_ta.append(out_list)
 
         time = torch.tensor(0, dtype=torch.int32)
 
@@ -241,15 +242,15 @@
         else:
             masking_fn = None
 
         if masking_fn is not None:
             # Mask for the T output will be base on the output of T - 1. In the
             # case T = 0, a zero filled tensor will be used.
             flat_zero_output = tuple(
-                torch.zeros_like(o) for o in nest.flatten(output_time_zero)
+                torch.zeros_like(o) for o in tree.flatten(output_time_zero)
             )
 
             def _step(time, output_ta_t, prev_output, *states):
                 """RNN step function.
 
                 Args:
                     time: Current timestep value.
@@ -258,37 +259,37 @@
                     *states: List of states.
 
                 Returns:
                     Tuple: `(time + 1, output_ta_t, output) + tuple(new_states)`
                 """
                 current_input = tuple(ta[time] for ta in input_ta)
                 # maybe set shape.
-                current_input = nest.pack_sequence_as(inputs, current_input)
+                current_input = pack_sequence_as(inputs, current_input)
                 mask_t = masking_fn(time)
                 output, new_states = step_function(
                     current_input, tuple(states) + tuple(constants)
                 )
                 # mask output
-                flat_output = nest.flatten(output)
+                flat_output = tree.flatten(output)
                 flat_mask_output = (
                     flat_zero_output
                     if zero_output_for_mask
-                    else nest.flatten(prev_output)
+                    else tree.flatten(prev_output)
                 )
                 flat_new_output = compute_masked_output(
                     mask_t, flat_output, flat_mask_output
                 )
 
                 # mask states
-                flat_state = nest.flatten(states)
-                flat_new_state = nest.flatten(new_states)
+                flat_state = tree.flatten(states)
+                flat_new_state = tree.flatten(new_states)
                 flat_final_state = compute_masked_output(
                     mask_t, flat_new_state, flat_state
                 )
-                new_states = nest.pack_sequence_as(new_states, flat_final_state)
+                new_states = pack_sequence_as(new_states, flat_final_state)
 
                 ta_index_to_write = time if return_all_outputs else 0
                 for ta, out in zip(output_ta_t, flat_new_output):
                     ta[ta_index_to_write] = out
 
                 return (time + 1, output_ta_t, tuple(flat_new_output)) + tuple(
                     new_states
@@ -318,28 +319,26 @@
                     output_ta_t: TensorArray.
                     *states: List of states.
 
                 Returns:
                     Tuple: `(time + 1,output_ta_t) + tuple(new_states)`
                 """
                 current_input = tuple(ta[time] for ta in input_ta)
-                current_input = nest.pack_sequence_as(inputs, current_input)
+                current_input = pack_sequence_as(inputs, current_input)
                 output, new_states = step_function(
                     current_input, tuple(states) + tuple(constants)
                 )
-                flat_new_state = nest.flatten(new_states)
+                flat_new_state = tree.flatten(new_states)
 
-                flat_output = nest.flatten(output)
+                flat_output = tree.flatten(output)
                 ta_index_to_write = time if return_all_outputs else 0
                 for ta, out in zip(output_ta_t, flat_output):
                     ta[ta_index_to_write] = out
 
-                new_states = nest.pack_sequence_as(
-                    initial_states, flat_new_state
-                )
+                new_states = pack_sequence_as(initial_states, flat_new_state)
                 return (time + 1, output_ta_t) + tuple(new_states)
 
             it = 0
             output_ta_t = output_ta
             new_states = states
             while time < time_steps_t and it < max_iterations:
                 final_outputs = _step(time, output_ta_t, *new_states)
@@ -356,19 +355,19 @@
             return torch.stack(max_list)
 
         output_ta = final_outputs[1]
 
         outputs = tuple(_stack(o) for o in output_ta)
         last_output = tuple(o[-1] for o in outputs)
 
-        outputs = nest.pack_sequence_as(output_time_zero, outputs)
-        last_output = nest.pack_sequence_as(output_time_zero, last_output)
+        outputs = pack_sequence_as(output_time_zero, outputs)
+        last_output = pack_sequence_as(output_time_zero, last_output)
 
     if not time_major:
-        outputs = nest.map_structure(swap_batch_timestep, outputs)
+        outputs = tree.map_structure(swap_batch_timestep, outputs)
 
     return last_output, outputs, new_states
 
 
 def lstm(*args, **kwargs):
     raise NotImplementedError
```

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/torch_module_wrapper.py` & `keras-core-0.1.1/keras_core/src/backend/torch/torch_module_wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/backend/torch/trainer.py` & `keras-core-0.1.1/keras_core/src/backend/torch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import warnings
 
 import numpy as np
-import tensorflow as tf
 import torch
+import tree
 
 from keras_core.src import backend
 from keras_core.src import callbacks as callbacks_module
 from keras_core.src import optimizers as optimizers_module
 from keras_core.src.backend.common import standardize_dtype
 from keras_core.src.backend.common.keras_tensor import KerasTensor
 from keras_core.src.backend.torch.core import is_tensor
@@ -39,28 +39,24 @@
         loss = self.compute_loss(
             x=x, y=y, y_pred=y_pred, sample_weight=sample_weight
         )
         self._loss_tracker.update_state(loss)
 
         # Compute gradients
         if self.trainable_weights:
-            # Backpropagation
-            trainable_weights = [v for v in self.trainable_weights]
-
             # Call torch.Tensor.backward() on the loss to compute gradients
             # for the weights.
             loss.backward()
 
+            trainable_weights = self.trainable_weights[:]
             gradients = [v.value.grad for v in trainable_weights]
 
             # Update weights
             with torch.no_grad():
-                self.optimizer.apply_gradients(
-                    zip(gradients, trainable_weights)
-                )
+                self.optimizer.apply(gradients, trainable_weights)
         else:
             warnings.warn("The model does not have any trainable weights.")
 
         return self.compute_metrics(x, y, y_pred, sample_weight=sample_weight)
 
     def test_step(self, data):
         (
@@ -157,15 +153,15 @@
             # Create symbolic tensors matching an input batch.
 
             def to_symbolic_input(v):
                 if is_tensor(v):
                     return KerasTensor(v.shape, standardize_dtype(v.dtype))
                 return v
 
-            data_batch = tf.nest.map_structure(to_symbolic_input, data_batch)
+            data_batch = tree.map_structure(to_symbolic_input, data_batch)
             (
                 x,
                 y,
                 sample_weight,
             ) = data_adapter_utils.unpack_x_y_sample_weight(data_batch)
             # Build all model state with `backend.compute_output_spec`.
             try:
@@ -442,20 +438,20 @@
                 epochs=1,
                 steps=epoch_iterator.num_batches,
                 model=self,
             )
 
         def append_to_outputs(batch_outputs, outputs):
             if outputs is None:
-                outputs = tf.nest.map_structure(
+                outputs = tree.map_structure(
                     lambda batch_output: [batch_output],
                     batch_outputs,
                 )
             else:
-                tf.__internal__.nest.map_structure_up_to(
+                tree.map_structure_up_to(
                     batch_outputs,
                     lambda output, batch_output: output.append(batch_output),
                     outputs,
                     batch_outputs,
                 )
             return outputs
 
@@ -467,18 +463,16 @@
         outputs = None
         for step, data in epoch_iterator.enumerate_epoch(return_type="np"):
             callbacks.on_predict_batch_begin(step)
             batch_outputs = self.predict_function(data)
             outputs = append_to_outputs(batch_outputs, outputs)
             callbacks.on_predict_batch_end(step, {"outputs": batch_outputs})
         callbacks.on_predict_end()
-        outputs = tf.nest.map_structure(backend.convert_to_numpy, outputs)
-        return tf.__internal__.nest.map_structure_up_to(
-            batch_outputs, np.concatenate, outputs
-        )
+        outputs = tree.map_structure(backend.convert_to_numpy, outputs)
+        return tree.map_structure_up_to(batch_outputs, np.concatenate, outputs)
 
     def train_on_batch(
         self,
         x,
         y=None,
         sample_weight=None,
         class_weight=None,
@@ -500,15 +494,15 @@
         data = (x, y, sample_weight)
 
         # Maybe build model
         self._symbolic_build(data)
         self.make_train_function()
 
         logs = self.train_function([data])
-        logs = tf.nest.map_structure(lambda x: np.array(x), logs)
+        logs = tree.map_structure(lambda x: np.array(x), logs)
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     def test_on_batch(
         self,
         x,
@@ -521,20 +515,20 @@
         data = (x, y, sample_weight)
 
         # Maybe build model
         self._symbolic_build(data)
         self.make_test_function()
 
         logs = self.test_function([data])
-        logs = tf.nest.map_structure(lambda x: np.array(x), logs)
+        logs = tree.map_structure(lambda x: np.array(x), logs)
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     def predict_on_batch(self, x):
         self.make_predict_function()
         batch_outputs = self.predict_function((x,))
-        batch_outputs = tf.nest.map_structure(
+        batch_outputs = tree.map_structure(
             backend.convert_to_numpy, batch_outputs
         )
         return batch_outputs
```

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/__init__.py` & `keras-core-0.1.1/keras_core/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/callback.py` & `keras-core-0.1.1/keras_core/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/callback_list.py` & `keras-core-0.1.1/keras_core/src/callbacks/callback_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.callbacks.callback import Callback
 from keras_core.src.callbacks.history import History
 from keras_core.src.callbacks.progbar_logger import ProgbarLogger
 
 
@@ -30,15 +30,15 @@
                 does not already exist in the `callbacks` list.
             add_progbar: Whether a `ProgbarLogger` callback should be added, if
                 one does not already exist in the `callbacks` list.
             model: The `Model` these callbacks are used with.
             **params: If provided, parameters will be passed to each `Callback`
                 via `Callback.set_params`.
         """
-        self.callbacks = nest.flatten(callbacks) if callbacks else []
+        self.callbacks = tree.flatten(callbacks) if callbacks else []
         self._add_default_callbacks(add_history, add_progbar)
 
         if model:
             self.set_model(model)
         if params:
             self.set_params(params)
```

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/csv_logger.py` & `keras-core-0.1.1/keras_core/src/callbacks/csv_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import collections
 import csv
 
 import numpy as np
-from tensorflow.io import gfile
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.callbacks.callback import Callback
 from keras_core.src.utils import file_utils
 
 
 @keras_core_export("keras_core.callbacks.CSVLogger")
@@ -37,21 +36,21 @@
         self.append = append
         self.writer = None
         self.keys = None
         self.append_header = True
 
     def on_train_begin(self, logs=None):
         if self.append:
-            if gfile.exists(self.filename):
-                with gfile.GFile(self.filename, "r") as f:
+            if file_utils.exists(self.filename):
+                with file_utils.File(self.filename, "r") as f:
                     self.append_header = not bool(len(f.readline()))
             mode = "a"
         else:
             mode = "w"
-        self.csv_file = gfile.GFile(self.filename, mode)
+        self.csv_file = file_utils.File(self.filename, mode)
 
     def on_epoch_end(self, epoch, logs=None):
         logs = logs or {}
 
         def handle_value(k):
             is_zero_dim_ndarray = isinstance(k, np.ndarray) and k.ndim == 0
             if isinstance(k, str):
```

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/early_stopping.py` & `keras-core-0.1.1/keras_core/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/history.py` & `keras-core-0.1.1/keras_core/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/lambda_callback.py` & `keras-core-0.1.1/keras_core/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/learning_rate_scheduler.py` & `keras-core-0.1.1/keras_core/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/model_checkpoint.py` & `keras-core-0.1.1/keras_core/src/callbacks/model_checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import re
 import warnings
 
 import numpy as np
-from tensorflow.io import gfile
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.callbacks.callback import Callback
 from keras_core.src.utils import file_utils
 from keras_core.src.utils import io_utils
 
 
@@ -215,16 +214,16 @@
             logs: the `logs` dict passed in to `on_batch_end` or `on_epoch_end`.
         """
         logs = logs or {}
 
         filepath = self._get_file_path(epoch, batch, logs)
         # Create host directory if it doesn't exist.
         dirname = os.path.dirname(filepath)
-        if dirname and not gfile.exists(dirname):
-            gfile.makedirs(dirname)
+        if dirname and not file_utils.exists(dirname):
+            file_utils.makedirs(dirname)
 
         try:
             if self.save_best_only:
                 current = logs.get(self.monitor)
                 if current is None:
                     warnings.warn(
                         f"Can save best model only with {self.monitor} "
@@ -298,15 +297,15 @@
                 f'Failed to format this callback filepath: "{self.filepath}". '
                 f"Reason: {e}"
             )
         return file_path
 
     def _checkpoint_exists(self, filepath):
         """Returns whether the checkpoint `filepath` refers to exists."""
-        return gfile.exists(filepath)
+        return file_utils.exists(filepath)
 
     def _get_most_recently_modified_file_matching_pattern(self, pattern):
         """Returns the most recently modified filepath matching pattern.
 
         In the rare case where there are more than one pattern-matching file
         having the same modified time that is most recent among all, return the
         filepath that is largest (by `>` operator, lexicographically using the
@@ -353,15 +352,15 @@
         base_name_regex = "^" + re.sub(r"{.*}", r".*", base_name) + "$"
 
         latest_mod_time = 0
         file_path_with_latest_mod_time = None
         n_file_with_latest_mod_time = 0
         file_path_with_largest_file_name = None
 
-        if gfile.exists(dir_name):
+        if file_utils.exists(dir_name):
             for file_name in os.listdir(dir_name):
                 # Only consider if `file_name` matches the pattern.
                 if re.match(base_name_regex, file_name):
                     file_path = os.path.join(dir_name, file_name)
                     mod_time = os.path.getmtime(file_path)
                     if (
                         file_path_with_largest_file_name is None
```

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/progbar_logger.py` & `keras-core-0.1.1/keras_core/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/reduce_lr_on_plateau.py` & `keras-core-0.1.1/keras_core/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/remote_monitor.py` & `keras-core-0.1.1/keras_core/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/tensorboard.py` & `keras-core-0.1.1/keras_core/src/callbacks/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import logging
 import os
 import sys
 import time
 import warnings
 
-import tensorflow.summary as summary
-from tensorflow import nest
-from tensorflow.compat.v1 import SummaryMetadata
-from tensorflow.io import gfile
+import tree
 
 from keras_core.src import backend
 from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.callbacks.callback import Callback
 from keras_core.src.layers import Embedding
 from keras_core.src.optimizers import Optimizer
 from keras_core.src.optimizers.schedules import learning_rate_schedule
+from keras_core.src.utils import file_utils
 
 
 @keras_core_export("keras_core.callbacks.TensorBoard")
 class TensorBoard(Callback):
     """Enable visualizations for TensorBoard.
 
     TensorBoard is a visualization tool provided with TensorFlow. A TensorFlow
@@ -167,15 +165,14 @@
         write_graph=True,
         write_images=False,
         write_steps_per_second=False,
         update_freq="epoch",
         profile_batch=0,
         embeddings_freq=0,
         embeddings_metadata=None,
-        **kwargs,
     ):
         super().__init__()
 
         self.log_dir = str(log_dir)
         self.histogram_freq = histogram_freq
         self.write_graph = write_graph
         self.write_images = write_images
@@ -192,14 +189,15 @@
                 f"profile_batch={profile_batch} (must be 0)"
             )
         self._init_profile_batch(profile_batch)
         self._global_train_batch = 0
         self._previous_epoch_iterations = 0
         self._train_accumulated_time = 0
         self._batch_start_time = 0
+        self._summary_module = None
 
         # Lazily initialized in order to avoid creating event files when
         # not needed.
         self._writers = {}
 
         # Used to restore any existing `SummaryWriter` after training ends.
         self._prev_summary_state = []
@@ -221,45 +219,57 @@
         if self.write_graph:
             self._write_keras_model_summary()
             self._should_write_train_graph = True
         if self.embeddings_freq:
             self._configure_embeddings()
 
     @property
+    def summary(self):
+        if self._summary_module is None:
+            import tensorflow.summary as summary
+
+            self._summary_module = summary
+        return self._summary_module
+
+    @property
     def _train_writer(self):
         if "train" not in self._writers:
-            self._writers["train"] = summary.create_file_writer(self._train_dir)
+            self._writers["train"] = self.summary.create_file_writer(
+                self._train_dir
+            )
         return self._writers["train"]
 
     @property
     def _val_writer(self):
         if "val" not in self._writers:
-            self._writers["val"] = summary.create_file_writer(self._val_dir)
+            self._writers["val"] = self.summary.create_file_writer(
+                self._val_dir
+            )
         return self._writers["val"]
 
     def _write_keras_model_train_graph(self):
         """Writes Keras model train_function graph to TensorBoard."""
         with self._train_writer.as_default():
-            with summary.record_if(True):
+            with self.summary.record_if(True):
                 train_fn = self.model.train_function
                 # If the train_function is a `tf.function`, we can write out a
                 # graph
                 if hasattr(train_fn, "function_spec"):
                     # TODO(b/243822285): Use _variable_creation_fn directly.
                     if hasattr(train_fn, "_concrete_stateful_fn"):
-                        summary.graph(train_fn._concrete_stateful_fn.graph)
+                        self.summary.graph(train_fn._concrete_stateful_fn.graph)
                     else:
-                        summary.graph(
+                        self.summary.graph(
                             train_fn._concrete_variable_creation_fn.graph
                         )
 
     def _write_keras_model_summary(self):
         """Writes Keras graph network summary to TensorBoard."""
         with self._train_writer.as_default():
-            with summary.record_if(True):
+            with self.summary.record_if(True):
                 if (
                     self.model.__class__.__name__ == "Functional"
                     or self.model.__class__.__name__ == "Sequential"
                 ):
                     keras_model_summary("keras", self.model, step=0)
 
     def _configure_embeddings(self):
@@ -294,28 +304,28 @@
                 "Unrecognized `Embedding` layer names passed to "
                 "`keras_core.callbacks.TensorBoard` `embeddings_metadata` "
                 f"argument: {self.embeddings_metadata.keys()}"
             )
 
         config_pbtxt = text_format.MessageToString(config)
         path = os.path.join(self._log_write_dir, "projector_config.pbtxt")
-        with gfile.GFile(path, "w") as f:
+        with file_utils.File(path, "w") as f:
             f.write(config_pbtxt)
 
     def _push_writer(self, writer, step):
         """Sets the default writer for custom batch-level summaries."""
         if self.update_freq == "epoch":
             return
 
         def should_record():
             return step % self.update_freq == 0
 
         summary_context = (
             writer.as_default(step),
-            summary.record_if(should_record),
+            self.summary.record_if(should_record),
         )
         self._prev_summary_state.append(summary_context)
         summary_context[0].__enter__()
         summary_context[1].__enter__()
 
     def _pop_writer(self):
         """Pops the current writer."""
@@ -357,15 +367,15 @@
             "signifies a range of batches "
             f"to profile. Found: {profile_batch}"
         )
 
         # Support legacy way of specifying "start,stop" or "start" as str.
         if isinstance(profile_batch, str):
             profile_batch = str(profile_batch).split(",")
-            profile_batch = nest.map_structure(int, profile_batch)
+            profile_batch = tree.map_structure(int, profile_batch)
 
         if isinstance(profile_batch, int):
             self._start_batch = profile_batch
             self._stop_batch = profile_batch
         elif (
             isinstance(profile_batch, (tuple, list)) and len(profile_batch) == 2
         ):
@@ -406,17 +416,17 @@
         self._close_writers()
 
     def on_test_begin(self, logs=None):
         self._push_writer(self._val_writer, self._val_step)
 
     def on_test_end(self, logs=None):
         if self.model.optimizer and hasattr(self.model.optimizer, "iterations"):
-            with summary.record_if(True), self._val_writer.as_default():
+            with self.summary.record_if(True), self._val_writer.as_default():
                 for name, value in logs.items():
-                    summary.scalar(
+                    self.summary.scalar(
                         "evaluation_" + name + "_vs_iterations",
                         value,
                         step=self.model.optimizer.iterations,
                     )
         self._pop_writer()
 
     def _implements_train_batch_hooks(self):
@@ -436,24 +446,26 @@
 
     def on_train_batch_end(self, batch, logs=None):
         if self._should_write_train_graph:
             self._write_keras_model_train_graph()
             self._should_write_train_graph = False
         if self.write_steps_per_second:
             batch_run_time = time.time() - self._batch_start_time
-            summary.scalar(
+            self.summary.scalar(
                 "batch_steps_per_second",
                 1.0 / batch_run_time,
                 step=self._train_step,
             )
 
         # `logs` isn't necessarily always a dict
         if isinstance(logs, dict):
             for name, value in logs.items():
-                summary.scalar("batch_" + name, value, step=self._train_step)
+                self.summary.scalar(
+                    "batch_" + name, value, step=self._train_step
+                )
 
         if not self._should_trace:
             return
 
         if self._is_tracing and self._global_train_batch >= self._stop_batch:
             self._stop_trace()
 
@@ -470,26 +482,26 @@
         if self.histogram_freq and epoch % self.histogram_freq == 0:
             self._log_weights(epoch)
 
         if self.embeddings_freq and epoch % self.embeddings_freq == 0:
             self._log_embeddings(epoch)
 
     def _start_trace(self):
-        summary.trace_on(graph=True, profiler=False)
+        self.summary.trace_on(graph=True, profiler=False)
         self._start_profiler(logdir=self.log_dir)
         self._is_tracing = True
 
     def _stop_trace(self, batch=None):
         """Logs the trace graph to TensorBoard."""
         if batch is None:
             batch = self._stop_batch
         with self._train_writer.as_default():
-            with summary.record_if(True):
+            with self.summary.record_if(True):
                 # TODO(b/126388999): Remove step info in the summary name.
-                summary.trace_export(name="batch_%d" % batch, step=batch)
+                self.summary.trace_export(name="batch_%d" % batch, step=batch)
         self._stop_profiler()
         self._is_tracing = False
 
     def _collect_learning_rate(self, logs):
         if isinstance(self.model.optimizer, Optimizer):
             lr_schedule = getattr(self.model.optimizer, "_learning_rate", None)
         else:
@@ -528,35 +540,35 @@
 
         train_logs = {k: v for k, v in logs.items() if not k.startswith("val_")}
         val_logs = {k: v for k, v in logs.items() if k.startswith("val_")}
         train_logs = self._collect_learning_rate(train_logs)
         if self.write_steps_per_second:
             train_logs["steps_per_second"] = self._compute_steps_per_second()
 
-        with summary.record_if(True):
+        with self.summary.record_if(True):
             if train_logs:
                 with self._train_writer.as_default():
                     for name, value in train_logs.items():
-                        summary.scalar("epoch_" + name, value, step=epoch)
+                        self.summary.scalar("epoch_" + name, value, step=epoch)
             if val_logs:
                 with self._val_writer.as_default():
                     for name, value in val_logs.items():
                         name = name[4:]  # Remove 'val_' prefix.
-                        summary.scalar("epoch_" + name, value, step=epoch)
+                        self.summary.scalar("epoch_" + name, value, step=epoch)
 
     def _log_weights(self, epoch):
         """Logs the weights of the Model to TensorBoard."""
         with self._train_writer.as_default():
-            with summary.record_if(True):
+            with self.summary.record_if(True):
                 for layer in self.model.layers:
                     for weight in layer.weights:
                         weight_name = weight.name.replace(":", "_")
                         # Add a suffix to prevent summary tag name collision.
                         histogram_weight_name = weight_name + "/histogram"
-                        summary.histogram(
+                        self.summary.histogram(
                             histogram_weight_name, weight, step=epoch
                         )
                         if self.write_images:
                             # Add a suffix to prevent summary tag name
                             # collision.
                             image_weight_name = weight_name + "/image"
                             self._log_weight_as_image(
@@ -583,15 +595,15 @@
                 shape = w_img.shape
             w_img = ops.reshape(w_img, [shape[0], shape[1], shape[2], 1])
 
         w_img = backend.convert_to_numpy(w_img)
         shape = w_img.shape
         # Not possible to handle 3D convnets etc.
         if len(shape) == 4 and shape[-1] in [1, 3, 4]:
-            summary.image(weight_name, w_img, step=epoch)
+            self.summary.image(weight_name, w_img, step=epoch)
 
     def _log_embeddings(self, epoch):
         embeddings_ckpt = os.path.join(
             self._log_write_dir,
             "train",
             f"keras_embedding.ckpt-{epoch}.weights.h5",
         )
@@ -648,14 +660,17 @@
         True on success, or False if no summary was written because no default
         summary writer was available.
 
     Raises:
         ValueError: if a default writer exists, but no step was provided and
             `tf.summary.experimental.get_step()` is `None`.
     """
+    import tensorflow.summary as summary
+    from tensorflow.compat.v1 import SummaryMetadata
+
     summary_metadata = SummaryMetadata()
     # Hard coding a plugin name. Please refer to go/tb-plugin-name-hardcode for
     # the rationale.
     summary_metadata.plugin_data.plugin_name = "graph_keras_model"
     # version number = 1
     summary_metadata.plugin_data.content = b"1"
```

### Comparing `keras-core-0.1.0/keras_core/src/callbacks/terminate_on_nan.py` & `keras-core-0.1.1/keras_core/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/constraints/__init__.py` & `keras-core-0.1.1/keras_core/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/constraints/constraints.py` & `keras-core-0.1.1/keras_core/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/california_housing.py` & `keras-core-0.1.1/keras_core/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/cifar.py` & `keras-core-0.1.1/keras_core/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/cifar10.py` & `keras-core-0.1.1/keras_core/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/cifar100.py` & `keras-core-0.1.1/keras_core/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/fashion_mnist.py` & `keras-core-0.1.1/keras_core/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/imdb.py` & `keras-core-0.1.1/keras_core/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/mnist.py` & `keras-core-0.1.1/keras_core/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/datasets/reuters.py` & `keras-core-0.1.1/keras_core/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/initializers/__init__.py` & `keras-core-0.1.1/keras_core/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/initializers/constant_initializers.py` & `keras-core-0.1.1/keras_core/src/initializers/constant_initializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         value: A Python scalar.
     """
 
     def __init__(self, value=0.0):
         self.value = float(value)
 
     def __call__(self, shape, dtype=None):
+        dtype = standardize_dtype(dtype)
         return self.value * ops.ones(shape=shape, dtype=dtype)
 
     def get_config(self):
         return {"value": self.value}
 
 
 @keras_core_export("keras_core.initializers.Zeros")
```

### Comparing `keras-core-0.1.0/keras_core/src/initializers/initializer.py` & `keras-core-0.1.1/keras_core/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/initializers/random_initializers.py` & `keras-core-0.1.1/keras_core/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/__init__.py` & `keras-core-0.1.1/keras_core/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/activations/activation.py` & `keras-core-0.1.1/keras_core/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/activations/elu.py` & `keras-core-0.1.1/keras_core/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/activations/leaky_relu.py` & `keras-core-0.1.1/keras_core/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/activations/prelu.py` & `keras-core-0.1.1/keras_core/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/activations/relu.py` & `keras-core-0.1.1/keras_core/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/activations/softmax.py` & `keras-core-0.1.1/keras_core/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/attention/additive_attention.py` & `keras-core-0.1.1/keras_core/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/attention/attention.py` & `keras-core-0.1.1/keras_core/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/attention/multi_head_attention.py` & `keras-core-0.1.1/keras_core/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/base_conv.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/base_conv_transpose.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/base_depthwise_conv.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/base_separable_conv.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/conv1d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/conv1d_transpose.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/conv2d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/conv2d_transpose.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/conv3d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/conv3d_transpose.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/depthwise_conv1d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/depthwise_conv2d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/separable_conv1d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/convolutional/separable_conv2d.py` & `keras-core-0.1.1/keras_core/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/dense.py` & `keras-core-0.1.1/keras_core/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/einsum_dense.py` & `keras-core-0.1.1/keras_core/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/embedding.py` & `keras-core-0.1.1/keras_core/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/identity.py` & `keras-core-0.1.1/keras_core/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/input_layer.py` & `keras-core-0.1.1/keras_core/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/lambda_layer.py` & `keras-core-0.1.1/keras_core/src/layers/core/lambda_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import types
 
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.saving import serialization_lib
 from keras_core.src.utils import python_utils
 from keras_core.src.utils import shape_utils
@@ -88,27 +88,27 @@
             # Leverage backend shape inference
             try:
                 inputs = shape_utils.map_shape_structure(
                     lambda x: backend.KerasTensor(x, dtype=self.compute_dtype),
                     input_shape,
                 )
                 output_spec = backend.compute_output_spec(self.call, inputs)
-                return nest.map_structure(lambda x: x.shape, output_spec)
+                return tree.map_structure(lambda x: x.shape, output_spec)
             except:
                 raise NotImplementedError(
                     "We could not automatically infer the shape of "
                     "the Lambda's output. Please specify the `output_shape` "
                     "argument for this Lambda layer."
                 )
 
         if callable(self._output_shape):
             return self._output_shape(input_shape)
 
         # Output shapes are passed directly and don't include batch dimension.
-        batch_size = nest.flatten(input_shape)[0]
+        batch_size = tree.flatten(input_shape)[0]
 
         def _add_batch(shape):
             return (batch_size,) + shape
 
         return shape_utils.map_shape_structure(_add_batch, self._output_shape)
 
     def call(self, inputs, mask=None, training=None):
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/masking.py` & `keras-core-0.1.1/keras_core/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/core/wrapper.py` & `keras-core-0.1.1/keras_core/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/input_spec.py` & `keras-core-0.1.1/keras_core/src/layers/input_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 
 
 @keras_core_export(["keras_core.InputSpec", "keras_core.layers.InputSpec"])
 class InputSpec:
@@ -130,15 +130,15 @@
     Raises:
         ValueError: in case of mismatch between
             the provided inputs and the expectations of the layer.
     """
     if not input_spec:
         return
 
-    input_spec = nest.flatten(input_spec)
+    input_spec = tree.flatten(input_spec)
     if isinstance(inputs, dict):
         # Flatten `inputs` by reference order if input spec names are provided
         names = [spec.name for spec in input_spec]
         if all(names):
             list_inputs = []
             for name in names:
                 if name not in inputs:
@@ -147,15 +147,15 @@
                         "You passed a data dictionary with keys "
                         f"{list(inputs.keys())}. "
                         f"Expected the following keys: {names}"
                     )
                 list_inputs.append(inputs[name])
             inputs = list_inputs
 
-    inputs = nest.flatten(inputs)
+    inputs = tree.flatten(inputs)
     if len(input_spec) != len(inputs):
         raise ValueError(
             f"Layer '{layer_name}' expected {len(input_spec)} input(s). "
             f"Received {len(inputs)} instead."
         )
     for x in inputs:
         # Having a shape/dtype is the only commonality of the various
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/layer.py` & `keras-core-0.1.1/keras_core/src/layers/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - RNG seed tracking
 - activity regularization
 """
 import collections
 import inspect
 import warnings
 
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import initializers
 from keras_core.src import mixed_precision
 from keras_core.src import regularizers
 from keras_core.src import utils
 from keras_core.src.api_export import keras_core_export
@@ -40,14 +40,16 @@
 
 if backend.backend() == "tensorflow":
     from keras_core.src.backend.tensorflow.layer import TFLayer as BackendLayer
 elif backend.backend() == "jax":
     from keras_core.src.backend.jax.layer import JaxLayer as BackendLayer
 elif backend.backend() == "torch":
     from keras_core.src.backend.torch.layer import TorchLayer as BackendLayer
+elif backend.backend() == "numpy":
+    from keras_core.src.backend.numpy.layer import NumpyLayer as BackendLayer
 else:
     raise RuntimeError(
         f"Backend '{backend.backend()}' must implement a layer mixin class."
     )
 
 
 @keras_core_export(["keras_core.Layer", "keras_core.layers.Layer"])
@@ -80,16 +82,16 @@
             weight dtype to differ. Default of `None` means to use
             `keras_core.mixed_precision.dtype_policy()`,
             which is a `float32` policy unless set to different value
             (via `keras_core.mixed_precision.set_dtype_policy()`).
 
     Attributes:
         name: The name of the layer (string).
-        dtype: The dtype of the layer's weights.
-        variable_dtype: Dtype of the layer's variables.
+        dtype: Dtype of the layer's weights. Alias of `layer.variable_dtype`.
+        variable_dtype: Dtype of the layer's weights.
         compute_dtype: The dtype of the layer's computations.
             Layers automatically cast inputs to this dtype, which causes
             the computations and output to also be in this dtype.
             When mixed precision is used with a
             `keras_core.mixed_precision.DTypePolicy`, this will be different
             than `variable_dtype`.
         trainable_weights: List of variables to be included in backprop.
@@ -289,20 +291,31 @@
                 ),
                 "seed_generators": (
                     lambda x: isinstance(x, backend.random.SeedGenerator),
                     seed_generators,
                 ),
             }
         )
+        if backend.backend() == "tensorflow":
+            # Remove attribute tracking for lists (TF-specific attribute)
+            _self_setattr_tracking = getattr(
+                self, "_self_setattr_tracking", True
+            )
+            self._self_setattr_tracking = False
+
         self._trainable_variables = trainable_variables
         self._non_trainable_variables = non_trainable_variables
         self._layers = layers
         self._metrics = metrics
         self._seed_generators = seed_generators
 
+        if backend.backend() == "tensorflow":
+            # Reset attribute tracking (TF-specific)
+            self._self_setattr_tracking = _self_setattr_tracking
+
     @property
     def input_spec(self):
         return self._input_spec
 
     @input_spec.setter
     def input_spec(self, value):
         self._input_spec = value
@@ -370,44 +383,40 @@
         initializer,
         dtype=None,
         trainable=True,
         regularizer=None,
         constraint=None,
         name=None,
     ):
-        # TODO: handle layout
-        self._check_super_called()
-        initializer = initializers.get(initializer)
-        variable = backend.Variable(
-            initializer=initializer,
+        """Add a weight variable to the layer.
+
+        Alias of `add_weight()`.
+        """
+        return self.add_weight(
             shape=shape,
-            dtype=dtype or self.variable_dtype,
+            initializer=initializer,
+            dtype=dtype,
             trainable=trainable,
+            regularizer=regularizer,
+            constraint=constraint,
             name=name,
         )
-        # Will be added to layer.losses
-        variable.regularizer = regularizer
-        variable.constraint = constraint
-        self._track_variable(variable)
-        return variable
 
     def add_weight(
         self,
         shape,
         initializer,
         dtype=None,
         trainable=True,
         regularizer=None,
         constraint=None,
         name=None,
     ):
         """Add a weight variable to the layer.
 
-        Alias of `add_variable()`.
-
         Args:
             shape: Shape tuple for the variable.
                 Must be fully-defined (no `None` entries).
             initializer: Initializer object to use to
                 populate the initial variable value,
                 or string name of a built-in initializer
                 (e.g. `"random_normal"`).
@@ -418,23 +427,29 @@
                 updates are managed manually.
             constraint: Contrainst object to call on the
                 variable after any optimizer update,
                 or string name of a built-in constraint.
             name: String name of the variable. Useful
                 for debugging purposes.
         """
-        return self.add_variable(
-            shape=shape,
+        # TODO: handle layout
+        self._check_super_called()
+        initializer = initializers.get(initializer)
+        variable = backend.Variable(
             initializer=initializer,
-            dtype=dtype,
+            shape=shape,
+            dtype=dtype or self.variable_dtype,
             trainable=trainable,
-            regularizer=regularizer,
-            constraint=constraint,
             name=name,
         )
+        # Will be added to layer.losses
+        variable.regularizer = regularizer
+        variable.constraint = constraint
+        self._track_variable(variable)
+        return variable
 
     @property
     def trainable(self):
         """Settable boolean, whether this layer should be trainable or not."""
         return self._trainable
 
     @trainable.setter
@@ -455,17 +470,21 @@
         for v in self._trainable_variables:
             v.trainable = value
         for layer in self._layers:
             layer.trainable = value
 
     @property
     def variables(self):
-        # Return only weights/rng state/metric variables
-        # of all Layers, recursively.
-        # Also deduplicate them.
+        """List of all layer state, including metric variables and random seeds.
+
+        This extends `layer.weights` to include all state used by the layer
+        including state for metrics and `SeedGenerator`s.
+        """
+        # Return all `Variables` associate with the layer including metrics
+        # and random seeds. Also deduplicate them.
         variables = []
         seen_ids = set()
         for v in self._trainable_variables + self._non_trainable_variables:
             if id(v) not in seen_ids:
                 variables.append(v)
                 seen_ids.add(id(v))
         for m in self._metrics:
@@ -477,28 +496,40 @@
                 if id(v) not in seen_ids:
                     variables.append(v)
                     seen_ids.add(id(v))
         return variables
 
     @property
     def trainable_variables(self):
+        """List of all trainable layer state.
+
+        This is equivalent to `layer.trainable_weights`.
+        """
         if not self.trainable:
             return []
         return [v for v in self.variables if v.trainable]
 
     @property
     def non_trainable_variables(self):
+        """List of all non-trainable layer state.
+
+        This extends `layer.non_trainable_weights` to include all state used by
+        the layer including state for metrics and `SeedGenerator`s.
+        """
         if not self.trainable:
             return self.variables
         return [v for v in self.variables if not v.trainable]
 
     @property
     def weights(self):
-        """List of weight variables of the layer."""
-        # Return only "own weights" of all Layers, recursively.
+        """List of all weight variables of the layer.
+
+        Unlike, `layer.variables` this excludes metric state and random seeds.
+        """
+        # Return only `Variables` directly owned by layers and sub-layers.
         # Also deduplicate them.
         weights = []
         seen_ids = set()
         for w in self._trainable_variables + self._non_trainable_variables:
             if id(w) not in seen_ids:
                 weights.append(w)
                 seen_ids.add(id(w))
@@ -507,29 +538,29 @@
                 if id(w) not in seen_ids:
                     weights.append(w)
                     seen_ids.add(id(w))
         return weights
 
     @property
     def trainable_weights(self):
-        """List of trainable weight variables of the layer.
+        """List of all trainable weight variables of the layer.
 
-        These are the weights that get updated by the optimizer
-        during training.
+        These are the weights that get updated by the optimizer during training.
         """
         if not self.trainable:
             return []
         return [v for v in self.weights if v.trainable]
 
     @property
     def non_trainable_weights(self):
-        """List of non-trainable weight variables of the layer.
+        """List of all non-trainable weight variables of the layer.
 
-        Non-trainable weights may include batch normalization statistics,
-        metric variables, or RNG seed variables.
+        These are the weights that should not be updated by the optimizer during
+        training. Unlike, `layer.non_trainable_variables` this excludes metric
+        state and random seeds.
         """
         if not self.trainable:
             return self.weights
         return [v for v in self.weights if not v.trainable]
 
     def get_weights(self):
         """Return the values of `layer.weights` as a list of NumPy arrays."""
@@ -551,15 +582,15 @@
                     "is not compatible with provided weight "
                     f"shape {value.shape}."
                 )
             variable.assign(value)
 
     @property
     def dtype(self):
-        """The dtype of the state (weights) of the layer."""
+        """Alias of `layer.variable_dtype`."""
         return self.variable_dtype
 
     @property
     def compute_dtype(self):
         """The dtype of the computations performed by the layer."""
         return self.dtype_policy.compute_dtype
 
@@ -608,21 +639,21 @@
                     x.dtype = self.compute_dtype
                 return x
             elif hasattr(x, "__array__"):
                 return backend.convert_to_tensor(x, dtype=self.compute_dtype)
             return x
 
         if self._convert_input_args:
-            args = nest.map_structure(maybe_convert, args)
-            kwargs = nest.map_structure(maybe_convert, kwargs)
+            args = tree.map_structure(maybe_convert, args)
+            kwargs = tree.map_structure(maybe_convert, kwargs)
 
         ##########################################################
         # 2. Enforce that only tensors can be passed positionally.
         if not self._allow_non_tensor_positional_args:
-            for arg in nest.flatten(args):
+            for arg in tree.flatten(args):
                 if not isinstance(arg, KerasTensor) and not backend.is_tensor(
                     arg
                 ):
                     raise ValueError(
                         "Only input tensors may be passed as "
                         "positional arguments. The following argument value "
                         f"should be passed as a keyword argument: {arg} "
@@ -671,25 +702,25 @@
         if len(call_spec.tensor_arguments_dict) == 1:
             if (
                 "mask" in call_spec.argument_names
                 and call_spec.arguments_dict["mask"] is None
             ):
                 arg_name = list(call_spec.tensor_arguments_dict.keys())[0]
                 only_tensor_arg = call_spec.tensor_arguments_dict[arg_name]
-                mask = nest.map_structure(
+                mask = tree.map_structure(
                     lambda x: getattr(x, "_keras_mask", None),
                     only_tensor_arg,
                 )
                 kwargs["mask"] = mask
         elif len(call_spec.tensor_arguments_dict) > 1:
             for k, v in call_spec.tensor_arguments_dict.items():
                 expected_mask_arg_name = f"{k}_mask"
                 if expected_mask_arg_name in call_spec.argument_names:
                     if call_spec.arguments_dict[expected_mask_arg_name] is None:
-                        mask = nest.map_structure(
+                        mask = tree.map_structure(
                             lambda x: getattr(x, "_keras_mask", None), v
                         )
                         kwargs[expected_mask_arg_name] = mask
 
         ####################
         # 7. Call the layer.
         try:
@@ -701,15 +732,15 @@
                         outputs = super().__call__(*args, **kwargs)
                 else:
                     outputs = super().__call__(*args, **kwargs)
                 if not self.built:
                     self.built = True
                 # Record activity regularizer loss.
                 if self.activity_regularizer is not None:
-                    for output in nest.flatten(outputs):
+                    for output in tree.flatten(outputs):
                         if backend.is_tensor(output):
                             self.add_loss(self.activity_regularizer(output))
 
             # Set masks on outputs,
             # provided only the first positional input arg and its mask.
             # TODO: consider extending this to all args and kwargs.
             previous_mask = getattr(call_spec.first_arg, "_keras_mask", None)
@@ -894,15 +925,15 @@
             ...
             def call(self, x):
                 self.add_loss(ops.sum(x))
                 return x
         ```
         """
         # Eager only.
-        losses = nest.flatten(loss)
+        losses = tree.flatten(loss)
         for x in losses:
             if not backend.is_tensor(x):
                 raise ValueError(
                     "`add_loss()` can only be called from inside `build()` or "
                     f"`call()`, on a tensor input. Received invalid value: {x}"
                 )
         if backend.in_stateless_scope():
@@ -1060,15 +1091,23 @@
                         if call_spec.eager:
                             # Will let the actual eager call do state-building
                             return
                         raise ValueError(
                             f"Layer '{self.name}' looks like it has "
                             "unbuilt state, but Keras is not able to "
                             "trace the layer `call()` in order to "
-                            "build it automatically. You must implement "
+                            "build it automatically. Possible causes:\n"
+                            "1. The `call()` method of your layer may be "
+                            "crashing. Try to `__call__()` the layer "
+                            "eagerly on some test input "
+                            "first to see if it works. "
+                            "E.g. `x = np.random.random((3, 4)); "
+                            "y = layer(x)`\n"
+                            "2. If the `call()` method is correct, "
+                            "then you may need to implement "
                             "the `def build(self, input_shape)` method on your "
                             "layer. It should create all variables used by the "
                             "layer (e.g. by calling `layer.build()` on all its "
                             "children layers)."
                         )
             self.built = True
 
@@ -1189,30 +1228,36 @@
             layers.append(layer)
             # Introspect recursively through sublayers.
             if recursive:
                 deque.extendleft(layer._layers)
         return layers
 
     def _set_mask_metadata(self, inputs, outputs, previous_mask):
-        flat_outputs = nest.flatten(outputs)
+        flat_outputs = tree.flatten(outputs)
 
         mask_already_computed = all(
             getattr(x, "_keras_mask", None) is not None for x in flat_outputs
         )
         if mask_already_computed:
             return
 
         output_masks = self.compute_mask(inputs, previous_mask)
         if output_masks is None:
             return
 
-        flat_masks = nest.flatten(output_masks)
+        flat_masks = tree.flatten(output_masks)
         for tensor, mask in zip(flat_outputs, flat_masks):
             if getattr(tensor, "_keras_mask", None) is None:
                 try:
+                    # Numpy backend does not support masking.
+                    if backend.backend() == "numpy":
+                        warnings.warn(
+                            "The NumPy backend does not support masking at this"
+                            "time. Masks will be ignored."
+                        )
                     tensor._keras_mask = mask
                 except AttributeError:
                     # It's a C type.
                     pass
 
     @python_utils.default
     def get_config(self):
@@ -1255,16 +1300,16 @@
         for name, value in bound_args.arguments.items():
             arg_dict[name] = value
             arg_names.append(name)
             if is_backend_tensor_or_symbolic(value):
                 tensor_args.append(value)
                 tensor_arg_names.append(name)
                 tensor_arg_dict[name] = value
-            elif nest.is_nested(value):
-                flat_values = nest.flatten(value)
+            elif tree.is_nested(value):
+                flat_values = tree.flatten(value)
                 if all(is_backend_tensor_or_symbolic(x) for x in flat_values):
                     tensor_args.append(value)
                     tensor_arg_names.append(name)
                     tensor_arg_dict[name] = value
                     nested_tensor_arg_names.append(name)
                 elif any(is_backend_tensor_or_symbolic(x) for x in flat_values):
                     raise ValueError(
@@ -1312,15 +1357,15 @@
         if k == "mask" or k.startswith("mask_"):
             # Do not include mask tensors in shapes dict
             continue
         if k == "kwargs" or k == "args":
             # Do not include catch-alls in shapes dict
             continue
         if k in call_spec.nested_tensor_argument_names:
-            shapes_dict[f"{k}_shape"] = nest.map_structure(
+            shapes_dict[f"{k}_shape"] = tree.map_structure(
                 lambda x: backend.standardize_shape(x.shape), v
             )
         else:
             shapes_dict[f"{k}_shape"] = backend.standardize_shape(v.shape)
     return shapes_dict
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/add.py` & `keras-core-0.1.1/keras_core/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/average.py` & `keras-core-0.1.1/keras_core/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/base_merge.py` & `keras-core-0.1.1/keras_core/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/concatenate.py` & `keras-core-0.1.1/keras_core/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/dot.py` & `keras-core-0.1.1/keras_core/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/maximum.py` & `keras-core-0.1.1/keras_core/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/minimum.py` & `keras-core-0.1.1/keras_core/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/multiply.py` & `keras-core-0.1.1/keras_core/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/merging/subtract.py` & `keras-core-0.1.1/keras_core/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/normalization/batch_normalization.py` & `keras-core-0.1.1/keras_core/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/normalization/group_normalization.py` & `keras-core-0.1.1/keras_core/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/normalization/layer_normalization.py` & `keras-core-0.1.1/keras_core/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/normalization/spectral_normalization.py` & `keras-core-0.1.1/keras_core/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/normalization/unit_normalization.py` & `keras-core-0.1.1/keras_core/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/average_pooling1d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/average_pooling2d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/average_pooling3d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/base_global_pooling.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/base_pooling.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/global_average_pooling1d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/global_average_pooling2d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/global_average_pooling3d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/global_max_pooling1d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/global_max_pooling2d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/global_max_pooling3d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/max_pooling1d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/max_pooling2d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/pooling/max_pooling3d.py` & `keras-core-0.1.1/keras_core/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/category_encoding.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/category_encoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import tensorflow as tf
-
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.CategoryEncoding")
 class CategoryEncoding(Layer):
     """A preprocessing layer which encodes integer features.
 
     This layer provides options for condensing data into a categorical encoding
@@ -81,14 +80,20 @@
         inputs: A 1D or 2D tensor of integer inputs.
         count_weights: A tensor in the same shape as `inputs` indicating the
             weight for each sample value when summing up in `count` mode.
             Not used in `"multi_hot"` or `"one_hot"` modes.
     """
 
     def __init__(self, num_tokens=None, output_mode="multi_hot", **kwargs):
+        if not tf.available:
+            raise ImportError(
+                "Layer CategoryEncoding requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(**kwargs)
 
         # Support deprecated names for output_modes.
         if output_mode == "binary":
             output_mode = "multi_hot"
         # 'output_mode' must be one of ("count", "one_hot", "multi_hot")
         if output_mode not in ("count", "one_hot", "multi_hot"):
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/center_crop.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/discretization.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/discretization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.Discretization")
 class Discretization(Layer):
     """A preprocessing layer which buckets continuous features by ranges.
 
     This layer will place each element of its input data into one of several
@@ -99,14 +99,20 @@
         epsilon=0.01,
         output_mode="int",
         sparse=False,
         name=None,
         dtype=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer Discretization requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name, dtype=dtype)
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
                 "`sparse` can only be set to True with the "
                 "TensorFlow backend."
             )
         self.layer = tf.keras.layers.Discretization(
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/feature_space.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/feature_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from tensorflow import data as tf_data
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import layers
 from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.saving import saving_lib
@@ -500,14 +499,16 @@
                 if preprocessor.input_mean is not None:
                     continue
             if hasattr(preprocessor, "adapt"):
                 adaptable_preprocessors.append(name)
         return adaptable_preprocessors
 
     def adapt(self, dataset):
+        from tensorflow import data as tf_data
+
         if not isinstance(dataset, tf_data.Dataset):
             raise ValueError(
                 "`adapt()` can only be called on a tf.data.Dataset. "
                 f"Received instead: {dataset} (of type {type(dataset)})"
             )
 
         for name in self._list_adaptable_preprocessors():
@@ -610,16 +611,16 @@
         all_specs = [
             self.features[name] for name in self._preprocessed_features_names
         ] + [
             self.crosses_by_name[name] for name in self._crossed_features_names
         ]
 
         for name, feature, spec in zip(all_names, all_features, all_specs):
-            if nest.is_nested(feature):
-                dtype = nest.flatten(feature)[0].dtype
+            if tree.is_nested(feature):
+                dtype = tree.flatten(feature)[0].dtype
             else:
                 dtype = feature.dtype
             dtype = backend.standardize_dtype(dtype)
 
             if spec.output_mode == "one_hot":
                 preprocessor = self.preprocessors.get(
                     name
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/hashed_crossing.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/hashed_crossing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import tensorflow as tf
-
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.HashedCrossing")
 class HashedCrossing(Layer):
     """A preprocessing layer which crosses features using the "hashing trick".
 
     This layer performs crosses of categorical features using the "hashing
@@ -72,14 +71,20 @@
         num_bins,
         output_mode="int",
         sparse=False,
         name=None,
         dtype=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer HashedCrossing requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         if output_mode == "int" and dtype is None:
             dtype = "int64"
         super().__init__(name=name, dtype=dtype)
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
                 "`sparse` can only be set to True with the "
                 "TensorFlow backend."
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/hashing.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/hashing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.Hashing")
 class Hashing(Layer):
     """A preprocessing layer which hashes and bins categorical features.
 
     This layer transforms categorical inputs to hashed output. It element-wise
@@ -140,14 +140,20 @@
         mask_value=None,
         salt=None,
         output_mode="int",
         sparse=False,
         name=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer Hashing requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name)
         self.layer = tf.keras.layers.Hashing(
             num_bins=num_bins,
             mask_value=mask_value,
             salt=salt,
             output_mode=output_mode,
             sparse=sparse,
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/integer_lookup.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/integer_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.IntegerLookup")
 class IntegerLookup(Layer):
     """A preprocessing layer that maps integers to (possibly encoded) indices.
 
     This layer maps a set of arbitrary integer input tokens into indexed integer
@@ -306,14 +306,20 @@
         invert=False,
         output_mode="int",
         sparse=False,
         pad_to_max_tokens=False,
         name=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer IntegerLookup requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name)
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
                 "`sparse` can only be set to True with the "
                 "TensorFlow backend."
             )
         self.layer = tf.keras.layers.IntegerLookup(
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/normalization.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import math
 
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.Normalization")
 class Normalization(Layer):
     """A preprocessing layer that normalizes continuous features.
 
     This layer will shift and scale inputs into a distribution centered around
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_brightness.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_contrast.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_crop.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_crop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.RandomCrop")
 class RandomCrop(Layer):
     """A preprocessing layer which randomly crops images during training.
 
     During training, this layer will randomly choose a location to crop images
@@ -49,14 +49,20 @@
         width: Integer, the width of the output shape.
         seed: Integer. Used to create a random seed.
         **kwargs: Base layer keyword arguments, such as
             `name` and `dtype`.
     """
 
     def __init__(self, height, width, seed=None, name=None, **kwargs):
+        if not tf.available:
+            raise ImportError(
+                "Layer RandomCrop requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name, **kwargs)
         self.seed = seed or backend.random.make_default_seed()
         self.layer = tf.keras.layers.RandomCrop(
             height=height,
             width=width,
             seed=self.seed,
             name=name,
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_flip.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_flip.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 HORIZONTAL = "horizontal"
 VERTICAL = "vertical"
 HORIZONTAL_AND_VERTICAL = "horizontal_and_vertical"
 
 
 @keras_core_export("keras_core.layers.RandomFlip")
@@ -42,14 +42,20 @@
         **kwargs: Base layer keyword arguments, such as
             `name` and `dtype`.
     """
 
     def __init__(
         self, mode=HORIZONTAL_AND_VERTICAL, seed=None, name=None, **kwargs
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer RandomFlip requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name)
         self.seed = seed or backend.random.make_default_seed()
         self.layer = tf.keras.layers.RandomFlip(
             mode=mode,
             name=name,
             seed=self.seed,
             **kwargs,
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_rotation.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_rotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.RandomRotation")
 class RandomRotation(Layer):
     """A preprocessing layer which randomly rotates images during training.
 
     This layer will apply random rotations to each image, filling empty space
@@ -82,14 +82,20 @@
         fill_mode="reflect",
         interpolation="bilinear",
         seed=None,
         fill_value=0.0,
         name=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer RandomRotation requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name, **kwargs)
         self.seed = seed or backend.random.make_default_seed()
         self.layer = tf.keras.layers.RandomRotation(
             factor=factor,
             fill_mode=fill_mode,
             interpolation=interpolation,
             seed=self.seed,
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_translation.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_translation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.RandomTranslation")
 class RandomTranslation(Layer):
     """A preprocessing layer which randomly translates images during training.
 
     This layer will apply random translations to each image during training,
@@ -72,14 +72,20 @@
         fill_mode="reflect",
         interpolation="bilinear",
         seed=None,
         fill_value=0.0,
         name=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer RandomTranslation requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name)
         self.layer = tf.keras.layers.RandomTranslation(
             height_factor=height_factor,
             width_factor=width_factor,
             fill_mode=fill_mode,
             interpolation=interpolation,
             seed=seed,
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/random_zoom.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/random_zoom.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.RandomZoom")
 class RandomZoom(Layer):
     """A preprocessing layer which randomly zooms images during training.
 
     This layer will randomly zoom in or out on each axis of an image
@@ -94,14 +94,20 @@
         fill_mode="reflect",
         interpolation="bilinear",
         seed=None,
         fill_value=0.0,
         name=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer RandomZoom requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name, **kwargs)
         self.seed = seed or backend.random.make_default_seed()
         self.layer = tf.keras.layers.RandomZoom(
             height_factor=height_factor,
             width_factor=width_factor,
             fill_mode=fill_mode,
             interpolation=interpolation,
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/rescaling.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/resizing.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/string_lookup.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/string_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.StringLookup")
 class StringLookup(Layer):
     """A preprocessing layer that maps strings to (possibly encoded) indices.
 
     This layer translates a set of arbitrary strings into integer output via a
@@ -304,14 +304,20 @@
         pad_to_max_tokens=False,
         sparse=False,
         encoding="utf-8",
         name=None,
         dtype=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer StringLookup requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         if output_mode == "int" and dtype is None:
             dtype = "int64"
         super().__init__(name=name)
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
                 "`sparse` can only be set to True with the "
                 "TensorFlow backend."
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/text_vectorization.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/text_vectorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.saving import serialization_lib
 from keras_core.src.utils import backend_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.layers.TextVectorization")
 class TextVectorization(Layer):
     """A preprocessing layer which maps text features to integer sequences.
 
     This layer has basic options for managing text in a Keras model. It
@@ -209,14 +209,20 @@
         idf_weights=None,
         sparse=False,
         ragged=False,
         encoding="utf-8",
         name=None,
         **kwargs,
     ):
+        if not tf.available:
+            raise ImportError(
+                "Layer TextVectorization requires TensorFlow. "
+                "Install it via `pip install tensorflow`."
+            )
+
         super().__init__(name=name)
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
                 "`sparse` can only be set to True with the "
                 "TensorFlow backend."
             )
         if ragged and backend.backend() != "tensorflow":
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/preprocessing/tf_data_layer.py` & `keras-core-0.1.1/keras_core/src/layers/preprocessing/tf_data_layer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from tensorflow import nest
+import tree
 
-from keras_core.src import backend
+import keras_core.src.backend
 from keras_core.src.layers.layer import Layer
 from keras_core.src.random.seed_generator import SeedGenerator
 from keras_core.src.utils import backend_utils
 from keras_core.src.utils import tracking
 
 
 class TFDataLayer(Layer):
@@ -18,19 +18,19 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.backend = backend_utils.DynamicBackend()
         self._allow_non_tensor_positional_args = True
 
     def __call__(self, inputs, **kwargs):
         if backend_utils.in_tf_graph() and not isinstance(
-            inputs, backend.KerasTensor
+            inputs, keras_core.backend.KerasTensor
         ):
             # We're in a TF graph, e.g. a tf.data pipeline.
             self.backend.set_backend("tensorflow")
-            inputs = nest.map_structure(
+            inputs = tree.map_structure(
                 lambda x: self.backend.convert_to_tensor(
                     x, dtype=self.compute_dtype
                 ),
                 inputs,
             )
             switch_convert_input_args = False
             if self._convert_input_args:
@@ -43,15 +43,15 @@
                 if switch_convert_input_args:
                     self._convert_input_args = True
             return outputs
         return super().__call__(inputs, **kwargs)
 
     @tracking.no_automatic_dependency_tracking
     def _get_seed_generator(self, backend=None):
-        if backend is None or backend == self.backend._backend:
+        if backend is None or backend == keras_core.backend.backend():
             return self.generator
         if not hasattr(self, "_backend_generators"):
             self._backend_generators = {}
         if backend in self._backend_generators:
             return self._backend_generators[backend]
         seed_generator = SeedGenerator(self.seed, backend=self.backend)
         self._backend_generators[backend] = seed_generator
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/regularization/activity_regularization.py` & `keras-core-0.1.1/keras_core/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/regularization/alpha_dropout.py` & `keras-core-0.1.1/keras_core/src/layers/regularization/dropout.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from keras_core.src import backend
-from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 
 
-@keras_core_export("keras_core.layers.AlphaDropout")
-class AlphaDropout(Layer):
-    """Applies Alpha Dropout to the input.
-
-    Alpha Dropout is a kind of dropout that keeps mean and variance of inputs
-    to their original values, in order to ensure the self-normalizing property
-    even after this dropout.
-    Alpha Dropout fits well to Scaled Exponential Linear Units
-    by randomly setting activations to the negative saturation value.
+@keras_core_export("keras_core.layers.Dropout")
+class Dropout(Layer):
+    """Applies dropout to the input.
+
+    The `Dropout` layer randomly sets input units to 0 with a frequency of
+    `rate` at each step during training time, which helps prevent overfitting.
+    Inputs not set to 0 are scaled up by `1 / (1 - rate)` such that the sum over
+    all inputs is unchanged.
+
+    Note that the `Dropout` layer only applies when `training` is set to `True`
+    in `call()`, such that no values are dropped during inference.
+    When using `model.fit`, `training` will be appropriately set to `True`
+    automatically. In other contexts, you can set the argument explicitly
+    to `True` when calling the layer.
+
+    (This is in contrast to setting `trainable=False` for a `Dropout` layer.
+    `trainable` does not affect the layer's behavior, as `Dropout` does
+    not have any variables/weights that can be frozen during training.)
 
     Args:
-        rate: float, drop probability (as with `Dropout`).
-            The multiplicative noise will have
-            standard deviation `sqrt(rate / (1 - rate))`.
+        rate: Float between 0 and 1. Fraction of the input units to drop.
         noise_shape: 1D integer tensor representing the shape of the
             binary dropout mask that will be multiplied with the input.
             For instance, if your inputs have shape
             `(batch_size, timesteps, features)` and
             you want the dropout mask to be the same for all timesteps,
             you can use `noise_shape=(batch_size, 1, features)`.
         seed: A Python integer to use as random seed.
@@ -30,45 +36,35 @@
         inputs: Input tensor (of any rank).
         training: Python boolean indicating whether the layer should behave in
             training mode (adding dropout) or in inference mode (doing nothing).
     """
 
     def __init__(self, rate, noise_shape=None, seed=None, **kwargs):
         super().__init__(**kwargs)
+        if not 0 <= rate <= 1:
+            raise ValueError(
+                f"Invalid value received for argument "
+                "`rate`. Expected a float value between 0 and 1. "
+                f"Received: rate={rate}"
+            )
         self.rate = rate
-        self.noise_shape = noise_shape
         self.seed = seed
+        self.noise_shape = noise_shape
         self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
+        self.built = True
 
     def call(self, inputs, training=False):
-        if training and 0.0 < self.rate < 1.0:
-            alpha = 1.6732632423543772848170429916717
-            scale = 1.0507009873554804934193349852946
-            alpha_p = -alpha * scale
-
-            noise_shape = (
-                self.noise_shape if self.noise_shape else ops.shape(inputs)
-            )
-
-            kept_idx = ops.greater_equal(
-                backend.random.uniform(noise_shape, seed=self.seed_generator),
+        if training and self.rate > 0:
+            return backend.random.dropout(
+                inputs,
                 self.rate,
+                noise_shape=self.noise_shape,
+                seed=self.seed_generator,
             )
-            kept_idx = ops.cast(kept_idx, dtype=inputs.dtype)
-
-            # Get affine transformation params
-            a = ((1 - self.rate) * (1 + self.rate * alpha_p**2)) ** -0.5
-            b = -a * alpha_p * self.rate
-
-            # Apply mask
-            x = inputs * kept_idx + alpha_p * (1 - kept_idx)
-
-            # Do affine transformation
-            return a * x + b
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/regularization/dropout.py` & `keras-core-0.1.1/keras_core/src/layers/regularization/gaussian_dropout.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,61 @@
+import math
+
 from keras_core.src import backend
+from keras_core.src import layers
+from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
-from keras_core.src.layers.layer import Layer
 
 
-@keras_core_export("keras_core.layers.Dropout")
-class Dropout(Layer):
-    """Applies dropout to the input.
-
-    The `Dropout` layer randomly sets input units to 0 with a frequency of
-    `rate` at each step during training time, which helps prevent overfitting.
-    Inputs not set to 0 are scaled up by `1 / (1 - rate)` such that the sum over
-    all inputs is unchanged.
-
-    Note that the `Dropout` layer only applies when `training` is set to `True`
-    in `call()`, such that no values are dropped during inference.
-    When using `model.fit`, `training` will be appropriately set to `True`
-    automatically. In other contexts, you can set the argument explicitly
-    to `True` when calling the layer.
-
-    (This is in contrast to setting `trainable=False` for a `Dropout` layer.
-    `trainable` does not affect the layer's behavior, as `Dropout` does
-    not have any variables/weights that can be frozen during training.)
+@keras_core_export("keras_core.layers.GaussianDropout")
+class GaussianDropout(layers.Layer):
+    """Apply multiplicative 1-centered Gaussian noise.
+
+    As it is a regularization layer, it is only active at training time.
 
     Args:
-        rate: Float between 0 and 1. Fraction of the input units to drop.
-        noise_shape: 1D integer tensor representing the shape of the
-            binary dropout mask that will be multiplied with the input.
-            For instance, if your inputs have shape
-            `(batch_size, timesteps, features)` and
-            you want the dropout mask to be the same for all timesteps,
-            you can use `noise_shape=(batch_size, 1, features)`.
-        seed: A Python integer to use as random seed.
+        rate: Float, drop probability (as with `Dropout`).
+            The multiplicative noise will have
+            standard deviation `sqrt(rate / (1 - rate))`.
+        seed: Integer, optional random seed to enable deterministic behavior.
 
     Call arguments:
         inputs: Input tensor (of any rank).
         training: Python boolean indicating whether the layer should behave in
             training mode (adding dropout) or in inference mode (doing nothing).
     """
 
-    def __init__(self, rate, noise_shape=None, seed=None, **kwargs):
+    def __init__(self, rate, seed=None, **kwargs):
         super().__init__(**kwargs)
         if not 0 <= rate <= 1:
             raise ValueError(
                 f"Invalid value received for argument "
                 "`rate`. Expected a float value between 0 and 1. "
                 f"Received: rate={rate}"
             )
         self.rate = rate
         self.seed = seed
-        self.noise_shape = noise_shape
         self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
-        self.built = True
 
     def call(self, inputs, training=False):
         if training and self.rate > 0:
-            return backend.random.dropout(
-                inputs,
-                self.rate,
-                noise_shape=self.noise_shape,
+            stddev = math.sqrt(self.rate / (1.0 - self.rate))
+            return inputs * backend.random.normal(
+                shape=ops.shape(inputs),
+                mean=1.0,
+                stddev=stddev,
                 seed=self.seed_generator,
             )
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
-            "noise_shape": self.noise_shape,
         }
         return {**base_config, **config}
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/regularization/gaussian_noise.py` & `keras-core-0.1.1/keras_core/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/regularization/spatial_dropout.py` & `keras-core-0.1.1/keras_core/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/cropping1d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/cropping2d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/cropping3d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/flatten.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/permute.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/repeat_vector.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/reshape.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/up_sampling1d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/up_sampling2d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/up_sampling3d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/zero_padding1d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/zero_padding2d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/reshaping/zero_padding3d.py` & `keras-core-0.1.1/keras_core/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/bidirectional.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import activations
 from keras_core.src import backend
 from keras_core.src import constraints
 from keras_core.src import initializers
 from keras_core.src import ops
 from keras_core.src import regularizers
@@ -545,15 +545,15 @@
 
         if self.return_state:
             batched_state_shape = (batch_size,) + state_shape
             return output_shape, batched_state_shape, batched_state_shape
         return output_shape
 
     def compute_mask(self, _, mask):
-        mask = nest.flatten(mask)[0]
+        mask = tree.flatten(mask)[0]
         output_mask = mask if self.return_sequences else None
         if self.return_state:
             state_mask = [None, None]
             return [output_mask] + state_mask
         else:
             return output_mask
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm1d.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm2d.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/conv_lstm3d.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/dropout_rnn_cell.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/gru.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/gru.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import activations
 from keras_core.src import backend
 from keras_core.src import constraints
 from keras_core.src import initializers
 from keras_core.src import ops
 from keras_core.src import regularizers
@@ -175,15 +175,15 @@
             )
         else:
             self.bias = None
         self.built = True
 
     def call(self, inputs, states, training=False):
         h_tm1 = (
-            states[0] if nest.is_nested(states) else states
+            states[0] if tree.is_nested(states) else states
         )  # previous state
 
         dp_mask = self.get_dropout_mask(inputs)
         rec_dp_mask = self.get_recurrent_dropout_mask(h_tm1)
 
         if self.use_bias:
             if not self.reset_after:
@@ -280,15 +280,15 @@
                     r * h_tm1, self.recurrent_kernel[:, 2 * self.units :]
                 )
 
             hh = self.activation(x_h + recurrent_h)
 
         # previous and candidate state mixed by update gate
         h = z * h_tm1 + (1 - z) * hh
-        new_state = [h] if nest.is_nested(states) else h
+        new_state = [h] if tree.is_nested(states) else h
         return h, new_state
 
     def get_config(self):
         config = {
             "units": self.units,
             "activation": activations.serialize(self.activation),
             "recurrent_activation": activations.serialize(
@@ -507,39 +507,44 @@
             unroll=unroll,
             activity_regularizer=activity_regularizer,
             **kwargs,
         )
         self.input_spec = InputSpec(ndim=3)
 
     def inner_loop(self, sequences, initial_state, mask, training=False):
-        if nest.is_nested(initial_state):
+        if tree.is_nested(initial_state):
             initial_state = initial_state[0]
-        if nest.is_nested(mask):
+        if tree.is_nested(mask):
             mask = mask[0]
 
         if not self.dropout and not self.recurrent_dropout:
             try:
                 # Backends are allowed to specify (optionally) optimized
                 # implementation of the inner GRU loop. In the case of
                 # TF for instance, it will leverage cuDNN when feasible, and
                 # it will raise NotImplementedError otherwise.
-                return backend.gru(
+                out = backend.gru(
                     sequences,
                     initial_state,
                     mask,
                     kernel=self.cell.kernel,
                     recurrent_kernel=self.cell.recurrent_kernel,
                     bias=self.cell.bias,
                     activation=self.cell.activation,
                     recurrent_activation=self.cell.recurrent_activation,
                     return_sequences=self.return_sequences,
                     go_backwards=self.go_backwards,
                     unroll=self.unroll,
                     reset_after=self.cell.reset_after,
                 )
+                # We disable jit_compile for the model in this case,
+                # since cuDNN ops aren't XLA compatible.
+                if backend.backend() == "tensorflow":
+                    self.supports_jit = False
+                return out
             except NotImplementedError:
                 pass
         return super().inner_loop(
             sequences, initial_state, mask=mask, training=training
         )
 
     def call(self, sequences, initial_state=None, mask=None, training=False):
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/lstm.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/lstm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import activations
 from keras_core.src import backend
 from keras_core.src import constraints
 from keras_core.src import initializers
 from keras_core.src import ops
 from keras_core.src import regularizers
@@ -489,37 +489,42 @@
             unroll=unroll,
             activity_regularizer=activity_regularizer,
             **kwargs,
         )
         self.input_spec = InputSpec(ndim=3)
 
     def inner_loop(self, sequences, initial_state, mask, training=False):
-        if nest.is_nested(mask):
+        if tree.is_nested(mask):
             mask = mask[0]
 
         if not self.dropout and not self.recurrent_dropout:
             try:
                 # Backends are allowed to specify (optionally) optimized
                 # implementation of the inner LSTM loop. In the case of
                 # TF for instance, it will leverage cuDNN when feasible, and
                 # it will raise NotImplementedError otherwise.
-                return backend.lstm(
+                out = backend.lstm(
                     sequences,
                     initial_state[0],
                     initial_state[1],
                     mask,
                     kernel=self.cell.kernel,
                     recurrent_kernel=self.cell.recurrent_kernel,
                     bias=self.cell.bias,
                     activation=self.cell.activation,
                     recurrent_activation=self.cell.recurrent_activation,
                     return_sequences=self.return_sequences,
                     go_backwards=self.go_backwards,
                     unroll=self.unroll,
                 )
+                # We disable jit_compile for the model in this case,
+                # since cuDNN ops aren't XLA compatible.
+                if backend.backend() == "tensorflow":
+                    self.supports_jit = False
+                return out
             except NotImplementedError:
                 pass
         return super().inner_loop(
             sequences, initial_state, mask=mask, training=training
         )
 
     def call(self, sequences, initial_state=None, mask=None, training=False):
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/rnn.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras_core.src.saving import serialization_lib
@@ -255,15 +255,15 @@
         return output_shape
 
     def compute_mask(self, _, mask):
         # Time step masks must be the same for each input.
         # This is because the mask for an RNN is of size [batch, time_steps, 1],
         # and specifies which time steps should be skipped, and a time step
         # must be skipped for all inputs.
-        mask = nest.flatten(mask)[0]
+        mask = tree.flatten(mask)[0]
         output_mask = mask if self.return_sequences else None
         if self.return_state:
             state_mask = [None for _ in self.state_size]
             return [output_mask] + state_mask
         else:
             return output_mask
 
@@ -284,15 +284,15 @@
                         f"batch size: sequence.shape={sequences_shape}"
                     )
                 self._create_state_variables(sequences_shape[0])
         self.built = True
 
     @tracking.no_automatic_dependency_tracking
     def _create_state_variables(self, batch_size):
-        self.states = nest.map_structure(
+        self.states = tree.map_structure(
             lambda value: backend.Variable(
                 value, trainable=False, dtype=self.variable_dtype
             ),
             self.get_initial_state(batch_size),
         )
 
     def get_initial_state(self, batch_size):
@@ -302,15 +302,15 @@
         else:
             return [
                 ops.zeros((batch_size, d), dtype=self.compute_dtype)
                 for d in self.state_size
             ]
 
         # RNN expect the states in a list, even if single state.
-        if not nest.is_nested(init_state):
+        if not tree.is_nested(init_state):
             init_state = [init_state]
         # Force the state to be a list in case it is a namedtuple eg
         # LSTMStateTuple.
         return list(init_state)
 
     def reset_states(self):
         # Compatibility alias.
@@ -324,19 +324,19 @@
     def inner_loop(self, sequences, initial_state, mask, training=False):
         cell_kwargs = {}
         if isinstance(self.cell, Layer) and self.cell._call_has_training_arg():
             cell_kwargs["training"] = training
 
         def step(inputs, states):
             output, new_states = self.cell(inputs, states, **cell_kwargs)
-            if not nest.is_nested(new_states):
+            if not tree.is_nested(new_states):
                 new_states = [new_states]
             return output, new_states
 
-        if not nest.is_nested(initial_state):
+        if not tree.is_nested(initial_state):
             initial_state = [initial_state]
 
         return backend.rnn(
             step,
             sequences,
             initial_state,
             go_backwards=self.go_backwards,
@@ -371,37 +371,37 @@
             if self.stateful:
                 initial_state = self.states
             else:
                 initial_state = self.get_initial_state(
                     batch_size=ops.shape(sequences)[0]
                 )
         # RNN expect the states in a list, even if single state.
-        if not nest.is_nested(initial_state):
+        if not tree.is_nested(initial_state):
             initial_state = [initial_state]
         initial_state = list(initial_state)
 
         # Cast states to compute dtype.
         # Note that states may be deeply nested
         # (e.g. in the stacked cells case).
-        initial_state = nest.map_structure(
+        initial_state = tree.map_structure(
             lambda x: backend.convert_to_tensor(x, dtype=self.compute_dtype),
             initial_state,
         )
 
         last_output, outputs, states = self.inner_loop(
             sequences=sequences,
             initial_state=initial_state,
             mask=mask,
             training=training,
         )
         self._maybe_reset_dropout_masks(self.cell)
 
         if self.stateful:
             for self_state, state in zip(
-                nest.flatten(self.states), nest.flatten(states)
+                tree.flatten(self.states), tree.flatten(states)
             ):
                 self_state.assign(state)
 
         if self.return_sequences:
             output = outputs
         else:
             output = last_output
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/simple_rnn.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/stacked_rnn_cells.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/stacked_rnn_cells.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.layer import Layer
 from keras_core.src.saving import serialization_lib
 
 
@@ -85,15 +85,15 @@
                     )
         return initial_states
 
     def call(self, inputs, states, training=False, **kwargs):
         # Call the cells in order and store the returned states.
         new_states = []
         for cell, states in zip(self.cells, states):
-            states = list(states) if nest.is_nested(states) else [states]
+            states = list(states) if tree.is_nested(states) else [states]
             if isinstance(cell, Layer) and cell._call_has_training_arg():
                 kwargs["training"] = training
             else:
                 kwargs.pop("training", None)
             cell_call_fn = cell.__call__ if callable(cell) else cell.call
             inputs, states = cell_call_fn(inputs, states, **kwargs)
             if len(states) == 1:
@@ -111,15 +111,15 @@
                 cell.built = True
             if getattr(cell, "output_size", None) is not None:
                 output_dim = cell.output_size
             elif isinstance(cell.state_size, (list, tuple)):
                 output_dim = cell.state_size[0]
             else:
                 output_dim = cell.state_size
-            batch_size = nest.flatten(input_shape)[0]
+            batch_size = tree.flatten(input_shape)[0]
             input_shape = (batch_size, output_dim)
         self.built = True
 
     def get_config(self):
         cells = []
         for cell in self.cells:
             cells.append(serialization_lib.serialize_keras_object(cell))
```

### Comparing `keras-core-0.1.0/keras_core/src/layers/rnn/time_distributed.py` & `keras-core-0.1.1/keras_core/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/losses/__init__.py` & `keras-core-0.1.1/keras_core/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/losses/loss.py` & `keras-core-0.1.1/keras_core/src/losses/loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import ops
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.utils import dtype_utils
 from keras_core.src.utils.naming import auto_name
 
@@ -30,18 +30,18 @@
         self.reduction = standardize_reduction(reduction)
 
     def __call__(self, y_true, y_pred, sample_weight=None):
         in_mask = getattr(y_pred, "_keras_mask", None)
 
         with ops.name_scope(self.name):
             dtype = backend.floatx()
-            y_pred = nest.map_structure(
+            y_pred = tree.map_structure(
                 lambda x: ops.convert_to_tensor(x, dtype=dtype), y_pred
             )
-            y_true = nest.map_structure(
+            y_true = tree.map_structure(
                 lambda x: ops.convert_to_tensor(x, dtype=dtype), y_true
             )
 
             losses = self.call(y_true, y_pred)
             out_mask = getattr(losses, "_keras_mask", None)
 
             if in_mask is not None and out_mask is not None:
```

### Comparing `keras-core-0.1.0/keras_core/src/losses/losses.py` & `keras-core-0.1.1/keras_core/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/__init__.py` & `keras-core-0.1.1/keras_core/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/accuracy_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/accuracy_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from keras_core.src.metrics import reduction_metrics
 
 
 def accuracy(y_true, y_pred):
     y_pred = ops.convert_to_tensor(y_pred)
     y_true = ops.convert_to_tensor(y_true, dtype=y_pred.dtype)
     y_true, y_pred = squeeze_to_same_rank(y_true, y_pred)
-    return ops.cast(ops.equal(y_true, y_pred), dtype=backend.floatx())
+    return ops.mean(
+        ops.cast(ops.equal(y_true, y_pred), dtype=backend.floatx()),
+        axis=-1,
+    )
 
 
 @keras_core_export("keras_core.metrics.Accuracy")
 class Accuracy(reduction_metrics.MeanMetricWrapper):
     """Calculates how often predictions equal labels.
 
     This metric creates two local variables, `total` and `count` that are used
@@ -131,15 +134,15 @@
 
     # If the shape of y_true is (num_samples, 1), squeeze to (num_samples,)
     if (
         (y_true_rank is not None)
         and (y_pred_rank is not None)
         and (len(y_true.shape) == len(y_pred.shape))
     ):
-        y_true = ops.squeeze(y_true, [-1])
+        y_true = ops.squeeze(y_true, -1)
         reshape_matches = True
     y_pred = ops.argmax(y_pred, axis=-1)
 
     # If the predicted output and actual output types don't match, force cast
     # them to match.
     if y_pred.dtype != y_true.dtype:
         y_pred = ops.cast(y_pred, dtype=y_true.dtype)
@@ -214,28 +217,28 @@
 
     # If the shape of y_true is (num_samples, 1), squeeze to (num_samples,)
     if (
         (y_true_rank is not None)
         and (y_pred_rank is not None)
         and (len(y_true.shape) == len(y_pred.shape))
     ):
-        y_true = ops.squeeze(y_true, [-1])
+        y_true = ops.squeeze(y_true, -1)
         reshape_matches = True
     y_pred = ops.argmax(y_pred, axis=-1)
 
     # If the predicted output and actual output types don't match, force cast
     # them to match.
     if y_pred.dtype != y_true.dtype:
         y_pred = ops.cast(y_pred, y_true.dtype)
     matches = ops.cast(ops.equal(y_true, y_pred), backend.floatx())
     if reshape_matches:
         matches = ops.reshape(matches, new_shape=y_true_org_shape)
     # if shape is (num_samples, 1) squeeze
     if len(matches.shape) > 1 and matches.shape[-1] == 1:
-        matches = ops.squeeze(matches, [-1])
+        matches = ops.squeeze(matches, -1)
     return matches
 
 
 @keras_core_export("keras_core.metrics.SparseCategoricalAccuracy")
 class SparseCategoricalAccuracy(reduction_metrics.MeanMetricWrapper):
     """Calculates how often predictions match integer labels.
```

### Comparing `keras-core-0.1.0/keras_core/src/metrics/confusion_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/f_score_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/hinge_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/iou_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/metric.py` & `keras-core-0.1.1/keras_core/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/metrics_utils.py` & `keras-core-0.1.1/keras_core/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/probabilistic_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/reduction_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/metrics/regression_metrics.py` & `keras-core-0.1.1/keras_core/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/mixed_precision/__init__.py` & `keras-core-0.1.1/keras_core/src/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/mixed_precision/dtype_policy.py` & `keras-core-0.1.1/keras_core/src/mixed_precision/dtype_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.backend.common import global_state
 
 
-@keras_core_export("keras_core.mixed_precision.DTypePolicy")
+@keras_core_export(
+    [
+        "keras_core.mixed_precision.DTypePolicy",
+        "keras_core.mixed_precision.Policy",
+    ]
+)
 class DTypePolicy:
     """A dtype policy for a Keras layer.
 
     A dtype policy determines a layer's computation and variable dtypes. Each
     layer has a policy. Policies can be passed to the `dtype` argument of layer
     constructors, or a global policy can be set with
     `keras_core.mixed_precision.set_dtype_policy`.
```

### Comparing `keras-core-0.1.0/keras_core/src/models/cloning.py` & `keras-core-0.1.1/keras_core/src/models/cloning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import utils
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers import Input
 from keras_core.src.layers import InputLayer
 from keras_core.src.models.functional import Functional
@@ -248,22 +248,22 @@
     if not isinstance(model, Functional):
         raise ValueError(
             "Expected `model` argument "
             f"to be a Functional Model instance. Received: model={model}"
         )
 
     if input_tensors is not None:
-        input_tensors = nest.flatten(input_tensors)
+        input_tensors = tree.flatten(input_tensors)
         if not all(isinstance(x, backend.KerasTensor) for x in input_tensors):
             raise ValueError(
                 "All entries in `input_tensors` must be KerasTensors. "
                 f"Received invalid values: inputs_tensors={input_tensors}"
             )
     else:
-        input_tensors = nest.map_structure(
+        input_tensors = tree.map_structure(
             lambda x: Input(x.shape, dtype=x.dtype, name=x.name), model.input
         )
 
     def operation_fn(layer):
         new_layer = clone_function(layer)
         return new_layer
```

### Comparing `keras-core-0.1.0/keras_core/src/models/functional.py` & `keras-core-0.1.1/keras_core/src/models/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import inspect
 import warnings
 
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import ops
 from keras_core.src.layers.input_spec import InputSpec
 from keras_core.src.layers.layer import Layer
 from keras_core.src.models.model import Model
 from keras_core.src.ops.function import Function
@@ -27,18 +27,18 @@
     The second argument specifies the output tensors that represent
     the outputs of this model. Both arguments can be a nested structure
     of tensors.
 
     Example:
 
     ```
-    inputs = {'x1': keras_core.Input(shape=(10,)),
-              'x2': keras_core.Input(shape=(1,))}
+    inputs = {'x1': keras_core.Input(shape=(10,), name='x1'),
+              'x2': keras_core.Input(shape=(1,), name='x2')}
     t = keras_core.layers.Dense(1, activation='relu')(inputs['x1'])
-    outputs = keras_core.layers.Add()([t, inputs['x2'])
+    outputs = keras_core.layers.Add()([t, inputs['x2']])
     model = keras_core.Model(inputs, outputs)
     ```
 
     A `Functional` model constructed using the Functional API can also
     include raw Keras Core ops.
 
     Example:
@@ -188,39 +188,39 @@
         return super().compute_output_spec(inputs)
 
     def build(self, input_shape):
         self.built = True
 
     @property
     def input_shape(self):
-        input_shapes = nest.map_structure(lambda x: x.shape, self.inputs)
+        input_shapes = tree.map_structure(lambda x: x.shape, self.inputs)
         if isinstance(input_shapes, list) and len(input_shapes) == 1:
             return input_shapes[0]
         return input_shapes
 
     @property
     def output_shape(self):
-        output_shapes = nest.map_structure(lambda x: x.shape, self.outputs)
+        output_shapes = tree.map_structure(lambda x: x.shape, self.outputs)
         if isinstance(output_shapes, list) and len(output_shapes) == 1:
             return output_shapes[0]
         return output_shapes
 
     def _assert_input_compatibility(self, *args):
         return super(Model, self)._assert_input_compatibility(*args)
 
     def _flatten_to_reference_inputs(self, inputs, allow_extra_keys=True):
         if isinstance(inputs, dict):
             ref_inputs = self._inputs_struct
-            if not nest.is_nested(ref_inputs):
+            if not tree.is_nested(ref_inputs):
                 ref_inputs = [self._inputs_struct]
             if isinstance(ref_inputs, dict):
                 # In the case that the graph is constructed with dict input
                 # tensors, We will use the original dict key to map with the
                 # keys in the input data. Note that the model.inputs is using
-                # nest.flatten to process the input tensors, which means the
+                # tree.flatten to process the input tensors, which means the
                 # dict input tensors are ordered by their keys.
                 ref_input_names = sorted(ref_inputs.keys())
             else:
                 ref_input_names = [
                     inp._keras_history.operation.name for inp in ref_inputs
                 ]
             # Raise an warning if there are more input data comparing to input
@@ -233,15 +233,15 @@
                     ),
                     stacklevel=2,
                 )
             # Flatten in the order `Input`s were passed during Model
             # construction.
             return [inputs[n] for n in ref_input_names]
         # Otherwise both ref inputs and inputs will already be in same order.
-        return nest.flatten(inputs)
+        return tree.flatten(inputs)
 
     def _convert_inputs_to_tensors(self, flat_inputs):
         flat_dtypes = [x.dtype for x in self._inputs]
         converted = []
         for x, dtype in zip(flat_inputs, flat_dtypes):
             if backend.is_tensor(x):
                 converted.append(backend.cast(x, dtype=dtype))
@@ -636,11 +636,11 @@
                     f"inbound_layer._inbound_nodes = {layer._inbound_nodes}\n"
                     f"inbound_node_index = {inbound_node_index}"
                 )
             inbound_node = layer._inbound_nodes[inbound_node_index]
             return inbound_node.output_tensors[inbound_tensor_index]
         return x
 
-    args = nest.map_structure(convert_revived_tensor, args)
-    kwargs = nest.map_structure(convert_revived_tensor, kwargs)
+    args = tree.map_structure(convert_revived_tensor, args)
+    kwargs = tree.map_structure(convert_revived_tensor, kwargs)
     return args, kwargs
```

### Comparing `keras-core-0.1.0/keras_core/src/models/model.py` & `keras-core-0.1.1/keras_core/src/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     from keras_core.src.backend.tensorflow.trainer import (
         TensorFlowTrainer as Trainer,
     )
 elif backend.backend() == "jax":
     from keras_core.src.backend.jax.trainer import JAXTrainer as Trainer
 elif backend.backend() == "torch":
     from keras_core.src.backend.torch.trainer import TorchTrainer as Trainer
+elif backend.backend() == "numpy":
+    from keras_core.src.backend.numpy.trainer import NumpyTrainer as Trainer
 else:
     raise RuntimeError(
         f"Backend '{backend.backend()}' must implement the Trainer class."
     )
 
 
 @keras_core_export(["keras_core.Model", "keras_core.models.Model"])
```

### Comparing `keras-core-0.1.0/keras_core/src/models/sequential.py` & `keras-core-0.1.1/keras_core/src/models/sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from tensorflow import nest
+import tree
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.layers.core.input_layer import InputLayer
 from keras_core.src.models.functional import Functional
 from keras_core.src.models.model import Model
 from keras_core.src.saving import serialization_lib
 from keras_core.src.utils import tracking
@@ -189,15 +189,15 @@
                 kwargs["training"] = training
             outputs = layer(inputs, **kwargs)
             inputs = outputs
 
             def _get_mask_from_keras_tensor(kt):
                 return getattr(kt, "_keras_mask", None)
 
-            mask = nest.map_structure(_get_mask_from_keras_tensor, outputs)
+            mask = tree.map_structure(_get_mask_from_keras_tensor, outputs)
         return outputs
 
     @property
     def layers(self):
         # Historically, `sequential.layers` only returns layers that were added
         # via `add`, and omits the auto-generated `InputLayer` that comes at the
         # bottom of the stack.
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/__init__.py` & `keras-core-0.1.1/keras_core/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/ops/core.py` & `keras-core-0.1.1/keras_core/src/ops/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,14 +26,38 @@
 
     def compute_output_spec(self, indices, values, shape):
         return KerasTensor(shape, dtype=values.dtype)
 
 
 @keras_core_export("keras_core.ops.scatter")
 def scatter(indices, values, shape):
+    """Returns a tensor of shape `shape` where `indices` are set to `values`.
+
+    At a high level, this operation does `zeros[indices] = updates` and
+    returns the output. It is equivalent to:
+
+    ```python
+    zeros = keras_core.ops.zeros(shape)
+    output = keras_core.ops.scatter_update(zeros, indices, values)
+    ```
+
+    Args:
+        indices: A tensor or list/tuple specifying
+            indices for the values in `values`.
+        updates: A tensor, the values to be set at `indices`.
+        shape: Shape of the output tensor.
+
+    Example:
+
+    >>> indices = [[0, 1], [1, 1]]
+    >>> values = np.array([1., 1.])
+    >>> keras_core.ops.scatter(indices, values, shape=(2, 2))
+    array([[0., 1.],
+           [0., 1.]])
+    """
     if any_symbolic_tensors((indices, values, shape)):
         return Scatter().symbolic_call(indices, values, shape)
     return backend.core.scatter(indices, values, shape)
 
 
 class ScatterUpdate(Operation):
     def call(self, inputs, indices, updates):
@@ -225,15 +249,14 @@
 
     >>> i = 0
     >>> cond = lambda i: i < 10
     >>> body = lambda i: i + 1
     >>> keras_core.ops.while_loop(cond, body, [i])[0]
     10
     """
-
     return backend.core.while_loop(
         cond,
         body,
         loop_vars,
         maximum_iterations=maximum_iterations,
     )
 
@@ -269,37 +292,86 @@
     >>> var = keras_core.ops.stop_gradient(var)
     """
     return backend.core.stop_gradient(variable)
 
 
 @keras_core_export("keras_core.ops.shape")
 def shape(x):
-    """Gets the shape of the tensor input."""
+    """Gets the shape of the tensor input.
+
+    Args:
+        x: A tensor. This function will try to access the `shape` attribute of
+            the input tensor.
+
+    Returns:
+        A tuple of integers or None values, indicating the shape of the input
+            tensor.
+
+    Example:
+
+    >>> x = keras_core.zeros((8, 12))
+    >>> keras_core.ops.shape(x)
+    (8, 12)
+    """
     if any_symbolic_tensors((x,)):
         return x.shape
     return backend.core.shape(x)
 
 
 @keras_core_export("keras_core.ops.cast")
 def cast(x, dtype):
-    """Cast a tensor to the desired dtype."""
+    """Cast a tensor to the desired dtype.
+
+    Args:
+        x: A tensor or variable.
+        dtype: The target type.
+
+    Returns:
+        A tensor of the specified `dtype`.
+
+    Example:
+
+    >>> x = keras_core.ops.arange(4)
+    >>> x = keras_core.ops.cast(x, dtype="float16")
+    """
     dtype = backend.standardize_dtype(dtype)
+
     if any_symbolic_tensors((x,)):
         return backend.KerasTensor(shape=x.shape, dtype=dtype)
     return backend.core.cast(x, dtype)
 
 
 @keras_core_export("keras_core.ops.convert_to_tensor")
 def convert_to_tensor(x, dtype=None):
-    """Convert a NumPy array to a tensor."""
+    """Convert a NumPy array to a tensor.
+
+    Args:
+        x: A NumPy array.
+        dtype: The target type.
+
+    Returns:
+        A tensor of the specified `dtype`.
+
+    Example:
+
+    >>> x = np.array([1, 2, 3])
+    >>> y = keras_core.ops.convert_to_tensor(x)
+    """
     return backend.convert_to_tensor(x, dtype=dtype)
 
 
 @keras_core_export("keras_core.ops.convert_to_numpy")
 def convert_to_numpy(x):
-    """Convert a tensor to a NumPy array."""
+    """Convert a tensor to a NumPy array.
+
+    Args:
+        x: A tensor.
+
+    Returns:
+        A NumPy array.
+    """
     if any_symbolic_tensors((x,)):
-        # This will raise a `ValueError` defined in the `KerasTensor` class. We
-        # trigger it rather than duplicate it here.
+        # This will raise a `ValueError` defined in the `KerasTensor` class.
+        # We trigger it rather than duplicate it here.
         return np.array(x)
     return backend.convert_to_numpy(x)
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/function.py` & `keras-core-0.1.1/keras_core/src/ops/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
 
-from tensorflow import nest
+import tree
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.backend import KerasTensor
 from keras_core.src.ops.operation import Operation
+from keras_core.src.utils.nest import pack_sequence_as
 
 
 @keras_core_export("keras_core.Function")
 class Function(Operation):
     """Class that encapsulates a computation graph of Keras operations.
 
     You can use a `Function` to capture the computation graph linking
@@ -41,18 +42,18 @@
             given only the values of `inputs`.
         name: String. The name of the function.
     """
 
     def __init__(self, inputs, outputs, name=None):
         super().__init__(name=name)
 
-        self._inputs_struct = nest.map_structure(lambda x: x, inputs)
-        self._outputs_struct = nest.map_structure(lambda x: x, outputs)
-        self._inputs = nest.flatten(inputs)
-        self._outputs = nest.flatten(outputs)
+        self._inputs_struct = tree.map_structure(lambda x: x, inputs)
+        self._outputs_struct = tree.map_structure(lambda x: x, outputs)
+        self._inputs = tree.flatten(inputs)
+        self._outputs = tree.flatten(outputs)
 
         (nodes, nodes_by_depth, operations, operations_by_depth) = map_graph(
             self._inputs, self._outputs
         )
         self._nodes = nodes
         self._nodes_by_depth = nodes_by_depth
         self._operations = operations
@@ -71,20 +72,20 @@
         return self._outputs
 
     def compute_output_spec(self, inputs):
         self._assert_input_compatibility(inputs)
         # Check if input shapes are identical to ref input shapes,
         # if so take a shortcut.
         shortcut = True
-        for x, x_ref in zip(nest.flatten(inputs), self._inputs):
+        for x, x_ref in zip(tree.flatten(inputs), self._inputs):
             if x.shape != x_ref.shape:
                 shortcut = False
                 break
         if shortcut:
-            return nest.map_structure(
+            return tree.map_structure(
                 lambda x: KerasTensor(shape=x.shape, dtype=x.dtype),
                 self._outputs_struct,
             )
         # No luck; take the long road through the graph.
         # Original Keras used a cache to avoid recomputing all this
         # when known input shapes where seen again. Perhaps a good
         # idea to bring that back.
@@ -99,15 +100,15 @@
 
     def _run_through_graph(self, inputs, operation_fn):
         """Execute the graph.
 
         At each node we compute outputs via
         `operation_fn(node.operation)(*args, **kwargs)`.
         """
-        inputs = nest.flatten(inputs)
+        inputs = tree.flatten(inputs)
 
         # Dictionary mapping reference tensors to computed tensors.
         tensor_dict = {}
         for x, y in zip(self.inputs, inputs):
             tensor_dict[id(x)] = y
 
         nodes_by_depth = self._nodes_by_depth
@@ -123,35 +124,35 @@
                 if any(id(x) not in tensor_dict for x in node.input_tensors):
                     continue  # Node is not computable, try skipping.
 
                 args, kwargs = node.arguments.fill_in(tensor_dict)
                 outputs = operation_fn(node.operation)(*args, **kwargs)
 
                 # Update tensor_dict.
-                for x, y in zip(node.outputs, nest.flatten(outputs)):
+                for x, y in zip(node.outputs, tree.flatten(outputs)):
                     tensor_dict[id(x)] = y
 
         output_tensors = []
         for x in self.outputs:
             output_tensors.append(tensor_dict[id(x)])
 
-        return nest.pack_sequence_as(self._outputs_struct, output_tensors)
+        return pack_sequence_as(self._outputs_struct, output_tensors)
 
     def _assert_input_compatibility(self, inputs):
         try:
-            nest.assert_same_structure(
+            tree.assert_same_structure(
                 inputs, self._inputs_struct, check_types=False
             )
         except ValueError:
             raise ValueError(
                 "Function was called with an invalid input structure. "
                 f"Expected input structure: {self._inputs_struct}\n"
                 f"Received input structure: {inputs}"
             )
-        for x, x_ref in zip(nest.flatten(inputs), self._inputs):
+        for x, x_ref in zip(tree.flatten(inputs), self._inputs):
             if len(x.shape) != len(x_ref.shape):
                 raise ValueError(
                     f"{self.__class__.__name__} was passed "
                     f"incompatible inputs. For input '{x_ref.name}', "
                     f"expected shape {x_ref.shape}, but received "
                     f"instead a tensor with shape {x.shape}."
                 )
@@ -261,26 +262,26 @@
     computable_tensors = set()
     for x in inputs:
         computable_tensors.add(x)
 
     operations_with_complete_input = []  # To provide a better error msg.
     for depth in depth_keys:
         for node in nodes_by_depth[depth]:
-            for x in nest.flatten(node.input_tensors):
+            for x in tree.flatten(node.input_tensors):
                 if x not in computable_tensors:
                     operation = node.operation
                     raise ValueError(
                         "Graph disconnected: cannot find parent for "
                         f"tensor {x} at operation '{operation}'. "
                         "The following previous operations were accessed "
                         f"without issue: {operations_with_complete_input}"
                     )
                 operations_with_complete_input.append(operation.name)
 
-            for x in nest.flatten(node.outputs):
+            for x in tree.flatten(node.outputs):
                 computable_tensors.add(x)
 
     # Ensure name unicity, which will be crucial for serialization
     # (since serialized nodes refer to operations by their name).
     all_names = [operation.name for operation in operations]
     for name in all_names:
         if all_names.count(name) != 1:
@@ -313,15 +314,15 @@
             will onlystore the index corresponding to the *first* time the
             operation seen.
     """
     finished_nodes = set()
     nodes_in_progress = set()
     nodes_in_decreasing_depth = []  # nodes from inputs -> outputs.
     operation_indices = {}  # operation -> in traversal order.
-    for output in nest.flatten(outputs):
+    for output in tree.flatten(outputs):
         _build_map_helper(
             output,
             finished_nodes,
             nodes_in_progress,
             nodes_in_decreasing_depth,
             operation_indices,
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/nn.py` & `keras-core-0.1.1/keras_core/src/ops/nn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,8 @@
-"""
-relu
-relu6
-sigmoid
-softplus
-softsign
-silu
-swish
-log_sigmoid
-leaky_relu
-hard_sigmoid
-elu
-selu
-gelu
-softmax
-log_softmax
-
-max_pooling
-average_pooling
-conv
-depthwise_conv
-separable_conv
-conv_transpose
-
-one_hot
-top_k
-in_top_k
-
-ctc ??
-"""
+"""Commonly-used neural network operations not included in NumPy."""
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.backend import KerasTensor
 from keras_core.src.backend import any_symbolic_tensors
 from keras_core.src.backend import standardize_data_format
 from keras_core.src.backend.common.backend_utils import (
@@ -360,38 +331,38 @@
     padding="valid",
     data_format=None,
 ):
     """Max pooling operation.
 
     Args:
         inputs: Tensor of rank N+2. `inputs` has shape
-            [batch_size] + inputs_spatial_shape + [num_channels] if
+            `(batch_size,) + inputs_spatial_shape + (num_channels,)` if
             `data_format="channels_last"`, or
-            [batch_size, num_channels] + inputs_spatial_shape if
+            `(batch_size, num_channels) + inputs_spatial_shape` if
             `data_format="channels_first"`. Pooling happens over the spatial
             dimensions only.
         pool_size: int or tuple/list of integers of size
             `len(inputs_spatial_shape)`, specifying the size of the pooling
             window for each spatial dimension of the input tensor. If
             `pool_size` is int, then every spatial dimension shares the same
             `pool_size`.
         strides: int or tuple/list of integers of size
             `len(inputs_spatial_shape)`. The stride of the sliding window for
             each spatial dimension of the input tensor. If `strides` is int,
             then every spatial dimension shares the same `strides`.
         padding: string, either `"valid"` or `"same"`. `"valid"` means no
-            padding is applied, and "same" results in padding evenly to the
+            padding is applied, and `"same"` results in padding evenly to the
             left/right or up/down of the input such that output has the
             same height/width dimension as the input when `strides=1`.
-        data_format: A string, either "channels_last" or `channels_first`.
+        data_format: A string, either `"channels_last"` or `"channels_first"`.
             `data_format` determines the ordering of the dimensions in the
-            inputs. If `data_format="channels_last"`, inputs is of shape
-            (batch_size, spatial_shape, channels) while if
-            `data_format="channels_first"`, inputs is of shape
-            (batch_size, channels, spatial_shape).
+            inputs. If `data_format="channels_last"`, `inputs` is of shape
+            `(batch_size, ..., channels)` while if
+            `data_format="channels_first"`, `inputs` is of shape
+            `(batch_size, channels, ...)`.
 
     Returns:
         A tensor of rank N+2, the result of the max pooling operation.
     """
     data_format = standardize_data_format(data_format)
     if any_symbolic_tensors((inputs,)):
         return MaxPool(
@@ -450,38 +421,38 @@
     padding="valid",
     data_format=None,
 ):
     """Average pooling operation.
 
     Args:
         inputs: Tensor of rank N+2. `inputs` has shape
-            [batch_size] + inputs_spatial_shape + [num_channels] if
+            `(batch_size,)` + inputs_spatial_shape + (num_channels,)` if
             `data_format="channels_last"`, or
-            [batch_size, num_channels] + inputs_spatial_shape if
+            `(batch_size, num_channels) + inputs_spatial_shape` if
             `data_format="channels_first"`. Pooling happens over the spatial
             dimensions only.
         pool_size: int or tuple/list of integers of size
             `len(inputs_spatial_shape)`, specifying the size of the pooling
             window for each spatial dimension of the input tensor. If
             `pool_size` is int, then every spatial dimension shares the same
             `pool_size`.
         strides: int or tuple/list of integers of size
             `len(inputs_spatial_shape)`. The stride of the sliding window for
             each spatial dimension of the input tensor. If `strides` is int,
             then every spatial dimension shares the same `strides`.
         padding: string, either `"valid"` or `"same"`. `"valid"` means no
-            padding is applied, and "same" results in padding evenly to the
+            padding is applied, and `"same"` results in padding evenly to the
             left/right or up/down of the input such that output has the
             same height/width dimension as the input when `strides=1`.
-        data_format: A string, either "channels_last" or `channels_first`.
+        data_format: A string, either `"channels_last"` or `"channels_first"`.
             `data_format` determines the ordering of the dimensions in the
-            inputs. If `data_format="channels_last"`, inputs is of shape
-            (batch_size, spatial_shape, channels) while if
-            `data_format="channels_first"`, inputs is of shape
-            (batch_size, channels, spatial_shape).
+            inputs. If `data_format="channels_last"`, `inputs` is of shape
+            `(batch_size, ..., channels)` while if
+            `data_format="channels_first"`, `inputs` is of shape
+            `(batch_size, channels, ...)`.
 
     Returns:
         A tensor of rank N+2, the result of the average pooling operation.
     """
     data_format = standardize_data_format(data_format)
     if any_symbolic_tensors((inputs,)):
         return AveragePool(
@@ -543,37 +514,36 @@
 ):
     """General N-D convolution.
 
     This ops supports 1D, 2D and 3D convolution.
 
     Args:
         inputs: Tensor of rank N+2. `inputs` has shape
-            [batch_size] + inputs_spatial_shape + [num_channels] if
+            `(batch_size,) + inputs_spatial_shape + (num_channels,)` if
             `data_format="channels_last"`, or
-            [batch_size, num_channels] + inputs_spatial_shape if
-            `data_format="channels_first"`. Pooling happens over the spatial
-            dimensions only.
+            `(batch_size, num_channels) + inputs_spatial_shape` if
+            `data_format="channels_first"`.
         kernel: Tensor of rank N+2. `kernel` has shape
-            [kernel_spatial_shape, num_input_channels, num_output_channels],
+            `(kernel_spatial_shape, num_input_channels, num_output_channels)`.
             `num_input_channels` should match the number of channels in
             `inputs`.
         strides: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the strides of the convolution along each spatial
             dimension. If `strides` is int, then every spatial dimension shares
             the same `strides`.
         padding: string, either `"valid"` or `"same"`. `"valid"` means no
-            padding is applied, and "same" results in padding evenly to the
+            padding is applied, and `"same"` results in padding evenly to the
             left/right or up/down of the input such that output has the
             same height/width dimension as the input when `strides=1`.
-        data_format: A string, either "channels_last" or `channels_first`.
+        data_format: A string, either `"channels_last"` or `"channels_first"`.
             `data_format` determines the ordering of the dimensions in the
-            inputs. If `data_format="channels_last"`, inputs is of shape
-            (batch_size, spatial_shape, channels) while if
-            `data_format="channels_first"`, inputs is of shape
-            (batch_size, channels, spatial_shape).
+            inputs. If `data_format="channels_last"`, `inputs` is of shape
+            `(batch_size, ..., channels)` while if
+            `data_format="channels_first"`, `inputs` is of shape
+            `(batch_size, channels, ...)`.
         dilation_rate: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the dilation rate to use for dilated convolution. If
             `dilation_rate` is int, then every spatial dimension shares
             the same `dilation_rate`.
 
     Returns:
         A tensor of rank N+2, the result of the conv operation.
@@ -641,37 +611,36 @@
 ):
     """General N-D depthwise convolution.
 
     This ops supports 1D and 2D depthwise convolution.
 
     Args:
         inputs: Tensor of rank N+2. `inputs` has shape
-            [batch_size] + inputs_spatial_shape + [num_channels] if
+            `(batch_size,)` + inputs_spatial_shape + (num_channels,)` if
             `data_format="channels_last"`, or
-            [batch_size, num_channels] + inputs_spatial_shape if
-            `data_format="channels_first"`. Pooling happens over the spatial
-            dimensions only.
+            `(batch_size, num_channels) + inputs_spatial_shape` if
+            `data_format="channels_first"`.
         kernel: Tensor of rank N+2. `kernel` has shape
             [kernel_spatial_shape, num_input_channels, num_channels_multiplier],
             `num_input_channels` should match the number of channels in
             `inputs`.
         strides: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the strides of the convolution along each spatial
             dimension. If `strides` is int, then every spatial dimension shares
             the same `strides`.
         padding: string, either `"valid"` or `"same"`. `"valid"` means no
-            padding is applied, and "same" results in padding evenly to the
+            padding is applied, and `"same"` results in padding evenly to the
             left/right or up/down of the input such that output has the
             same height/width dimension as the input when `strides=1`.
-        data_format: A string, either "channels_last" or `channels_first`.
+        data_format: A string, either `"channels_last"` or `"channels_first"`.
             `data_format` determines the ordering of the dimensions in the
-            inputs. If `data_format="channels_last"`, inputs is of shape
-            (batch_size, spatial_shape, channels) while if
-            `data_format="channels_first"`, inputs is of shape
-            (batch_size, channels, spatial_shape).
+            inputs. If `data_format="channels_last"`, `inputs` is of shape
+            `(batch_size, ..., channels)` while if
+            `data_format="channels_first"`, `inputs` is of shape
+            `(batch_size, channels, ...)`.
         dilation_rate: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the dilation rate to use for dilated convolution. If
             `dilation_rate` is int, then every spatial dimension shares
             the same `dilation_rate`.
 
     Returns:
         A tensor of rank N+2, the result of the depthwise conv operation.
@@ -752,40 +721,39 @@
     """General N-D separable convolution.
 
     This ops supports 1D and 2D separable convolution. `separable_conv` is
     a depthwise conv followed by a pointwise conv.
 
     Args:
         inputs: Tensor of rank N+2. `inputs` has shape
-            [batch_size] + inputs_spatial_shape + [num_channels] if
+            `(batch_size,)` + inputs_spatial_shape + (num_channels,)` if
             `data_format="channels_last"`, or
-            [batch_size, num_channels] + inputs_spatial_shape if
-            `data_format="channels_first"`. Pooling happens over the spatial
-            dimensions only.
+            `(batch_size, num_channels) + inputs_spatial_shape` if
+            `data_format="channels_first"`.
         depthwise_kernel: Tensor of rank N+2. `depthwise_kernel` has shape
             [kernel_spatial_shape, num_input_channels, num_channels_multiplier],
             `num_input_channels` should match the number of channels in
             `inputs`.
         pointwise_kernel: Tensor of rank N+2. `pointwise_kernel` has shape
-            [ones_like(kernel_spatial_shape),
-            num_input_channels * num_channels_multiplier, num_output_channels].
+            `(*ones_like(kernel_spatial_shape),
+            num_input_channels * num_channels_multiplier, num_output_channels)`.
         strides: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the strides of the convolution along each spatial
             dimension. If `strides` is int, then every spatial dimension shares
             the same `strides`.
         padding: string, either `"valid"` or `"same"`. `"valid"` means no
-            padding is applied, and "same" results in padding evenly to the
+            padding is applied, and `"same"` results in padding evenly to the
             left/right or up/down of the input such that output has the
             same height/width dimension as the input when `strides=1`.
-        data_format: A string, either "channels_last" or `channels_first`.
+        data_format: A string, either `"channels_last"` or `"channels_first"`.
             `data_format` determines the ordering of the dimensions in the
-            inputs. If `data_format="channels_last"`, inputs is of shape
-            (batch_size, spatial_shape, channels) while if
-            `data_format="channels_first"`, inputs is of shape
-            (batch_size, channels, spatial_shape).
+            inputs. If `data_format="channels_last"`, `inputs` is of shape
+            `(batch_size, ..., channels)` while if
+            `data_format="channels_first"`, `inputs` is of shape
+            `(batch_size, channels, ...)`.
         dilation_rate: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the dilation rate to use for dilated convolution. If
             `dilation_rate` is int, then every spatial dimension shares
             the same `dilation_rate`.
 
     Returns:
         A tensor of rank N+2, the result of the depthwise conv operation.
@@ -873,44 +841,43 @@
 ):
     """General N-D convolution transpose.
 
     Also known as de-convolution. This ops supports 1D, 2D and 3D convolution.
 
     Args:
         inputs: Tensor of rank N+2. `inputs` has shape
-            [batch_size] + inputs_spatial_shape + [num_channels] if
+            `(batch_size,)` + inputs_spatial_shape + (num_channels,)` if
             `data_format="channels_last"`, or
-            [batch_size, num_channels] + inputs_spatial_shape if
-            `data_format="channels_first"`. Pooling happens over the spatial
-            dimensions only.
+            `(batch_size, num_channels) + inputs_spatial_shape` if
+            `data_format="channels_first"`.
         kernel: Tensor of rank N+2. `kernel` has shape
             [kernel_spatial_shape, num_output_channels, num_input_channels],
             `num_input_channels` should match the number of channels in
             `inputs`.
         strides: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the strides of the convolution along each spatial
             dimension. If `strides` is int, then every spatial dimension shares
             the same `strides`.
         padding: string, either `"valid"` or `"same"`. `"valid"` means no
-            padding is applied, and "same" results in padding evenly to the
+            padding is applied, and `"same"` results in padding evenly to the
             left/right or up/down of the input such that output has the
             same height/width dimension as the input when `strides=1`.
         output_padding: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the amount of padding along the height and width of
             the output tensor. Can be a single integer to specify the same
             value for all spatial dimensions. The amount of output padding
             along a given dimension must be lower than the stride along that
-            same dimension. If set to None (default), the output shape is
+            same dimension. If set to `None` (default), the output shape is
             inferred.
-        data_format: A string, either "channels_last" or `channels_first`.
+        data_format: A string, either `"channels_last"` or `"channels_first"`.
             `data_format` determines the ordering of the dimensions in the
-            inputs. If `data_format="channels_last"`, inputs is of shape
-            (batch_size, spatial_shape, channels) while if
-            `data_format="channels_first"`, inputs is of shape
-            (batch_size, channels, spatial_shape).
+            inputs. If `data_format="channels_last"`, `inputs` is of shape
+            `(batch_size, ..., channels)` while if
+            `data_format="channels_first"`, `inputs` is of shape
+            `(batch_size, channels, ...)`.
         dilation_rate: int or int tuple/list of `len(inputs_spatial_shape)`,
             specifying the dilation rate to use for dilated convolution. If
             `dilation_rate` is int, then every spatial dimension shares
             the same `dilation_rate`.
 
     Returns:
         A tensor of rank N+2, the result of the conv operation.
@@ -955,14 +922,45 @@
                 f"received {self.axis}."
             )
         return KerasTensor(x_shape, dtype=self.dtype)
 
 
 @keras_core_export(["keras_core.ops.one_hot", "keras_core.ops.nn.one_hot"])
 def one_hot(x, num_classes, axis=-1, dtype=None):
+    """Converts integer tensor `x` into a one-hot tensor.
+
+    The one-hot encoding is a representation where each integer value is
+    converted into a binary vector with a length equal to `num_classes`,
+    and the index corresponding to the integer value is marked as 1, while
+    all other indices are marked as 0.
+
+    Args:
+        x : Integer tensor to be encoded. The shape can be
+            arbitrary, but the dtype should be integer.
+        num_classes: Number of classes for the one-hot encoding.
+        axis: Axis along which the encoding is performed. Default is
+            -1, which represents the last axis.
+        dtype: (Optional) Data type of the output tensor. If not
+            provided, it defaults to the default data type of the backend.
+
+    Returns:
+        Integer tensor: One-hot encoded tensor with the same shape as `x`
+        except for the specified `axis` dimension, which will have
+        a length of `num_classes`. The dtype of the output tensor
+        is determined by `dtype` or the default data type of the backend.
+
+    Example:
+
+    >>> x = keras_core.ops.convert_to_tensor([1, 3, 2, 0])
+    >>> one_hot(x, num_classes=4)
+    array([[0. 1. 0. 0.]
+           [0. 0. 0. 1.]
+           [0. 0. 1. 0.]
+           [1. 0. 0. 0.]], shape=(4, 4), dtype=float32)
+    """
     if any_symbolic_tensors((x,)):
         return OneHot(num_classes, axis=axis, dtype=dtype).symbolic_call(x)
     return backend.nn.one_hot(
         x, num_classes, axis=axis, dtype=dtype or backend.floatx()
     )
 
 
@@ -989,14 +987,45 @@
 @keras_core_export(
     [
         "keras_core.ops.binary_crossentropy",
         "keras_core.ops.nn.binary_crossentropy",
     ]
 )
 def binary_crossentropy(target, output, from_logits=False):
+    """Computes binary cross-entropy loss between target and output tensor.
+
+    The binary cross-entropy loss is commonly used in binary
+    classification tasks where each input sample belongs to one
+    of the two classes. It measures the dissimilarity between the
+    target and output probabilities or logits.
+
+    Args:
+        target: The target tensor representing the true binary labels.
+            Its shape should match the shape of the `output` tensor.
+        output: The output tensor representing the predicted probabilities
+            or logits. Its shape should match the shape of the
+            `target` tensor.
+        from_logits: (optional) Whether `output` is a tensor of logits or
+            probabilities.
+            Set it to `True` if `output` represents logits; otherwise,
+            set it to `False` if `output` represents probabilities.
+            Default is `False`.
+
+    Returns:
+        Integer tensor: The computed binary cross-entropy loss between
+        `target` and `output`.
+
+    Example:
+
+    >>> target = keras_core.ops.convert_to_tensor([0, 1, 1, 0])
+    >>> output = keras_core.ops.convert_to_tensor([0.1, 0.9, 0.8, 0.2])
+    >>> binary_crossentropy(target, output)
+    array([0.10536054 0.10536054 0.22314355 0.22314355],
+          shape=(4,), dtype=float32)
+    """
     if any_symbolic_tensors((target, output)):
         return BinaryCrossentropy(from_logits=from_logits).symbolic_call(
             target, output
         )
     return backend.nn.binary_crossentropy(
         target, output, from_logits=from_logits
     )
@@ -1032,14 +1061,55 @@
 @keras_core_export(
     [
         "keras_core.ops.categorical_crossentropy",
         "keras_core.ops.nn.categorical_crossentropy",
     ]
 )
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
+    """Computes categorical cross-entropy loss between target and output tensor.
+
+    The categorical cross-entropy loss is commonly used in multi-class
+    classification tasks where each input sample can belong to one of
+    multiple classes. It measures the dissimilarity
+    between the target and output probabilities or logits.
+
+    Args:
+        target: The target tensor representing the true categorical labels.
+            Its shape should match the shape of the `output` tensor
+            except for the last dimension.
+        output: The output tensor representing the predicted probabilities
+            or logits. Its shape should match the shape of the `target`
+            tensor except for the last dimension.
+        from_logits: (optional) Whether `output` is a tensor of logits or
+            probabilities.
+            Set it to `True` if `output` represents logits; otherwise,
+            set it to `False` if `output` represents probabilities.
+            Default is `False`.
+        axis: (optional) The axis along which the categorical cross-entropy
+            is computed.
+            Default is -1, which corresponds to the last dimension of
+            the tensors.
+
+    Returns:
+        Integer tensor: The computed categorical cross-entropy loss between
+        `target` and `output`.
+
+    Example:
+
+    >>> target = keras_core.ops.convert_to_tensor(
+    ... [[1, 0, 0],
+    ...  [0, 1, 0],
+    ...  [0, 0, 1]])
+    >>> output = keras_core.ops.convert_to_tensor(
+    ... [[0.9, 0.05, 0.05],
+    ...  [0.1, 0.8, 0.1],
+    ...  [0.2, 0.3, 0.5]])
+    >>> categorical_crossentropy(target, output)
+    array([0.10536054 0.22314355 0.6931472 ], shape=(3,), dtype=float32)
+    """
     if any_symbolic_tensors((target, output)):
         return CategoricalCrossentropy(
             from_logits=from_logits, axis=axis
         ).symbolic_call(target, output)
     return backend.nn.categorical_crossentropy(
         target, output, from_logits=from_logits, axis=axis
     )
@@ -1078,14 +1148,53 @@
 @keras_core_export(
     [
         "keras_core.ops.sparse_categorical_crossentropy",
         "keras_core.ops.nn.sparse_categorical_crossentropy",
     ]
 )
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
+    """Computes sparse categorical cross-entropy loss.
+
+    The sparse categorical cross-entropy loss is similar to categorical
+    cross-entropy, but it is used when the target tensor contains integer
+    class labels instead of one-hot encoded vectors. It measures the
+    dissimilarity between the target and output probabilities or logits.
+
+    Args:
+        target: The target tensor representing the true class labels as
+            integers. Its shape should match the shape of the `output`
+            tensor except for the last dimension.
+        output: The output tensor representing the predicted probabilities
+            or logits.
+            Its shape should match the shape of the `target` tensor except
+            for the last dimension.
+        from_logits: (optional) Whether `output` is a tensor of logits
+            or probabilities.
+            Set it to `True` if `output` represents logits; otherwise,
+            set it to `False` if `output` represents probabilities.
+            Default is `False`.
+        axis: (optional) The axis along which the sparse categorical
+            cross-entropy is computed.
+            Default is -1, which corresponds to the last dimension
+            of the tensors.
+
+    Returns:
+        Integer tensor: The computed sparse categorical cross-entropy
+        loss between `target` and `output`.
+
+    Example:
+
+    >>> target = keras_core.ops.convert_to_tensor([0, 1, 2], dtype=int32)
+    >>> output = keras_core.ops.convert_to_tensor(
+    ... [[0.9, 0.05, 0.05],
+    ...  [0.1, 0.8, 0.1],
+    ...  [0.2, 0.3, 0.5]])
+    >>> sparse_categorical_crossentropy(target, output)
+    array([0.10536056 0.22314355 0.6931472 ], shape=(3,), dtype=float32)
+    """
     if any_symbolic_tensors((target, output)):
         return SparseCategoricalCrossentropy(
             from_logits=from_logits, axis=axis
         ).symbolic_call(target, output)
     return backend.nn.sparse_categorical_crossentropy(
         target, output, from_logits=from_logits, axis=axis
     )
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/node.py` & `keras-core-0.1.1/keras_core/src/ops/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
 
-from tensorflow import nest
+import tree
 
 from keras_core.src.backend import KerasTensor
 from keras_core.src.ops.symbolic_arguments import SymbolicArguments
 
 
 class Node:
     """A `Node` describes an operation `__call__()` event.
@@ -39,15 +39,15 @@
     """
 
     def __init__(
         self, operation, call_args=None, call_kwargs=None, outputs=None
     ):
         self.operation = operation
         self.arguments = SymbolicArguments(*call_args, **call_kwargs)
-        self.outputs = [] if outputs is None else nest.flatten(outputs)
+        self.outputs = [] if outputs is None else tree.flatten(outputs)
         for x in self.outputs:
             if not isinstance(x, KerasTensor):
                 raise ValueError(
                     "All operation outputs must be tensors. "
                     f"Operation {operation} returned a non-tensor. "
                     f"Non-tensor received: {x}"
                 )
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/numpy.py` & `keras-core-0.1.1/keras_core/src/ops/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,30 @@
 from keras_core.src.backend import any_symbolic_tensors
 from keras_core.src.ops import operation_utils
 from keras_core.src.ops.operation import Operation
 from keras_core.src.ops.operation_utils import reduce_shape
 
 
 def broadcast_shapes(shape1, shape2):
-    # Broadcast input shapes to a unified shape.
-    # Convert to list for mutability.
+    """Broadcast input shapes to a unified shape.
+
+    Convert to list for mutability.
+
+    Args:
+        shape1: A tuple or list of integers.
+        shape2: A tuple or list of integers.
+
+    Returns:
+        output_shape (list of integers or `None`): The broadcasted shape.
+
+    Example:
+
+    >>> broadcast_shapes((5, 3), (1, 3))
+    [5, 3]
+    """
     shape1 = list(shape1)
     shape2 = list(shape2)
     origin_shape1 = shape1
     origin_shape2 = shape2
 
     if len(shape1) > len(shape2):
         shape2 = [1] * (len(shape1) - len(shape2)) + shape2
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/operation.py` & `keras-core-0.1.1/keras_core/src/ops/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import textwrap
 
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.backend.common.keras_tensor import any_symbolic_tensors
 from keras_core.src.ops.node import Node
 from keras_core.src.utils import python_utils
 from keras_core.src.utils import traceback_utils
@@ -89,15 +89,15 @@
         arg_names = inspect.getfullargspec(cls.__init__).args
         kwargs.update(dict(zip(arg_names[1 : len(args) + 1], args)))
         instance = super(Operation, cls).__new__(cls)
         # For safety, we only rely on auto-configs for a small set of
         # serializable types.
         supported_types = (str, int, float, bool, type(None))
         try:
-            flat_arg_values = nest.flatten(kwargs)
+            flat_arg_values = tree.flatten(kwargs)
             auto_config = True
             for value in flat_arg_values:
                 if not isinstance(value, supported_types):
                     auto_config = False
                     break
         except TypeError:
             auto_config = False
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/operation_utils.py` & `keras-core-0.1.1/keras_core/src/ops/operation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 
 import numpy as np
-from tensorflow import nest
+import tree
 
 
 def compute_pooling_output_shape(
     input_shape,
     pool_size,
     strides,
     padding="valid",
@@ -223,15 +223,15 @@
     operation, node_index, _ = tensor._keras_history
     if not operation or not operation._inbound_nodes:
         return [tensor]
     else:
         node = operation._inbound_nodes[node_index]
         if node.is_input:
             # Reached input node, stop recursion.
-            return nest.flatten(node.input_tensors)
+            return tree.flatten(node.input_tensors)
         else:
             source_tensors = []
             for tensor in node.input_tensors:
                 previous_sources = get_source_inputs(tensor)
                 # Avoid input redundancy.
                 for x in previous_sources:
                     if all(x is not t for t in source_tensors):
```

### Comparing `keras-core-0.1.0/keras_core/src/ops/symbolic_arguments.py` & `keras-core-0.1.1/keras_core/src/ops/symbolic_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src.backend import KerasTensor
 
 
 class SymbolicArguments:
     def __init__(self, *args, **kwargs):
-        # TODO: validation
-        self.args = nest.map_structure(lambda x: x, args)
-        self.kwargs = nest.map_structure(lambda x: x, kwargs)
-        self._flat_arguments = nest.flatten((self.args, self.kwargs))
+        self.args = tree.map_structure(lambda x: x, args)
+        self.kwargs = tree.map_structure(lambda x: x, kwargs)
+        self._flat_arguments = tree.flatten((self.args, self.kwargs))
 
         # Used to avoid expensive `nest` operations in the most common case.
         if (
             not self.kwargs
             and len(self.args) == 1
             and isinstance(self.args[0], KerasTensor)
         ):
@@ -22,16 +21,16 @@
 
         self.keras_tensors = []
         for arg in self._flat_arguments:
             if isinstance(arg, KerasTensor):
                 self.keras_tensors.append(arg)
 
     def convert(self, conversion_fn):
-        args = nest.map_structure(conversion_fn, self.args)
-        kwargs = nest.map_structure(conversion_fn, self.kwargs)
+        args = tree.map_structure(conversion_fn, self.args)
+        kwargs = tree.map_structure(conversion_fn, self.kwargs)
         return args, kwargs
 
     def fill_in(self, tensor_dict):
         """Maps KerasTensors to computed values using `tensor_dict`.
 
         `tensor_dict` maps `KerasTensor` instances to their current values.
         """
```

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/__init__.py` & `keras-core-0.1.1/keras_core/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/adadelta.py` & `keras-core-0.1.1/keras_core/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/adafactor.py` & `keras-core-0.1.1/keras_core/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/adagrad.py` & `keras-core-0.1.1/keras_core/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/adam.py` & `keras-core-0.1.1/keras_core/src/optimizers/adam.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,14 @@
                     self.add_variable_from_reference(
                         reference_variable=var, name="vhat"
                     )
                 )
 
     def update_step(self, gradient, variable, learning_rate):
         """Update step given gradient and the associated model variable."""
-        beta_1_power = None
-        beta_2_power = None
         lr = ops.cast(learning_rate, variable.dtype)
         gradient = ops.cast(gradient, variable.dtype)
         local_step = ops.cast(self.iterations + 1, variable.dtype)
         beta_1_power = ops.power(
             ops.cast(self.beta_1, variable.dtype), local_step
         )
         beta_2_power = ops.power(
```

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/adamax.py` & `keras-core-0.1.1/keras_core/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/base_optimizer.py` & `keras-core-0.1.1/keras_core/src/optimizers/base_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,26 @@
             self._learning_rate = learning_rate
 
     def _track_variable(self, variable):
         self._tracker.add_to_store("variables", variable)
 
     @tracking.no_automatic_dependency_tracking
     def build(self, variables):
+        if self.use_ema:
+            self._model_variables_moving_average = []
+            self._ema_vars_initialized = False
         for i, variable in enumerate(variables):
             self._trainable_variables_indices[self._var_key(variable)] = i
+            if self.use_ema:
+                self._model_variables_moving_average.append(
+                    self.add_variable_from_reference(
+                        variable,
+                        "average",
+                    )
+                )
         self._trainable_variables = variables[:]
         self.built = True
 
     def _var_key(self, variable):
         # Helper function to get a stable ID and the variable instance mapping.
         return id(variable)
 
@@ -179,15 +189,14 @@
     def apply(self, grads, trainable_variables=None):
         """
         `grads` should be a list of gradient tensors
         with 1:1 mapping to the list of variables the optimizer was built with.
 
         `variables` can be provided on the first call to build the optimizer.
         """
-        grads = list(grads)
         if len(grads) == 0:
             # It is possible that the grad is empty. In this case,
             # `apply_gradients` is a no-op.
             return
 
         if trainable_variables is None:
             if not self.built:
@@ -210,24 +219,23 @@
             # Optionally build optimizer.
             if not self.built:
                 with ops.name_scope(self.name):
                     self.build(trainable_variables)
                 self.built = True
             self._check_variables_are_known(trainable_variables)
 
-        grads_and_vars = list(zip(grads, self._trainable_variables))
-
         with ops.name_scope(self.name):
             # Filter empty gradients.
-            grads_and_vars = self._filter_empty_gradients(grads_and_vars)
-            if len(list(grads_and_vars)) == 0:
+            grads, trainable_variables = self._filter_empty_gradients(
+                grads, trainable_variables
+            )
+            if len(list(grads)) == 0:
                 return
 
             # Apply clipping and weight decay.
-            grads, trainable_variables = zip(*grads_and_vars)
             grads = self._clip_gradients(grads)
             self._apply_weight_decay(trainable_variables)
 
             # Apply gradient updates.
             self._internal_apply_gradients(
                 list(zip(grads, trainable_variables))
             )
@@ -349,27 +357,35 @@
             self._learning_rate, learning_rate_schedule.LearningRateSchedule
         ):
             return self._learning_rate(self.iterations)
         elif callable(self._learning_rate):
             return self._learning_rate(self.iterations)
         return self._learning_rate
 
-    def _filter_empty_gradients(self, grads_and_vars):
-        filtered = [(g, v) for g, v in grads_and_vars if g is not None]
-        if not filtered:
-            raise ValueError("No gradients provided for any variable.")
-        if len(filtered) < len(grads_and_vars):
-            missing_grad_vars = [v for g, v in grads_and_vars if g is None]
-            warnings.warn(
-                "Gradients do not exist for variables "
-                f"{[v.name for v in missing_grad_vars]} when minimizing the "
-                "loss. If you're using `model.compile()`, did you forget to "
-                "provide a `loss` argument?"
-            )
-        return filtered
+    def _filter_empty_gradients(self, grads, vars):
+        for grad in grads:
+            if grad is None:
+                # Filtering is required.
+                filtered = [
+                    (g, v) for g, v in zip(grads, vars) if g is not None
+                ]
+                if not filtered:
+                    raise ValueError("No gradients provided for any variable.")
+                if len(filtered) < len(grads):
+                    missing_grad_vars = [
+                        v for g, v in zip(grads, vars) if g is None
+                    ]
+                    warnings.warn(
+                        "Gradients do not exist for variables "
+                        f"{[v.name for v in missing_grad_vars]} when "
+                        "minimizing the loss. If using `model.compile()`, "
+                        "did you forget to provide a `loss` argument?"
+                    )
+                return zip(*filtered)
+        return grads, vars
 
     def _clip_gradients(self, grads):
         if self.clipnorm and self.clipnorm > 0:
             clipped_grads = []
             for g in grads:
                 if g is None:
                     clipped_grads.append(g)
@@ -457,17 +473,22 @@
 
     def _update_model_variables_moving_average(self, var_list):
         """Update the stored moving average using the latest value."""
         if self.use_ema:
             for var, average in zip(
                 var_list, self._model_variables_moving_average
             ):
-                average.assign(
-                    self.ema_momentum * average + (1 - self.ema_momentum) * var
-                )
+                if self._ema_vars_initialized:
+                    average.assign(
+                        self.ema_momentum * average
+                        + (1 - self.ema_momentum) * var
+                    )
+                else:
+                    average.assign(var)
+            self._ema_vars_initialized = True
 
     def _overwrite_model_variables_with_average_value(self, var_list):
         """Overwrite model variables with its moving average."""
         if len(var_list) != len(self._model_variables_moving_average):
             raise ValueError(
                 f"The length of model variables ({len(var_list)}) to "
                 "override does not match the length of model variables "
```

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/ftrl.py` & `keras-core-0.1.1/keras_core/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/nadam.py` & `keras-core-0.1.1/keras_core/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/optimizer.py` & `keras-core-0.1.1/keras_core/src/optimizers/optimizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.optimizers import base_optimizer
 
 if backend.backend() == "tensorflow":
-    from keras_core.src.backend.tensorflow import optimizer as tf_optimizer
+    from keras_core.src.backend.tensorflow.optimizer import TFOptimizer
 
-    BackendOptimizer = tf_optimizer.TFOptimizer
+    BackendOptimizer = TFOptimizer
+elif backend.backend() == "torch":
+    from keras_core.src.backend.torch.optimizers import TorchOptimizer
+
+    BackendOptimizer = TorchOptimizer
 else:
     BackendOptimizer = base_optimizer.BaseOptimizer
 
 
 @keras_core_export(["keras_core.Optimizer", "keras_core.optimizers.Optimizer"])
 class Optimizer(BackendOptimizer):
     pass
```

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/rmsprop.py` & `keras-core-0.1.1/keras_core/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/schedules/__init__.py` & `keras-core-0.1.1/keras_core/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/schedules/learning_rate_schedule.py` & `keras-core-0.1.1/keras_core/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/optimizers/sgd.py` & `keras-core-0.1.1/keras_core/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/random/random.py` & `keras-core-0.1.1/keras_core/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/random/seed_generator.py` & `keras-core-0.1.1/keras_core/src/random/seed_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random as python_random
 
 import numpy as np
 
+from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 
 
 @keras_core_export("keras_core.random.SeedGenerator")
 class SeedGenerator:
     """Generates variable seeds upon each call to a RNG-using function.
 
@@ -26,30 +27,30 @@
     """
 
     def __init__(self, seed, **kwargs):
         custom_backend = kwargs.pop("backend", None)
         if kwargs:
             raise ValueError(f"Unrecognized keyword arguments: {kwargs}")
         if custom_backend is not None:
-            backend = custom_backend
+            self.backend = custom_backend
         else:
-            from keras_core.src import backend
+            self.backend = backend
 
         if seed is None:
             seed = make_default_seed()
         if not isinstance(seed, int):
             raise ValueError(
                 "Argument `seed` must be an integer. " f"Received: seed={seed}"
             )
 
         def seed_initializer(*args, **kwargs):
             dtype = kwargs.get("dtype", None)
-            return backend.convert_to_tensor([seed, 0], dtype=dtype)
+            return self.backend.convert_to_tensor([seed, 0], dtype=dtype)
 
-        self.state = backend.Variable(
+        self.state = self.backend.Variable(
             seed_initializer,
             shape=(2,),
             dtype="uint32",
             trainable=False,
             name="seed_generator_state",
         )
 
@@ -61,15 +62,17 @@
 def draw_seed(seed):
     from keras_core.src.backend import convert_to_tensor
 
     if isinstance(seed, SeedGenerator):
         seed_state = seed.state
         # Use * 1 to create a copy
         new_seed_value = seed_state.value * 1
-        increment = convert_to_tensor(np.array([0, 1]), dtype="uint32")
+        increment = seed.backend.convert_to_tensor(
+            np.array([0, 1]), dtype="uint32"
+        )
         seed.state.assign(seed_state + increment)
         return new_seed_value
     elif isinstance(seed, int):
         return convert_to_tensor([seed, 0], dtype="uint32")
     elif seed is None:
         return convert_to_tensor([make_default_seed(), 0], dtype="uint32")
     raise ValueError(
```

### Comparing `keras-core-0.1.0/keras_core/src/regularizers/__init__.py` & `keras-core-0.1.1/keras_core/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/regularizers/regularizers.py` & `keras-core-0.1.1/keras_core/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/saving/__init__.py` & `keras-core-0.1.1/keras_core/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/saving/legacy/legacy_h5_format.py` & `keras-core-0.1.1/keras_core/src/saving/legacy/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/saving/object_registration.py` & `keras-core-0.1.1/keras_core/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/saving/saving_api.py` & `keras-core-0.1.1/keras_core/src/saving/saving_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import zipfile
 
-from tensorflow.io import gfile
-
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.saving import saving_lib
 from keras_core.src.saving.legacy import legacy_h5_format
+from keras_core.src.utils import file_utils
 from keras_core.src.utils import io_utils
 
 try:
     import h5py
 except ImportError:
     h5py = None
 
@@ -106,24 +105,24 @@
 
     is_keras_zip = str(filepath).endswith(".keras") and zipfile.is_zipfile(
         filepath
     )
 
     # Support for remote zip files
     if (
-        saving_lib.is_remote_path(filepath)
-        and not gfile.isdir(filepath)
+        file_utils.is_remote_path(filepath)
+        and not file_utils.isdir(filepath)
         and not is_keras_zip
     ):
         local_path = os.path.join(
             saving_lib.get_temp_dir(), os.path.basename(filepath)
         )
 
         # Copy from remote to temporary local directory
-        gfile.copy(filepath, local_path, overwrite=True)
+        file_utils.copy(filepath, local_path, overwrite=True)
 
         # Switch filepath to local zipfile for loading model
         if zipfile.is_zipfile(local_path):
             filepath = local_path
             is_keras_zip = True
 
     if is_keras_zip:
```

### Comparing `keras-core-0.1.0/keras_core/src/saving/saving_lib.py` & `keras-core-0.1.1/keras_core/src/saving/saving_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Python-based idempotent model-saving functionality."""
 
 import datetime
 import io
 import json
 import os
-import re
 import tempfile
 import warnings
 import zipfile
 
 import numpy as np
-from tensorflow.io import gfile
 
 from keras_core.src.backend.common import global_state
 from keras_core.src.layers.layer import Layer
 from keras_core.src.losses.loss import Loss
 from keras_core.src.metrics.metric import Metric
 from keras_core.src.optimizers.optimizer import Optimizer
 from keras_core.src.saving.serialization_lib import ObjectSharingScope
 from keras_core.src.saving.serialization_lib import deserialize_keras_object
 from keras_core.src.saving.serialization_lib import serialize_keras_object
+from keras_core.src.utils import file_utils
 from keras_core.src.utils import naming
-
-keras_version = "0.0.0"  # TODO
+from keras_core.src.version import __version__ as keras_version
 
 try:
     import h5py
 except ImportError:
     h5py = None
 
 _CONFIG_FILENAME = "config.json"
@@ -82,16 +80,15 @@
     config_json = json.dumps(serialized_model_dict)
     metadata_json = json.dumps(
         {
             "keras_version": keras_version,
             "date_saved": datetime.datetime.now().strftime("%Y-%m-%d@%H:%M:%S"),
         }
     )
-    # TODO(rameshsampath): Need a better logic for local vs remote path
-    if is_remote_path(filepath):
+    if file_utils.is_remote_path(filepath):
         # Remote path. Zip to local drive and copy to remote
         zip_filepath = os.path.join(get_temp_dir(), "tmp_model.keras")
     else:
         zip_filepath = filepath
 
     with zipfile.ZipFile(zip_filepath, "w") as zf:
         with zf.open(_METADATA_FILENAME, "w") as f:
@@ -120,32 +117,32 @@
             assets_store=asset_store,
             inner_path="",
             visited_trackables=set(),
         )
         weights_store.close()
         asset_store.close()
 
-    if is_remote_path(filepath):
+    if file_utils.is_remote_path(filepath):
         # Using gfile context manager doesn't close zip file when
         # writing to GCS. Hence writing to local and copying to filepath.
-        gfile.copy(zip_filepath, filepath, overwrite=True)
+        file_utils.copy(zip_filepath, filepath, overwrite=True)
         os.remove(zip_filepath)
 
 
 def load_model(filepath, custom_objects=None, compile=True, safe_mode=True):
     """Load a zip archive representing a Keras model."""
 
     filepath = str(filepath)
     if not filepath.endswith(".keras"):
         raise ValueError(
             "Invalid filename: expected a `.keras` extension. "
             f"Received: filepath={filepath}"
         )
 
-    with gfile.GFile(filepath, mode="r+b") as gfile_handle, zipfile.ZipFile(
+    with file_utils.File(filepath, mode="r+b") as gfile_handle, zipfile.ZipFile(
         gfile_handle, "r"
     ) as zf:
         with zf.open(_CONFIG_FILENAME, "r") as f:
             config_json = f.read()
 
         # Note: we should NOT use a custom JSON decoder. Anything that
         # needs custom decoding must be handled in deserialize_keras_object.
@@ -235,33 +232,27 @@
         weights_store=weights_store,
         assets_store=None,
         inner_path="",
         skip_mismatch=skip_mismatch,
         visited_trackables=set(),
     )
     weights_store.close()
-    if temp_dir and gfile.exists(temp_dir):
-        gfile.rmtree(temp_dir)
+    if temp_dir and file_utils.exists(temp_dir):
+        file_utils.rmtree(temp_dir)
     if archive:
         archive.close()
 
 
-def is_remote_path(filepath):
-    if re.match(r"^(/cns|/cfs|/gcs|.*://).*$", str(filepath)):
-        return True
-    return False
-
-
 def _write_to_zip_recursively(zipfile_to_save, system_path, zip_path):
-    if not gfile.isdir(system_path):
+    if not file_utils.isdir(system_path):
         zipfile_to_save.write(system_path, zip_path)
     else:
-        for file_name in gfile.listdir(system_path):
-            system_file_path = gfile.join(system_path, file_name)
-            zip_file_path = gfile.join(zip_path, file_name)
+        for file_name in file_utils.listdir(system_path):
+            system_file_path = file_utils.join(system_path, file_name)
+            zip_file_path = file_utils.join(zip_path, file_name)
             _write_to_zip_recursively(
                 zipfile_to_save, system_file_path, zip_file_path
             )
 
 
 def _walk_trackable(trackable):
     if isinstance(trackable, Layer):
@@ -304,23 +295,23 @@
     # Recursively save state of children trackables (layers, optimizers, etc.)
     for child_attr, child_obj in _walk_trackable(trackable):
         if _is_keras_trackable(child_obj):
             _save_state(
                 child_obj,
                 weights_store,
                 assets_store,
-                inner_path=gfile.join(inner_path, child_attr),
+                inner_path=file_utils.join(inner_path, child_attr),
                 visited_trackables=visited_trackables,
             )
         elif isinstance(child_obj, (list, dict, tuple, set)):
             _save_container_state(
                 child_obj,
                 weights_store,
                 assets_store,
-                inner_path=gfile.join(inner_path, child_attr),
+                inner_path=file_utils.join(inner_path, child_attr),
                 visited_trackables=visited_trackables,
             )
 
 
 def _load_state(
     trackable,
     weights_store,
@@ -366,24 +357,24 @@
     # Recursively load states for Keras trackables such as layers/optimizers.
     for child_attr, child_obj in _walk_trackable(trackable):
         if _is_keras_trackable(child_obj):
             _load_state(
                 child_obj,
                 weights_store,
                 assets_store,
-                inner_path=gfile.join(inner_path, child_attr),
+                inner_path=file_utils.join(inner_path, child_attr),
                 skip_mismatch=skip_mismatch,
                 visited_trackables=visited_trackables,
             )
         elif isinstance(child_obj, (list, dict, tuple, set)):
             _load_container_state(
                 child_obj,
                 weights_store,
                 assets_store,
-                inner_path=gfile.join(inner_path, child_attr),
+                inner_path=file_utils.join(inner_path, child_attr),
                 skip_mismatch=skip_mismatch,
                 visited_trackables=visited_trackables,
             )
 
 
 def _save_container_state(
     container, weights_store, assets_store, inner_path, visited_trackables
@@ -403,15 +394,15 @@
                 name = f"{name}_{used_names[name]}"
             else:
                 used_names[name] = 0
             _save_state(
                 trackable,
                 weights_store,
                 assets_store,
-                inner_path=gfile.join(inner_path, name),
+                inner_path=file_utils.join(inner_path, name),
                 visited_trackables=visited_trackables,
             )
 
 
 def _load_container_state(
     container,
     weights_store,
@@ -432,15 +423,15 @@
                 name = f"{name}_{used_names[name]}"
             else:
                 used_names[name] = 0
             _load_state(
                 trackable,
                 weights_store,
                 assets_store,
-                inner_path=gfile.join(inner_path, name),
+                inner_path=file_utils.join(inner_path, name),
                 skip_mismatch=skip_mismatch,
                 visited_trackables=visited_trackables,
             )
 
 
 class DiskIOStore:
     """Asset store backed by disk storage.
@@ -457,48 +448,48 @@
         self.root_path = root_path
         self.archive = archive
         self.tmp_dir = None
         if self.archive:
             self.tmp_dir = get_temp_dir()
             if self.mode == "r":
                 self.archive.extractall(path=self.tmp_dir)
-            self.working_dir = gfile.join(self.tmp_dir, self.root_path)
+            self.working_dir = file_utils.join(self.tmp_dir, self.root_path)
             if self.mode == "w":
-                gfile.makedirs(self.working_dir)
+                file_utils.makedirs(self.working_dir)
         else:
             if mode == "r":
                 self.working_dir = root_path
             else:
                 self.tmp_dir = get_temp_dir()
-                self.working_dir = gfile.join(self.tmp_dir, self.root_path)
-                gfile.makedirs(self.working_dir)
+                self.working_dir = file_utils.join(self.tmp_dir, self.root_path)
+                file_utils.makedirs(self.working_dir)
 
     def make(self, path):
         if not path:
             return self.working_dir
-        path = gfile.join(self.working_dir, path)
-        if not gfile.exists(path):
-            gfile.makedirs(path)
+        path = file_utils.join(self.working_dir, path)
+        if not file_utils.exists(path):
+            file_utils.makedirs(path)
         return path
 
     def get(self, path):
         if not path:
             return self.working_dir
-        path = gfile.join(self.working_dir, path)
-        if gfile.exists(path):
+        path = file_utils.join(self.working_dir, path)
+        if file_utils.exists(path):
             return path
         return None
 
     def close(self):
         if self.mode == "w" and self.archive:
             _write_to_zip_recursively(
                 self.archive, self.working_dir, self.root_path
             )
-        if self.tmp_dir and gfile.exists(self.tmp_dir):
-            gfile.rmtree(self.tmp_dir)
+        if self.tmp_dir and file_utils.exists(self.tmp_dir):
+            file_utils.rmtree(self.tmp_dir)
 
 
 class H5IOStore:
     def __init__(self, root_path, archive=None, mode="r"):
         """Numerical variable store backed by HDF5.
 
         If `archive` is specified, then `root_path` refers to the filename
```

### Comparing `keras-core-0.1.0/keras_core/src/saving/serialization_lib.py` & `keras-core-0.1.1/keras_core/src/saving/serialization_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import importlib
 import inspect
 import types
 import warnings
 
 import numpy as np
-import tensorflow as tf
 
 from keras_core.src import api_export
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.backend.common import global_state
 from keras_core.src.saving import object_registration
 from keras_core.src.utils import python_utils
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 PLAIN_TYPES = (str, int, float, bool)
 
 # List of Keras modules with built-in string representations for Keras defaults
 BUILTIN_MODULES = (
     "activations",
     "constraints",
@@ -155,15 +155,15 @@
             "class_name": "__keras_tensor__",
             "config": {
                 "shape": obj.shape,
                 "dtype": obj.dtype,
                 "keras_history": history,
             },
         }
-    if isinstance(obj, tf.TensorShape):
+    if tf.available and isinstance(obj, tf.TensorShape):
         return obj.as_list() if obj._dims is not None else None
     if backend.is_tensor(obj):
         return {
             "class_name": "__tensor__",
             "config": {
                 "value": backend.convert_to_numpy(obj).tolist(),
                 "dtype": backend.standardize_dtype(obj.dtype),
@@ -177,15 +177,15 @@
                     "value": obj.tolist(),
                     "dtype": backend.standardize_dtype(obj.dtype),
                 },
             }
         else:
             # Treat numpy floats / etc as plain types.
             return obj.item()
-    if isinstance(obj, tf.DType):
+    if tf.available and isinstance(obj, tf.DType):
         return obj.name
     if isinstance(obj, types.FunctionType) and obj.__name__ == "<lambda>":
         warnings.warn(
             "The object being serialized includes a `lambda`. This is unsafe. "
             "In order to reload the object, you will have to pass "
             "`safe_mode=False` to the loading function. "
             "Please avoid using `lambda` in the "
@@ -195,15 +195,15 @@
         )
         return {
             "class_name": "__lambda__",
             "config": {
                 "value": python_utils.func_dump(obj),
             },
         }
-    if isinstance(obj, tf.TypeSpec):
+    if tf.available and isinstance(obj, tf.TypeSpec):
         ts_config = obj._serialize()
         # TensorShape and tf.DType conversion
         ts_config = list(
             map(
                 lambda x: x.as_list()
                 if isinstance(x, tf.TensorShape)
                 else (x.name if isinstance(x, tf.DType) else x),
@@ -463,15 +463,14 @@
         safe_mode: Boolean, whether to disallow unsafe `lambda` deserialization.
             When `safe_mode=False`, loading an object has the potential to
             trigger arbitrary code execution. This argument is only
             applicable to the Keras v3 model format. Defaults to `True`.
 
     Returns:
         The object described by the `config` dictionary.
-
     """
     safe_scope_arg = in_safe_mode()  # Enforces SafeModeScope
     safe_mode = safe_scope_arg if safe_scope_arg is not None else safe_mode
 
     module_objects = kwargs.pop("module_objects", None)
     custom_objects = custom_objects or {}
     tlco = global_state.get_global_attribute("custom_objects_scope_dict", {})
@@ -600,24 +599,24 @@
                 "This carries a potential risk of arbitrary code execution "
                 "and thus it is disallowed by default. If you trust the "
                 "source of the saved model, you can pass `safe_mode=False` to "
                 "the loading function in order to allow `lambda` loading, "
                 "or call `keras_core.config.enable_unsafe_deserialization()`."
             )
         return python_utils.func_load(inner_config["value"])
-    if config["class_name"] == "__typespec__":
+    if tf is not None and config["class_name"] == "__typespec__":
         obj = _retrieve_class_or_fn(
             config["spec_name"],
             config["registered_name"],
             config["module"],
             obj_type="class",
             full_config=config,
             custom_objects=custom_objects,
         )
-        # Conversion to TensorShape and tf.DType
+        # Conversion to TensorShape and DType
         inner_config = map(
             lambda x: tf.TensorShape(x)
             if isinstance(x, list)
             else (getattr(tf, x) if hasattr(tf.dtypes, str(x)) else x),
             inner_config,
         )
         return obj._deserialize(tuple(inner_config))
```

### Comparing `keras-core-0.1.0/keras_core/src/testing/test_case.py` & `keras-core-0.1.1/keras_core/src/testing/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import shutil
 import tempfile
 import unittest
 
 import numpy as np
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import ops
 from keras_core.src import utils
 from keras_core.src.models import Model
 from keras_core.src.utils import traceback_utils
 
@@ -253,25 +253,25 @@
                     output_shape = [v.shape for v in expected_output_shape]
                     self.assertEqual(
                         expected_output_shape,
                         output_shape,
                         msg="Unexpected output shape",
                     )
                 if expected_output_dtype is not None:
-                    output_dtype = nest.flatten(output)[0].dtype
+                    output_dtype = tree.flatten(output)[0].dtype
                     self.assertEqual(
                         expected_output_dtype,
                         backend.standardize_dtype(output_dtype),
                         msg="Unexpected output dtype",
                     )
             if eager:
                 if expected_output is not None:
                     self.assertEqual(type(expected_output), type(output))
                     for ref_v, v in zip(
-                        nest.flatten(expected_output), nest.flatten(output)
+                        tree.flatten(expected_output), tree.flatten(output)
                     ):
                         self.assertAllClose(
                             ref_v, v, msg="Unexpected output value"
                         )
                 if expected_num_losses is not None:
                     self.assertLen(layer.losses, expected_num_losses)
 
@@ -282,18 +282,18 @@
                     self.layer = layer
 
                 def call(self, x):
                     return self.layer(x)
 
             model = TestModel(layer)
             model.compile(optimizer="sgd", loss="mse", jit_compile=True)
-            input_data = nest.map_structure(
+            input_data = tree.map_structure(
                 lambda x: backend.convert_to_numpy(x), input_data
             )
-            output_data = nest.map_structure(
+            output_data = tree.map_structure(
                 lambda x: backend.convert_to_numpy(x), output_data
             )
             model.fit(input_data, output_data, verbose=0)
 
         # Build test.
         if input_shape is not None:
             layer = layer_cls(**init_kwargs)
```

### Comparing `keras-core-0.1.0/keras_core/src/testing/test_utils.py` & `keras-core-0.1.1/keras_core/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/trainers/compile_utils.py` & `keras-core-0.1.1/keras_core/src/trainers/compile_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src import losses as losses_module
 from keras_core.src import metrics as metrics_module
 from keras_core.src import ops
 from keras_core.src.utils.naming import get_object_name
 
@@ -210,15 +210,15 @@
                         f"output. Received:\n{argument_name}={metrics}"
                     )
         if num_outputs == 1:
             if not metrics:
                 flat_metrics.append(None)
             else:
                 if isinstance(metrics, dict):
-                    metrics = nest.flatten(metrics)
+                    metrics = tree.flatten(metrics)
                 if not isinstance(metrics, list):
                     metrics = [metrics]
                 if not all(is_function_like(m) for m in metrics):
                     raise ValueError(
                         f"Expected all entries in the `{argument_name}` list "
                         f"to be metric objects. Received instead:\n"
                         f"{argument_name}={metrics}"
@@ -302,15 +302,15 @@
     def _flatten_y(self, y):
         if isinstance(y, dict) and self.output_names:
             result = []
             for name in self.output_names:
                 if name in y:
                     result.append(y[name])
             return result
-        return nest.flatten(y)
+        return tree.flatten(y)
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         if not self.built:
             self.build(y_true, y_pred)
         y_true = self._flatten_y(y_true)
         y_pred = self._flatten_y(y_pred)
         for m, y_t, y_p in zip(self._flat_metrics, y_true, y_pred):
@@ -442,28 +442,28 @@
                     raise ValueError(
                         "In the dict argument `loss`, key "
                         f"'{name}' does not correspond to any model output. "
                         f"Received:\nloss={loss}"
                     )
         if num_outputs == 1:
             if isinstance(loss, dict):
-                loss = nest.flatten(loss)
+                loss = tree.flatten(loss)
             if isinstance(loss, list) and len(loss) == 1:
                 loss = loss[0]
             if not is_function_like(loss):
                 raise ValueError(
                     "When there is only a single output, the `loss` argument "
                     "must be a callable. "
                     f"Received instead:\nloss={loss} of type {type(loss)}"
                 )
 
-        if is_function_like(loss) and nest.is_nested(y_pred):
+        if is_function_like(loss) and tree.is_nested(y_pred):
             # The model has multiple outputs but only one loss fn
             # was provided. Broadcast loss to all outputs.
-            loss = nest.map_structure(lambda x: loss, y_pred)
+            loss = tree.map_structure(lambda x: loss, y_pred)
 
         # Iterate over all possible loss formats:
         # plain function, list/tuple, dict
         if is_function_like(loss):
             flat_losses.append(get_loss(loss, y_true, y_pred))
             if loss_weights:
                 if not isinstance(loss_weights, float):
@@ -474,15 +474,15 @@
                         f"Received instead: loss_weights={loss_weights} of "
                         f"type {type(loss_weights)}"
                     )
                 flat_loss_weights.append(loss_weights)
             else:
                 flat_loss_weights.append(1.0)
         elif isinstance(loss, (list, tuple)):
-            loss = nest.flatten(loss)
+            loss = tree.flatten(loss)
             if len(loss) != len(y_pred):
                 raise ValueError(
                     "For a model with multiple outputs, "
                     "when providing the `loss` argument as a list, "
                     "it should have as many entries as the model has outputs. "
                     f"Received:\nloss={loss}\nof length {len(loss)} "
                     f"whereas the model has {len(y_pred)} outputs."
@@ -593,15 +593,15 @@
     def _flatten_y(self, y):
         if isinstance(y, dict) and self.output_names:
             result = []
             for name in self.output_names:
                 if name in y:
                     result.append(y[name])
             return result
-        return nest.flatten(y)
+        return tree.flatten(y)
 
     def call(self, y_true, y_pred, sample_weight=None):
         if not self.built:
             self.build(y_true, y_pred)
 
         y_true = self._flatten_y(y_true)
         y_pred = self._flatten_y(y_pred)
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/array_data_adapter.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/array_data_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import math
 
 import numpy as np
-import tensorflow as tf
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src.trainers.data_adapters import data_adapter_utils
 from keras_core.src.trainers.data_adapters.data_adapter import DataAdapter
+from keras_core.src.utils.nest import lists_to_tuples
 
 try:
     import pandas
 except ImportError:
     pandas = None
 
 
@@ -36,15 +36,15 @@
         x, y, sample_weight = convert_to_arrays((x, y, sample_weight))
         if sample_weight is not None:
             if class_weight is not None:
                 raise ValueError(
                     "You cannot `class_weight` and `sample_weight` "
                     "at the same time."
                 )
-            if tf.nest.is_nested(y):
+            if tree.is_nested(y):
                 if isinstance(sample_weight, np.ndarray):
                     is_samplewise = len(sample_weight.shape) == 1 or (
                         len(sample_weight.shape) == 2
                         and sample_weight.shape[1] == 1
                     )
                     if not is_samplewise:
                         raise ValueError(
@@ -52,41 +52,41 @@
                             "a single `sample_weight` array, it should only "
                             "have one scalar score per sample "
                             "(i.e. shape `(num_samples,)`). If you want to use "
                             "non-scalar sample weights, pass a `sample_weight` "
                             "argument with one array per model output."
                         )
                     # Replicate the same sample_weight array on all outputs.
-                    sample_weight = tf.nest.map_structure(
+                    sample_weight = tree.map_structure(
                         lambda _: sample_weight, y
                     )
                 else:
                     try:
-                        tf.nest.assert_same_structure(y, sample_weight)
+                        tree.assert_same_structure(y, sample_weight)
                     except ValueError:
                         raise ValueError(
                             "You should provide one `sample_weight` array per "
                             "output in `y`. The two structures did not match:\n"
                             f"- y: {y}\n"
                             f"- sample_weight: {sample_weight}\n"
                         )
         if class_weight is not None:
-            if tf.nest.is_nested(y):
+            if tree.is_nested(y):
                 raise ValueError(
                     "`class_weight` is only supported for Models with a single "
                     "output."
                 )
             sample_weight = data_adapter_utils.class_weight_to_sample_weights(
                 y, class_weight
             )
 
         inputs = data_adapter_utils.pack_x_y_sample_weight(x, y, sample_weight)
 
         data_adapter_utils.check_data_cardinality(inputs)
-        num_samples = set(i.shape[0] for i in nest.flatten(inputs)).pop()
+        num_samples = set(i.shape[0] for i in tree.flatten(inputs)).pop()
         self._num_samples = num_samples
         self._inputs = inputs
 
         # If batch_size is not passed but steps is, calculate from the input
         # data.  Defaults to `32` for backwards compatibility.
         if not batch_size:
             batch_size = int(math.ceil(num_samples / steps)) if steps else 32
@@ -100,17 +100,19 @@
         inputs = self._inputs
         if self._shuffle:
             inputs = data_adapter_utils.sync_shuffle(
                 inputs, num_samples=self._num_samples
             )
         for i in range(self._size):
             start, stop = i * self._batch_size, (i + 1) * self._batch_size
-            yield tf.nest.map_structure(lambda x: x[start:stop], inputs)
+            yield tree.map_structure(lambda x: x[start:stop], inputs)
 
     def get_tf_dataset(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
         inputs = self._inputs
         shuffle = self._shuffle
         batch_size = self._batch_size
         num_samples = self._num_samples
         num_full_batches = int(self._num_samples // batch_size)
 
         # Vectorized version of shuffle.
@@ -172,69 +174,73 @@
                         indices, [num_in_full_batch], [self._partial_batch_size]
                     )
                 )
                 flat_dataset = flat_dataset.concatenate(index_remainder)
 
             return flat_dataset
 
+        def slice_inputs(indices_dataset, inputs):
+            """Slice inputs into a Dataset of batches.
+
+            Given a Dataset of batch indices and the unsliced inputs,
+            this step slices the inputs in a parallelized fashion
+            and produces a dataset of input batches.
+
+            Args:
+                indices_dataset: A Dataset of batched indices.
+                inputs: A python data structure that contains the inputs,
+                    targets, and possibly sample weights.
+
+            Returns:
+                A Dataset of input batches matching the batch indices.
+            """
+            dataset = tf.data.Dataset.zip(
+                (indices_dataset, tf.data.Dataset.from_tensors(inputs).repeat())
+            )
+
+            def grab_batch(i, data):
+                return tree.map_structure(
+                    lambda d: tf.gather(d, i, axis=0), data
+                )
+
+            dataset = dataset.map(
+                grab_batch, num_parallel_calls=tf.data.AUTOTUNE
+            )
+
+            # Default optimizations are disabled to avoid the overhead of
+            # (unnecessary) input pipeline graph serialization & deserialization
+            options = tf.data.Options()
+            options.experimental_optimization.apply_default_optimizations = (
+                False
+            )
+            if self._shuffle:
+                options.experimental_external_state_policy = (
+                    tf.data.experimental.ExternalStatePolicy.IGNORE
+                )
+            dataset = dataset.with_options(options)
+            return dataset
+
         indices_dataset = indices_dataset.flat_map(slice_batch_indices)
 
-        dataset = self.slice_inputs(indices_dataset, inputs)
+        dataset = slice_inputs(indices_dataset, inputs)
 
         if shuffle == "batch":
 
             def shuffle_batch(*batch):
-                return tf.nest.map_structure(tf.random.shuffle, batch)
+                return tree.map_structure(tf.random.shuffle, batch)
 
             dataset = dataset.map(shuffle_batch)
 
         options = tf.data.Options()
         options.experimental_distribute.auto_shard_policy = (
             tf.data.experimental.AutoShardPolicy.DATA
         )
         dataset = dataset.with_options(options)
         return dataset.prefetch(tf.data.AUTOTUNE)
 
-    def slice_inputs(self, indices_dataset, inputs):
-        """Slice inputs into a Dataset of batches.
-
-        Given a Dataset of batch indices and the unsliced inputs,
-        this step slices the inputs in a parallelized fashion
-        and produces a dataset of input batches.
-
-        Args:
-            indices_dataset: A Dataset of batched indices.
-            inputs: A python data structure that contains the inputs, targets,
-                and possibly sample weights.
-
-        Returns:
-            A Dataset of input batches matching the batch indices.
-        """
-        dataset = tf.data.Dataset.zip(
-            (indices_dataset, tf.data.Dataset.from_tensors(inputs).repeat())
-        )
-
-        def grab_batch(i, data):
-            return tf.nest.map_structure(
-                lambda d: tf.gather(d, i, axis=0), data
-            )
-
-        dataset = dataset.map(grab_batch, num_parallel_calls=tf.data.AUTOTUNE)
-
-        # Default optimizations are disabled to avoid the overhead of
-        # (unnecessary) input pipeline graph serialization and deserialization
-        options = tf.data.Options()
-        options.experimental_optimization.apply_default_optimizations = False
-        if self._shuffle:
-            options.experimental_external_state_policy = (
-                tf.data.experimental.ExternalStatePolicy.IGNORE
-            )
-        dataset = dataset.with_options(options)
-        return dataset
-
     @property
     def num_batches(self):
         return self._size
 
     @property
     def batch_size(self):
         return self._batch_size
@@ -262,15 +268,15 @@
     def can_convert_single_array(x):
         is_none = x is None
         known_type = isinstance(x, data_adapter_utils.ARRAY_TYPES)
         convertable_type = hasattr(x, "__array__")
         return is_none or known_type or convertable_type
 
     return all(
-        tf.nest.flatten(tf.nest.map_structure(can_convert_single_array, arrays))
+        tree.flatten(tree.map_structure(can_convert_single_array, arrays))
     )
 
 
 def convert_to_arrays(arrays, dtype=None):
     """Process array-like inputs.
 
     This function:
@@ -291,33 +297,37 @@
         if x is None:
             return x
         if pandas is not None:
             if isinstance(x, pandas.Series):
                 x = np.expand_dims(x.to_numpy(dtype=dtype), axis=-1)
             elif isinstance(x, pandas.DataFrame):
                 x = x.to_numpy(dtype=dtype)
-        if isinstance(x, (tf.Tensor, tf.Variable)):
-            x = x.numpy()
-        if isinstance(x, tf.RaggedTensor):
+        if is_tf_ragged_tensor(x):
+            from keras_core.src.utils.module_utils import tensorflow as tf
+
             return tf.cast(x, dtype=dtype)
         if not isinstance(x, np.ndarray):
             # Using `__array__` should handle `tf.Tensor`, `jax.np.ndarray`,
             # `torch.Tensor`, as well as any other tensor-like object that has
             # added numpy support.
             if hasattr(x, "__array__"):
-                x = np.array(x, dtype=dtype)
+                x = backend.convert_to_numpy(x).astype(dtype)
             else:
                 raise ValueError(
                     "Expected a NumPy array, tf.Tensor, tf.RaggedTensor, "
                     "jax.np.ndarray, torch.Tensor, Pandas Dataframe, or "
                     "Pandas Series. Received invalid input: "
                     f"{x} (of type {type(x)})"
                 )
         if x.dtype == object:
             return x
         if not x.dtype == dtype:
             x = x.astype(dtype)
         return x
 
-    arrays = tf.nest.map_structure(convert_single_array, arrays)
-    return tf.__internal__.nest.list_to_tuple(arrays)
+    arrays = tree.map_structure(convert_single_array, arrays)
+    return lists_to_tuples(arrays)
+
+
+def is_tf_ragged_tensor(x):
+    return x.__class__.__name__ == "RaggedTensor"
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/data_adapter.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/data_adapter_utils.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import math
 
 import numpy as np
-import tensorflow as tf
+import tree
 
+from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 
 try:
     import pandas
 except ImportError:
     pandas = None
 
 
 # Leave jax, tf, and torch arrays off this list. Instead we will use
 # `__array__` to detect these types. Doing so allows us to avoid importing a
 # backend framework we are not currently using just to do type-checking.
-ARRAY_TYPES = (np.ndarray, tf.RaggedTensor)
+ARRAY_TYPES = (np.ndarray,)
+if backend.backend() == "tensorflow":
+    from keras_core.src.utils.module_utils import tensorflow as tf
+
+    ARRAY_TYPES = ARRAY_TYPES + (np.ndarray, tf.RaggedTensor)
 if pandas:
     ARRAY_TYPES = ARRAY_TYPES + (pandas.Series, pandas.DataFrame)
 
 
 @keras_core_export("keras_core.utils.unpack_x_y_sample_weight")
 def unpack_x_y_sample_weight(data):
     """Unpacks user-provided data tuple.
@@ -26,16 +31,16 @@
     This is a convenience utility to be used when overriding
     `Model.train_step`, `Model.test_step`, or `Model.predict_step`.
     This utility makes it easy to support data of the form `(x,)`,
     `(x, y)`, or `(x, y, sample_weight)`.
 
     Standalone usage:
 
-    >>> features_batch = tf.ones((10, 5))
-    >>> labels_batch = tf.zeros((10, 5))
+    >>> features_batch = ops.ones((10, 5))
+    >>> labels_batch = ops.zeros((10, 5))
     >>> data = (features_batch, labels_batch)
     >>> # `y` and `sample_weight` will default to `None` if not provided.
     >>> x, y, sample_weight = unpack_x_y_sample_weight(data)
     >>> sample_weight is None
     True
 
     Args:
@@ -63,35 +68,35 @@
 
 
 @keras_core_export("keras_core.utils.pack_x_y_sample_weight")
 def pack_x_y_sample_weight(x, y=None, sample_weight=None):
     """Packs user-provided data into a tuple.
 
     This is a convenience utility for packing data into the tuple formats
-    that `Model.fit` uses.
+    that `Model.fit()` uses.
 
     Standalone usage:
 
-    >>> x = tf.ones((10, 1))
+    >>> x = ops.ones((10, 1))
     >>> data = pack_x_y_sample_weight(x)
-    >>> isinstance(data, tf.Tensor)
+    >>> isinstance(data, ops.Tensor)
     True
-    >>> y = tf.ones((10, 1))
+    >>> y = ops.ones((10, 1))
     >>> data = pack_x_y_sample_weight(x, y)
     >>> isinstance(data, tuple)
     True
     >>> x, y = data
 
     Args:
         x: Features to pass to `Model`.
         y: Ground-truth targets to pass to `Model`.
         sample_weight: Sample weight for each element.
 
     Returns:
-        Tuple in the format used in `Model.fit`.
+        Tuple in the format used in `Model.fit()`.
     """
     if y is None:
         # For single x-input, we do no tuple wrapping since in this case
         # there is no ambiguity. This also makes NumPy and Dataset
         # consistent in that the user does not have to wrap their Dataset
         # data in an unnecessary tuple.
         if not isinstance(x, tuple or list):
@@ -108,35 +113,35 @@
     """Datasets will stack any list of tensors, so we convert them to tuples."""
     if isinstance(maybe_list, list):
         return tuple(maybe_list)
     return maybe_list
 
 
 def check_data_cardinality(data):
-    num_samples = set(int(i.shape[0]) for i in tf.nest.flatten(data))
+    num_samples = set(int(i.shape[0]) for i in tree.flatten(data))
     if len(num_samples) > 1:
         msg = (
             "Data cardinality is ambiguous. "
             "Make sure all arrays contain the same number of samples."
         )
         for label, single_data in zip(["x", "y", "sample_weight"], data):
             sizes = ", ".join(
-                str(i.shape[0]) for i in tf.nest.flatten(single_data)
+                str(i.shape[0]) for i in tree.flatten(single_data)
             )
             msg += f"'{label}' sizes: {sizes}\n"
         raise ValueError(msg)
 
 
 def sync_shuffle(data, num_samples=None):
     if num_samples is None:
-        num_samples_set = set(int(i.shape[0]) for i in tf.nest.flatten(data))
+        num_samples_set = set(int(i.shape[0]) for i in tree.flatten(data))
         assert len(num_samples_set) == 1
         num_samples = num_samples_set.pop()
     p = np.random.permutation(num_samples)
-    return tf.nest.map_structure(lambda x: x[p], data)
+    return tree.map_structure(lambda x: x[p], data)
 
 
 def train_validation_split(arrays, validation_split):
     """Split arrays into train and validation subsets in deterministic order.
 
     The last part of data will become validation data.
 
@@ -150,20 +155,20 @@
     Returns:
         `(train_arrays, validation_arrays)`
     """
 
     def _can_split(t):
         return isinstance(t, ARRAY_TYPES) or t is None
 
-    flat_arrays = tf.nest.flatten(arrays)
+    flat_arrays = tree.flatten(arrays)
     unsplitable = [type(t) for t in flat_arrays if not _can_split(t)]
     if unsplitable:
         raise ValueError(
             "Argument `validation_split` is only supported "
-            "for tf.Tensors or NumPy "
+            "for tensors or NumPy "
             "arrays. Found incompatible type in the input: {unsplitable}"
         )
 
     if all(t is None for t in flat_arrays):
         return arrays, arrays
 
     first_non_none = None
@@ -186,18 +191,18 @@
         )
 
     def _split(t, start, end):
         if t is None:
             return t
         return t[start:end]
 
-    train_arrays = tf.nest.map_structure(
+    train_arrays = tree.map_structure(
         lambda x: _split(x, start=0, end=split_at), arrays
     )
-    val_arrays = tf.nest.map_structure(
+    val_arrays = tree.map_structure(
         lambda x: _split(x, start=split_at, end=batch_dim), arrays
     )
     return train_arrays, val_arrays
 
 
 def class_weight_to_sample_weights(y, class_weight):
     sample_weight = np.ones(shape=(y.shape[0],), dtype=y.dtype)
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/generator_data_adapter.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 import itertools
 
-import tensorflow as tf
+import tree
 
 from keras_core.src.trainers.data_adapters.data_adapter import DataAdapter
 
 
 class GeneratorDataAdapter(DataAdapter):
     """Adapter for Python generators."""
 
-    def __init__(self, x):
-        data, generator = peek_and_restore(x)
+    def __init__(self, generator):
+        data, generator = peek_and_restore(generator)
         self.generator = generator
+        self._output_signature = None
         if not isinstance(data, tuple):
             raise ValueError(
                 "When passing a Python generator to a Keras model, "
                 "the generator must return a tuple, either "
                 "(input,) or (inputs, targets) or "
                 "(inputs, targets, sample_weights). "
                 f"Received: {data}"
             )
 
+    def _set_tf_output_signature(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
+        data, generator = peek_and_restore(self.generator)
+        self.generator = generator
+
         def get_tensor_spec(x):
             shape = x.shape
             if len(shape) < 1:
                 raise ValueError(
                     "When passing a Python generator to a Keras model, "
                     "the arrays returned by the generator "
                     "must be at least rank 1. Received: "
                     f"{x} of rank {len(x.shape)}"
                 )
             shape = list(shape)
             shape[0] = None  # The batch size is not guaranteed to be static.
             return tf.TensorSpec(shape=shape, dtype=x.dtype.name)
 
-        self._output_signature = tf.nest.map_structure(get_tensor_spec, data)
+        self._output_signature = tree.map_structure(get_tensor_spec, data)
 
     def get_numpy_iterator(self):
         for batch in self.generator:
             yield batch
 
     def get_tf_dataset(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
+        if self._output_signature is None:
+            self._set_tf_output_signature()
         ds = tf.data.Dataset.from_generator(
             self.get_numpy_iterator,
             output_signature=self._output_signature,
         )
         ds = ds.prefetch(tf.data.AUTOTUNE)
         return ds
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import threading
 import time
 import warnings
 import weakref
 from contextlib import closing
 
 import numpy as np
-import tensorflow as tf
+import tree
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.trainers.data_adapters import data_adapter_utils
 from keras_core.src.trainers.data_adapters.data_adapter import DataAdapter
 
 
 @keras_core_export(["keras_core.utils.PyDataset", "keras_core.utils.Sequence"])
@@ -181,33 +181,36 @@
         class_weight=None,
         shuffle=False,
     ):
         self.py_dataset = x
         self.class_weight = class_weight
         self.enqueuer = None
         self.shuffle = shuffle
+        self._output_signature = None
 
-        # Grab the first example
-        batch = self.py_dataset[0]
-        # Run checks on it and format it
-        batch = self._standardize_batch(batch)
+    def _set_tf_output_signature(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
 
         def get_tensor_spec(x):
             shape = x.shape
             if len(shape) < 1:
                 raise ValueError(
                     "The arrays returned by PyDataset.__getitem__() "
                     "must be at least rank 1. Received: "
                     f"{x} of rank {len(x.shape)}"
                 )
             shape = list(shape)
             shape[0] = None  # The batch size is not guaranteed to be static.
             return tf.TensorSpec(shape=shape, dtype=x.dtype.name)
 
-        self._output_signature = tf.nest.map_structure(get_tensor_spec, batch)
+        # Grab the first example
+        batch = self.py_dataset[0]
+        # Run checks on it and format it
+        batch = self._standardize_batch(batch)
+        self._output_signature = tree.map_structure(get_tensor_spec, batch)
 
     def _standardize_batch(self, batch):
         if isinstance(batch, np.ndarray):
             batch = (batch,)
         if isinstance(batch, list):
             batch = tuple(batch)
         if not isinstance(batch, tuple) or len(batch) not in {1, 2, 3}:
@@ -266,14 +269,19 @@
         for i, batch in enumerate(gen_fn()):
             batch = self._standardize_batch(batch)
             yield batch
             if i >= len(self.py_dataset) - 1 and self.enqueuer:
                 self.enqueuer.stop()
 
     def get_tf_dataset(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
+        if self._output_signature is None:
+            self._set_tf_output_signature()
+
         ds = tf.data.Dataset.from_generator(
             self.get_numpy_iterator,
             output_signature=self._output_signature,
         )
         if self.shuffle:
             ds = ds.shuffle(8)
         ds = ds.prefetch(tf.data.AUTOTUNE)
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-import tensorflow as tf
+import tree
 
 from keras_core.src.trainers.data_adapters import data_adapter_utils
 from keras_core.src.trainers.data_adapters.data_adapter import DataAdapter
 
 
 class TFDatasetAdapter(DataAdapter):
     """Adapter that handles `tf.data.Dataset`."""
 
     def __init__(self, dataset, class_weight=None):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
         if not isinstance(dataset, tf.data.Dataset):
             raise ValueError(
                 "Expected argument `dataset` to be a tf.data.Dataset. "
                 f"Received: {dataset}"
             )
         if class_weight is not None:
             dataset = dataset.map(
                 make_class_weight_map_fn(class_weight)
             ).prefetch(tf.data.AUTOTUNE)
         self._dataset = dataset
 
     def get_numpy_iterator(self):
         for batch in self._dataset:
-            yield tf.nest.map_structure(lambda x: x.numpy(), batch)
+            yield tree.map_structure(lambda x: x.numpy(), batch)
 
     def get_tf_dataset(self):
         return self._dataset
 
     @property
     def num_batches(self):
         cardinality = int(self._dataset.cardinality())
         # Return None for Unknown and Infiite cardinality datasets
         if cardinality < 0:
             return None
         return cardinality
 
     @property
     def batch_size(self):
-        first_element_spec = tf.nest.flatten(self._dataset.element_spec)[0]
+        first_element_spec = tree.flatten(self._dataset.element_spec)[0]
         return first_element_spec.shape[0]
 
     @property
     def has_partial_batch(self):
         return None
 
     @property
@@ -58,14 +60,16 @@
         class_weight: A map where the keys are integer class ids and values are
             the class weights, e.g. `{0: 0.2, 1: 0.6, 2: 0.3}`
 
     Returns:
         A function that can be used with `tf.data.Dataset.map` to apply class
         weighting.
     """
+    from keras_core.src.utils.module_utils import tensorflow as tf
+
     class_weight_tensor = tf.convert_to_tensor(
         [
             class_weight.get(int(c), 1.0)
             for c in range(max(class_weight.keys()) + 1)
         ]
     )
 
@@ -73,15 +77,15 @@
         """Convert `class_weight` to `sample_weight`."""
         x, y, sw = data_adapter_utils.unpack_x_y_sample_weight(data)
         if sw is not None:
             raise ValueError(
                 "You cannot `class_weight` and `sample_weight` "
                 "at the same time."
             )
-        if tf.nest.is_nested(y):
+        if tree.is_nested(y):
             raise ValueError(
                 "`class_weight` is only supported for Models with a single "
                 "output."
             )
 
         if y.shape.rank >= 2:
             y_classes = tf.__internal__.smart_cond.smart_cond(
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/data_adapters/torch_data_adapter.py` & `keras-core-0.1.1/keras_core/src/trainers/data_adapters/torch_data_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import tensorflow as tf
+import tree
 
 from keras_core.src.trainers.data_adapters.data_adapter import DataAdapter
 
 
 class TorchDataLoaderAdapter(DataAdapter):
     """Adapter that handles `torch.utils.data.DataLoader`."""
 
@@ -18,27 +18,31 @@
         self._dataloader = dataloader
         self._batch_size = dataloader.batch_size
         self._size = len(dataloader)
         self._partial_batch_size = len(dataloader.dataset) % self._batch_size
 
     def get_numpy_iterator(self):
         for batch in self._dataloader:
-            yield tuple(tf.nest.map_structure(lambda x: x.numpy(), batch))
+            yield tuple(tree.map_structure(lambda x: x.numpy(), batch))
 
     def get_torch_dataloader(self):
         return self._dataloader
 
     def get_tf_dataset(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
         output_signature = self.peek_and_get_tensor_spec()
         return tf.data.Dataset.from_generator(
             self.get_numpy_iterator,
             output_signature=output_signature,
         )
 
     def peek_and_get_tensor_spec(self):
+        from keras_core.src.utils.module_utils import tensorflow as tf
+
         batch_data = next(iter(self._dataloader))
 
         def get_tensor_spec(x):
             shape = x.shape
             if len(shape) < 1:
                 raise ValueError(
                     "When passing a Pytorch DataLoader to a Keras model, "
@@ -50,15 +54,15 @@
             shape[0] = None  # The batch size is not guaranteed to be static.
 
             # No easy way to get string representation of dtype in torch
             # TODO: Figure out a better way to achieve this
             dtype = str(x.dtype).replace("torch.", "")
             return tf.TensorSpec(shape=shape, dtype=dtype)
 
-        return tuple(tf.nest.map_structure(get_tensor_spec, batch_data))
+        return tuple(tree.map_structure(get_tensor_spec, batch_data))
 
     @property
     def num_batches(self):
         return self._size
 
     @property
     def batch_size(self):
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/epoch_iterator.py` & `keras-core-0.1.1/keras_core/src/trainers/epoch_iterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,20 @@
 4. in __iter__, iterate, either for a fixed number of steps
 or until there is no data
 
 """
 import types
 import warnings
 
-import tensorflow as tf
-
 from keras_core.src.trainers.data_adapters import array_data_adapter
 from keras_core.src.trainers.data_adapters import generator_data_adapter
 from keras_core.src.trainers.data_adapters import py_dataset_adapter
 from keras_core.src.trainers.data_adapters import tf_dataset_adapter
 from keras_core.src.trainers.data_adapters import torch_data_adapter
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 class EpochIterator:
     def __init__(
         self,
         x,
         y=None,
@@ -73,15 +72,15 @@
                 y,
                 sample_weight=sample_weight,
                 class_weight=class_weight,
                 shuffle=shuffle,
                 batch_size=batch_size,
                 steps=steps_per_epoch,
             )
-        elif isinstance(x, tf.data.Dataset):
+        elif tf.available and isinstance(x, tf.data.Dataset):
             self.data_adapter = tf_dataset_adapter.TFDatasetAdapter(
                 x, class_weight=class_weight
             )
             # Unsupported args: y, sample_weight, shuffle
             if y is not None:
                 raise_unsupported_arg("y", "the targets", "tf.data.Dataset")
             if sample_weight is not None:
@@ -166,21 +165,27 @@
             if not self._current_iterator:
                 self._current_iterator = self._get_iterator(return_type)
                 self._insufficient_data = False
 
             for step in range(self.steps_per_epoch):
                 if self._insufficient_data:
                     break
+
+                if tf.available:
+                    errors = (StopIteration, tf.errors.OutOfRangeError)
+                else:
+                    errors = (StopIteration,)
+
                 try:
                     data = next(self._current_iterator)
                     buffer.append(data)
                     if len(buffer) == self.steps_per_execution:
                         yield step - len(buffer) + 1, buffer
                         buffer = []
-                except (StopIteration, tf.errors.OutOfRangeError):
+                except errors:
                     warnings.warn(
                         "Your input ran out of data; interrupting epoch. "
                         "Make sure that your dataset or generator can generate "
                         "at least `steps_per_epoch * epochs` batches. "
                         "You may need to use the `.repeat()` "
                         "function when building your dataset.",
                         stacklevel=2,
```

### Comparing `keras-core-0.1.0/keras_core/src/trainers/trainer.py` & `keras-core-0.1.1/keras_core/src/trainers/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             output_names = None
         if loss is not None:
             self._compile_loss = CompileLoss(
                 loss, loss_weights, output_names=output_names
             )
         else:
             self._compile_loss = None
-        if metrics is not None:
+        if metrics is not None or weighted_metrics is not None:
             self._compile_metrics = CompileMetrics(
                 metrics, weighted_metrics, output_names=output_names
             )
         else:
             self._compile_metrics = None
         if jit_compile == "auto":
             if run_eagerly:
@@ -767,15 +767,15 @@
         return True
     return False
 
 
 def model_supports_jit(model):
     if platform.system() == "Darwin" and "arm" in platform.processor().lower():
         if backend.backend() == "tensorflow":
-            import tensorflow as tf
+            from keras_core.src.utils.module_utils import tensorflow as tf
 
             if tf.config.list_physical_devices("GPU"):
                 return False
     if all(x.supports_jit for x in model._flatten_layers()):
         return True
     return False
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/__init__.py` & `keras-core-0.1.1/keras_core/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/argument_validation.py` & `keras-core-0.1.1/keras_core/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/backend_utils.py` & `keras-core-0.1.1/keras_core/src/utils/backend_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from keras_core.src import backend as backend_module
 
 
 def in_tf_graph():
     if "tensorflow" in sys.modules:
-        import tensorflow as tf
+        from keras_core.src.utils.module_utils import tensorflow as tf
 
         return not tf.executing_eagerly()
     return False
 
 
 class DynamicBackend:
     """A class that can be used to switch from one backend to another.
@@ -45,8 +45,16 @@
             from keras_core.src.backend import jax as jax_backend
 
             return getattr(jax_backend, name)
         if self._backend == "torch":
             from keras_core.src.backend import torch as torch_backend
 
             return getattr(torch_backend, name)
+        if self._backend == "numpy":
+            # TODO (ariG23498):
+            # The import `from keras_core.src.backend import numpy as numpy_backend`
+            # is not working. This is a temporary fix.
+            # The import is redirected to `keras_core.backend.numpy.numpy.py`
+            from keras_core.src import backend as numpy_backend
+
+            return getattr(numpy_backend, name)
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/code_stats.py` & `keras-core-0.1.1/keras_core/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/dataset_utils.py` & `keras-core-0.1.1/keras_core/src/utils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import tensorflow as tf
-
 from keras_core.src.api_export import keras_core_export
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.utils.split_dataset")
 def split_dataset(
     dataset, left_size=None, right_size=None, shuffle=False, seed=None
 ):
     """Splits a dataset into a left half and a right half (e.g. train / test).
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/dtype_utils.py` & `keras-core-0.1.1/keras_core/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/file_utils.py` & `keras-core-0.1.1/keras_core/src/utils/file_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import hashlib
 import os
 import pathlib
+import re
 import shutil
 import tarfile
 import urllib
 import warnings
 import zipfile
 from urllib.request import urlretrieve
 
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.utils import io_utils
+from keras_core.src.utils.module_utils import gfile
 from keras_core.src.utils.progbar import Progbar
 
 
 def path_to_string(path):
     """Convert `PathLike` objects to their string representation.
 
     If given a non-string typed path object, converts it to its string
@@ -376,7 +378,97 @@
     hasher = resolve_hasher(algorithm, file_hash)
 
     if str(hash_file(fpath, hasher, chunk_size)) == str(file_hash):
         return True
     else:
         return False
 
+
+def is_remote_path(filepath):
+    """Returns `True` for paths that represent a remote GCS location."""
+    # TODO: improve generality.
+    if re.match(r"^(/cns|/cfs|/gcs|.*://).*$", str(filepath)):
+        return True
+    return False
+
+
+# Below are gfile-replacement utils.
+
+
+def _raise_if_no_gfile(path):
+    raise ValueError(
+        "Handling remote paths requires installing TensorFlow "
+        f"(in order to use gfile). Received path: {path}"
+    )
+
+
+def exists(path):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.exists(path)
+        else:
+            _raise_if_no_gfile(path)
+    return os.path.exists(path)
+
+
+def File(path, mode="r"):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.GFile(path, mode=mode)
+        else:
+            _raise_if_no_gfile(path)
+    return open(path, mode=mode)
+
+
+def join(path, *paths):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.join(path, *paths)
+        else:
+            _raise_if_no_gfile(path)
+    return os.path.join(path, *paths)
+
+
+def isdir(path):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.isdir(path)
+        else:
+            _raise_if_no_gfile(path)
+    return os.path.isdir(path)
+
+
+def rmtree(path):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.rmtree(path)
+        else:
+            _raise_if_no_gfile(path)
+    return shutil.rmtree
+
+
+def listdir(path):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.listdir(path)
+        else:
+            _raise_if_no_gfile(path)
+    return os.listdir(path)
+
+
+def copy(src, dst):
+    if is_remote_path(src) or is_remote_path(dst):
+        if gfile.available:
+            return gfile.copy(src, dst)
+        else:
+            _raise_if_no_gfile(f"src={src} dst={dst}")
+    return shutil.copy(src, dst)
+
+
+def makedirs(path):
+    if is_remote_path(path):
+        if gfile.available:
+            return gfile.makedirs(path)
+        else:
+            _raise_if_no_gfile(path)
+    return os.makedirs(path)
+
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/image_utils.py` & `keras-core-0.1.1/keras_core/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/io_utils.py` & `keras-core-0.1.1/keras_core/src/utils/io_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -54,14 +54,45 @@
     Returns:
         Boolean, `True` if interactive logging is enabled,
         and `False` otherwise.
     """
     return global_state.get_global_setting("interactive_logging", True)
 
 
+def set_logging_verbosity(level):
+    """Sets the verbosity level for logging.
+
+    Supported log levels are as follows:
+
+    - `"FATAL"` (least verbose)
+    - `"ERROR"`
+    - `"WARNING"`
+    - `"INFO"`
+    - `"DEBUG"` (most verbose)
+
+    Args:
+        level: A string corresponding to the level of verbosity for logging.
+    """
+    valid_levels = {
+        "FATAL": logging.FATAL,
+        "ERROR": logging.ERROR,
+        "WARNING": logging.WARNING,
+        "INFO": logging.INFO,
+        "DEBUG": logging.DEBUG,
+    }
+    verbosity = valid_levels.get(level)
+    if verbosity is None:
+        raise ValueError(
+            "Please pass a valid level for logging verbosity. "
+            f"Expected one of: {set(valid_levels.keys())}. "
+            f"Received: {level}"
+        )
+    logging.set_verbosity(verbosity)
+
+
 def print_msg(message, line_break=True):
     """Print the message to absl logging or stdout."""
     if is_interactive_logging_enabled():
         if line_break:
             sys.stdout.write(message + "\n")
         else:
             sys.stdout.write(message)
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/model_visualization.py` & `keras-core-0.1.1/keras_core/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/naming.py` & `keras-core-0.1.1/keras_core/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/numerical_utils.py` & `keras-core-0.1.1/keras_core/src/utils/numerical_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         raise ValueError(
             "Argument `order` must be an int >= 1. " f"Received: order={order}"
         )
     if isinstance(x, np.ndarray):
         # NumPy input
         norm = np.atleast_1d(np.linalg.norm(x, order, axis))
         norm[norm == 0] = 1
+
+        # axis cannot be `None`
+        axis = axis or -1
         return x / np.expand_dims(norm, axis)
 
     # Backend tensor input
     if len(x.shape) == 0:
         x = ops.expand_dims(x, axis=0)
     epsilon = backend.epsilon()
     if order == 2:
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/progbar.py` & `keras-core-0.1.1/keras_core/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/python_utils.py` & `keras-core-0.1.1/keras_core/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/rng_utils.py` & `keras-core-0.1.1/keras_core/src/utils/rng_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 
 import numpy as np
-import tensorflow as tf
 
+from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
+from keras_core.src.utils.module_utils import tensorflow as tf
 
 
 @keras_core_export("keras_core.utils.set_random_seed")
 def set_random_seed(seed):
     """Sets all random seeds (Python, NumPy, and backend framework, e.g. TF).
 
     You can use this utility to make almost any Keras program fully
@@ -17,15 +18,15 @@
     involved.
 
     Calling this utility is equivalent to the following:
 
     ```python
     import random
     import numpy as np
-    import tensorflow as tf
+    from keras_core.utils.module_utils import tensorflow as tf
     random.seed(seed)
     np.random.seed(seed)
     tf.random.set_seed(seed)
     ```
 
     Note that the TensorFlow seed is set even if you're not using TensorFlow
     as your backend framework, since many workflows leverage `tf.data`
@@ -38,9 +39,14 @@
     if not isinstance(seed, int):
         raise ValueError(
             "Expected `seed` argument to be an integer. "
             f"Received: seed={seed} (of type {type(seed)})"
         )
     random.seed(seed)
     np.random.seed(seed)
-    tf.random.set_seed(seed)
+    if tf.available:
+        tf.random.set_seed(seed)
+    if backend.backend() == "torch":
+        import torch
+
+        torch.manual_seed(seed)
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/sequence_utils.py` & `keras-core-0.1.1/keras_core/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/src/utils/shape_utils.py` & `keras-core-0.1.1/keras_core/src/utils/shape_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     if isinstance(x, (list, tuple)):
         if all(isinstance(e, (int, type(None))) for e in x):
             return True
     return False
 
 
 def map_shape_structure(fn, struct):
-    """Variant of nest.map_structure that operates on shape tuples."""
+    """Variant of tree.map_structure that operates on shape tuples."""
     if is_shape_tuple(struct):
         return fn(tuple(struct))
     if isinstance(struct, list):
         return [map_shape_structure(fn, e) for e in struct]
     if isinstance(struct, tuple):
         return tuple(map_shape_structure(fn, e) for e in struct)
     if isinstance(struct, dict):
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/summary_utils.py` & `keras-core-0.1.1/keras_core/src/utils/summary_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import math
 import re
 import shutil
 
 import rich
-from tensorflow import nest
+import rich.console
+import rich.markup
+
+# See https://github.com/keras-team/keras-core/issues/448
+# for below imports
+import rich.table
+import tree
 
 from keras_core.src import backend
 from keras_core.src.utils import dtype_utils
 from keras_core.src.utils import io_utils
 
 
 def count_params(weights):
@@ -76,15 +82,15 @@
 
     def format_shape(shape):
         highlighted = [highlight_number(x) for x in shape]
         return "(" + ", ".join(highlighted) + ")"
 
     for i in range(len(layer._inbound_nodes)):
         outputs = layer._inbound_nodes[i].output_tensors
-        output_shapes = nest.map_structure(
+        output_shapes = tree.map_structure(
             lambda x: format_shape(x.shape), outputs
         )
     if len(output_shapes) == 1:
         return output_shapes[0]
     out = str(output_shapes)
     out = out.replace("'", "")
     return out
@@ -143,15 +149,15 @@
     else:
         layers = model._operations
         sequential_like = True
         nodes_by_depth = model._nodes_by_depth.values()
         nodes = []
         for v in nodes_by_depth:
             if (len(v) > 1) or (
-                len(v) == 1 and len(nest.flatten(v[0].input_tensors)) > 1
+                len(v) == 1 and len(tree.flatten(v[0].input_tensors)) > 1
             ):
                 # if the model has multiple nodes
                 # or if the nodes have multiple inbound_layers
                 # the model is no longer sequential
                 sequential_like = False
                 break
             nodes += v
@@ -182,16 +188,16 @@
         header = ["Layer (type)", "Output Shape", "Param #", "Connected to"]
         alignment = ["left", "left", "right", "left"]
         relevant_nodes = []
         for v in model._nodes_by_depth.values():
             relevant_nodes += v
 
     if show_trainable:
-        default_line_length += 8
-        positions = [p * 0.88 for p in positions] + [1.0]
+        default_line_length += 12
+        positions = [p * 0.90 for p in positions] + [1.0]
         header.append("Trainable")
         alignment.append("center")
 
     # Compute columns widths
     default_line_length = min(
         default_line_length, shutil.get_terminal_size().columns - 4
     )
@@ -252,19 +258,22 @@
         else:
             params = highlight_number(f"{layer.count_params():,}")
 
         fields = [name, output_shape, params]
         if not sequential_like:
             fields.append(get_connections(layer))
         if show_trainable:
-            fields.append(
-                bold_text("Y", color=34)
-                if layer.trainable
-                else bold_text("N", color=9)
-            )
+            if layer.weights:
+                fields.append(
+                    bold_text("Y", color=34)
+                    if layer.trainable
+                    else bold_text("N", color=9)
+                )
+            else:
+                fields.append(bold_text("-"))
         return fields
 
     def print_layer(layer, nested_level=0):
         if nested_level:
             prefix = "   " * nested_level + "└" + " "
         else:
             prefix = ""
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/traceback_utils.py` & `keras-core-0.1.1/keras_core/src/utils/traceback_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 import os
 import traceback
 import types
 from functools import wraps
 
-from tensorflow import errors as tf_errors
-from tensorflow import nest
+import tree
 
 from keras_core.src import backend
 from keras_core.src.api_export import keras_core_export
 from keras_core.src.backend.common import global_state
 
 _EXCLUDED_PATHS = (
     os.path.abspath(os.path.join(__file__, "..", "..")),
@@ -138,14 +137,18 @@
             was called with.
         object_name: String, display name of the class/function being called,
             e.g. `'layer "layer_name" (LayerClass)'`.
 
     Returns:
         A wrapped version of `fn`.
     """
+    if backend.backend() == "tensorflow":
+        from tensorflow import errors as tf_errors
+    else:
+        tf_errors = None
 
     @wraps(fn)
     def error_handler(*args, **kwargs):
         if not is_traceback_filtering_enabled():
             return fn(*args, **kwargs)
 
         signature = None
@@ -164,42 +167,42 @@
                 # Likely unbindable arguments
                 raise e
 
             # Add argument context
             arguments_context = []
             for arg in list(signature.parameters.values()):
                 if arg.name in bound_signature.arguments:
-                    value = nest.map_structure(
+                    value = tree.map_structure(
                         format_argument_value,
                         bound_signature.arguments[arg.name],
                     )
                 else:
                     value = arg.default
                 arguments_context.append(f"  • {arg.name}={value}")
             if arguments_context:
                 arguments_context = "\n".join(arguments_context)
                 # Get original error message and append information to it.
-                if isinstance(e, tf_errors.OpError):
+                if tf_errors is not None and isinstance(e, tf_errors.OpError):
                     message = e.message
                 elif e.args:
                     # Canonically, the 1st argument in an exception is the error
-                    # message.  This works for all built-in Python exceptions.
+                    # message. This works for all built-in Python exceptions.
                     message = e.args[0]
                 else:
                     message = ""
                 display_name = f"{object_name if object_name else fn.__name__}"
                 message = (
                     f"Exception encountered when calling {display_name}.\n\n"
                     f"\x1b[1m{message}\x1b[0m\n\n"
                     f"Arguments received by {display_name}:\n"
                     f"{arguments_context}"
                 )
 
                 # Reraise exception, with added context
-                if isinstance(e, tf_errors.OpError):
+                if tf_errors is not None and isinstance(e, tf_errors.OpError):
                     new_e = e.__class__(e.node_def, e.op, message, e.error_code)
                 else:
                     try:
                         # For standard exceptions such as ValueError, TypeError,
                         # etc.
                         new_e = e.__class__(message)
                     except TypeError:
@@ -223,14 +226,16 @@
         # to keep messages readable
         if backend.backend() == "tensorflow":
             tensor_cls = "tf.Tensor"
         elif backend.backend() == "jax":
             tensor_cls = "jnp.ndarray"
         elif backend.backend() == "torch":
             tensor_cls = "torch.Tensor"
+        elif backend.backend() == "numpy":
+            tensor_cls = "np.ndarray"
         else:
             tensor_cls = "array"
 
         return (
             f"{tensor_cls}(shape={value.shape}, "
             f"dtype={backend.standardize_dtype(value.dtype)})"
         )
```

### Comparing `keras-core-0.1.0/keras_core/src/utils/tracking.py` & `keras-core-0.1.1/keras_core/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core/utils/__init__.py` & `keras-core-0.1.1/keras_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-core-0.1.0/keras_core.egg-info/PKG-INFO` & `keras-core-0.1.1/keras_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras-core
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 
 ## Backwards compatibility
 
 Keras Core is intended to work as a drop-in replacement for `tf.keras` (when using the TensorFlow backend). Just take your
 existing `tf.keras` code, change the `keras` imports to `keras_core`, make sure that your calls to `model.save()` are using
 the up-to-date `.keras` format, and you're done.
 
-If your `tf.keras` model does not include custom compoments, you can start running it on top of JAX or PyTorch immediately.
+If your `tf.keras` model does not include custom components, you can start running it on top of JAX or PyTorch immediately.
 
 If it does include custom components (e.g. custom layers or a custom `train_step()`), it is usually possible to convert it
 to a backend-agnostic implementation in just a few minutes.
 
 In addition, Keras models can consume datasets in any format, regardless of the backend you're using:
 you can train your models with your existing `tf.data.Dataset` pipelines or PyTorch `DataLoaders`.
```

### Comparing `keras-core-0.1.0/keras_core.egg-info/SOURCES.txt` & `keras-core-0.1.1/keras_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 keras_core/preprocessing/image/__init__.py
 keras_core/preprocessing/sequence/__init__.py
 keras_core/random/__init__.py
 keras_core/regularizers/__init__.py
 keras_core/saving/__init__.py
 keras_core/src/__init__.py
 keras_core/src/api_export.py
+keras_core/src/version.py
 keras_core/src/activations/__init__.py
 keras_core/src/activations/activations.py
 keras_core/src/applications/__init__.py
 keras_core/src/applications/convnext.py
 keras_core/src/applications/densenet.py
 keras_core/src/applications/efficientnet.py
 keras_core/src/applications/efficientnet_v2.py
@@ -92,14 +93,24 @@
 keras_core/src/backend/jax/layer.py
 keras_core/src/backend/jax/math.py
 keras_core/src/backend/jax/nn.py
 keras_core/src/backend/jax/numpy.py
 keras_core/src/backend/jax/random.py
 keras_core/src/backend/jax/rnn.py
 keras_core/src/backend/jax/trainer.py
+keras_core/src/backend/numpy/__init__.py
+keras_core/src/backend/numpy/core.py
+keras_core/src/backend/numpy/image.py
+keras_core/src/backend/numpy/layer.py
+keras_core/src/backend/numpy/math.py
+keras_core/src/backend/numpy/nn.py
+keras_core/src/backend/numpy/numpy.py
+keras_core/src/backend/numpy/random.py
+keras_core/src/backend/numpy/rnn.py
+keras_core/src/backend/numpy/trainer.py
 keras_core/src/backend/tensorflow/__init__.py
 keras_core/src/backend/tensorflow/core.py
 keras_core/src/backend/tensorflow/image.py
 keras_core/src/backend/tensorflow/layer.py
 keras_core/src/backend/tensorflow/math.py
 keras_core/src/backend/tensorflow/nn.py
 keras_core/src/backend/tensorflow/numpy.py
@@ -115,14 +126,22 @@
 keras_core/src/backend/torch/math.py
 keras_core/src/backend/torch/nn.py
 keras_core/src/backend/torch/numpy.py
 keras_core/src/backend/torch/random.py
 keras_core/src/backend/torch/rnn.py
 keras_core/src/backend/torch/torch_module_wrapper.py
 keras_core/src/backend/torch/trainer.py
+keras_core/src/backend/torch/optimizers/__init__.py
+keras_core/src/backend/torch/optimizers/torch_adadelta.py
+keras_core/src/backend/torch/optimizers/torch_adam.py
+keras_core/src/backend/torch/optimizers/torch_adamw.py
+keras_core/src/backend/torch/optimizers/torch_optimizer.py
+keras_core/src/backend/torch/optimizers/torch_parallel_optimizer.py
+keras_core/src/backend/torch/optimizers/torch_rmsprop.py
+keras_core/src/backend/torch/optimizers/torch_sgd.py
 keras_core/src/callbacks/__init__.py
 keras_core/src/callbacks/callback.py
 keras_core/src/callbacks/callback_list.py
 keras_core/src/callbacks/csv_logger.py
 keras_core/src/callbacks/early_stopping.py
 keras_core/src/callbacks/history.py
 keras_core/src/callbacks/lambda_callback.py
@@ -237,15 +256,14 @@
 keras_core/src/layers/preprocessing/rescaling.py
 keras_core/src/layers/preprocessing/resizing.py
 keras_core/src/layers/preprocessing/string_lookup.py
 keras_core/src/layers/preprocessing/text_vectorization.py
 keras_core/src/layers/preprocessing/tf_data_layer.py
 keras_core/src/layers/regularization/__init__.py
 keras_core/src/layers/regularization/activity_regularization.py
-keras_core/src/layers/regularization/alpha_dropout.py
 keras_core/src/layers/regularization/dropout.py
 keras_core/src/layers/regularization/gaussian_dropout.py
 keras_core/src/layers/regularization/gaussian_noise.py
 keras_core/src/layers/regularization/spatial_dropout.py
 keras_core/src/layers/reshaping/__init__.py
 keras_core/src/layers/reshaping/cropping1d.py
 keras_core/src/layers/reshaping/cropping2d.py
@@ -353,15 +371,17 @@
 keras_core/src/utils/code_stats.py
 keras_core/src/utils/dataset_utils.py
 keras_core/src/utils/dtype_utils.py
 keras_core/src/utils/file_utils.py
 keras_core/src/utils/image_utils.py
 keras_core/src/utils/io_utils.py
 keras_core/src/utils/model_visualization.py
+keras_core/src/utils/module_utils.py
 keras_core/src/utils/naming.py
+keras_core/src/utils/nest.py
 keras_core/src/utils/numerical_utils.py
 keras_core/src/utils/progbar.py
 keras_core/src/utils/python_utils.py
 keras_core/src/utils/rng_utils.py
 keras_core/src/utils/sequence_utils.py
 keras_core/src/utils/shape_utils.py
 keras_core/src/utils/summary_utils.py
```

### Comparing `keras-core-0.1.0/setup.py` & `keras-core-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,33 +19,36 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     raise RuntimeError("Unable to find version string.")
 
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
-VERSION = get_version("keras_core/__init__.py")
+if os.path.exists("keras_core/version.py"):
+    VERSION = get_version("keras_core/version.py")
+else:
+    VERSION = get_version("keras_core/__init__.py")
 
 setup(
     name="keras-core",
     description="Multi-backend Keras.",
     long_description_content_type="text/markdown",
     long_description=README,
     version=VERSION,
     url="https://github.com/keras-team/keras-core",
     author="Keras team",
     author_email="keras-users@googlegroups.com",
     license="Apache License 2.0",
     install_requires=[
-        "tensorflow",
         "absl-py",
         "numpy",
         "rich",
         "namex",
         "h5py",
+        "dm-tree",
     ],
     # Supported Python versions
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

