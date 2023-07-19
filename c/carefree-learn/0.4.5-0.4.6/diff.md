# Comparing `tmp/carefree-learn-0.4.5.tar.gz` & `tmp/carefree-learn-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-learn-0.4.5.tar", last modified: Mon May 22 14:46:50 2023, max compression
+gzip compressed data, was "carefree-learn-0.4.6.tar", last modified: Wed Jul 19 04:27:09 2023, max compression
```

## Comparing `carefree-learn-0.4.5.tar` & `carefree-learn-0.4.6.tar`

### file list

```diff
@@ -1,361 +1,363 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.054180 carefree-learn-0.4.5/
--rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/LICENSE
--rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7575 2023-05-22 14:46:50.054180 carefree-learn-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.918865 carefree-learn-0.4.5/carefree_learn.egg-info/
--rw-rw-rw-   0        0        0     7575 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10736 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      644 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.922850 carefree-learn-0.4.5/cflearn/
--rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.924843 carefree-learn-0.4.5/cflearn/api/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/api/__init__.py
--rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.5/cflearn/api/api.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.926836 carefree-learn-0.4.5/cflearn/api/cv/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/api/cv/__init__.py
--rw-rw-rw-   0        0        0    74341 2023-05-22 14:45:42.000000 carefree-learn-0.4.5/cflearn/api/cv/diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.928830 carefree-learn-0.4.5/cflearn/api/cv/third_party/
--rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/blip.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.929827 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/api.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.931820 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/predictor.py
--rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/transforms.py
--rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.932816 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/
--rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
--rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/base.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.934809 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.936803 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/
--rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
--rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
--rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
--rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.937801 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/
--rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
--rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
--rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.942783 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
--rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
--rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
--rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
--rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
--rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
--rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
--rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
--rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
--rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modifiers.py
--rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/ops.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.942783 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/utils/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/utils/__init__.py
--rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/utils/misc.py
--rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/isnet.py
--rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/lama.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.944777 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/__init__.py
--rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/api.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.947766 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/__init__.py
--rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/base_model.py
--rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/blocks.py
--rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/dpt_depth.py
--rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net.py
--rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
--rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/transforms.py
--rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/vit.py
--rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.948763 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/__init__.py
--rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/api.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.949759 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.951753 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/api.py
--rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/body.py
--rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/hand.py
--rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/model.py
--rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/util.py
--rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/prompt.py
--rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.5/cflearn/api/cv/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.952749 carefree-learn-0.4.5/cflearn/api/ml/
--rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/api/ml/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/api/ml/ddr.py
--rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/api/schema.py
--rw-rw-rw-   0        0        0     2983 2023-05-17 13:13:35.000000 carefree-learn-0.4.5/cflearn/api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.952749 carefree-learn-0.4.5/cflearn/api/zoo/
--rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.5/cflearn/api/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.954743 carefree-learn-0.4.5/cflearn/callbacks/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.5/cflearn/callbacks/classification.py
--rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.5/cflearn/callbacks/general.py
--rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.5/cflearn/callbacks/generator.py
--rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.955739 carefree-learn-0.4.5/cflearn/data/
--rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.5/cflearn/data/__init__.py
--rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.5/cflearn/data/array.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.955739 carefree-learn-0.4.5/cflearn/data/blocks/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.959727 carefree-learn-0.4.5/cflearn/data/blocks/cv/
--rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/crop.py
--rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/hwc_to_chw.py
--rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/image_folder.py
--rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/normalize.py
--rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/to_numpy.py
--rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/tuple_to_batch.py
--rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/flatten.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.963713 carefree-learn-0.4.5/cflearn/data/blocks/ml/
--rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/__init__.py
--rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/file.py
--rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/gather.py
--rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/nan_handler.py
--rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/preprocessor.py
--rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/recognizer.py
--rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/schema.py
--rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/splitter.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.964710 carefree-learn-0.4.5/cflearn/data/ml/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/ml/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.5/cflearn/data/ml/api.py
--rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/ml/datasets.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.966704 carefree-learn-0.4.5/cflearn/data/pytorch/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/pytorch/__init__.py
--rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.5/cflearn/data/pytorch/api.py
--rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.5/cflearn/data/pytorch/datasets.py
--rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.5/cflearn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.967700 carefree-learn-0.4.5/cflearn/dist/
--rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/dist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.969694 carefree-learn-0.4.5/cflearn/dist/ml/
--rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/dist/ml/__init__.py
--rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/experiment.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.971687 carefree-learn-0.4.5/cflearn/dist/ml/runs/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/dist/ml/runs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/runs/_utils.py
--rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/runs/basic.py
--rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/task.py
--rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/inference.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.975674 carefree-learn-0.4.5/cflearn/losses/
--rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/losses/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.5/cflearn/losses/basic.py
--rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/losses/gan.py
--rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.5/cflearn/losses/lpips.py
--rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/losses/vae.py
--rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.978666 carefree-learn-0.4.5/cflearn/misc/
--rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.5/cflearn/misc/__init__.py
--rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.5/cflearn/misc/available.json
--rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/misc/mixins.py
--rw-rw-rw-   0        0        0    44325 2023-05-19 13:03:56.000000 carefree-learn-0.4.5/cflearn/misc/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.979662 carefree-learn-0.4.5/cflearn/models/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/bases.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.980659 carefree-learn-0.4.5/cflearn/models/cv/
--rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.982385 carefree-learn-0.4.5/cflearn/models/cv/ae/
--rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/__init__.py
--rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/common.py
--rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/kl.py
--rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/vq.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.983389 carefree-learn-0.4.5/cflearn/models/cv/classifier/
--rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/classifier/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/classifier/vanilla.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.987376 carefree-learn-0.4.5/cflearn/models/cv/decoder/
--rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/__init__.py
--rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/attn.py
--rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/schema.py
--rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan.py
--rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan_v2.py
--rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/vanilla.py
--rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.990365 carefree-learn-0.4.5/cflearn/models/cv/diffusion/
--rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.992358 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/
--rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/clip.py
--rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/rescaler.py
--rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/schema.py
--rw-rw-rw-   0        0        0    29604 2023-05-19 13:31:09.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/ddpm.py
--rw-rw-rw-   0        0        0    10675 2023-05-18 07:21:12.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/ldm.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.995377 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/
--rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/basic.py
--rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/ddim.py
--rw-rw-rw-   0        0        0    13157 2023-05-21 02:40:49.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/k_samplers.py
--rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/plms.py
--rw-rw-rw-   0        0        0     7804 2023-05-21 03:23:44.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/schema.py
--rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/solver.py
--rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/utils.py
--rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/unet.py
--rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.999364 carefree-learn-0.4.5/cflearn/models/cv/encoder/
--rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/attn.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.001358 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/
--rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/api.py
--rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/core.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.003351 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/
--rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/__init__.py
--rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/mobilenet.py
--rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/resnet.py
--rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/transformer.py
--rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/vgg.py
--rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/register.py
--rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/fnet.py
--rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/mixer.py
--rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/perceiver.py
--rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/pool_former.py
--rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/schema.py
--rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/transformer.py
--rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/vanilla.py
--rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.004348 carefree-learn-0.4.5/cflearn/models/cv/gan/
--rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/__init__.py
--rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/discriminators.py
--rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/schema.py
--rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/vanilla.py
--rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/general.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.005344 carefree-learn-0.4.5/cflearn/models/cv/translator/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/translator/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/translator/rrdb.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.006342 carefree-learn-0.4.5/cflearn/models/implicit/
--rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/implicit/__init__.py
--rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/implicit/siren.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.011325 carefree-learn-0.4.5/cflearn/models/ml/
--rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/base.py
--rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.5/cflearn/models/ml/ddr.py
--rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.5/cflearn/models/ml/encoders.py
--rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/fcnn.py
--rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/linear.py
--rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/mixed_stacked.py
--rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/nbm.py
--rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/ndt.py
--rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/rnn.py
--rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/wnd.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.013318 carefree-learn-0.4.5/cflearn/models/multimodal/
--rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/multimodal/__init__.py
--rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.5/cflearn/models/multimodal/clip.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/multimodal/constants.py
--rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.5/cflearn/models/multimodal/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.013318 carefree-learn-0.4.5/cflearn/models/nlp/
--rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.015312 carefree-learn-0.4.5/cflearn/models/nlp/encoder/
--rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/encoder/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/encoder/constants.py
--rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/encoder/transformer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.016307 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/clip.py
--rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.018302 carefree-learn-0.4.5/cflearn/models/nlp/transformers/
--rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/__init__.py
--rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/core.py
--rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/opus.py
--rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/simbert.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.019298 carefree-learn-0.4.5/cflearn/models/schemas/
--rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.5/cflearn/models/schemas/__init__.py
--rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/models/schemas/custom.py
--rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/schemas/cv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.021292 carefree-learn-0.4.5/cflearn/modules/
--rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.030262 carefree-learn-0.4.5/cflearn/modules/blocks/
--rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.5/cflearn/modules/blocks/__init__.py
--rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.5/cflearn/modules/blocks/activations.py
--rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.5/cflearn/modules/blocks/attentions.py
--rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.5/cflearn/modules/blocks/common.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.031259 carefree-learn-0.4.5/cflearn/modules/blocks/convs/
--rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/convs/__init__.py
--rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.5/cflearn/modules/blocks/convs/basic.py
--rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.5/cflearn/modules/blocks/convs/residual.py
--rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.5/cflearn/modules/blocks/customs.py
--rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/modules/blocks/high_level.py
--rw-rw-rw-   0        0        0    15078 2023-05-16 07:51:00.000000 carefree-learn-0.4.5/cflearn/modules/blocks/hijacks.py
--rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.5/cflearn/modules/blocks/hooks.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.032255 carefree-learn-0.4.5/cflearn/modules/blocks/implementations/
--rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/implementations/__init__.py
--rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/implementations/perceiver.py
--rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.036242 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/
--rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/__init__.py
--rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/api.py
--rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
--rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/poolers.py
--rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/schema.py
--rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/token_mixers.py
--rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/norms.py
--rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.5/cflearn/modules/blocks/utils.py
--rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/optimizers.py
--rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.5/cflearn/modules/schedulers.py
--rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/monitors.py
--rw-rw-rw-   0        0        0      744 2023-05-19 03:26:36.000000 carefree-learn-0.4.5/cflearn/parameters.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.039231 carefree-learn-0.4.5/cflearn/pipeline/
--rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/__init__.py
--rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.5/cflearn/pipeline/api.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.041225 carefree-learn-0.4.5/cflearn/pipeline/blocks/
--rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/__init__.py
--rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/basic.py
--rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/ml.py
--rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/utils.py
--rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.5/cflearn/pipeline/core.py
--rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/schema.py
--rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/third_party.py
--rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/register.py
--rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.5/cflearn/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.042221 carefree-learn-0.4.5/cflearn/scripts/
--rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.5/cflearn/scripts/__init__.py
--rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/scripts/sd.py
--rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/trainer.py
--rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/types.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.044216 carefree-learn-0.4.5/cflearn/zoo/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.888455 carefree-learn-0.4.5/cflearn/zoo/configs/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.886462 carefree-learn-0.4.5/cflearn/zoo/configs/ae/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.045211 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/
--rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f16.json
--rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f4.json
--rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.047205 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/
--rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/f4.json
--rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/f4_no_attn.json
--rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.887460 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.047205 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ddpm/
--rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ddpm/default.json
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.050195 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/
--rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/default.json
--rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd.json
--rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
--rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
--rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
--rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/vq.json
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.887460 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.052188 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/
--rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/chinese.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/default.json
--rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/large.json
--rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.888455 carefree-learn-0.4.5/cflearn/zoo/configs/sr/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.052188 carefree-learn-0.4.5/cflearn/zoo/configs/sr/esr/
--rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/sr/esr/anime.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/sr/esr/default.json
--rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.5/cflearn/zoo/core.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.053184 carefree-learn-0.4.5/cflearn/zoo/models/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/models/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/models/clip.py
--rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/models/schema.py
--rw-rw-rw-   0        0        0      383 2023-05-22 14:46:50.058168 carefree-learn-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1748 2023-05-22 14:46:08.000000 carefree-learn-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.613054 carefree-learn-0.4.6/
+-rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7575 2023-07-19 04:27:09.613054 carefree-learn-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.452103 carefree-learn-0.4.6/carefree_learn.egg-info/
+-rw-rw-rw-   0        0        0     7575 2023-07-19 04:27:09.000000 carefree-learn-0.4.6/carefree_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10798 2023-07-19 04:27:09.000000 carefree-learn-0.4.6/carefree_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 04:27:09.000000 carefree-learn-0.4.6/carefree_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      651 2023-07-19 04:27:09.000000 carefree-learn-0.4.6/carefree_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 04:27:09.000000 carefree-learn-0.4.6/carefree_learn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.455096 carefree-learn-0.4.6/cflearn/
+-rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.457089 carefree-learn-0.4.6/cflearn/api/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/api/__init__.py
+-rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.6/cflearn/api/api.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.458086 carefree-learn-0.4.6/cflearn/api/cv/
+-rw-rw-rw-   0        0        0      107 2023-06-16 01:49:46.000000 carefree-learn-0.4.6/cflearn/api/cv/__init__.py
+-rw-rw-rw-   0        0        0     3479 2023-06-16 01:49:46.000000 carefree-learn-0.4.6/cflearn/api/cv/annotator.py
+-rw-rw-rw-   0        0        0    76201 2023-07-17 08:33:04.000000 carefree-learn-0.4.6/cflearn/api/cv/diffusion.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.460079 carefree-learn-0.4.6/cflearn/api/cv/third_party/
+-rw-rw-rw-   0        0        0      176 2023-06-13 07:15:16.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/blip.py
+-rw-rw-rw-   0        0        0     4485 2023-06-14 03:02:47.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/hed.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.461076 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/api.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.462072 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/__init__.py
+-rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/predictor.py
+-rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/transforms.py
+-rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.463069 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/mconfigs/
+-rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
+-rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/mconfigs/base.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.464066 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.466059 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/
+-rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
+-rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
+-rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
+-rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.467055 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/
+-rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
+-rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
+-rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.470046 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
+-rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
+-rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
+-rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
+-rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
+-rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
+-rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
+-rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
+-rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
+-rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modifiers.py
+-rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/ops.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.471043 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/utils/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/utils/misc.py
+-rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/isnet.py
+-rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/lama.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.472039 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/__init__.py
+-rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/api.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.475030 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/base_model.py
+-rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/blocks.py
+-rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/dpt_depth.py
+-rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/midas_net.py
+-rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/transforms.py
+-rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/vit.py
+-rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.476026 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/api.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.477023 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.479016 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/api.py
+-rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/body.py
+-rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/hand.py
+-rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/model.py
+-rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/util.py
+-rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/api/cv/third_party/prompt.py
+-rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.6/cflearn/api/cv/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.480013 carefree-learn-0.4.6/cflearn/api/ml/
+-rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/api/ml/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/api/ml/ddr.py
+-rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/api/schema.py
+-rw-rw-rw-   0        0        0     3217 2023-05-31 08:15:52.000000 carefree-learn-0.4.6/cflearn/api/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.480013 carefree-learn-0.4.6/cflearn/api/zoo/
+-rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.6/cflearn/api/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.482006 carefree-learn-0.4.6/cflearn/callbacks/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.6/cflearn/callbacks/classification.py
+-rw-rw-rw-   0        0        0     9604 2023-07-19 04:26:27.000000 carefree-learn-0.4.6/cflearn/callbacks/general.py
+-rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.6/cflearn/callbacks/generator.py
+-rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.483002 carefree-learn-0.4.6/cflearn/data/
+-rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.6/cflearn/data/__init__.py
+-rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.6/cflearn/data/array.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.484000 carefree-learn-0.4.6/cflearn/data/blocks/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.486989 carefree-learn-0.4.6/cflearn/data/blocks/cv/
+-rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/crop.py
+-rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/hwc_to_chw.py
+-rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/image_folder.py
+-rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/normalize.py
+-rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/to_numpy.py
+-rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/cv/tuple_to_batch.py
+-rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/flatten.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.488983 carefree-learn-0.4.6/cflearn/data/blocks/ml/
+-rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/__init__.py
+-rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/file.py
+-rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/gather.py
+-rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/nan_handler.py
+-rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/preprocessor.py
+-rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/recognizer.py
+-rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/schema.py
+-rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.6/cflearn/data/blocks/ml/splitter.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.489979 carefree-learn-0.4.6/cflearn/data/ml/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/ml/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.6/cflearn/data/ml/api.py
+-rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/ml/datasets.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.490975 carefree-learn-0.4.6/cflearn/data/pytorch/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/data/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.6/cflearn/data/pytorch/api.py
+-rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.6/cflearn/data/pytorch/datasets.py
+-rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.6/cflearn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.490975 carefree-learn-0.4.6/cflearn/dist/
+-rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/dist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.491972 carefree-learn-0.4.6/cflearn/dist/ml/
+-rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/dist/ml/__init__.py
+-rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/dist/ml/experiment.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.492969 carefree-learn-0.4.6/cflearn/dist/ml/runs/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/dist/ml/runs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/dist/ml/runs/_utils.py
+-rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/dist/ml/runs/basic.py
+-rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/dist/ml/task.py
+-rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/inference.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.493966 carefree-learn-0.4.6/cflearn/losses/
+-rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/losses/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.6/cflearn/losses/basic.py
+-rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/losses/gan.py
+-rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.6/cflearn/losses/lpips.py
+-rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/losses/vae.py
+-rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.500942 carefree-learn-0.4.6/cflearn/misc/
+-rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.6/cflearn/misc/__init__.py
+-rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.6/cflearn/misc/available.json
+-rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/misc/mixins.py
+-rw-rw-rw-   0        0        0    44325 2023-05-19 13:03:56.000000 carefree-learn-0.4.6/cflearn/misc/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.500942 carefree-learn-0.4.6/cflearn/models/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/__init__.py
+-rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/bases.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.501939 carefree-learn-0.4.6/cflearn/models/cv/
+-rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.503932 carefree-learn-0.4.6/cflearn/models/cv/ae/
+-rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.6/cflearn/models/cv/ae/__init__.py
+-rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.6/cflearn/models/cv/ae/common.py
+-rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.6/cflearn/models/cv/ae/kl.py
+-rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.6/cflearn/models/cv/ae/vq.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.503932 carefree-learn-0.4.6/cflearn/models/cv/classifier/
+-rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/classifier/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/classifier/vanilla.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.505926 carefree-learn-0.4.6/cflearn/models/cv/decoder/
+-rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/__init__.py
+-rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/attn.py
+-rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/schema.py
+-rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/style_gan.py
+-rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/style_gan_v2.py
+-rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/vanilla.py
+-rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/decoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.507918 carefree-learn-0.4.6/cflearn/models/cv/diffusion/
+-rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.508915 carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/
+-rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/__init__.py
+-rw-rw-rw-   0        0        0    10071 2023-06-17 08:21:08.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/clip.py
+-rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/rescaler.py
+-rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/schema.py
+-rw-rw-rw-   0        0        0    30870 2023-07-17 08:34:31.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/ddpm.py
+-rw-rw-rw-   0        0        0    10675 2023-05-18 07:21:12.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/ldm.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.512903 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/
+-rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/basic.py
+-rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/ddim.py
+-rw-rw-rw-   0        0        0    13157 2023-05-21 02:40:49.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/k_samplers.py
+-rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/plms.py
+-rw-rw-rw-   0        0        0     7912 2023-07-17 09:42:25.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/schema.py
+-rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/solver.py
+-rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/utils.py
+-rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/unet.py
+-rw-rw-rw-   0        0        0      772 2023-07-17 08:33:40.000000 carefree-learn-0.4.6/cflearn/models/cv/diffusion/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.516889 carefree-learn-0.4.6/cflearn/models/cv/encoder/
+-rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/__init__.py
+-rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/attn.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.517885 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/
+-rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/api.py
+-rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/core.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.518882 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/
+-rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/__init__.py
+-rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/mobilenet.py
+-rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/resnet.py
+-rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/transformer.py
+-rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/vgg.py
+-rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/register.py
+-rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/fnet.py
+-rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/mixer.py
+-rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/perceiver.py
+-rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/pool_former.py
+-rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/schema.py
+-rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/transformer.py
+-rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/vanilla.py
+-rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/models/cv/encoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.520876 carefree-learn-0.4.6/cflearn/models/cv/gan/
+-rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/gan/__init__.py
+-rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/cv/gan/discriminators.py
+-rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.6/cflearn/models/cv/gan/schema.py
+-rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/gan/vanilla.py
+-rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/general.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.520876 carefree-learn-0.4.6/cflearn/models/cv/translator/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/cv/translator/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/cv/translator/rrdb.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.521872 carefree-learn-0.4.6/cflearn/models/implicit/
+-rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/implicit/__init__.py
+-rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/models/implicit/siren.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.524862 carefree-learn-0.4.6/cflearn/models/ml/
+-rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/base.py
+-rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.6/cflearn/models/ml/ddr.py
+-rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.6/cflearn/models/ml/encoders.py
+-rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/fcnn.py
+-rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/linear.py
+-rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/mixed_stacked.py
+-rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/nbm.py
+-rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/ndt.py
+-rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/rnn.py
+-rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/ml/wnd.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.526856 carefree-learn-0.4.6/cflearn/models/multimodal/
+-rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/multimodal/__init__.py
+-rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.6/cflearn/models/multimodal/clip.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/multimodal/constants.py
+-rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.6/cflearn/models/multimodal/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.526856 carefree-learn-0.4.6/cflearn/models/nlp/
+-rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.527852 carefree-learn-0.4.6/cflearn/models/nlp/encoder/
+-rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/encoder/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/encoder/constants.py
+-rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/encoder/transformer.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.528848 carefree-learn-0.4.6/cflearn/models/nlp/tokenizers/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/nlp/tokenizers/clip.py
+-rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/tokenizers/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.529846 carefree-learn-0.4.6/cflearn/models/nlp/transformers/
+-rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/transformers/__init__.py
+-rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.6/cflearn/models/nlp/transformers/core.py
+-rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/transformers/opus.py
+-rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/models/nlp/transformers/simbert.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.530844 carefree-learn-0.4.6/cflearn/models/schemas/
+-rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.6/cflearn/models/schemas/__init__.py
+-rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/models/schemas/custom.py
+-rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/models/schemas/cv.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.532835 carefree-learn-0.4.6/cflearn/modules/
+-rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.536827 carefree-learn-0.4.6/cflearn/modules/blocks/
+-rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.6/cflearn/modules/blocks/__init__.py
+-rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.6/cflearn/modules/blocks/activations.py
+-rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.6/cflearn/modules/blocks/attentions.py
+-rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.6/cflearn/modules/blocks/common.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.537824 carefree-learn-0.4.6/cflearn/modules/blocks/convs/
+-rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/blocks/convs/__init__.py
+-rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.6/cflearn/modules/blocks/convs/basic.py
+-rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.6/cflearn/modules/blocks/convs/residual.py
+-rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.6/cflearn/modules/blocks/customs.py
+-rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/modules/blocks/high_level.py
+-rw-rw-rw-   0        0        0    15144 2023-06-13 07:03:57.000000 carefree-learn-0.4.6/cflearn/modules/blocks/hijacks.py
+-rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.6/cflearn/modules/blocks/hooks.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.538820 carefree-learn-0.4.6/cflearn/modules/blocks/implementations/
+-rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/blocks/implementations/__init__.py
+-rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/blocks/implementations/perceiver.py
+-rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mappings.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.540813 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/
+-rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/__init__.py
+-rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/api.py
+-rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
+-rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/poolers.py
+-rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/schema.py
+-rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/token_mixers.py
+-rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/blocks/norms.py
+-rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.6/cflearn/modules/blocks/utils.py
+-rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.6/cflearn/modules/optimizers.py
+-rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.6/cflearn/modules/schedulers.py
+-rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/monitors.py
+-rw-rw-rw-   0        0        0      744 2023-05-19 03:26:36.000000 carefree-learn-0.4.6/cflearn/parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.542807 carefree-learn-0.4.6/cflearn/pipeline/
+-rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/pipeline/__init__.py
+-rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.6/cflearn/pipeline/api.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.543803 carefree-learn-0.4.6/cflearn/pipeline/blocks/
+-rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/pipeline/blocks/__init__.py
+-rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.6/cflearn/pipeline/blocks/basic.py
+-rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/pipeline/blocks/ml.py
+-rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/pipeline/blocks/utils.py
+-rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.6/cflearn/pipeline/core.py
+-rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/pipeline/schema.py
+-rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/pipeline/third_party.py
+-rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/register.py
+-rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.6/cflearn/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.543803 carefree-learn-0.4.6/cflearn/scripts/
+-rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.6/cflearn/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/scripts/sd.py
+-rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.6/cflearn/trainer.py
+-rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/types.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.544799 carefree-learn-0.4.6/cflearn/zoo/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.425089 carefree-learn-0.4.6/cflearn/zoo/configs/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.424093 carefree-learn-0.4.6/cflearn/zoo/configs/ae/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.555287 carefree-learn-0.4.6/cflearn/zoo/configs/ae/kl/
+-rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/ae/kl/f16.json
+-rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/zoo/configs/ae/kl/f4.json
+-rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/ae/kl/f8.json
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.567246 carefree-learn-0.4.6/cflearn/zoo/configs/ae/vq/
+-rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/ae/vq/f4.json
+-rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/ae/vq/f4_no_attn.json
+-rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/ae/vq/f8.json
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.424093 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.571181 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ddpm/
+-rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ddpm/default.json
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.591131 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/
+-rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/default.json
+-rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/sd.json
+-rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
+-rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
+-rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
+-rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/vq.json
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.425089 carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.605085 carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/clip/
+-rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/clip/chinese.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/clip/default.json
+-rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/clip/large.json
+-rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.425089 carefree-learn-0.4.6/cflearn/zoo/configs/sr/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.611064 carefree-learn-0.4.6/cflearn/zoo/configs/sr/esr/
+-rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/configs/sr/esr/anime.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/zoo/configs/sr/esr/default.json
+-rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.6/cflearn/zoo/core.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:27:09.612057 carefree-learn-0.4.6/cflearn/zoo/models/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/models/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.6/cflearn/zoo/models/clip.py
+-rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.6/cflearn/zoo/models/schema.py
+-rw-rw-rw-   0        0        0      448 2023-07-19 04:27:09.617044 carefree-learn-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1755 2023-07-19 04:26:57.000000 carefree-learn-0.4.6/setup.py
```

### Comparing `carefree-learn-0.4.5/LICENSE` & `carefree-learn-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/PKG-INFO` & `carefree-learn-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.5
+Version: 0.4.6
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.5.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.6.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.5/README.md` & `carefree-learn-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/carefree_learn.egg-info/PKG-INFO` & `carefree-learn-0.4.6/carefree_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.5
+Version: 0.4.6
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.5.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.6.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.5/carefree_learn.egg-info/SOURCES.txt` & `carefree-learn-0.4.6/carefree_learn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 cflearn/trainer.py
 cflearn/types.py
 cflearn/api/__init__.py
 cflearn/api/api.py
 cflearn/api/schema.py
 cflearn/api/utils.py
 cflearn/api/cv/__init__.py
+cflearn/api/cv/annotator.py
 cflearn/api/cv/diffusion.py
 cflearn/api/cv/translator.py
 cflearn/api/cv/third_party/__init__.py
 cflearn/api/cv/third_party/blip.py
+cflearn/api/cv/third_party/hed.py
 cflearn/api/cv/third_party/isnet.py
 cflearn/api/cv/third_party/lama.py
 cflearn/api/cv/third_party/prompt.py
 cflearn/api/cv/third_party/iharm/__init__.py
 cflearn/api/cv/third_party/iharm/api.py
 cflearn/api/cv/third_party/iharm/inference/__init__.py
 cflearn/api/cv/third_party/iharm/inference/predictor.py
```

### Comparing `carefree-learn-0.4.5/carefree_learn.egg-info/requires.txt` & `carefree-learn-0.4.6/carefree_learn.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 filelock
 accelerate
 safetensors
-carefree-toolkit>=0.3.5
+carefree-toolkit>=0.3.7
 
 [cv]
 ftfy
 lmdb
 regex
 transformers
 albumentations
@@ -46,14 +46,14 @@
 onnx-simplifier>=0.4.1
 open_clip_torch
 faiss-cpu
 protobuf==3.19.4
 ortools>=9.3.0
 sacremoses
 sentencepiece
-mlflow
+mlflow>=2.5.0
 plotly
 
 [onnx]
 onnx
 onnxruntime
 onnx-simplifier>=0.4.1
```

### Comparing `carefree-learn-0.4.5/cflearn/__init__.py` & `carefree-learn-0.4.6/cflearn/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/api.py` & `carefree-learn-0.4.6/cflearn/api/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/diffusion.py` & `carefree-learn-0.4.6/cflearn/api/cv/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import json
+import time
 import torch
 import random
 
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
 
-from abc import abstractmethod
-from abc import ABC
 from PIL import Image
 from enum import Enum
 from tqdm import tqdm
 from torch import Tensor
 from typing import Any
 from typing import Dict
 from typing import List
@@ -28,38 +27,39 @@
 from dataclasses import dataclass
 from cftool.cv import to_rgb
 from cftool.cv import to_uint8
 from cftool.cv import read_image
 from cftool.cv import save_images
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
+from cftool.cv import ImageBox
 from cftool.cv import ReadImageResponse
 from cftool.misc import safe_execute
 from cftool.misc import print_warning
 from cftool.misc import shallow_copy_dict
 from cftool.types import arr_type
 from cftool.types import tensor_dict_type
+from cftool.types import TNumberPair
 from safetensors.torch import load_file
 from cflearn.misc.toolkit import _get_file_size
 
+from .annotator import annotators
+from .annotator import Annotator
 from ..zoo import ldm_sd
 from ..zoo import ldm_sd_v2
 from ..zoo import ldm_sd_v2_base
 from ..zoo import ldm_sd_tag
 from ..zoo import ldm_sd_inpainting
 from ..zoo import ldm_sr
 from ..zoo import ldm_semantic
 from ..zoo import ldm_celeba_hq
 from ..zoo import ldm_inpainting
 from ..zoo import DLZoo
 from ..utils import APIMixin
 from ..utils import WeightsPool
-from .third_party import MiDaSAPI
-from .third_party import MLSDDetector
-from .third_party import OpenposeDetector
 from ...data import ArrayData
 from ...schema import DataConfig
 from ...constants import INPUT_KEY
 from ...constants import PREDICTIONS_KEY
 from ...parameters import OPT
 from ...data.utils import predict_array_data
 from ...data.utils import TensorBatcher
@@ -79,24 +79,27 @@
 from ...models.cv.ae.common import IAutoEncoder
 from ...models.cv.diffusion.utils import get_timesteps
 from ...models.cv.diffusion.utils import CONCAT_KEY
 from ...models.cv.diffusion.utils import CONCAT_TYPE
 from ...models.cv.diffusion.utils import HYBRID_TYPE
 from ...models.cv.diffusion.utils import CROSS_ATTN_KEY
 from ...models.cv.diffusion.utils import CONTROL_HINT_KEY
+from ...models.cv.diffusion.utils import CONTROL_HINT_END_KEY
 from ...models.cv.diffusion.utils import CONTROL_HINT_START_KEY
 from ...models.cv.diffusion.cond_models import CLIPTextConditionModel
 from ...models.cv.diffusion.samplers.ddim import DDIMMixin
 from ...models.cv.diffusion.samplers.solver import DPMSolver
 from ...models.cv.diffusion.samplers.k_samplers import KSamplerMixin
 
 try:
     import cv2
+
+    INTER_LANCZOS4 = cv2.INTER_LANCZOS4
 except:
-    cv2 = None
+    cv2 = INTER_LANCZOS4 = None
 
 
 class switch_sampler_context:
     def __init__(self, api: "DiffusionAPI", sampler: Optional[str]):
         self.api = api
         self.m_sampler = api.sampler.__identifier__
         self.target_sampler = sampler
@@ -131,15 +134,14 @@
     original_image: Image.Image
     original_mask: Image.Image
     wh_ratio: Tuple[float, float]
     crop_res: Optional["CropResponse"]
 
 
 T = TypeVar("T", bound="DiffusionAPI")
-TAnnotator = TypeVar("TAnnotator", bound="Annotator")
 
 
 class SDVersions(str, Enum):
     v1_5_BC = ""
     v1_5 = "v1.5"
     ANIME = "anime"
     ANIME_ANYTHING = "anime_anything"
@@ -189,114 +191,98 @@
     return tuple(map(get_suitable_size, new_size, (anchor, anchor)))  # type: ignore
 
 
 def get_highres_steps(num_steps: int, fidelity: float) -> int:
     return int(num_steps / min(1.0 - fidelity, 0.999))
 
 
-def _convert_external(m: "DiffusionAPI", tag: str, sub_folder: Optional[str]) -> str:
+def _convert_external(
+    m: "DiffusionAPI",
+    tag: str,
+    sub_folder: Optional[str],
+    *,
+    convert_fn: Optional[Callable] = None,
+) -> str:
     external_root = OPT.external_dir
     if sub_folder is not None:
         external_root = os.path.join(external_root, sub_folder)
     lock_path = os.path.join(external_root, "load_external.lock")
     lock = FileLock(lock_path)
     with lock:
         converted_sizes_path = os.path.join(external_root, "sizes.json")
         sizes: Dict[str, int]
         if not os.path.isfile(converted_sizes_path):
             sizes = {}
         else:
             with open(converted_sizes_path, "r") as f:
                 sizes = json.load(f)
-        converted_path = os.path.join(external_root, f"{tag}_converted.pt")
-        v_size = sizes.get(tag)
-        f_size = (
-            None
-            if not os.path.isfile(converted_path)
-            else _get_file_size(converted_path)
-        )
-        if f_size is None or v_size != f_size:
-            if f_size is not None:
-                print(f"> '{tag}' has been converted but size mismatch")
-            print(f"> converting external weights '{tag}'")
-            model_path = os.path.join(external_root, f"{tag}.ckpt")
-            if not os.path.isfile(model_path):
-                st_path = os.path.join(external_root, f"{tag}.safetensors")
-                if not os.path.isfile(st_path):
-                    raise FileNotFoundError(f"cannot find '{tag}'")
-                torch.save(load_file(st_path), model_path)
-
+    converted_path = os.path.join(external_root, f"{tag}_converted.pt")
+    if not os.path.isfile(converted_path):
+        f_size = None
+    else:
+        f_size = _get_file_size(converted_path)
+    v_size = sizes.get(tag)
+    if f_size is None or v_size != f_size:
+        if f_size is not None:
+            print(f"> '{tag}' has been converted but size mismatch")
+        print(f"> converting external weights '{tag}'")
+        model_path = os.path.join(external_root, f"{tag}.ckpt")
+        if not os.path.isfile(model_path):
+            st_path = os.path.join(external_root, f"{tag}.safetensors")
+            if not os.path.isfile(st_path):
+                raise FileNotFoundError(f"cannot find '{tag}'")
+            torch.save(load_file(st_path), model_path)
+        if convert_fn is not None:
+            d = convert_fn(model_path, m)
+        else:
             import cflearn
 
             d = cflearn.scripts.sd.convert(model_path, m, load=False)
-
-            torch.save(d, converted_path)
-            sizes[tag] = _get_file_size(converted_path)
-        with open(converted_sizes_path, "w") as f:
-            json.dump(sizes, f)
-        return converted_path
+        torch.save(d, converted_path)
+        sizes[tag] = _get_file_size(converted_path)
+        with lock:
+            with open(converted_sizes_path, "w") as f:
+                json.dump(sizes, f)
+    return converted_path
 
 
 class InpaintingMode(str, Enum):
     NORMAL = "normal"
     MASKED = "masked"
 
 
-TLtRb = Tuple[int, int, int, int]
-
-
 @dataclass
 class InpaintingSettings:
     mode: InpaintingMode = InpaintingMode.NORMAL
-    mask_blur: Optional[Union[int, Tuple[int, int]]] = None
-    mask_padding: Optional[Union[int, Tuple[int, int]]] = 32
+    mask_blur: TNumberPair = None
+    mask_padding: TNumberPair = 32
     mask_binary_threshold: Optional[int] = 32
+    target_wh: TNumberPair = None
+    padding_mode: Optional[str] = None
 
 
 class CropResponse(NamedTuple):
-    lt_rb: TLtRb
+    lt_rb: ImageBox
+    wh: Tuple[int, int]
     cropped_mask: np.ndarray
     resized_image_tensor: np.ndarray
     resized_mask_tensor: np.ndarray
 
 
-def get_mask_lt_rb(uint8_mask: np.ndarray, threshold: Optional[int]) -> TLtRb:
-    ys, xs = np.where(uint8_mask > (threshold or 0))
-    lt = xs.min().item(), ys.min().item()
-    rb = xs.max().item(), ys.max().item()
-    return *lt, *rb
-
-
-def crop_with(inp: np.ndarray, lt_rb: TLtRb) -> np.ndarray:
-    return inp[lt_rb[1] : lt_rb[3], lt_rb[0] : lt_rb[2]]
-
-
-def crop_tensor_with(inp: Tensor, lt_rb: TLtRb) -> Tensor:
-    return inp[..., lt_rb[1] : lt_rb[3], lt_rb[0] : lt_rb[2]]
-
-
 def resize(
     inp: np.ndarray,
     wh: Tuple[int, int],
-    interpolation: int = cv2.INTER_LANCZOS4,
+    interpolation: int = INTER_LANCZOS4,
 ) -> np.ndarray:
     return cv2.resize(inp, wh, interpolation=interpolation)
 
 
-def crop_masked_area(
-    image_tensor: np.ndarray,
-    mask_tensor: np.ndarray,
-    settings: InpaintingSettings,
-) -> CropResponse:
-    image = image_tensor[0].transpose(1, 2, 0)
-    mask = mask_tensor[0, 0]
-    h, w = image.shape[:2]
-    l, t, r, b = get_mask_lt_rb(to_uint8(mask), settings.mask_binary_threshold)
-    if settings.mask_padding is not None:
-        padding = settings.mask_padding
+def adjust_lt_rb(lt_rb: ImageBox, w: int, h: int, padding: TNumberPair) -> ImageBox:
+    l, t, r, b = lt_rb.tuple
+    if padding is not None:
         if isinstance(padding, int):
             padding = padding, padding
         l = max(0, l - padding[0])
         t = max(0, t - padding[1])
         r = min(w, r + padding[0])
         b = min(h, b + padding[1])
     cropped_h, cropped_w = b - t, r - l
@@ -323,53 +309,73 @@
             b = min(h, cropped_h + dh * 2)
         elif b + dh > h:
             b = h
             t = max(0, h - cropped_h - dh * 2)
         else:
             t -= dh
             b += dh
+    return ImageBox(l, t, r, b)
+
+
+def crop_masked_area(
+    image_tensor: np.ndarray,
+    mask_tensor: np.ndarray,
+    settings: InpaintingSettings,
+) -> CropResponse:
+    image = image_tensor[0].transpose(1, 2, 0)
+    mask = mask_tensor[0, 0]
+    h, w = image.shape[:2]
+    lt_rb = ImageBox.from_mask(to_uint8(mask), settings.mask_binary_threshold)
+    lt_rb = adjust_lt_rb(lt_rb, w, h, settings.mask_padding)
     # finalize
-    lt_rb = l, t, r, b
-    cropped_image = crop_with(image, lt_rb)
-    cropped_mask = crop_with(mask, lt_rb)
+    if settings.target_wh is not None:
+        if isinstance(settings.target_wh, int):
+            w = h = settings.target_wh
+        else:
+            w, h = settings.target_wh
+    cropped_image = lt_rb.crop(image)
+    cropped_mask = lt_rb.crop(mask)
     resized_image = resize(cropped_image, (w, h))
     resized_mask = resize(cropped_mask, (w, h), cv2.INTER_NEAREST)
     resized_image = resized_image.transpose(2, 0, 1)[None]
     resized_mask = resized_mask[None, None]
-    return CropResponse(lt_rb, cropped_mask, resized_image, resized_mask)
+    return CropResponse(lt_rb, (w, h), cropped_mask, resized_image, resized_mask)
 
 
 def normalize_image_to_diffusion(image: Image.Image) -> np.ndarray:
     return np.array(image).astype(np.float32) / 127.5 - 1.0
 
 
 def recover_with(
     original: Image.Image,
     sampled: Tensor,
     crop: CropResponse,
     wh_ratio: Tuple[float, float],
     settings: InpaintingSettings,
 ) -> Tensor:
-    l, t, r, b = crop.lt_rb
+    l, t, r, b = crop.lt_rb.tuple
     w_ratio, h_ratio = wh_ratio
     l = round(l * w_ratio)
     t = round(t * h_ratio)
     r = round(r * w_ratio)
     b = round(b * h_ratio)
     c_mask = crop.cropped_mask
     if settings.mask_padding is None:
         c_blurred_mask = c_mask
     else:
         blur = settings.mask_padding
         if isinstance(blur, int):
             blur = blur, blur
-        c_blurred_mask = cv2.blur(c_mask, blur)
+        if blur[0] > 0 and blur[1] > 0:
+            c_blurred_mask = cv2.blur(c_mask, blur)
+        else:
+            c_blurred_mask = c_mask
     sampled_array = sampled.numpy().transpose([0, 2, 3, 1])
     o_array = normalize_image_to_diffusion(to_rgb(original))
-    c_o_array = crop_with(o_array, (l, t, r, b))
+    c_o_array = ImageBox(l, t, r, b).crop(o_array)
     ch, cw = c_o_array.shape[:2]
     if ch != c_blurred_mask.shape[0] or cw != c_blurred_mask.shape[1]:
         c_blurred_mask = resize(c_blurred_mask, (cw, ch))
     c_blurred_mask = c_blurred_mask[..., None]
     mixed: List[np.ndarray] = []
     for i_sampled in sampled_array:
         i_sampled = resize(i_sampled, (cw, ch))
@@ -383,68 +389,66 @@
 def crop_controlnet(kwargs: Dict[str, Any], crop_res: Optional[CropResponse]) -> None:
     if crop_res is None:
         return
     hint: Optional[List[Tuple[str, Tensor]]] = kwargs.get(CONTROL_HINT_KEY, None)
     if hint is None:
         return
     for i, h in enumerate(hint):
-        h_h, h_w = h[1].shape[-2:]
-        h_tensor = crop_tensor_with(h[1], crop_res.lt_rb)
-        h_tensor = F.interpolate(h_tensor, (h_h, h_w), mode="bilinear")
+        hw, hh = crop_res.wh
+        h_tensor = crop_res.lt_rb.crop_tensor(h[1])
+        h_tensor = F.interpolate(h_tensor, (hh, hw), mode="bilinear")
         hint[i] = h[0], h_tensor
 
 
 class CroppedResponse(NamedTuple):
     image: np.ndarray
     mask: np.ndarray
     wh_ratio: Tuple[float, float]
     crop_res: Optional[CropResponse]
 
 
 def get_cropped(
     image_res: ReadImageResponse,
     mask_res: ReadImageResponse,
-    inpainting_settings: Optional[InpaintingSettings],
+    settings: Optional[InpaintingSettings],
 ) -> CroppedResponse:
     ow, oh = image_res.original_size
     ih, iw = image_res.image.shape[-2:]
     wh_ratio = ow / iw, oh / ih
-    if inpainting_settings is None or inpainting_settings.mode == InpaintingMode.NORMAL:
+    if settings is None or settings.mode == InpaintingMode.NORMAL:
         crop_res = None
         cropped_image = image_res.image
         cropped_mask = mask_res.image
-    elif inpainting_settings.mode == InpaintingMode.MASKED:
-        crop_res = crop_masked_area(
-            image_res.image,
-            mask_res.image,
-            inpainting_settings,
-        )
+    elif settings.mode == InpaintingMode.MASKED:
+        crop_res = crop_masked_area(image_res.image, mask_res.image, settings)
         cropped_image = crop_res.resized_image_tensor
         cropped_mask = crop_res.resized_mask_tensor
     else:
-        raise ValueError(f"Unknown inpainting mode: {inpainting_settings.mode}")
-    if inpainting_settings is not None:
-        if inpainting_settings.mask_blur is not None:
-            cropped_mask = cv2.blur(
-                cropped_mask[0][0],
-                (inpainting_settings.mask_blur, inpainting_settings.mask_blur),
-            )
-            cropped_mask = cropped_mask[None, None]
+        raise ValueError(f"Unknown inpainting mode: {settings.mode}")
+    if settings is not None:
+        if settings.mask_blur is not None:
+            blur = settings.mask_blur
+            if isinstance(blur, int):
+                blur = blur, blur
+            if blur[0] > 0 and blur[1] > 0:
+                cropped_mask = cv2.blur(cropped_mask[0][0], blur)
+                cropped_mask = cropped_mask[None, None]
     return CroppedResponse(cropped_image, cropped_mask, wh_ratio, crop_res)
 
 
 class DiffusionAPI(APIMixin):
     m: DDPM
     sampler: ISampler
     cond_model: Optional[nn.Module]
     first_stage: Optional[IAutoEncoder]
     latest_seed: int
     latest_variation_seed: Optional[int]
     sd_weights: WeightsPool
     current_sd_version: Optional[str]
+    _random_state: Optional[tuple] = None
 
     def __init__(
         self,
         m: DDPM,
         device: torch.device,
         *,
         use_amp: bool = False,
@@ -609,30 +613,34 @@
         original_size: Optional[Tuple[int, int]] = None,
         alpha: Optional[np.ndarray] = None,
         cond: Optional[Any] = None,
         cond_concat: Optional[Tensor] = None,
         unconditional_cond: Optional[Any] = None,
         hint: Optional[Union[Tensor, tensor_dict_type]] = None,
         hint_start: Optional[Union[float, Dict[str, float]]] = None,
+        hint_end: Optional[Union[float, Dict[str, float]]] = None,
         num_steps: Optional[int] = None,
         clip_output: bool = True,
         callback: Optional[Callable[[Tensor], Tensor]] = None,
         batch_size: Optional[int] = None,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
+        if self._random_state is None:
+            self._random_state = random.getstate()
         o_kw_backup = dict(
             seed=seed,
             variations=variations,
             alpha=alpha,
             cond=cond,
             cond_concat=cond_concat,
             unconditional_cond=unconditional_cond,
             hint=hint,
             hint_start=hint_start,
+            hint_end=hint_end,
             num_steps=num_steps,
             clip_output=clip_output,
             callback=callback,
             batch_size=batch_size,
             verbose=verbose,
         )
         if batch_size is None:
@@ -782,19 +790,21 @@
                             CROSS_ATTN_KEY: i_cond,
                             CONCAT_KEY: cond_concat,
                         }
                     if hint is not None:
                         if isinstance(i_cond, dict):
                             i_cond[CONTROL_HINT_KEY] = hint
                             i_cond[CONTROL_HINT_START_KEY] = hint_start
+                            i_cond[CONTROL_HINT_END_KEY] = hint_end
                         else:
                             i_cond = {
                                 CROSS_ATTN_KEY: i_cond,
                                 CONTROL_HINT_KEY: hint,
                                 CONTROL_HINT_START_KEY: hint_start,
+                                CONTROL_HINT_END_KEY: hint_end,
                             }
                     with switch_sampler_context(self, i_kw.get("sampler")):
                         if highres_info is not None:
                             # highres workaround
                             i_kw["return_latent"] = True
                         i_sampled = self.m.decode(i_z, cond=i_cond, **i_kw)
                         if highres_info is not None:
@@ -845,14 +855,17 @@
                     )
             concat = torch.cat([concat, alpha], dim=1)
         if export_path is not None:
             save_images(concat, export_path)
         self.empty_cuda_cache()
         if registered_custom:
             self.cond_model.clear_custom()
+        if self._random_state is not None:
+            random.setstate(self._random_state)
+            self._random_state = None
         return concat
 
     def txt2img(
         self,
         txt: Union[str, List[str]],
         export_path: Optional[str] = None,
         *,
@@ -902,43 +915,20 @@
         callback: Optional[Callable[[Tensor], Tensor]] = None,
         use_background_guidance: bool = False,
         use_reference: bool = False,
         reference_fidelity: float = 0.2,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
-        def get_z_ref_pack(
-            normalized_image_: np.ndarray,
-            normalized_mask_: np.ndarray,
-        ) -> Tuple[Tensor, Tensor, Tensor]:
-            z_ref = self._get_z(normalized_image_)
-            z_ref_mask = 1.0 - F.interpolate(
-                torch.from_numpy(normalized_mask_).to(z_ref),
-                z_ref.shape[-2:],
-                mode="bicubic",
-            )
-            if seed is not None:
-                seed_everything(seed)
-            z_ref_noise = torch.randn_like(z_ref)
-            return z_ref, z_ref_mask, z_ref_noise
-
         def get_z_info_from(
-            z_ref_: Optional[Tensor],
-            fidelity_: float,
-            shape_: Tuple[int, int],
+            z_ref_: Optional[Tensor], fidelity_: float, shape_: Tuple[int, int]
         ) -> Tuple[Optional[Tensor], Optional[Tuple[int, int]]]:
-            if z_ref_ is None:
-                z = None
-                size = tuple(map(lambda n: n * self.size_info.factor, shape_))
-            else:
-                size = None
-                args = z_ref_, num_steps, fidelity_, seed
-                z, _, start_step = self._q_sample(*args, **kwargs)
-                kwargs["start_step"] = start_step
-            return z, size  # type: ignore
+            return self._get_z_info_from(
+                z_ref_, fidelity_, shape_, seed, num_steps, kwargs
+            )
 
         def paste_original(
             original_: Image.Image,
             mask_: Image.Image,
             sampled_: Tensor,
         ) -> Tensor:
             rgb = to_rgb(original_)
@@ -951,18 +941,23 @@
 
         if inpainting_settings is None:
             inpainting_settings = InpaintingSettings()
         txt_list, num_samples = get_txt_cond(txt, num_samples)
 
         # raw inpainting
         if use_raw_inpainting:
-            image_res = read_image(image, max_wh, anchor=anchor)
+            image_res = read_image(
+                image,
+                max_wh,
+                anchor=anchor,
+                padding_mode=inpainting_settings.padding_mode,
+            )
             mask_res = read_image(mask, max_wh, anchor=anchor, to_mask=True)
             cropped_res = get_cropped(image_res, mask_res, inpainting_settings)
-            z_ref_pack = get_z_ref_pack(cropped_res.image, cropped_res.mask)
+            z_ref_pack = self._get_z_ref_pack(cropped_res.image, cropped_res.mask, seed)
             z_ref, z_ref_mask, z_ref_noise = z_ref_pack
             z, size = get_z_info_from(
                 z_ref if use_reference else None,
                 reference_fidelity,
                 z_ref.shape[-2:][::-1],
             )
             kw = shallow_copy_dict(kwargs)
@@ -1010,15 +1005,16 @@
         )
         # sampling
         with switch_sampler_context(self, kwargs.get("sampler")):
             # calculate `z_ref` stuffs based on `use_image_guidance`
             if not use_background_guidance:
                 z_ref = z_ref_mask = z_ref_noise = None
             else:
-                z_ref, z_ref_mask, z_ref_noise = get_z_ref_pack(res.image, res.mask)
+                z_ref_pack = self._get_z_ref_pack(res.image, res.mask, seed)
+                z_ref, z_ref_mask, z_ref_noise = z_ref_pack
             # calculate `z` based on `z_ref`, if needed
             z_shape = res.remained_image_cond.shape[-2:][::-1]
             if not use_reference:
                 args = None, reference_fidelity, z_shape
             elif z_ref is not None:
                 args = z_ref, reference_fidelity, z_shape
             else:
@@ -1489,14 +1485,50 @@
         z = img if isinstance(img, Tensor) else torch.from_numpy(img)
         if self.use_half:
             z = z.half()
         z = z.to(self.device)
         z = self.m._preprocess(z, deterministic=True)
         return z
 
+    def _get_z_ref_pack(
+        self,
+        image_tensor: np.ndarray,
+        mask_tensor: np.ndarray,
+        seed: Optional[int],
+    ) -> Tuple[Tensor, Tensor, Tensor]:
+        z_ref = self._get_z(image_tensor)
+        z_ref_mask = 1.0 - F.interpolate(
+            torch.from_numpy(mask_tensor).to(z_ref),
+            z_ref.shape[-2:],
+            mode="bicubic",
+        )
+        if seed is not None:
+            seed_everything(seed)
+        z_ref_noise = torch.randn_like(z_ref)
+        return z_ref, z_ref_mask, z_ref_noise
+
+    def _get_z_info_from(
+        self,
+        z_ref: Optional[Tensor],
+        fidelity: float,
+        shape: Tuple[int, int],
+        seed: Optional[int],
+        num_steps: Optional[int],
+        kwargs: Dict[str, Any],
+    ) -> Tuple[Optional[Tensor], Optional[Tuple[int, int]]]:
+        if z_ref is None:
+            z = None
+            size = tuple(map(lambda n: n * self.size_info.factor, shape))
+        else:
+            size = None
+            args = z_ref, num_steps, fidelity, seed
+            z, _, start_step = self._q_sample(*args, **kwargs)
+            kwargs["start_step"] = start_step
+        return z, size  # type: ignore
+
     def _get_identical_size_with(self, pivot: Tensor) -> Tuple[int, int]:
         return tuple(  # type: ignore
             map(
                 lambda n: n * self.size_info.factor,
                 pivot.shape[-2:][::-1],
             )
         )
@@ -1554,16 +1586,27 @@
         max_wh: int,
         anchor: int,
         mask_image_fn: Callable[[np.ndarray, np.ndarray], np.ndarray],
         mask_cond_fn: Callable[[np.ndarray], Tensor],
         inpainting_settings: Optional[InpaintingSettings] = None,
     ) -> MaskedCond:
         # handle mask stuffs
-        image_res = read_image(image, max_wh, anchor=anchor)
         mask_res = read_image(mask, max_wh, anchor=anchor, to_mask=True)
+        read_image_kw = {}
+        if inpainting_settings is not None:
+            if inpainting_settings.padding_mode is not None:
+                o_mask = mask_res.original
+                if o_mask.mode == "RGBA":
+                    padding_mask = o_mask.split()[-1]
+                else:
+                    padding_mask = o_mask.convert("L")
+                padding_mask.save("padding_mask_debug.png")
+                read_image_kw["padding_mask"] = padding_mask
+                read_image_kw["padding_mode"] = inpainting_settings.padding_mode
+        image_res = read_image(image, max_wh, anchor=anchor, **read_image_kw)
         cropped_res = get_cropped(image_res, mask_res, inpainting_settings)
         c_image = cropped_res.image
         c_mask = cropped_res.mask
         bool_mask = np.round(c_mask) >= 0.5
         remained_mask = (~bool_mask).astype(np.float16 if self.use_half else np.float32)
         remained_image = mask_image_fn(remained_mask, c_image)
         # construct condition tensor
@@ -1596,14 +1639,16 @@
         fidelity: float,
         seed: Optional[int],
         variations: Optional[List[Tuple[int, float]]] = None,
         variation_seed: Optional[int] = None,
         variation_strength: Optional[float] = None,
         **kwargs: Any,
     ) -> Tuple[Tensor, Tensor, int]:
+        if self._random_state is None:
+            self._random_state = random.getstate()
         if num_steps is None:
             num_steps = self.sampler.default_steps
         t = min(num_steps, round((1.0 - fidelity) * (num_steps + 1)))
         ts = get_timesteps(t, 1, z.device)
         if isinstance(self.sampler, (DDIMMixin, KSamplerMixin, DPMSolver)):
             kw = shallow_copy_dict(self.sampler.sample_kwargs)
             kw["total_step"] = num_steps
@@ -1699,140 +1744,69 @@
 
 
 class ControlNetHints(str, Enum):
     DEPTH = "depth"
     CANNY = "canny"
     POSE = "pose"
     MLSD = "mlsd"
-
-
-class Annotator(ABC):
-    @abstractmethod
-    def __init__(self, device: torch.device) -> None:
-        pass
-
-    @abstractmethod
-    def to(self: TAnnotator, device: torch.device, *, use_half: bool) -> TAnnotator:
-        pass
-
-    @abstractmethod
-    def annotate(self, uint8_rgb: np.ndarray, **kwargs: Any) -> np.ndarray:
-        pass
-
-
-class DepthAnnotator(Annotator):
-    def __init__(self, device: torch.device) -> None:
-        self.m = MiDaSAPI(device)
-
-    def to(self, device: torch.device, *, use_half: bool) -> "DepthAnnotator":
-        self.m.to(device, use_half=use_half)
-        return self
-
-    def annotate(self, uint8_rgb: np.ndarray) -> np.ndarray:  # type: ignore
-        return self.m.detect_depth(uint8_rgb)
-
-
-class CannyAnnotator(Annotator):
-    def __init__(self, device: torch.device) -> None:
-        if cv2 is None:
-            raise ValueError("`cv2` is needed for `CannyAnnotator`")
-
-    def to(self, device: torch.device, *, use_half: bool) -> "CannyAnnotator":
-        return self
-
-    def annotate(  # type: ignore
-        self,
-        uint8_rgb: np.ndarray,
-        *,
-        low_threshold: int,
-        high_threshold: int,
-    ) -> np.ndarray:
-        return cv2.Canny(uint8_rgb, low_threshold, high_threshold)
-
-
-class PoseAnnotator(Annotator):
-    def __init__(self, device: torch.device) -> None:
-        self.m = OpenposeDetector(device)
-
-    def to(self, device: torch.device, *, use_half: bool) -> "PoseAnnotator":
-        self.m.to(device, use_half=use_half)
-        return self
-
-    def annotate(self, uint8_rgb: np.ndarray) -> np.ndarray:  # type: ignore
-        return self.m(uint8_rgb)[0]
-
-
-class MLSDAnnotator(Annotator):
-    def __init__(self, device: torch.device) -> None:
-        self.m = MLSDDetector(device)
-
-    def to(self, device: torch.device, *, use_half: bool) -> "MLSDAnnotator":
-        self.m.to(device, use_half=use_half)
-        return self
-
-    def annotate(  # type: ignore
-        self,
-        uint8_rgb: np.ndarray,
-        *,
-        value_threshold: float,
-        distance_threshold: float,
-    ) -> np.ndarray:
-        return self.m(uint8_rgb, value_threshold, distance_threshold)
+    SOFTEDGE = "softedge"
 
 
 class ControlledDiffusionAPI(DiffusionAPI):
     loaded: Dict[ControlNetHints, bool]
-    annotators: Dict[ControlNetHints, Annotator]
+    annotators: Dict[Union[str, ControlNetHints], Annotator]
     base_sd_versions: Dict[ControlNetHints, str]
     controlnet_weights: Dict[ControlNetHints, tensor_dict_type]
+    controlnet_latest_usage: Dict[ControlNetHints, float]
 
-    control_defaults = {
+    control_mappings = {
         ControlNetHints.DEPTH: "ldm.sd_v1.5.control.diff.depth",
         ControlNetHints.CANNY: "ldm.sd_v1.5.control.diff.canny",
         ControlNetHints.POSE: "ldm.sd_v1.5.control.diff.pose",
         ControlNetHints.MLSD: "ldm.sd_v1.5.control.diff.mlsd",
     }
-    annotator_classes: Dict[ControlNetHints, Type[Annotator]] = {
-        ControlNetHints.DEPTH: DepthAnnotator,
-        ControlNetHints.CANNY: CannyAnnotator,
-        ControlNetHints.POSE: PoseAnnotator,
-        ControlNetHints.MLSD: MLSDAnnotator,
-    }
 
     def __init__(
         self,
         m: DDPM,
         device: torch.device,
         *,
         use_amp: bool = False,
         use_half: bool = False,
         clip_skip: int = 0,
         hint_channels: int = 3,
-        num_pool: int = 4,
+        num_pool: Optional[Union[str, int]] = "all",
         lazy: bool = False,
     ):
         super().__init__(
             m,
             device,
             use_amp=use_amp,
             use_half=use_half,
             clip_skip=clip_skip,
         )
-        pool = sorted(self.control_defaults)
-        selected_pool = pool[: min(num_pool, len(pool))]
+        default_cnet = sorted(self.control_mappings)[0]
         self.lazy = lazy
-        self.m.make_control_net({k: hint_channels for k in selected_pool}, lazy)
-        assert self.m.control_model is not None
+        if num_pool is None:
+            self.num_pool = None
+        else:
+            if num_pool == "all":
+                num_pool = len(ControlNetHints)
+            self.num_pool = num_pool if isinstance(num_pool, int) else None
+        self.hint_channels = hint_channels
+        self.m.make_control_net({default_cnet: hint_channels}, lazy)
+        assert isinstance(self.m.control_model, nn.ModuleDict)
+        self.control_model = self.m.control_model
         freeze(self.m.control_model)
-        self.loaded = {k: False for k in selected_pool}
+        self.loaded = {}
         self.annotators = {}
-        self.num_pool = num_pool
         self.control_model = self.m.control_model
         self.base_sd_versions = {}
         self.controlnet_weights = {}
+        self.controlnet_latest_usage = {}
 
     def to(
         self,
         device: torch.device,
         *,
         use_amp: bool = False,
         use_half: bool = False,
@@ -1840,73 +1814,133 @@
     ) -> None:
         super().to(device, use_amp=use_amp, use_half=use_half)
         if not no_annotator and not self.lazy:
             for annotator in self.annotators.values():
                 self._annotator_to(annotator)
 
     @property
+    def preset_control_hints(self) -> List[ControlNetHints]:
+        return list(self.control_mappings)
+
+    @property
     def available_control_hints(self) -> List[ControlNetHints]:
         return list(self.controlnet_weights)
 
     def set_tome_info(self, tome_info: Optional[Dict[str, Any]]) -> None:
         super().set_tome_info(tome_info)
         if self.control_model is not None:
             if isinstance(self.control_model, ControlNet):
                 self.control_model.set_tome_info(tome_info)
             else:
                 for m in self.control_model.values():
                     m.set_tome_info(tome_info)
 
     def prepare_control(self, hints2tags: Dict[ControlNetHints, str]) -> None:
         root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
+        any_new = False
         for hint, tag in hints2tags.items():
-            self.controlnet_weights[hint] = torch.load(download_model(tag, root=root))
-
-    def prepare_control_defaults(self) -> None:
-        self.prepare_control(self.control_defaults)
+            if hint not in self.control_model:
+                any_new = True
+                self.m.make_control_net(self.hint_channels, self.lazy, target_key=hint)
+            if hint not in self.controlnet_weights:
+                try:
+                    d = torch.load(download_model(tag, root=root))
+                except:
+
+                    def fn(p: str, m: ControlledDiffusionAPI) -> tensor_dict_type:
+                        import cflearn
+
+                        return cflearn.scripts.sd.convert_controlnet(p)
+
+                    p = _convert_external(self, tag, "controlnet", convert_fn=fn)
+                    d = torch.load(p)
+                self.loaded[hint] = False
+                self.controlnet_weights[hint] = d
+            elif hint not in self.loaded:
+                self.loaded[hint] = False
+        if any_new:
+            freeze(self.m.control_model)
+
+    def remove_control(self, hints: List[ControlNetHints]) -> None:
+        for hint in hints:
+            if hint in self.loaded:
+                del self.loaded[hint]
+            if hint in self.controlnet_weights:
+                del self.controlnet_weights[hint]
+            if hint in self.controlnet_latest_usage:
+                del self.controlnet_latest_usage[hint]
+            if hint in self.control_model:
+                m = self.control_model.pop(hint)
+                m.to("cpu")
+                del m
+            if hint in self.base_sd_versions:
+                del self.base_sd_versions[hint]
 
     def switch_control(
         self,
         *hints: ControlNetHints,
         base_md: Optional[tensor_dict_type] = None,
     ) -> None:
         if self.m.control_model is None:
             raise ValueError("`control_model` is not built yet")
 
-        hints_list = list(hints)
-        if len(hints_list) > self.num_pool:
-            print_warning(
-                f"number of target hints ({len(hints_list)}) exceeds "
-                f"number of pool ({self.num_pool}), "
-                f"so only {self.num_pool} hints will be activated"
-            )
-            random.shuffle(hints_list)
-            hints_list = hints_list[: self.num_pool]
+        for hint in hints:
+            self.controlnet_latest_usage[hint] = time.time()
 
-        target = set(hints_list)
-        current = set(self.loaded)
-        not_current = sorted(target - current)
-        if not_current:
-            not_target = sorted(current - target)
-            for i, i_not_current in enumerate(not_current):
-                pop_key = not_target[i]
-                self.m.rename_control_net(pop_key, i_not_current)
-                self.loaded[i_not_current] = False
-                self.loaded.pop(pop_key)
+        target = set(hints)
+        # if `hint` does not exist in `control_mappings`, it means it is an
+        # external controlnet, so it should be left as-is
+        target_mapping = {h: self.control_mappings.get(h, h) for h in target}
+        self.prepare_control(target_mapping)
+
+        current = set(self.control_model.keys())
+        if self.num_pool is None or len(current) > self.num_pool:
+            to_remove = list(current - target)
+            if to_remove:
+                if self.num_pool is None:
+                    print_warning(
+                        "`num_pool` is set to `None`, redundant controlnets "
+                        f"({to_remove}) will be removed"
+                    )
+                    self.remove_control(to_remove)
+                else:
+                    usages = [self.controlnet_latest_usage.get(h, 0) for h in to_remove]
+                    sorted_indices = np.argsort(usages)
+                    diff = len(current) - self.num_pool
+                    remove_indices = sorted_indices[:diff]
+                    to_remove = [to_remove[i] for i in remove_indices]
+                    print_warning(
+                        "current number of controlnets exceeds `num_pool` "
+                        f"({self.num_pool}), {to_remove} will be removed"
+                    )
+                    self.remove_control(to_remove)
 
         sorted_target = sorted(target)
         loaded_list = [self.loaded[hint] for hint in sorted_target]
         base_list = [self.base_sd_versions.get(hint) for hint in sorted_target]
+        if base_md is None:
+            base_md_id = None
+        else:
+            base_md_id = str(id(base_md))
         need_offset_list = [
             base is None
-            or self.current_sd_version is None
-            or base_md is not None
-            or get_sd_tag(base) != get_sd_tag(self.current_sd_version)
+            or (base_md is not None and base != base_md_id)
+            or (
+                base_md is None
+                and (
+                    self.current_sd_version is None
+                    or get_sd_tag(base) != get_sd_tag(self.current_sd_version)
+                )
+            )
             for base in base_list
         ]
+        for i, hint in enumerate(sorted_target):
+            # external controlnets should not offset
+            if hint == target_mapping[hint]:
+                need_offset_list[i] = False
         if all(loaded_list) and not any(need_offset_list):
             return
         iterator = zip(loaded_list, sorted_target, need_offset_list)
         for loaded, hint, need_offset in iterator:
             if loaded and not need_offset:
                 continue
             d = self.controlnet_weights.get(hint)
@@ -1915,51 +1949,47 @@
                     f"cannot find ControlNet weights called '{hint}', "
                     f"available weights are: {', '.join(self.available_control_hints)}"
                 )
             if need_offset:
                 d = offset_cnet_weights(d, api=self, base_md=base_md)
             self.m.load_control_net_with(hint, d)
             self.loaded[hint] = True
-            # if `base_md` is provided, should reset cache settings
-            if base_md is not None:
-                self.base_sd_versions.pop(hint, None)
+            if base_md_id is not None:
+                self.base_sd_versions[hint] = base_md_id
             else:
                 if self.current_sd_version is not None:
                     self.base_sd_versions[hint] = self.current_sd_version
 
-    def prepare_annotator(self, hint: ControlNetHints) -> None:
+    def prepare_annotator(self, hint: Union[str, ControlNetHints]) -> None:
         if hint not in self.annotators:
-            annotator_class = self.annotator_classes.get(hint)
+            annotator_class = annotators.get(hint)
             if annotator_class is None:
-                raise ValueError(f"annotator for '{hint}' is not implemented")
+                print_warning(f"annotator '{hint}' is not implemented")
+                return
             if self.lazy:
                 annotator = annotator_class("cpu")
             else:
                 annotator = annotator_class(self.device)
                 self._annotator_to(annotator)
             self.annotators[hint] = annotator
 
     def prepare_annotators(self) -> None:
-        for hint in self.controlnet_weights:
+        for hint in ControlNetHints:
             self.prepare_annotator(hint)
 
     def get_hint_of(
         self,
-        hint: ControlNetHints,
+        hint: Union[str, ControlNetHints],
         uint8_rgb: np.ndarray,
         **kwargs: Any,
     ) -> np.ndarray:
-        if not self.loaded.get(hint):
-            raise ValueError(f"'{hint}' is not loaded yet, please call `switch` first.")
+        self.prepare_annotator(hint)
         annotator = self.annotators.get(hint)
         if annotator is None:
-            raise ValueError(
-                f"annotator for '{hint}' is not prepared yet, "
-                "please call `prepare_annotator`/`prepare_annotators` first."
-            )
+            return uint8_rgb
         if self.lazy:
             self._annotator_to(annotator)
         kwargs["uint8_rgb"] = uint8_rgb
         out = safe_execute(annotator.annotate, kwargs)
         if len(out.shape) == 2:
             out = out[..., None]
         if out.shape[-1] == 1:
```

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/blip.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/blip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/api.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/predictor.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/transforms.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/inference/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/base.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/mconfigs/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/dih_model.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/dih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/unet.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/modeling/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/ops.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/iharm/model/ops.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/isnet.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/isnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/lama.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/lama.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/api.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/blocks.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/dpt_depth.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/midas_net.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net_custom.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/transforms.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/vit.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/core/vit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/utils.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/midas/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/api.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/utils.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/api.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/body.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/body.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/hand.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/model.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/util.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/openpose/util.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/third_party/prompt.py` & `carefree-learn-0.4.6/cflearn/api/cv/third_party/prompt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/cv/translator.py` & `carefree-learn-0.4.6/cflearn/api/cv/translator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/ml/ddr.py` & `carefree-learn-0.4.6/cflearn/api/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/schema.py` & `carefree-learn-0.4.6/cflearn/api/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/api/utils.py` & `carefree-learn-0.4.6/cflearn/api/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,27 @@
             use_amp=use_amp,
             use_half=use_half,
             **kwargs,
         )
 
 
 class Weights(ILoadableItem[tensor_dict_type]):
-    def __init__(self, path: str, *, init: bool = False):
-        super().__init__(lambda: torch.load(path), init=init)
+    def __init__(
+        self,
+        path: str,
+        *,
+        init: bool = False,
+        force_keep: bool = False,
+    ):
+        super().__init__(lambda: torch.load(path), init=init, force_keep=force_keep)
 
 
 class WeightsPool(ILoadablePool[tensor_dict_type]):
-    def register(self, key: str, path: str) -> None:  # type: ignore
-        super().register(key, lambda init: Weights(path, init=init))
+    def register(
+        self,
+        key: str,
+        path: str,
+        *,
+        force_keep: bool = False,
+    ) -> None:  # type: ignore
+        init_fn = lambda init: Weights(path, init=init, force_keep=force_keep)
+        super().register(key, init_fn)
```

### Comparing `carefree-learn-0.4.5/cflearn/api/zoo/__init__.py` & `carefree-learn-0.4.6/cflearn/api/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/callbacks/classification.py` & `carefree-learn-0.4.6/cflearn/callbacks/classification.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/callbacks/general.py` & `carefree-learn-0.4.6/cflearn/callbacks/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 from ..constants import SCORES_FILE
 
 try:
     import mlflow
     from mlflow.exceptions import MlflowException
     from mlflow.utils.mlflow_tags import MLFLOW_USER
     from mlflow.utils.mlflow_tags import MLFLOW_RUN_NAME
-    from mlflow.tracking.fluent import _RUN_ID_ENV_VAR
+    from mlflow.environment_variables import MLFLOW_RUN_ID
 except:
     mlflow = None
     MlflowException = None
     MLFLOW_USER = None
     MLFLOW_RUN_NAME = None
-    _RUN_ID_ENV_VAR = None
+    MLFLOW_RUN_ID = None
 
 
 def parse_mlflow_uri(path: str) -> str:
     delim = "/" if platform.system() == "Windows" else ""
     return f"file://{delim}{path}"
 
 
@@ -144,17 +144,16 @@
                 experiment_id = experiment.experiment_id
             else:
                 experiment_id = self.mlflow_client.create_experiment(name)
             lock._stuffs = [os.path.join(tracking_dir, experiment_id)]
 
         run = None
         from_external = False
-        if _RUN_ID_ENV_VAR in os.environ:
-            existing_run_id = os.environ[_RUN_ID_ENV_VAR]
-            del os.environ[_RUN_ID_ENV_VAR]
+        if existing_run_id := MLFLOW_RUN_ID.get():
+            del os.environ[MLFLOW_RUN_ID.name]
             try:
                 run = self.mlflow_client.get_run(existing_run_id)
                 from_external = True
             except MlflowException:
                 print_warning(
                     "`run_id` is found in environment but "
                     "corresponding mlflow run does not exist. This might cause by "
```

### Comparing `carefree-learn-0.4.5/cflearn/callbacks/generator.py` & `carefree-learn-0.4.6/cflearn/callbacks/generator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/constants.py` & `carefree-learn-0.4.6/cflearn/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/array.py` & `carefree-learn-0.4.6/cflearn/data/array.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/cv/crop.py` & `carefree-learn-0.4.6/cflearn/data/blocks/cv/crop.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/cv/image_folder.py` & `carefree-learn-0.4.6/cflearn/data/blocks/cv/image_folder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/cv/normalize.py` & `carefree-learn-0.4.6/cflearn/data/blocks/cv/normalize.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/cv/to_numpy.py` & `carefree-learn-0.4.6/cflearn/data/blocks/cv/to_numpy.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/cv/tuple_to_batch.py` & `carefree-learn-0.4.6/cflearn/data/blocks/cv/tuple_to_batch.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/ml/file.py` & `carefree-learn-0.4.6/cflearn/data/blocks/ml/file.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/ml/gather.py` & `carefree-learn-0.4.6/cflearn/data/blocks/ml/gather.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/ml/nan_handler.py` & `carefree-learn-0.4.6/cflearn/data/blocks/ml/nan_handler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/ml/preprocessor.py` & `carefree-learn-0.4.6/cflearn/data/blocks/ml/preprocessor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/ml/recognizer.py` & `carefree-learn-0.4.6/cflearn/data/blocks/ml/recognizer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/blocks/ml/splitter.py` & `carefree-learn-0.4.6/cflearn/data/blocks/ml/splitter.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/ml/api.py` & `carefree-learn-0.4.6/cflearn/data/ml/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/ml/datasets.py` & `carefree-learn-0.4.6/cflearn/data/ml/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/pytorch/api.py` & `carefree-learn-0.4.6/cflearn/data/pytorch/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/pytorch/datasets.py` & `carefree-learn-0.4.6/cflearn/data/pytorch/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/data/utils.py` & `carefree-learn-0.4.6/cflearn/data/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/dist/ml/experiment.py` & `carefree-learn-0.4.6/cflearn/dist/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/dist/ml/runs/_utils.py` & `carefree-learn-0.4.6/cflearn/dist/ml/runs/_utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/dist/ml/task.py` & `carefree-learn-0.4.6/cflearn/dist/ml/task.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/inference.py` & `carefree-learn-0.4.6/cflearn/inference.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/losses/basic.py` & `carefree-learn-0.4.6/cflearn/losses/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/losses/gan.py` & `carefree-learn-0.4.6/cflearn/losses/gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/losses/lpips.py` & `carefree-learn-0.4.6/cflearn/losses/lpips.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/losses/vae.py` & `carefree-learn-0.4.6/cflearn/losses/vae.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/metrics.py` & `carefree-learn-0.4.6/cflearn/metrics.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/misc/available.json` & `carefree-learn-0.4.6/cflearn/misc/available.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/misc/mixins.py` & `carefree-learn-0.4.6/cflearn/misc/mixins.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/misc/toolkit.py` & `carefree-learn-0.4.6/cflearn/misc/toolkit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/bases.py` & `carefree-learn-0.4.6/cflearn/models/bases.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/ae/common.py` & `carefree-learn-0.4.6/cflearn/models/cv/ae/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/ae/kl.py` & `carefree-learn-0.4.6/cflearn/models/cv/ae/kl.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/ae/vq.py` & `carefree-learn-0.4.6/cflearn/models/cv/ae/vq.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/classifier/vanilla.py` & `carefree-learn-0.4.6/cflearn/models/cv/classifier/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/decoder/attn.py` & `carefree-learn-0.4.6/cflearn/models/cv/decoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/decoder/schema.py` & `carefree-learn-0.4.6/cflearn/models/cv/decoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan.py` & `carefree-learn-0.4.6/cflearn/models/cv/decoder/style_gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan_v2.py` & `carefree-learn-0.4.6/cflearn/models/cv/decoder/style_gan_v2.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/decoder/vanilla.py` & `carefree-learn-0.4.6/cflearn/models/cv/decoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/decoder/vqgan.py` & `carefree-learn-0.4.6/cflearn/models/cv/decoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/clip.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,16 @@
         return self.m.token_embedding.weight.data
 
     def register_custom(self, embeddings: Dict[str, List[List[float]]]) -> None:
         existing = self.embeddings
         dtype = existing.dtype
         device = existing.device
         for name, embedding in embeddings.items():
+            if embedding is None:
+                continue
             tensor = torch.asarray(embedding, dtype=dtype, device=device)
             embedding_dim = self.embeddings.shape[1]
             if tensor.shape[1] != embedding_dim:
                 raise ValueError(
                     f"dimension of the custom embedding '{name}' is not correct "
                     f"(expected {embedding_dim}, got {tensor.shape[1]})"
                 )
```

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/rescaler.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/rescaler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/schema.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/cond_models/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/ddpm.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/ddpm.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .utils import ADM_TYPE
 from .utils import CONCAT_KEY
 from .utils import CONCAT_TYPE
 from .utils import HYBRID_TYPE
 from .utils import CROSS_ATTN_KEY
 from .utils import CROSS_ATTN_TYPE
 from .utils import CONTROL_HINT_KEY
+from .utils import CONTROL_HINT_END_KEY
 from .utils import CONTROL_HINT_START_KEY
 from .samplers import is_misc_key
 from .samplers import ISampler
 from .samplers import DDPMQSampler
 from .cond_models import condition_models
 from .cond_models import specialized_condition_models
 from ...schemas import CustomTrainStep
@@ -496,23 +497,27 @@
             else:
                 raise ValueError(f"unrecognized condition type {cond_type} occurred")
         if self.control_model is not None:
             if not isinstance(cond, dict):
                 raise ValueError("`cond` should be a dict when `control_model` is used")
             hint = cond.get(CONTROL_HINT_KEY)
             hint_start = cond.get(CONTROL_HINT_START_KEY)
+            hint_end = cond.get(CONTROL_HINT_END_KEY)
             check_hint_start = lambda start: start is None or start * total_step <= step
+            check_hint_end = lambda end: end is None or end * total_step >= step
             if hint is None:
                 raise ValueError("`hint` should be provided for `control_model`")
             if isinstance(self.control_model, ControlNet):
                 if not isinstance(hint, Tensor):
                     raise ValueError("`hint` should be a Tensor for single control")
-                if hint_start is not None and isinstance(hint_start, dict):
+                if hint_start is not None and isinstance(hint_start, list):
                     raise ValueError("`hint_start` should be float for single control")
-                if not check_hint_start(hint_start):
+                if hint_end is not None and isinstance(hint_end, list):
+                    raise ValueError("`hint_end` should be float for single control")
+                if not check_hint_start(hint_start) or not check_hint_end(hint_end):
                     ctrl = None
                 else:
                     ctrl = self.control_model(net, hint, timesteps=timesteps, **cond_kw)
                     if self.control_scales is None:
                         scales = [1.0] * self.num_control_scales
                     else:
                         if isinstance(self.control_scales[0], list):
@@ -520,23 +525,27 @@
                         scales = self.control_scales  # type: ignore
                     ctrl = [c * scale for c, scale in zip(ctrl, scales)]
             else:
                 if not isinstance(hint, list):
                     raise ValueError("`hint` should be a list for control settings")
                 if not isinstance(hint_start, list):
                     raise ValueError("`hint_start` should be a list of Optional[float]")
+                if not isinstance(hint_end, list):
+                    raise ValueError("`hint_end` should be a list of Optional[float]")
                 target_keys = set(self.control_model.keys())
                 hint_types = set(pair[0] for pair in hint)
                 if hint_types - target_keys:
                     msg = f"`hint` ({hint_types}) should not exceed following keys: {', '.join(sorted(target_keys))}"
                     raise ValueError(msg)
                 ctrl = [0.0] * self.num_control_scales
                 any_activated = False
-                for i, ((i_type, i_hint), i_start) in enumerate(zip(hint, hint_start)):
-                    if not check_hint_start(i_start):
+                for i, ((i_type, i_hint), i_start, i_end) in enumerate(
+                    zip(hint, hint_start, hint_end)
+                ):
+                    if not check_hint_start(i_start) or not check_hint_end(i_end):
                         continue
                     any_activated = True
                     i_cmodel = self.control_model[i_type]
                     # inpainting workaround
                     if i_cmodel.in_channels == net.shape[1]:
                         cnet = net
                     else:
@@ -580,31 +589,44 @@
             - extract_to(self.sqrt_one_minus_alphas_cumprod, ts, num_dim) * v
         )
 
     def make_control_net(
         self,
         hint_channels: Union[int, Dict[str, int]],
         lazy: bool = False,
+        *,
+        target_key: Optional[str] = None,
     ) -> None:
         def _make(n: int) -> ControlNet:
             # temporarily make inpainting compatible
             kw = shallow_copy_dict(self.unet_kw)
             kw["in_channels"] = 4
             return ControlNet(hint_channels=n, **kw)  # type: ignore
 
-        self.control_model_lazy = lazy
-        if isinstance(hint_channels, int):
-            self.control_model = _make(hint_channels)
+        if target_key is not None:
+            if not isinstance(self.control_model, nn.ModuleDict):
+                msg = "`target_key` can only be used in multi `ControlNet`"
+                raise ValueError(msg)
+            if not isinstance(hint_channels, int):
+                msg = "`hint_channels` should be int when `target_key` is used"
+                raise ValueError(msg)
+            if target_key not in self.control_model:
+                self.control_model[target_key] = _make(hint_channels)
         else:
-            self.control_model = nn.ModuleDict(
-                {
-                    key: _make(key_channels)
-                    for key, key_channels in hint_channels.items()
-                }
-            )
+            if isinstance(hint_channels, int):
+                self.control_model = _make(hint_channels)
+            else:
+                self.control_model = nn.ModuleDict(
+                    {
+                        key: _make(key_channels)
+                        for key, key_channels in hint_channels.items()
+                    }
+                )
+
+        self.control_model_lazy = lazy
         if not lazy:
             self._control_model_to()
 
     def rename_control_net(self, old: str, new: str) -> None:
         if not isinstance(self.control_model, nn.ModuleDict):
             msg = "`rename_control_net` is only available when multiple `ControlNet` are used"
             raise ValueError(msg)
@@ -647,14 +669,15 @@
             def __enter__(self) -> None:
                 if self.m is not None and self.lazy:
                     self.to()
 
             def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
                 if self.m is not None and self.lazy:
                     self.to("cpu")
+                    torch.cuda.empty_cache()
 
         return _(self)
 
     def _q_sample(
         self,
         net: Tensor,
         timesteps: Tensor,
```

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/ldm.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/ldm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/basic.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/ddim.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/ddim.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/k_samplers.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/k_samplers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/plms.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/plms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/schema.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,28 @@
 from cftool.misc import WithRegister
 
 from ..utils import cond_type
 from ..utils import extract_to
 from ..utils import get_timesteps
 from ..utils import CONCAT_KEY
 from ..utils import CONTROL_HINT_KEY
+from ..utils import CONTROL_HINT_END_KEY
 from ..utils import CONTROL_HINT_START_KEY
 
 
 samplers: Dict[str, Type["ISampler"]] = {}
 
 
 def is_misc_key(key: str) -> bool:
-    return key in (CONCAT_KEY, CONTROL_HINT_KEY, CONTROL_HINT_START_KEY)
+    return key in (
+        CONCAT_KEY,
+        CONTROL_HINT_KEY,
+        CONTROL_HINT_START_KEY,
+        CONTROL_HINT_END_KEY,
+    )
 
 
 class Denoise(Protocol):
     def __call__(
         self,
         image: Tensor,
         timesteps: Tensor,
```

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/solver.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/solver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/utils.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/unet.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/diffusion/utils.py` & `carefree-learn-0.4.6/cflearn/models/cv/diffusion/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 CONCAT_KEY = "concat"
 CONCAT_TYPE = "concat"
 HYBRID_TYPE = "hybrid"
 CROSS_ATTN_KEY = "context"
 CROSS_ATTN_TYPE = "cross_attn"
 CONTROL_HINT_KEY = "hint"
 CONTROL_HINT_START_KEY = "hint_start"
+CONTROL_HINT_END_KEY = "hint_end"
 
 
 def extract_to(array: Tensor, indices: Tensor, num_dim: int) -> Tensor:
     b = indices.shape[0]
     out = array.gather(-1, indices).contiguous()
     return out.view(b, *([1] * (num_dim - 1)))
```

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/attn.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/api.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/core.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/resnet.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/transformer.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/vgg.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/models/vgg.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/register.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/backbone/register.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/fnet.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/fnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/mixer.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/mixer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/perceiver.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/pool_former.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/pool_former.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/schema.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/transformer.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/vanilla.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/encoder/vqgan.py` & `carefree-learn-0.4.6/cflearn/models/cv/encoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/gan/discriminators.py` & `carefree-learn-0.4.6/cflearn/models/cv/gan/discriminators.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/gan/schema.py` & `carefree-learn-0.4.6/cflearn/models/cv/gan/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/gan/vanilla.py` & `carefree-learn-0.4.6/cflearn/models/cv/gan/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/general.py` & `carefree-learn-0.4.6/cflearn/models/cv/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/cv/translator/rrdb.py` & `carefree-learn-0.4.6/cflearn/models/cv/translator/rrdb.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/implicit/siren.py` & `carefree-learn-0.4.6/cflearn/models/implicit/siren.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/base.py` & `carefree-learn-0.4.6/cflearn/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/ddr.py` & `carefree-learn-0.4.6/cflearn/models/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/encoders.py` & `carefree-learn-0.4.6/cflearn/models/ml/encoders.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/fcnn.py` & `carefree-learn-0.4.6/cflearn/models/ml/fcnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/linear.py` & `carefree-learn-0.4.6/cflearn/models/ml/linear.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/mixed_stacked.py` & `carefree-learn-0.4.6/cflearn/models/ml/mixed_stacked.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/nbm.py` & `carefree-learn-0.4.6/cflearn/models/ml/nbm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/ndt.py` & `carefree-learn-0.4.6/cflearn/models/ml/ndt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/rnn.py` & `carefree-learn-0.4.6/cflearn/models/ml/rnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/ml/wnd.py` & `carefree-learn-0.4.6/cflearn/models/ml/wnd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/multimodal/clip.py` & `carefree-learn-0.4.6/cflearn/models/multimodal/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/multimodal/schema.py` & `carefree-learn-0.4.6/cflearn/models/multimodal/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/nlp/encoder/transformer.py` & `carefree-learn-0.4.6/cflearn/models/nlp/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/clip.py` & `carefree-learn-0.4.6/cflearn/models/nlp/tokenizers/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/schema.py` & `carefree-learn-0.4.6/cflearn/models/nlp/tokenizers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/nlp/transformers/core.py` & `carefree-learn-0.4.6/cflearn/models/nlp/transformers/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/nlp/transformers/opus.py` & `carefree-learn-0.4.6/cflearn/models/nlp/transformers/opus.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/nlp/transformers/simbert.py` & `carefree-learn-0.4.6/cflearn/models/nlp/transformers/simbert.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/schemas/custom.py` & `carefree-learn-0.4.6/cflearn/models/schemas/custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/models/schemas/cv.py` & `carefree-learn-0.4.6/cflearn/models/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/__init__.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/activations.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/activations.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/attentions.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/attentions.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/common.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/convs/basic.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/convs/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/convs/residual.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/convs/residual.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/customs.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/customs.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/high_level.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/high_level.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/hijacks.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/hijacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,23 +130,23 @@
         else:
             updown = (up[..., 0, 0] @ down[..., 0, 0])[..., None, None]
         updown = self.scale * self.alpha_scale * updown
         return updown
 
     def before_forward(self, inp: Tensor, index: Optional[int] = None) -> Tensor:
         if not self.injected:
+            self.to(self.m.weight)
             weight = self.m.weight
             updown = self.get_updown()
             self.inject(weight, updown, index)
         return inp
 
     @classmethod
     def create_with(cls, m: IBasicHijackMixin, rank: int) -> "ILoRAMappingHook":
         self = cls(*m.args, rank=rank, **m.kwargs)
-        self.to(m.weight)
         self._ms = [m]
         return self
 
 
 class LoRALinearHook(ILoRAMappingHook):
     def __init__(
         self,
@@ -254,14 +254,16 @@
         self.to_v.set_scale(scale)
         self.injected = False
 
     def before_forward(self, inp: Tensor, index: Optional[int] = None) -> Tensor:
         if not self.injected:
             in_w = self.m.in_w
             hooks = [self.to_q, self.to_k, self.to_v]
+            for h in hooks:
+                h.to(in_w)
             updown = torch.vstack([h.get_updown() for h in hooks])
             assert in_w is not None, "should be self_attn in lora"
             self.inject(in_w, updown, index)
         return inp
 
     @classmethod
     def create_with(cls, m: IAttention, rank: int) -> "LoRAAttentionHook":
```

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/hooks.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/hooks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/implementations/perceiver.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/implementations/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/mappings.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/mappings.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/api.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/channel_mixers.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/channel_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/poolers.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/poolers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/schema.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/token_mixers.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/mixed_stacks/token_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/norms.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/norms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/blocks/utils.py` & `carefree-learn-0.4.6/cflearn/modules/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/optimizers.py` & `carefree-learn-0.4.6/cflearn/modules/optimizers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/modules/schedulers.py` & `carefree-learn-0.4.6/cflearn/modules/schedulers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/monitors.py` & `carefree-learn-0.4.6/cflearn/monitors.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/parameters.py` & `carefree-learn-0.4.6/cflearn/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/pipeline/api.py` & `carefree-learn-0.4.6/cflearn/pipeline/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/pipeline/blocks/basic.py` & `carefree-learn-0.4.6/cflearn/pipeline/blocks/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/pipeline/blocks/ml.py` & `carefree-learn-0.4.6/cflearn/pipeline/blocks/ml.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/pipeline/blocks/utils.py` & `carefree-learn-0.4.6/cflearn/pipeline/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/pipeline/core.py` & `carefree-learn-0.4.6/cflearn/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/pipeline/third_party.py` & `carefree-learn-0.4.6/cflearn/pipeline/third_party.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/schema.py` & `carefree-learn-0.4.6/cflearn/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/scripts/sd.py` & `carefree-learn-0.4.6/cflearn/scripts/sd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/trainer.py` & `carefree-learn-0.4.6/cflearn/trainer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/types.py` & `carefree-learn-0.4.6/cflearn/types.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f4.json` & `carefree-learn-0.4.6/cflearn/zoo/configs/ae/kl/f4.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ddpm/default.json` & `carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ddpm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/default.json` & `carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/vq.json` & `carefree-learn-0.4.6/cflearn/zoo/configs/diffusion/ldm/vq.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/chinese.json` & `carefree-learn-0.4.6/cflearn/zoo/configs/multimodal/clip/chinese.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/core.py` & `carefree-learn-0.4.6/cflearn/zoo/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/cflearn/zoo/models/clip.py` & `carefree-learn-0.4.6/cflearn/zoo/models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.5/setup.py` & `carefree-learn-0.4.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.4.5"
+VERSION = "0.4.6"
 DESCRIPTION = "Deep Learning with PyTorch made easy"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 cv_requires = [
     "ftfy",
     "lmdb",
@@ -33,30 +33,30 @@
     name="carefree-learn",
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     install_requires=[
         "filelock",
         "accelerate",
         "safetensors",
-        "carefree-toolkit>=0.3.5",
+        "carefree-toolkit>=0.3.7",
     ],
     extras_require={
         "onnx": onnx_requires,
         "cv": cv_requires,
         "cv_full": cv_full_requires,
         "full": cv_full_requires
         + onnx_requires
         + [
             "open_clip_torch",
             "faiss-cpu",
             "protobuf==3.19.4",
             "ortools>=9.3.0",
             "sacremoses",
             "sentencepiece",
-            "mlflow",
+            "mlflow>=2.5.0",
             "plotly",
         ],
     },
     author="carefree0910",
     author_email="syameimaru.saki@gmail.com",
     url="https://github.com/carefree0910/carefree-learn",
     download_url=f"https://github.com/carefree0910/carefree-learn/archive/v{VERSION}.tar.gz",
```

