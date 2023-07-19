# Comparing `tmp/prolog_primitives-1.2.0.tar.gz` & `tmp/prolog_primitives-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-1.2.0.tar", last modified: Sat Jul 15 16:27:09 2023, max compression
+gzip compressed data, was "prolog_primitives-1.2.1.tar", last modified: Wed Jul 19 12:27:05 2023, max compression
```

## Comparing `prolog_primitives-1.2.0.tar` & `prolog_primitives-1.2.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/nt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.491995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.491995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.491995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.169938 prolog_primitives-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-19 12:27:05.169938 prolog_primitives-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 12:27:05.000000 prolog_primitives-1.2.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.161938 prolog_primitives-1.2.1/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.161938 prolog_primitives-1.2.1/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/basic/nt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.161938 prolog_primitives-1.2.1/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 12:26:35.000000 prolog_primitives-1.2.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.165938 prolog_primitives-1.2.1/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.165938 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.165938 prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.165938 prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.165938 prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.169938 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:27:05.161938 prolog_primitives-1.2.1/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-19 12:27:05.000000 prolog_primitives-1.2.1/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-19 12:27:05.000000 prolog_primitives-1.2.1/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:27:05.000000 prolog_primitives-1.2.1/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:27:04.000000 prolog_primitives-1.2.1/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-19 12:27:05.000000 prolog_primitives-1.2.1/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 12:27:05.000000 prolog_primitives-1.2.1/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:27:05.169938 prolog_primitives-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-19 12:25:16.000000 prolog_primitives-1.2.1/setup.py
```

### Comparing `prolog_primitives-1.2.0/LICENSE` & `prolog_primitives-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/PKG-INFO` & `prolog_primitives-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 1.2.0
+Version: 1.2.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/Session.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/basic/nt.py` & `prolog_primitives-1.2.1/prolog_primitives/basic/nt.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-1.2.1/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-1.2.1/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-1.2.1/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-1.2.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-1.2.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 theoryFromDatasetPrimitive, schemaTrasformation,
                 normalizePrimitive, one_hot_encodePrimitive, dropPrimitive,
                 fitPrimitive, transformPrimitive, inputLayerPrimitive,
                 denseLayerPrimitive, outputLayerPrimitive, neuralNetworkPrimitive,
                 trainPrimitive, predictPrimitive, classifyPrimitive, msePrimitive,
                 maePrimitive, accuracyPrimitive, recallPrimitive, rPrimitive]
 
-    initialport = 8080
+    initialport = 8100
     port = initialport
     executor = ThreadPoolExecutor(max_workers=len(primitives))
 
     for primitive in primitives:
         #future = executor.submit(launchPrimitive, primitive, port)
         launchPrimitive(primitive, port)
         port += 1
```

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/score.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/predictors/train.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.2.1/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.2.1/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 1.2.0
+Version: 1.2.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.2.0/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.2.1/prolog_primitives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.2.0/setup.py` & `prolog_primitives-1.2.1/setup.py`

 * *Files identical despite different names*

