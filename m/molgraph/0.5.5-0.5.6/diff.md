# Comparing `tmp/molgraph-0.5.5.tar.gz` & `tmp/molgraph-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.5.tar", last modified: Mon Jul 17 15:21:04 2023, max compression
+gzip compressed data, was "molgraph-0.5.6.tar", last modified: Wed Jul 19 15:00:44 2023, max compression
```

## Comparing `molgraph-0.5.5.tar` & `molgraph-0.5.6.tar`

### file list

```diff
@@ -1,112 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.5/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-17 15:21:04.196512 molgraph-0.5.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5998 2023-07-17 15:20:50.000000 molgraph-0.5.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.5/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.5/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.5/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.5/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.5/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.5/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.5/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.5/molgraph/chemistry/vis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      923 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/internal.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.5/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12927 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11735 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9923 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11863 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10845 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17229 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.5/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10192 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11264 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10555 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.5/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9981 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10871 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    26003 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.5/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16323 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14494 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.5/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10772 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.5/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3455 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3031 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.5/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11065 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4593 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9737 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4258 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11887 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6688 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20500 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.192512 molgraph-0.5.5/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.5/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6405 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4687 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3332 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6274 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5369 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.5/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2449 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.5/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.5/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6987 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7101 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.5/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10961 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6905 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.5/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23586 2023-07-17 14:06:48.000000 molgraph-0.5.5/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13073 2023-07-17 14:06:52.000000 molgraph-0.5.5/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.196512 molgraph-0.5.5/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.5/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.5/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1877 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    51973 2023-07-17 15:20:50.000000 molgraph-0.5.5/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 15:21:04.188512 molgraph-0.5.5/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3329 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-17 15:21:04.000000 molgraph-0.5.5/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-17 15:21:04.196512 molgraph-0.5.5/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1418 2023-07-17 15:20:50.000000 molgraph-0.5.5/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.6/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-19 15:00:44.027500 molgraph-0.5.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5998 2023-07-17 15:20:50.000000 molgraph-0.5.6/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.019500 molgraph-0.5.6/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.019500 molgraph-0.5.6/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       81 2023-07-18 13:59:25.000000 molgraph-0.5.6/molgraph/applications/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10465 2023-07-19 14:41:48.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.6/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.6/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21162 2023-07-19 14:31:44.000000 molgraph-0.5.6/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.6/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.6/molgraph/chemistry/vis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      923 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/internal.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.6/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12927 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11735 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9923 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11863 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10845 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17229 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.6/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10192 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11264 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10555 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.6/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9981 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10871 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26149 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.6/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16323 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14494 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.6/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10772 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.6/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3829 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3031 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.6/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11065 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4593 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9633 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4258 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11887 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6688 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20500 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.6/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6405 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4687 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3332 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6274 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5369 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.6/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2382 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.6/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      984 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6987 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7101 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10961 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6905 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.6/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    27436 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20236 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.6/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.6/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1877 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    51982 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.019500 molgraph-0.5.6/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-19 15:00:44.027500 molgraph-0.5.6/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1418 2023-07-17 15:20:50.000000 molgraph-0.5.6/setup.py
```

### Comparing `molgraph-0.5.5/LICENSE` & `molgraph-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/PKG-INFO` & `molgraph-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.5
+Version: 0.5.6
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.5.5/README.md` & `molgraph-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/_filter_warnings.py` & `molgraph-0.5.6/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/__init__.py` & `molgraph-0.5.6/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.6/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.6/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.6/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.6/molgraph/chemistry/benchmark/tf_records.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,37 +97,46 @@
 
         inputs[key] = [
             value[i * chunk_size: (i + 1) * chunk_size]
             for i in range(num_files)
         ]
 
     input_keys = list(inputs.keys())
-    inputs = list(inputs.values())
+    input_chunks = list(inputs.values())
 
     os.makedirs(path, exist_ok=True)
 
     _specs_to_json(spec, os.path.join(path, 'spec.json'))
 
     paths = [
         os.path.join(path, f'tfrecord-{i:04d}.tfrecord')
         for i in range(num_files)
     ]
 
-    inputs.insert(0, paths)
+    input_chunks.insert(0, paths)
+    input_chunks = zip(*input_chunks)
+
+    write_tfrecords_to_file_fn = partial(
+        _write_tfrecords_to_file,
+        input_keys=input_keys,
+        encoder=encoder,
+        device=device
+    )
+
+    pool = multiprocessing.Pool(processes)
+
+    for input_chunk in input_chunks:
+
+        #write_tfrecords_to_file_fn(input_chunk)
+
+        _ = pool.apply(write_tfrecords_to_file_fn, (input_chunk,))
+
+    pool.close()
+    pool.join()
 
-    with multiprocessing.Pool(processes) as pool:
-        pool.map(
-            func=partial(
-                _write_tfrecords_to_file,
-                input_keys=input_keys,
-                encoder=encoder,
-                device=device
-            ),
-            iterable=zip(*inputs)
-        )
 
 def load(
     path: str,
     extract_tuple: Optional[Union[List[str], Tuple[str]]] = None,
     shuffle_tf_records: bool = False,
 ) -> tf.data.Dataset:
     '''Loads TF records.
@@ -236,31 +245,33 @@
     input_keys: List[str],
     encoder: Union[MolecularGraphEncoder, MolecularGraphEncoder3D],
     device: str = '/cpu:0',
 ) -> None:
     '''Writes data to a tf record file. This function is called from
     `write_tfrecords`.
     '''
-    path, *inputs = inputs
-    inputs = list(zip(*inputs))
+    path, *inps = inputs
+    inps = list(zip(*inps))
     with tf.device(device), tf.io.TFRecordWriter(path) as writer:
-        for inp in inputs:
+        for inp in inps:
             inp = dict(zip(input_keys, inp))
             x = inp.pop('x')
             tensor = encoder(x)
             if tensor is None:
                 continue
             data = tensor._data.copy()
             data.pop('graph_indicator')
             example = tf.nest.map_structure(
                 lambda x: _to_bytes_feature(x), data)
             for k, v in inp.items():
                 example[k] = _to_bytes_feature(v)
             serialized = _serialize_example(example)
             writer.write(serialized)
+    
+    del inputs, input_keys, encoder, device
 
 def _parse_features(
     example_proto: tf.Tensor,
     specs: Dict[str, Union[GraphTensorSpec, tf.TensorSpec]],
     extract_tuple: Optional[Union[List[str], Tuple[str]]] = None,
 ) -> Dict[str, Union[GraphTensor, tf.Tensor]]:
```

### Comparing `molgraph-0.5.5/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.6/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.6/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/encoders.py` & `molgraph-0.5.6/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/features.py` & `molgraph-0.5.6/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.6/molgraph/chemistry/molecular_encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,14 @@
                     graph_tensor_list = pool.map(
                         func=partial(self.call, **kwargs),
                         iterable=inputs)
 
                 graph_tensor_list = [
                     gt for gt in graph_tensor_list if gt is not None]
 
-                # The list of `GraphTensor`s is concatenated to generate a single
-                # `GraphTensor` (disjoint [molecular] graph). The `separate` method
-                # is called to make the nested structures of the `GraphTensor`
-                # ragged. This will allow for batching of the `GraphTensor`.
                 return tf.stack(graph_tensor_list, axis=0)
 
             return self.call(inputs, **kwargs)
 
 
 @dataclass
 class MolecularGraphEncoder(BaseMolecularGraphEncoder):
```

### Comparing `molgraph-0.5.5/molgraph/chemistry/ops.py` & `molgraph-0.5.6/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/chemistry/vis.py` & `molgraph-0.5.6/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/internal.py` & `molgraph-0.5.6/molgraph/internal.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/__init__.py` & `molgraph-0.5.6/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.6/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.6/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.6/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.6/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.6/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.6/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.6/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.6/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.6/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.6/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.6/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.6/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.6/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/gnn_layer.py` & `molgraph-0.5.6/molgraph/layers/gnn_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,32 +505,35 @@
                 A Python dictionary of parameters to initialize and build a 
                 layer instance. The config is usually obtained from 
                 ``get_config()`` of another layer instance (of the same class).
         
         Returns:
             A layer instance.
         '''
-        graph_tensor_spec = config.pop('graph_tensor_spec', None)
+        serialized_gt_spec = config.pop('graph_tensor_spec', None)
         update_step = config.pop('update_step')
         config['update_step'] = (
             None if update_step is None else layers.deserialize(update_step))
         layer = cls(**config)
-        if graph_tensor_spec is None:
+        if serialized_gt_spec is None:
+            deserialized_gt_spec = None
             warn(
                 (
                  'A GraphTensorSpec could not be obtained from the config, '
                  'indicating that the layer from which the config was '
                  'previously obtained was not yet built. Proceeding to '
                  'initialize the layer without building it.'
                 ),
                 UserWarning,
                 stacklevel=2
             )
         else:
-            layer.build_from_signature(graph_tensor_spec)
+            deserialized_gt_spec = GraphTensorSpec(
+                serialized_gt_spec['config'][0])
+            layer.build_from_signature(deserialized_gt_spec)
         return layer
 
     def get_config(self) -> dict:
         '''Returns the configuration of the layer.
         
         Returns:
             Python dictionary with the layer's parameters. Can be used to
```

### Comparing `molgraph-0.5.5/molgraph/layers/gnn_ops.py` & `molgraph-0.5.6/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.6/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.6/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.6/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.6/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from typing import Optional
+from typing import Union
+from typing import Tuple
 
 from molgraph.internal import register_keras_serializable 
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 @register_keras_serializable(package='molgraph')
@@ -34,35 +36,43 @@
     GraphTensor(
       edge_src=<tf.RaggedTensor: shape=(2, None), dtype=int32>,
       edge_dst=<tf.RaggedTensor: shape=(2, None), dtype=int32>,
       node_feature=<tf.RaggedTensor: shape=(2, None, 2), dtype=float32>,
       edge_score=<tf.RaggedTensor: shape=(2, None, 1), dtype=float32>)
 
     Args:
-        apply_sigmoid (bool):
-            Whether to apply a sigmoid activaton on the edge scores. 
-            Default to False.
+        normalize (bool):
+            Whether to apply normalization on the edge scores. Produces cosine
+            similarity values in the range -1 to 1. Default to False.
+        axes (int, tuple):
+            The axes (or axis) to perform the dot product. Default to 1.
         data_field (str, None):
             Name of the data added to the GraphTensor instance. If None,
             the output will be a ``tf.Tensor`` or ``tf.RaggedTensor`` 
             containing the dot product between incident node features.
             If str, a GraphTensor instance with a new data field "data_field"
             will be outputted. Default to "edge_score".
     '''
     def __init__(
         self, 
-        apply_sigmoid: bool = False, 
+        normalize: bool = False, 
+        axes: Union[int, Tuple[int, ...]] = 1,
         data_field: Optional[str] = 'edge_score',
         **kwargs
     ):
         super().__init__(**kwargs)
-        self._apply_sigmoid = apply_sigmoid
+        self._dot_normalize = normalize
+        self._dot_axes = axes
         self._data_field = data_field
+        self._dot_layer = keras.layers.Dot(axes=axes, normalize=normalize)
 
-    def call(self, tensor: GraphTensor) -> GraphTensor:
+    def call(
+        self, 
+        tensor: GraphTensor
+    ) -> Union[GraphTensor, tf.Tensor, tf.RaggedTensor]:
         '''Defines the computation from inputs to outputs.
 
         This method should not be called directly, but indirectly
         via ``__call__()``. Upon first call, the layer is automatically
         built via ``build()``.
 
         Args:
@@ -70,30 +80,34 @@
                 Input to the layer.
 
         Returns:
             A ``tf.Tensor`` or `tf.RaggedTensor` based on the node_feature
             field of the inputted ``GraphTensor``.
         '''
         tensor_orig = tensor
-        if isinstance(tensor.node_feature, tf.RaggedTensor):
+
+        if tensor.is_ragged():
             tensor = tensor.merge()
         
-        adjacency = tf.stack([
-            tensor.edge_src, tensor.edge_dst], axis=1)
-        node_feature_incident = tf.gather(
-            tensor.node_feature, adjacency)
-        edge_score = tf.reduce_sum(
-            tf.reduce_prod(node_feature_incident, axis=1), axis=1, keepdims=True)
-        if self._apply_sigmoid:
-            edge_score = tf.nn.sigmoid(edge_score)
-        if self._data_field is None:
-            return edge_score
-        return tensor_orig.update({self._data_field: edge_score})
+        node_feature_src = tf.gather(
+            tensor.node_feature, tensor.edge_src)
+
+        node_feature_dst = tf.gather(
+            tensor.node_feature, tensor.edge_dst)
+
+        edge_score = self._dot_layer([node_feature_src, node_feature_dst])
+
+        if self._data_field is not None:
+            return tensor_orig.update({self._data_field: edge_score})
+        
+        tensor_orig = tensor_orig.update({'edge_score': edge_score})
+        return tensor_orig.edge_score
 
     def get_config(self):
         config = super().get_config()
         config.update({
-            'apply_sigmoid': self._apply_sigmoid,
+            'normalize': self._dot_normalize,
+            'axes': self._dot_axes,
             'data_field': self._data_field,
         })
         return config
```

### Comparing `molgraph-0.5.5/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.6/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.6/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,16 +142,14 @@
             **kwargs
         )
 
         self.output_dim = output_dim
         self.embeddings_initializer = initializers.get(embeddings_initializer)
         self.embeddings_regularizer = regularizers.get(embeddings_regularizer)
         self.embeddings_constraint = constraints.get(embeddings_constraint)
-        self._vocabulary_size = None
-        self._built_from_vocabulary_size = False
 
     def adapt(self, data, batch_size=None, steps=None):
         '''Adapts the layer to data.
 
         When adapting the layer to the data, ``build()`` will be called
         automatically (to initialize the relevant attributes). After adaption,
         the layer is finalized and ready to be used.
@@ -169,16 +167,25 @@
         '''
         if not isinstance(data, GraphTensor):
             data = data.map(
                 lambda x: getattr(x, self.feature))
         else:
             data = getattr(data, self.feature)
         super().adapt(data, batch_size=batch_size, steps=steps)
-        self._vocabulary_size = self.vocabulary_size()
 
+        self.embeddings = self.add_weight(
+            shape=(self.vocabulary_size(), self.output_dim),
+            dtype=tf.float32,
+            initializer=self.embeddings_initializer,
+            name='embeddings',
+            regularizer=self.embeddings_regularizer,
+            constraint=self.embeddings_constraint,
+            experimental_autocast=False
+        )
+        
     def call(self, tensor: GraphTensor) -> GraphTensor:
         '''Defines the computation from inputs to outputs.
 
         This method should not be called directly, but indirectly
         via ``__call__()``. Upon first call, the layer is automatically
         built via ``build()``.
 
@@ -188,59 +195,46 @@
 
         Returns:
             GraphTensor:
                 A ``GraphTensor`` with updated features. Either the
                 ``node_feature`` component or the ``edge_feature``
                 component (of the ``GraphTensor``) are updated.
         '''
-        if not self._built_from_vocabulary_size:
-            self._build_from_vocabulary_size(self._vocabulary_size)
-
         tensor = tensor.update({
             self.feature: super().call(getattr(tensor, self.feature))
         })
         return tensor.update({
             self.feature: tf.nn.embedding_lookup(
                 self.embeddings, getattr(tensor, self.feature))
         })
-
-    def _build_from_vocabulary_size(self, vocabulary_size):
-        self._built_from_vocabulary_size = True
-
-        self.embeddings = self.add_weight(
-            shape=(vocabulary_size, self.output_dim),
-            dtype=tf.float32,
-            initializer=self.embeddings_initializer,
-            name='embeddings',
-            regularizer=self.embeddings_regularizer,
-            constraint=self.embeddings_constraint,
-            experimental_autocast=False
-        )
+    
+    def build(self, input_shape):
+        super().build(input_shape)
+        if not hasattr(self, 'embeddings'):
+            with tf.init_scope():
+                self.embeddings = self.add_weight(
+                    shape=(self.vocabulary_size(), self.output_dim),
+                    dtype=tf.float32,
+                    initializer=self.embeddings_initializer,
+                    name='embeddings',
+                    regularizer=self.embeddings_regularizer,
+                    constraint=self.embeddings_constraint,
+                    experimental_autocast=False
+                )
 
     def compute_output_shape(
         self, 
         input_shape: tf.TensorShape
     ) -> tf.TensorShape:
         return tf.TensorShape(
             input_shape[:-1]).concatenate([self.output_dim])
-    
-    @classmethod
-    def from_config(cls, config):
-        vocabulary_size = config.pop('vocabulary_size')
-        layer = cls(**config)
-        if vocabulary_size is None:
-            pass
-        else:
-            layer._build_from_vocabulary_size(vocabulary_size)
-        return layer
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({
-            'vocabulary_size': self._vocabulary_size,
             'output_dim': self.output_dim,
             'embeddings_initializer': initializers.serialize(
                 self.embeddings_initializer),
             'embeddings_regularizer': regularizers.serialize(
                 self.embeddings_regularizer),
             'embeddings_constraint': constraints.serialize(
                 self.embeddings_constraint),
```

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.6/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.6/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.6/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.6/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.6/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.6/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/losses/link_losses.py` & `molgraph-0.5.6/molgraph/losses/link_losses.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,22 +20,21 @@
             label_smoothing=label_smoothing,
             axis=axis,
             reduction=reduction,
             name=name,
         )
 
     def call(self, positive_score, negative_score):
-        # TODO: Only works when scores are defined as y_true, why?
-        y_true = tf.concat([
+        y_pred = tf.concat([
             positive_score, negative_score
         ], axis=0)
-        y_pred = tf.concat([
+        y_true = tf.concat([
             tf.ones_like(positive_score), tf.zeros_like(negative_score)
         ], axis=0)
-        return super().call(y_pred, y_true)
+        return super().call(y_true, y_pred)
 
 
 # TODO: Make it work for len(y_true) != len(y_pred)
 @register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveMarginLoss(keras.losses.Loss):
 
     def __init__(
```

### Comparing `molgraph-0.5.5/molgraph/losses/masked_losses.py` & `molgraph-0.5.6/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.6/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.6/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/models/__init__.py` & `molgraph-0.5.6/molgraph/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from molgraph.models.interpretability.saliency import SmoothGradSaliencyMapping
 from molgraph.models.mpnn import MPNN
 from molgraph.models.dmpnn import DMPNN
 from molgraph.models.dgin import DGIN
 
 from molgraph.models.pretraining.autoencoders import GraphAutoEncoder
 from molgraph.models.pretraining.autoencoders import GraphVariationalAutoEncoder
-from molgraph.models.pretraining.masked_modeling import MaskedGraphModeling
+from molgraph.models.pretraining.masked_modeling import GraphMasking
 
 # aliases
-VanillaSaliencyMapping = SaliencyMapping
 GVAE = GraphVAE = GraphVariationalAutoEncoder 
 GAE = GraphAE = GraphAutoEncoder
+MaskedGraphModeling = GraphMasking
 
-Saliency = SaliencyMapping
+Saliency = VanillaSaliencyMapping = SaliencyMapping
 IntegratedSaliency = IntegratedSaliencyMapping
 SmoothGradSaliency = SmoothGradSaliencyMapping
-GradCAM = GradientActivation = GradientActivationMapping
+GradCAM = GradientActivation = GradientActivationMapping
```

### Comparing `molgraph-0.5.5/molgraph/models/dgin.py` & `molgraph-0.5.6/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/models/dmpnn.py` & `molgraph-0.5.6/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.6/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.6/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/models/mpnn.py` & `molgraph-0.5.6/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.6/molgraph/models/pretraining/autoencoders.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 from molgraph.internal import register_keras_serializable 
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 from molgraph.layers.postprocessing.dot_product_incident import DotProductIncident
 
-from molgraph.losses.link_losses import LinkBinaryCrossentropy
+
+# TODO: Improve negative graph sampler. Need to distinguish separate but
+#       equivalent atoms.
 
     
 @register_keras_serializable(package='molgraph')
 class GraphAutoEncoder(keras.Model):
     '''Graph AutoEncoder (GAE) based on Kipf and Welling [#]_.
     
     Args:
@@ -34,39 +36,69 @@
         balanced_class_weighting (bool):
             Whether balanced class weighting should be performed. For
             instance, if there are twice as many negative edges, should
             each negative edge be weighted 0.5 for the loss?
     
     **Example:**
 
-    >>> # Obtain GraphTensor instance
-    >>> atom_encoder = molgraph.chemistry.Featurizer([
-    ...     molgraph.chemistry.features.Symbol({'C', 'N', 'O', 'P', 'Na'}),
-    ...     molgraph.chemistry.features.Hybridization(),
-    ... ])
-    >>> bond_encoder = molgraph.chemistry.Featurizer([
-    ...     molgraph.chemistry.features.BondType(),
-    ...     molgraph.chemistry.features.Rotatable()
-    ... ])
-    >>> molgraph_encoder = molgraph.chemistry.MolecularGraphEncoder(
-    ...     atom_encoder, bond_encoder)
-    >>> dataset = molgraph.chemistry.datasets.get('esol', splitter=None)
-    >>> graph_tensor = molgraph_encoder(dataset['x'])
+    >>> # Replace this graph_tensor with a large dataset of graphs
+    >>> # Also accepts featurized graph tensors (via `chemistry.Featurizer`)
+    >>> graph_tensor = molgraph.GraphTensor(
+    ...    data={
+    ...        'edge_src': [1, 4, 0, 2, 3, 1, 1, 0],
+    ...        'edge_dst': [0, 0, 1, 1, 1, 2, 3, 4],
+    ...        'node_feature': [
+    ...            'Sym:C|Hyb:SP3', 
+    ...            'Sym:C|Hyb:SP2', 
+    ...            'Sym:O|Hyb:SP2',
+    ...            'Sym:O|Hyb:SP2', 
+    ...            'Sym:N|Hyb:SP3'
+    ...        ],
+    ...        'edge_feature': [
+    ...            'BonTyp:SINGLE|Rot:1', 
+    ...            'BonTyp:SINGLE|Rot:0',
+    ...            'BonTyp:SINGLE|Rot:1', 
+    ...            'BonTyp:DOUBLE|Rot:0',
+    ...            'BonTyp:SINGLE|Rot:0', 
+    ...            'BonTyp:DOUBLE|Rot:0',
+    ...            'BonTyp:SINGLE|Rot:0', 
+    ...            'BonTyp:SINGLE|Rot:0'
+    ...        ],
+    ...        'graph_indicator': [0, 0, 0, 0, 0],
+    ...    }
+    ... )
+    >>> graph_tensor = graph_tensor.separate()
+    >>> node_embedding = molgraph.layers.NodeEmbeddingLookup(
+    ...    32, mask_token='[MASK]'
+    ... )
+    >>> edge_embedding = molgraph.layers.EdgeEmbeddingLookup(
+    ...    32, mask_token='[MASK]'
+    ... )
+    >>> node_embedding.adapt(graph_tensor)
+    >>> edge_embedding.adapt(graph_tensor)
     >>> # Obtain GraphAutoEncoder model
     >>> encoder = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
+    ...     node_embedding,
+    ...     edge_embedding,
     ...     molgraph.layers.GATv2Conv(128),
     ...     molgraph.layers.GATv2Conv(128),
     ...     molgraph.layers.GATv2Conv(128),
     ... ])
-    >>> decoder = molgraph.layers.DotProductIncident(apply_sigmoid=True)
+    >>> decoder = molgraph.layers.DotProductIncident(normalize=True)
     >>> gae = molgraph.models.GraphAutoEncoder(encoder, decoder)
-    >>> gae.compile('adam', loss=molgraph.losses.LinkBinaryCrossentropy())
+    >>> gae.compile('adam')
     >>> _ = gae.fit(graph_tensor, batch_size=32, epochs=50, verbose=0)
     >>> reconstruction_loss = gae.evaluate(graph_tensor, verbose=0)
+    >>> encoder.save( # doctest: +SKIP
+    ...     '/tmp/my_pretrained_encoder_model'
+    ... ) 
+    >>> loaded_encoder = tf.saved_model.load( # doctest: +SKIP
+    ...     '/tmp/my_pretrained_encoder_model'
+    ... )
 
     References:
         .. [#] https://arxiv.org/pdf/1611.07308.pdf
     '''
     def __init__(
         self, 
         encoder: tf.keras.layers.Layer, 
@@ -75,144 +107,145 @@
         balanced_class_weighting: bool = False,
         **kwargs
     ):
         super().__init__(**kwargs)
         self.encoder = encoder
         self.decoder = (
             decoder if decoder is not None 
-            else DotProductIncident(apply_sigmoid=True)
+            else DotProductIncident(normalize=True)
         )
         self.negative_graph_sampler = (
             negative_graph_sampler if negative_graph_sampler is not None 
             else NegativeGraphSampler(1)
         )
         self.balanced_class_weighting = balanced_class_weighting
-        self.reconstruction_loss_tracker = keras.metrics.Mean(
-            name="rec_loss")
-    
-    def compile(self, optimizer, loss=None, *args, **kwargs):
-        super().compile(
-            optimizer=optimizer, loss=None, metrics=None, *args, **kwargs)
-        if loss is None:
-            self.reconstruction_loss = LinkBinaryCrossentropy(name='lbc_loss')
-        else:
-            self.reconstruction_loss = loss
-    
+        self.reconstruction_loss_tracker = keras.metrics.Mean(name="rec_loss")
+
     @property
     def metrics(self):
         return [
             self.reconstruction_loss_tracker
         ]
-    
-    @staticmethod
-    def compute_balanced_class_weighting(edge_score_pos, edge_score_neg):
-        num_positives = tf.shape(edge_score_pos)[0]
-        num_negatives = tf.shape(edge_score_neg)[0]
-        ratio = tf.cast(num_positives / num_negatives, edge_score_pos.dtype)
-        sample_weight = tf.concat([[1.], [ratio]], axis=0)
-        sample_weight = tf.repeat(sample_weight, [num_positives, num_negatives])
-        sample_weight = tf.reshape(sample_weight, [-1, 1])
-        return sample_weight
         
     def train_step(self, tensor: GraphTensor):
         
-        if isinstance(tensor.node_feature, tf.RaggedTensor):
+        if tensor.is_ragged():
             tensor = tensor.merge()
             
         with tf.GradientTape() as tape:
             encoded = self(tensor, training=True)
             encoded_neg = self.negative_graph_sampler(encoded)
             decoded_neg = self.decoder(encoded_neg)
             decoded_pos = self.decoder(encoded)
             
             if self.balanced_class_weighting:
-                sample_weight = self.compute_balanced_class_weighting(
+                sample_weight = _compute_balanced_class_weighting(
                     decoded_pos.edge_score, decoded_neg.edge_score)
             else:
-                sample_weight = None
-            
-            reconstruction_loss = self.reconstruction_loss(
-                decoded_pos.edge_score, 
-                decoded_neg.edge_score,
-                sample_weight=sample_weight)
+                sample_weight = 1.
             
+            if self.loss_fn is None:
+                scores = tf.concat([
+                    decoded_pos.edge_score * -1., 
+                    decoded_neg.edge_score], axis=0)
+                reconstruction_loss = scores * sample_weight
+                reconstruction_loss = tf.reduce_mean(reconstruction_loss)
+            else:
+                reconstruction_loss = self.loss_fn(
+                    decoded_pos.edge_score, 
+                    decoded_neg.edge_score, 
+                    sample_weight=sample_weight)
+                
             reg_loss = sum(self.losses)
 
             loss = reconstruction_loss + reg_loss
             
         trainable_variables = self.trainable_variables
         gradients = tape.gradient(loss, trainable_variables)
         self.optimizer.apply_gradients(zip(gradients, trainable_variables))
 
         self.reconstruction_loss_tracker.update_state(reconstruction_loss)
 
         return {m.name: m.result() for m in self.metrics}
     
     def test_step(self, tensor: GraphTensor):
         
-        if isinstance(tensor.node_feature, tf.RaggedTensor):
+        if tensor.is_ragged():
             tensor = tensor.merge()
-            
+
         encoded = self(tensor, training=False)
         encoded_neg = self.negative_graph_sampler(encoded)
         decoded_neg = self.decoder(encoded_neg)
         decoded_pos = self.decoder(encoded)
         
         if self.balanced_class_weighting:
-            sample_weight = self.compute_balanced_class_weighting(
+            sample_weight = _compute_balanced_class_weighting(
                 decoded_pos.edge_score, decoded_neg.edge_score)
         else:
-            sample_weight = None
+            sample_weight = 1.
 
-        reconstruction_loss = self.reconstruction_loss(
-            decoded_pos.edge_score, 
-            decoded_neg.edge_score,
-            sample_weight=sample_weight)
+        if self.loss_fn is None:
+            scores = tf.concat([
+                decoded_pos.edge_score * -1., 
+                decoded_neg.edge_score], axis=0)
+            reconstruction_loss = scores * sample_weight
+            reconstruction_loss = tf.reduce_mean(reconstruction_loss)
+        else:
+            reconstruction_loss = self.loss_fn(
+                decoded_pos.edge_score, 
+                decoded_neg.edge_score, 
+                sample_weight=sample_weight)
         
         self.reconstruction_loss_tracker.update_state(reconstruction_loss)
 
         return {m.name: m.result() for m in self.metrics}
     
-    # TODO: What should be returned by .predict() ?
-    #       Right now used for debugging.
     def predict_step(self, tensor: GraphTensor) -> GraphTensor:
         
-        if isinstance(tensor.node_feature, tf.RaggedTensor):
+        tensor_orig = tensor
+        if tensor.is_ragged():
             tensor = tensor.merge()
-            ragged = True
-        else:
-            ragged = False
-        
-        # TODO: training = True necessary for GVAE. Otherwise scores always 1. Why?
-        encoded = self(tensor, training=True)
 
-        encoded_neg = self.negative_graph_sampler(encoded)
-        decoded_neg = self.decoder(encoded_neg)
-        decoded_pos = self.decoder(encoded)
-        return {
-            'encoded': encoded,
-            'decoded_positive': decoded_pos, 
-            'decoded_negative': decoded_neg
-        }
-        # if ragged:
-        #     return encoded.separate()
-        # return encoded
+        encoded = self(tensor, training=False)
+        decoded = self.decoder(encoded)
+        return tensor_orig.update({
+            'edge_score': decoded.edge_score}).edge_score
         
     def call(self, tensor: GraphTensor) -> GraphTensor:
         return self.encoder(tensor)
-    
-    def get_config(self):
-        config = super().get_config()
-        config.update({
-            'encoder': layers.serialize(self.encoder),
-            'decoder': layers.serialize(self.decoder),
-            'negative_graph_sampler': layers.serialize(self.negative_graph_sampler),
-            'balanced_class_weighting': self.balanced_class_weighting,
-        })
 
+    def compile(self, optimizer, loss=None, *args, **kwargs):
+        '''Configures the model for training.
+        
+        Args:
+            optimizer (tf.keras.optimizers.Optimizer):
+                The optimizer to use for training.
+            loss (None, tf.keras.losses.Loss):
+                The loss function to use. If None, a default loss function
+                will be used. This loss function simply just tried to 
+                maximize the values of the positive edges and minimize the
+                values of the negative edges. If a custom loss function is used,
+                be aware that the inputs to the loss functions are: positive 
+                edge scores (`y_true` ) and negative edge scores (`y_pred`);
+                both resulting from `molgraph.layers.DotProductIncident(...)`.
+                Default to None.
+            metrics (None):
+                This argument will be ignored (at least for now).
+            *args:
+                See tf.keras.Model.compile documentation.
+            **kwargs:
+                See tf.keras.Model.compile documentation.
+        '''
+        super().compile(
+            optimizer=optimizer, loss=None, metrics=None, *args, **kwargs)
+        
+        if loss is not None:
+            self.loss_fn = loss
+        else:
+            self.loss_fn = None
 
     def fit(
         self, 
         x, 
         y: Any = None, 
         batch_size: Optional[int] = None, 
         epochs: int = 1, 
@@ -296,22 +329,33 @@
                 32 will be used. Default to `None`.
             *args: 
                 See tf.keras.Model.evaluate documentaton.
             **kwargs:
                 See tf.keras.Model.evaluate documentation.
         
         Returns:
-            A dictionary of `GraphTensor` instances, including an encoded
-            `GraphTensor` as well as decoded `GraphTensor`s.
+            `tf.Tensor` or `tf.RaggedTensor` of edge scores, corresponding to 
+            the inputted `GraphTensor` instance.
         '''
         return super().predict(
             x=x, batch_size=batch_size, *args, **kwargs)
 
-      
-# TODO: instead of beta_initial/end/incr, pass a scheduler?
+    def get_config(self):
+        config = super().get_config()
+        config.update({
+            'encoder': layers.serialize(self.encoder),
+            'decoder': layers.serialize(self.decoder),
+            'negative_graph_sampler': layers.serialize(
+                self.negative_graph_sampler),
+            'balanced_class_weighting': self.balanced_class_weighting,
+        })
+        return config
+    
+
+# TODO: instead of beta initial/end/incr, pass a scheduler?
 @register_keras_serializable(package='molgraph')
 class GraphVariationalAutoEncoder(GraphAutoEncoder):
     '''Graph Variational AutoEncoder (GAE) based on Kipf and Welling [#]_.
     
     Args:
         encoder (tf.keras.layers.Layer):
             The encoder part of the autoencoder. The encoder could be
@@ -326,60 +370,92 @@
             GraphTensor instance with negative edges. If None, 
             ``NegativeGraphSampler`` will be used. Default to None.
         balanced_class_weighting (bool):
             Whether balanced class weighting should be performed. For
             instance, if there are twice as many negative edges, should
             each negative edge be weighted 0.5 for the loss?
         beta_initial (float):
-            placeholder
+            Initial beta value (which is multiplied with the kl loss). 
+            Default to 0.0.
         beta_end (float):
-            placeholder
+            End beta value. Default to 0.1.
         beta_incr (float):
-            placeholder
+            The increment rate of the beta value (updated each train step).
+            Default to 1e-6.
     
     **Example:**
 
-    >>> # Obtain GraphTensor instance
-    >>> atom_encoder = molgraph.chemistry.Featurizer([
-    ...     molgraph.chemistry.features.Symbol({'C', 'N', 'O', 'P', 'Na'}),
-    ...     molgraph.chemistry.features.Hybridization(),
-    ... ])
-    >>> bond_encoder = molgraph.chemistry.Featurizer([
-    ...     molgraph.chemistry.features.BondType(),
-    ...     molgraph.chemistry.features.Rotatable()
-    ... ])
-    >>> molgraph_encoder = molgraph.chemistry.MolecularGraphEncoder(
-    ...     atom_encoder, bond_encoder)
-    >>> dataset = molgraph.chemistry.datasets.get('esol', splitter=None)
-    >>> graph_tensor = molgraph_encoder(dataset['x'])
+    >>> # Replace this graph_tensor with a large dataset of graphs
+    >>> # Also accepts featurized graph tensors (via `chemistry.Featurizer`)
+    >>> graph_tensor = molgraph.GraphTensor(
+    ...    data={
+    ...        'edge_src': [1, 4, 0, 2, 3, 1, 1, 0],
+    ...        'edge_dst': [0, 0, 1, 1, 1, 2, 3, 4],
+    ...        'node_feature': [
+    ...            'Sym:C|Hyb:SP3', 
+    ...            'Sym:C|Hyb:SP2', 
+    ...            'Sym:O|Hyb:SP2',
+    ...            'Sym:O|Hyb:SP2', 
+    ...            'Sym:N|Hyb:SP3'
+    ...        ],
+    ...        'edge_feature': [
+    ...            'BonTyp:SINGLE|Rot:1', 
+    ...            'BonTyp:SINGLE|Rot:0',
+    ...            'BonTyp:SINGLE|Rot:1', 
+    ...            'BonTyp:DOUBLE|Rot:0',
+    ...            'BonTyp:SINGLE|Rot:0', 
+    ...            'BonTyp:DOUBLE|Rot:0',
+    ...            'BonTyp:SINGLE|Rot:0', 
+    ...            'BonTyp:SINGLE|Rot:0'
+    ...        ],
+    ...        'graph_indicator': [0, 0, 0, 0, 0],
+    ...    }
+    ... )
+    >>> graph_tensor = graph_tensor.separate()
+    >>> node_embedding = molgraph.layers.NodeEmbeddingLookup(
+    ...    32, mask_token='[MASK]'
+    ... )
+    >>> edge_embedding = molgraph.layers.EdgeEmbeddingLookup(
+    ...    32, mask_token='[MASK]'
+    ... )
+    >>> node_embedding.adapt(graph_tensor)
+    >>> edge_embedding.adapt(graph_tensor)
     >>> # Obtain the encoder of GVAE
     >>> encoder_inputs = tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec)
-    >>> encoder_x = molgraph.layers.GATv2Conv(128, name='shared_conv')(encoder_inputs)
+    >>> encoder_x = node_embedding(encoder_inputs)
+    >>> encoder_x = edge_embedding(encoder_x)
+    >>> encoder_x = molgraph.layers.GATv2Conv(128, name='shared_conv')(encoder_x)
     >>> encoder_x_mean = molgraph.layers.GATv2Conv(128, name='loc_conv')(encoder_x)
     >>> encoder_x_log_var = molgraph.layers.GATv2Conv(128, name='log_var_conv')(encoder_x)
     >>> encoder = tf.keras.Model(encoder_inputs, [encoder_x_mean, encoder_x_log_var])
     >>> # Obtain the decoder of GVAE
-    >>> decoder = molgraph.layers.DotProductIncident(apply_sigmoid=True)
+    >>> decoder = molgraph.layers.DotProductIncident(normalize=True)
     >>> # Obtain, train and evaluate GVAE model
     >>> gvae = molgraph.models.GraphVariationalAutoEncoder(encoder, decoder)
-    >>> gvae.compile('adam', loss=molgraph.losses.LinkBinaryCrossentropy())
+    >>> gvae.compile('adam')
     >>> _ = gvae.fit(graph_tensor, batch_size=32, epochs=50, verbose=0)
     >>> total_loss, rec_loss, kl_loss = gvae.evaluate(graph_tensor, verbose=0)
-    
+    >>> encoder.save( # doctest: +SKIP
+    ...     '/tmp/my_pretrained_encoder_model'
+    ... ) 
+    >>> loaded_encoder = tf.saved_model.load( # doctest: +SKIP
+    ...     '/tmp/my_pretrained_encoder_model'
+    ... )
+
     References:
         .. [#] https://arxiv.org/pdf/1611.07308.pdf
     '''
     def __init__(
         self, 
         encoder: tf.keras.layers.Layer, 
         decoder: Optional[tf.keras.layers.Layer] = None, 
         negative_graph_sampler: Optional[tf.keras.layers.Layer] = None,
         balanced_class_weighting: bool = False,
         beta_initial: float = 0.00,
-        beta_end: float = 0.05,
+        beta_end: float = 0.1,
         beta_incr: float = 1e-6,
         **kwargs
     ):
         super().__init__(
             encoder=encoder, 
             decoder=decoder, 
             negative_graph_sampler=negative_graph_sampler, 
@@ -389,16 +465,15 @@
         self.kl_loss_tracker = keras.metrics.Mean(name="kl_loss")
         self.beta_initial = beta_initial
         self.beta_end = beta_end
         self.beta_incr = beta_incr
         self.beta = tf.Variable(
             initial_value=beta_initial, 
             dtype=tf.float32, 
-            trainable=False
-        )
+            trainable=False)
         
     @property
     def metrics(self):
         return [
             self.total_loss_tracker,
             self.reconstruction_loss_tracker,
             self.kl_loss_tracker,
@@ -413,23 +488,30 @@
 
             encoded = self(tensor, training=True)
             encoded_neg = self.negative_graph_sampler(encoded)
             decoded_neg = self.decoder(encoded_neg)
             decoded_pos = self.decoder(encoded)
             
             if self.balanced_class_weighting:
-                sample_weight = self.compute_balanced_class_weighting(
+                sample_weight = _compute_balanced_class_weighting(
                     decoded_pos.edge_score, decoded_neg.edge_score)
             else:
-                sample_weight = None
+                sample_weight = 1.
 
-            reconstruction_loss = self.reconstruction_loss(
-                decoded_pos.edge_score, 
-                decoded_neg.edge_score,
-                sample_weight=sample_weight)
+            if self.loss_fn is None:
+                scores = tf.concat([
+                    decoded_pos.edge_score * -1., 
+                    decoded_neg.edge_score], axis=0)
+                reconstruction_loss = scores * sample_weight
+                reconstruction_loss = tf.reduce_mean(reconstruction_loss)
+            else:
+                reconstruction_loss = self.loss_fn(
+                    decoded_pos.edge_score, 
+                    decoded_neg.edge_score, 
+                    sample_weight=sample_weight)
             
             kl_loss = self.kl_loss(
                 encoded.node_feature_mean, encoded.node_feature_log_var)
             
             reg_loss = sum(self.losses)
             
             total_loss = reconstruction_loss + kl_loss
@@ -456,24 +538,31 @@
             
         encoded = self(tensor, training=False)
         encoded_neg = self.negative_graph_sampler(encoded)
         decoded_neg = self.decoder(encoded_neg)
         decoded_pos = self.decoder(encoded)
         
         if self.balanced_class_weighting:
-            sample_weight = self.compute_balanced_class_weighting(
+            sample_weight = _compute_balanced_class_weighting(
                 decoded_pos.edge_score, decoded_neg.edge_score)
         else:
-            sample_weight = None
+            sample_weight = 1.
 
-        reconstruction_loss = self.reconstruction_loss(
-            decoded_pos.edge_score, 
-            decoded_neg.edge_score,
-            sample_weight=sample_weight)
-        
+        if self.loss_fn is None:
+            scores = tf.concat([
+                decoded_pos.edge_score * -1., 
+                decoded_neg.edge_score], axis=0)
+            reconstruction_loss = scores * sample_weight
+            reconstruction_loss = tf.reduce_mean(reconstruction_loss)
+        else:
+            reconstruction_loss = self.loss_fn(
+                decoded_pos.edge_score, 
+                decoded_neg.edge_score, 
+                sample_weight=sample_weight)
+    
         kl_loss = self.kl_loss(
             encoded.node_feature_mean, encoded.node_feature_log_var)
         
         total_loss = reconstruction_loss + kl_loss
         
         self.total_loss_tracker.update_state(total_loss)
         self.reconstruction_loss_tracker.update_state(reconstruction_loss)
@@ -484,15 +573,16 @@
     def call(self, tensor: GraphTensor, training: bool) -> GraphTensor:
         (tensor_z_mean, tensor_z_log_var) = self.encoder(tensor)
         
         z_mean = tensor_z_mean.node_feature
         z_log_var = tensor_z_log_var.node_feature
 
         if training:
-            z = z_mean + tf.exp(0.5 * z_log_var) * tf.random.normal(tf.shape(z_log_var))
+            z_shape = tf.shape(z_log_var)
+            z = z_mean + tf.exp(0.5 * z_log_var) * tf.random.normal(z_shape)
         else:
             z = z_mean
  
         return tensor_z_mean.update({
             'node_feature': z,
             'node_feature_mean': z_mean,
             'node_feature_log_var': z_log_var,
@@ -510,14 +600,16 @@
     def get_config(self):
         config = super().get_config()
         config.update({
             'beta_initial': self.beta_initial,
             'beta_end': self.beta_end,
             'beta_incr': self.beta_incr
         })
+        return config
+
 
 @register_keras_serializable(package='molgraph')
 class NaiveNegativeGraphSampler(layers.Layer):
     
     '''Samples a negative graphs, or rather, a graph with negative edges.
     
     It is a "naive" implementation as it simply just shuffles `edge_dst` of
@@ -548,14 +640,15 @@
         return tensor.__class__(**data)
     
     def get_config(self):
         config = super().get_config()
         config.update({'k': self.k})
         return config
     
+
 @register_keras_serializable(package='molgraph')
 class NegativeGraphSampler(NaiveNegativeGraphSampler):
     
     '''Samples a negative graphs, or rather, a graph with negative edges.
     
     This is a "non-naive" implementation as it makes sure that the original
     (positive) edges do not exist in the set of negative edges.
@@ -603,8 +696,18 @@
         edge_src_neg = tf.gather(tensor.edge_src, edges[:, 0])
         edge_dst_neg = tf.gather(tensor.edge_dst, edges[:, 1])
         
         data = tensor._data.copy()
         data['edge_src'] = edge_src_neg
         data['edge_dst'] = edge_dst_neg
 
-        return tensor.__class__(**data)
+        return tensor.__class__(**data)
+    
+
+def _compute_balanced_class_weighting(edge_score_pos, edge_score_neg):
+    num_positives = tf.shape(edge_score_pos)[0] # num positive edges
+    num_negatives = tf.shape(edge_score_neg)[0] # num negative edges
+    ratio = tf.cast(num_positives / num_negatives, edge_score_pos.dtype)
+    sample_weight = tf.concat([[1.], [ratio]], axis=0)
+    sample_weight = tf.repeat(sample_weight, [num_positives, num_negatives])
+    sample_weight = tf.reshape(sample_weight, [-1, 1])
+    return sample_weight
```

### Comparing `molgraph-0.5.5/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.6/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.6/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.5/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.6/molgraph/tensors/graph_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
                 exponentiate=exponentiate,
                 clip_values=clip_values)
             
         data['node_feature'] = gnn_ops.propagate_node_features(
             node_feature=data['node_feature'],
             edge_src=data['edge_src'],
             edge_dst=data['edge_dst'],
-            edge_weight=data.get('edge_weight', None),
+            edge_weight=data.pop('edge_weight', None),
             mode=mode)
         
         if residual is not None:
             if isinstance(residual, tf.RaggedTensor):
                 residual = residual.flat_values
             data['node_feature'] += residual
 
@@ -566,14 +566,15 @@
                 output_units=output_units,
                 axis=reduce_axis)
         
         graph_tensor = self.__class__(data)
 
         if not self.is_ragged():
             return graph_tensor 
+        
         return graph_tensor.separate()
 
     def is_ragged(self):
         '''Checks whether nested data are ragged.
         
         Returns:
             bool: A boolean indicating whether nested data are ragged.
```

### Comparing `molgraph-0.5.5/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.6/molgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.5
+Version: 0.5.6
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.5.5/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.6/molgraph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 molgraph/internal.py
 molgraph.egg-info/PKG-INFO
 molgraph.egg-info/SOURCES.txt
 molgraph.egg-info/dependency_links.txt
 molgraph.egg-info/requires.txt
 molgraph.egg-info/top_level.txt
 molgraph/applications/__init__.py
-molgraph/applications/graph_transformer.py
 molgraph/chemistry/__init__.py
 molgraph/chemistry/conformer_generator.py
 molgraph/chemistry/conformer_utils.py
 molgraph/chemistry/encoders.py
 molgraph/chemistry/features.py
 molgraph/chemistry/molecular_encoders.py
 molgraph/chemistry/ops.py
```

### Comparing `molgraph-0.5.5/setup.py` & `molgraph-0.5.6/setup.py`

 * *Files identical despite different names*

