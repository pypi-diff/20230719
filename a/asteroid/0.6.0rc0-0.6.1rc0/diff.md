# Comparing `tmp/asteroid-0.6.0rc0.tar.gz` & `tmp/asteroid-0.6.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asteroid-0.6.0rc0.tar", last modified: Tue Jun 28 15:03:37 2022, max compression
+gzip compressed data, was "asteroid-0.6.1rc0.tar", last modified: Wed Jul 19 11:26:18 2023, max compression
```

## Comparing `asteroid-0.6.0rc0.tar` & `asteroid-0.6.1rc0.tar`

### file list

```diff
@@ -1,106 +1,103 @@
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.564834 asteroid-0.6.0rc0/
--rw-r--r--   0 mparient (661056) incub    (200102)     1072 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/LICENSE
--rw-r--r--   0 mparient (661056) incub    (200102)       86 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/MANIFEST.in
--rw-r--r--   0 mparient (661056) incub    (200102)    10578 2022-06-28 15:03:37.564834 asteroid-0.6.0rc0/PKG-INFO
--rw-r--r--   0 mparient (661056) incub    (200102)     9893 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/README.md
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.555834 asteroid-0.6.0rc0/asteroid/
--rw-r--r--   0 mparient (661056) incub    (200102)      687 2022-06-28 15:02:58.000000 asteroid-0.6.0rc0/asteroid/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6954 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/binarize.py
--rw-r--r--   0 mparient (661056) incub    (200102)     7493 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/complex_nn.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.558834 asteroid-0.6.0rc0/asteroid/data/
--rw-r--r--   0 mparient (661056) incub    (200102)      774 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/data/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6904 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/avspeech_dataset.py
--rwxrwxrwx   0 mparient (661056) incub    (200102)      337 2021-02-03 20:05:19.000000 asteroid-0.6.0rc0/asteroid/data/basic_design.py
--rw-r--r--   0 mparient (661056) incub    (200102)     7914 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/dampvsep_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2023 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/dns_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3224 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/fuss_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4275 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/kinect_wsj.py
--rw-r--r--   0 mparient (661056) incub    (200102)     9486 2022-03-22 08:55:41.000000 asteroid-0.6.0rc0/asteroid/data/librimix_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     9299 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/musdb18_dataset.py
--rwxrwxrwx   0 mparient (661056) incub    (200102)      295 2020-12-17 00:35:39.000000 asteroid-0.6.0rc0/asteroid/data/scaler.py
--rw-r--r--   0 mparient (661056) incub    (200102)     9015 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/sms_wsj_dataset.py
--rwxrwxrwx   0 mparient (661056) incub    (200102)     1053 2020-12-17 00:35:39.000000 asteroid-0.6.0rc0/asteroid/data/toy_data.py
--rw-r--r--   0 mparient (661056) incub    (200102)      795 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/utils.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1555 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/data/vad_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     7591 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/wham_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6984 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/whamr_dataset.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4942 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/data/wsj0_mix.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.558834 asteroid-0.6.0rc0/asteroid/dsp/
--rw-r--r--   0 mparient (661056) incub    (200102)      343 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)    19738 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/dsp/beamforming.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3090 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/consistency.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1808 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/deltas.py
--rw-r--r--   0 mparient (661056) incub    (200102)      390 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/normalization.py
--rw-r--r--   0 mparient (661056) incub    (200102)    12108 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/overlap_add.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2815 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/spatial.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1108 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/dsp/vad.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.559834 asteroid-0.6.0rc0/asteroid/engine/
--rw-r--r--   0 mparient (661056) incub    (200102)      106 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/engine/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2484 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/engine/optimizers.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6550 2022-06-28 14:59:55.000000 asteroid-0.6.0rc0/asteroid/engine/schedulers.py
--rw-r--r--   0 mparient (661056) incub    (200102)     8041 2022-06-28 14:59:55.000000 asteroid-0.6.0rc0/asteroid/engine/system.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.560834 asteroid-0.6.0rc0/asteroid/losses/
--rw-r--r--   0 mparient (661056) incub    (200102)     1377 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1363 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/bark_matrix_16k.mat
--rw-r--r--   0 mparient (661056) incub    (200102)      932 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/bark_matrix_8k.mat
--rw-r--r--   0 mparient (661056) incub    (200102)     3039 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/losses/cluster.py
--rw-r--r--   0 mparient (661056) incub    (200102)    10449 2022-06-28 07:00:17.000000 asteroid-0.6.0rc0/asteroid/losses/mixit_wrapper.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2421 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/mse.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3274 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/multi_scale_spectral.py
--rw-r--r--   0 mparient (661056) incub    (200102)    15177 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/pit_wrapper.py
--rw-r--r--   0 mparient (661056) incub    (200102)    21985 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/pmsqe.py
--rw-r--r--   0 mparient (661056) incub    (200102)    10227 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/sdr.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6126 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/sinkpit_wrapper.py
--rw-r--r--   0 mparient (661056) incub    (200102)      563 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/losses/soft_f1.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2611 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/losses/stoi.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.562834 asteroid-0.6.0rc0/asteroid/masknn/
--rw-r--r--   0 mparient (661056) incub    (200102)      280 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1407 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/_dccrn_architectures.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4441 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/_dcunet_architectures.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3656 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/_local.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2029 2022-04-04 13:24:38.000000 asteroid-0.6.0rc0/asteroid/masknn/activations.py
--rw-r--r--   0 mparient (661056) incub    (200102)     8865 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/attention.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3832 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/base.py
--rw-r--r--   0 mparient (661056) incub    (200102)    31017 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/masknn/convolutional.py
--rw-r--r--   0 mparient (661056) incub    (200102)     5397 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/norms.py
--rw-r--r--   0 mparient (661056) incub    (200102)    26119 2022-03-31 09:03:30.000000 asteroid-0.6.0rc0/asteroid/masknn/recurrent.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4457 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/masknn/tac.py
--rw-r--r--   0 mparient (661056) incub    (200102)    16542 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/metrics.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.563834 asteroid-0.6.0rc0/asteroid/models/
--rw-r--r--   0 mparient (661056) incub    (200102)     1692 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/models/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)    11062 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/base_models.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4387 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/models/conv_tasnet.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1570 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/dccrnet.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2943 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/dcunet.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6200 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/demask.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4145 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/dprnn_tasnet.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3964 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/dptnet.py
--rw-r--r--   0 mparient (661056) incub    (200102)    12278 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/fasnet.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3840 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/lstm_tasnet.py
--rw-r--r--   0 mparient (661056) incub    (200102)    12980 2022-06-26 19:37:16.000000 asteroid-0.6.0rc0/asteroid/models/publisher.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6726 2022-06-26 20:43:19.000000 asteroid-0.6.0rc0/asteroid/models/sudormrf.py
--rwxrwxrwx   0 mparient (661056) incub    (200102)    14629 2021-05-07 14:56:38.000000 asteroid-0.6.0rc0/asteroid/models/x_umx.py
--rw-r--r--   0 mparient (661056) incub    (200102)     6253 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/models/zenodo.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.563834 asteroid-0.6.0rc0/asteroid/scripts/
--rw-r--r--   0 mparient (661056) incub    (200102)        0 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/scripts/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     7294 2022-06-26 18:26:34.000000 asteroid-0.6.0rc0/asteroid/scripts/asteroid_cli.py
--rw-r--r--   0 mparient (661056) incub    (200102)     1419 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/scripts/asteroid_versions.py
--rw-r--r--   0 mparient (661056) incub    (200102)     7556 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/separate.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.564834 asteroid-0.6.0rc0/asteroid/utils/
--rw-r--r--   0 mparient (661056) incub    (200102)      862 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/utils/__init__.py
--rw-r--r--   0 mparient (661056) incub    (200102)     2677 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/utils/deprecation_utils.py
--rw-r--r--   0 mparient (661056) incub    (200102)     3497 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/utils/generic_utils.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4858 2021-12-06 08:29:33.000000 asteroid-0.6.0rc0/asteroid/utils/hub_utils.py
--rw-r--r--   0 mparient (661056) incub    (200102)     4097 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/utils/parser_utils.py
--rw-r--r--   0 mparient (661056) incub    (200102)      944 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/utils/test_utils.py
--rw-r--r--   0 mparient (661056) incub    (200102)     7434 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/asteroid/utils/torch_utils.py
-drwxr-xr-x   0 mparient (661056) incub    (200102)        0 2022-06-28 15:03:37.555834 asteroid-0.6.0rc0/asteroid.egg-info/
--rwxrwxrwx   0 mparient (661056) incub    (200102)    10578 2022-06-28 15:03:37.000000 asteroid-0.6.0rc0/asteroid.egg-info/PKG-INFO
--rwxrwxrwx   0 mparient (661056) incub    (200102)     2594 2022-06-28 15:03:37.000000 asteroid-0.6.0rc0/asteroid.egg-info/SOURCES.txt
--rwxrwxrwx   0 mparient (661056) incub    (200102)        1 2022-06-28 15:03:37.000000 asteroid-0.6.0rc0/asteroid.egg-info/dependency_links.txt
--rwxrwxrwx   0 mparient (661056) incub    (200102)      271 2022-06-28 15:03:37.000000 asteroid-0.6.0rc0/asteroid.egg-info/entry_points.txt
--rwxrwxrwx   0 mparient (661056) incub    (200102)      275 2022-06-28 15:03:37.000000 asteroid-0.6.0rc0/asteroid.egg-info/requires.txt
--rwxrwxrwx   0 mparient (661056) incub    (200102)        9 2022-06-28 15:03:37.000000 asteroid-0.6.0rc0/asteroid.egg-info/top_level.txt
--rw-r--r--   0 mparient (661056) incub    (200102)      349 2021-12-06 08:29:21.000000 asteroid-0.6.0rc0/pyproject.toml
--rw-r--r--   0 mparient (661056) incub    (200102)       38 2022-06-28 15:03:37.564834 asteroid-0.6.0rc0/setup.cfg
--rw-r--r--   0 mparient (661056) incub    (200102)     2350 2022-06-28 15:01:44.000000 asteroid-0.6.0rc0/setup.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.992491 asteroid-0.6.1rc0/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1072 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/LICENSE
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)       86 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/MANIFEST.in
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    10712 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/PKG-INFO
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    10047 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/README.md
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.972491 asteroid-0.6.1rc0/asteroid/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      687 2023-07-19 11:22:00.000000 asteroid-0.6.1rc0/asteroid/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6954 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/binarize.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     7493 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/complex_nn.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.972491 asteroid-0.6.1rc0/asteroid/data/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      774 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6904 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/avspeech_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     7914 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/dampvsep_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2023 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/dns_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3224 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/fuss_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4275 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/kinect_wsj.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     9485 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/librimix_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     9299 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/musdb18_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     9015 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/sms_wsj_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      791 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/utils.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1555 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/vad_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     7591 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/wham_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6984 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/whamr_dataset.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4942 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/data/wsj0_mix.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/dsp/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      343 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    19890 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/beamforming.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3088 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/consistency.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1808 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/deltas.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      390 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/normalization.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    12105 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/overlap_add.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2815 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/spatial.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1108 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/dsp/vad.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/engine/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      106 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/engine/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2484 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/engine/optimizers.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6548 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/engine/schedulers.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     8041 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/engine/system.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/losses/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1377 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1363 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/bark_matrix_16k.mat
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      932 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/bark_matrix_8k.mat
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3039 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/cluster.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    10449 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/mixit_wrapper.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2421 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/mse.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3274 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/multi_scale_spectral.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    15177 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/pit_wrapper.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    21981 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/pmsqe.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    10209 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/sdr.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6126 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/sinkpit_wrapper.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      563 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/soft_f1.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2611 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/losses/stoi.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/masknn/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      280 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1407 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/_dccrn_architectures.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4441 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/_dcunet_architectures.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3656 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/_local.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2029 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/activations.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     8865 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/attention.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3832 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/base.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    31005 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/convolutional.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     5401 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/norms.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    26113 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/recurrent.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4457 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/masknn/tac.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    16542 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/metrics.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/models/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1692 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    11059 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/base_models.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4387 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/conv_tasnet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1570 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/dccrnet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2943 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/dcunet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6198 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/demask.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4145 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/dprnn_tasnet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3964 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/dptnet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    12278 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/fasnet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3840 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/lstm_tasnet.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    12978 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/publisher.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6722 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/sudormrf.py
+-rwxr-xr-x   0 mpariente  (1000) mpariente  (1000)    14627 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/x_umx.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     6250 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/models/zenodo.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/scripts/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/scripts/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     7294 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/scripts/asteroid_cli.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     1419 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/scripts/asteroid_versions.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     7556 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/separate.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.982491 asteroid-0.6.1rc0/asteroid/utils/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      862 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/__init__.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2677 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/deprecation_utils.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     3497 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/generic_utils.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4945 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/hub_utils.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     4301 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/parser_utils.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      944 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/test_utils.py
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     7434 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/asteroid/utils/torch_utils.py
+drwxr-xr-x   0 mpariente  (1000) mpariente  (1000)        0 2023-07-19 11:26:17.972491 asteroid-0.6.1rc0/asteroid.egg-info/
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)    10712 2023-07-19 11:26:17.000000 asteroid-0.6.1rc0/asteroid.egg-info/PKG-INFO
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2514 2023-07-19 11:26:17.000000 asteroid-0.6.1rc0/asteroid.egg-info/SOURCES.txt
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)        1 2023-07-19 11:26:17.000000 asteroid-0.6.1rc0/asteroid.egg-info/dependency_links.txt
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      270 2023-07-19 11:26:17.000000 asteroid-0.6.1rc0/asteroid.egg-info/entry_points.txt
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      293 2023-07-19 11:26:17.000000 asteroid-0.6.1rc0/asteroid.egg-info/requires.txt
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)        9 2023-07-19 11:26:17.000000 asteroid-0.6.1rc0/asteroid.egg-info/top_level.txt
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)      349 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/pyproject.toml
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)       38 2023-07-19 11:26:17.992491 asteroid-0.6.1rc0/setup.cfg
+-rw-r--r--   0 mpariente  (1000) mpariente  (1000)     2368 2023-07-19 11:20:34.000000 asteroid-0.6.1rc0/setup.py
```

### Comparing `asteroid-0.6.0rc0/LICENSE` & `asteroid-0.6.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/PKG-INFO` & `asteroid-0.6.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: asteroid
-Version: 0.6.0rc0
+Version: 0.6.1rc0
 Summary: PyTorch-based audio source separation toolkit
 Home-page: https://github.com/asteroid-team/asteroid
 Author: Manuel Pariente
 Author-email: manuel.pariente@loria.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -128,14 +127,15 @@
 * [x] [DualPathRNN](./egs/wham/DPRNN) ([Luo et al.](https://arxiv.org/abs/1910.06379))
 * [x] [Two step learning](./egs/wham/TwoStep)([Tzinis et al.](https://arxiv.org/abs/1910.09804))
 * [x] [SudoRMRFNet](./asteroid/models/sudormrf.py) ([Tzinis et al.](https://arxiv.org/abs/2007.06833))
 * [x] [DPTNet](./asteroid/models/dptnet.py) ([Chen et al.](https://arxiv.org/abs/2007.13975))
 * [x] [DCCRNet](./asteroid/models/dccrnet.py) ([Hu et al.](https://arxiv.org/abs/2008.00264))
 * [x] [DCUNet](./asteroid/models/dcunet.py) ([Choi et al.](https://arxiv.org/abs/1903.03107))
 * [x] [CrossNet-Open-Unmix](./asteroid/models/x_umx.py) ([Sawata et al.](https://arxiv.org/abs/2010.04228))
+* [x] [Multi-Decoder DPRNN](./egs/wsj0-mix-var/Multi-Decoder-DPRNN) ([Zhu et al.](http://www.isle.illinois.edu/speech_web_lg/pubs/2021/zhu2021multi.pdf))
 * [ ] Open-Unmix (coming) ([Stöter et al.](https://sigsep.github.io/open-unmix/))
 * [ ] Wavesplit (coming) ([Zeghidour et al.](https://arxiv.org/abs/2002.08933))
 
 ## Supported datasets
 ([↑up to contents](#contents))
 * [x] [WSJ0-2mix](./egs/wsj0-mix) / WSJ03mix ([Hershey et al.](https://arxiv.org/abs/1508.04306))
 * [x] [WHAM](./egs/wham) ([Wichern et al.](https://arxiv.org/abs/1907.01160))
@@ -225,9 +225,7 @@
 [codecov]: https://codecov.io/gh/asteroid-team/asteroid
 [slack-badge]: https://img.shields.io/badge/slack-chat-green.svg?logo=slack
 [slack-invite]: https://join.slack.com/t/asteroid-dev/shared_invite/zt-cn9y85t3-QNHXKD1Et7qoyzu1Ji5bcA
 
 [comment]: <> (Others)
 [issue]: https://github.com/asteroid-team/asteroid/issues/new
 [pr]: https://github.com/asteroid-team/asteroid/compare
-
-
```

### Comparing `asteroid-0.6.0rc0/README.md` & `asteroid-0.6.1rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 * [x] [DualPathRNN](./egs/wham/DPRNN) ([Luo et al.](https://arxiv.org/abs/1910.06379))
 * [x] [Two step learning](./egs/wham/TwoStep)([Tzinis et al.](https://arxiv.org/abs/1910.09804))
 * [x] [SudoRMRFNet](./asteroid/models/sudormrf.py) ([Tzinis et al.](https://arxiv.org/abs/2007.06833))
 * [x] [DPTNet](./asteroid/models/dptnet.py) ([Chen et al.](https://arxiv.org/abs/2007.13975))
 * [x] [DCCRNet](./asteroid/models/dccrnet.py) ([Hu et al.](https://arxiv.org/abs/2008.00264))
 * [x] [DCUNet](./asteroid/models/dcunet.py) ([Choi et al.](https://arxiv.org/abs/1903.03107))
 * [x] [CrossNet-Open-Unmix](./asteroid/models/x_umx.py) ([Sawata et al.](https://arxiv.org/abs/2010.04228))
+* [x] [Multi-Decoder DPRNN](./egs/wsj0-mix-var/Multi-Decoder-DPRNN) ([Zhu et al.](http://www.isle.illinois.edu/speech_web_lg/pubs/2021/zhu2021multi.pdf))
 * [ ] Open-Unmix (coming) ([Stöter et al.](https://sigsep.github.io/open-unmix/))
 * [ ] Wavesplit (coming) ([Zeghidour et al.](https://arxiv.org/abs/2002.08933))
 
 ## Supported datasets
 ([↑up to contents](#contents))
 * [x] [WSJ0-2mix](./egs/wsj0-mix) / WSJ03mix ([Hershey et al.](https://arxiv.org/abs/1508.04306))
 * [x] [WHAM](./egs/wham) ([Wichern et al.](https://arxiv.org/abs/1907.01160))
```

### Comparing `asteroid-0.6.0rc0/asteroid/__init__.py` & `asteroid-0.6.1rc0/asteroid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from .models import ConvTasNet, DCCRNet, DCUNet, DPRNNTasNet, DPTNet, LSTMTasNet, DeMask
 from .utils import deprecation_utils, torch_utils  # noqa
 
 project_root = str(pathlib.Path(__file__).expanduser().absolute().parent.parent)
-__version__ = "0.6.0rc0"
+__version__ = "0.6.1rc0"
 
 
 def show_available_models():
     from .utils.hub_utils import MODELS_URLS_HASHTABLE
 
     print(" \n".join(list(MODELS_URLS_HASHTABLE.keys())))
```

### Comparing `asteroid-0.6.0rc0/asteroid/binarize.py` & `asteroid-0.6.1rc0/asteroid/binarize.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/complex_nn.py` & `asteroid-0.6.1rc0/asteroid/complex_nn.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/__init__.py` & `asteroid-0.6.1rc0/asteroid/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/avspeech_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/avspeech_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/dampvsep_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/dampvsep_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/dns_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/dns_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/fuss_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/fuss_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/kinect_wsj.py` & `asteroid-0.6.1rc0/asteroid/data/kinect_wsj.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/librimix_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/librimix_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             data_license = [librispeech_license]
         else:
             data_license = [librispeech_license, wham_noise_license]
         infos["licenses"] = data_license
         return infos
 
     def _dataset_name(self):
-        """ Differentiate between 2 and 3 sources."""
+        """Differentiate between 2 and 3 sources."""
         return f"Libri{self.n_src}Mix"
 
 
 librispeech_license = dict(
     title="LibriSpeech ASR corpus",
     title_link="http://www.openslr.org/12",
     author="Vassil Panayotov",
```

### Comparing `asteroid-0.6.0rc0/asteroid/data/musdb18_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/musdb18_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/sms_wsj_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/sms_wsj_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/utils.py` & `asteroid-0.6.1rc0/asteroid/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     Output of the default collate function is expected to return two objects:
     inputs and targets.
     """
     # Inputs (batch, time) / targets (batch, n_src, time)
     inputs, targets = default_collate(batch)
     batch, n_src, _ = targets.shape
 
-    energies = torch.sum(targets ** 2, dim=-1, keepdim=True)
+    energies = torch.sum(targets**2, dim=-1, keepdim=True)
     new_src = []
     for i in range(targets.shape[1]):
         new_s = targets[torch.randperm(batch), i, :]
-        new_s = new_s * torch.sqrt(energies[:, i] / (new_s ** 2).sum(-1, keepdims=True))
+        new_s = new_s * torch.sqrt(energies[:, i] / (new_s**2).sum(-1, keepdims=True))
         new_src.append(new_s)
 
     targets = torch.stack(new_src, dim=1)
     inputs = targets.sum(1)
     return inputs, targets
```

### Comparing `asteroid-0.6.0rc0/asteroid/data/vad_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/vad_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/wham_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/wham_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/whamr_dataset.py` & `asteroid-0.6.1rc0/asteroid/data/whamr_dataset.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/data/wsj0_mix.py` & `asteroid-0.6.1rc0/asteroid/data/wsj0_mix.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/dsp/beamforming.py` & `asteroid-0.6.1rc0/asteroid/dsp/beamforming.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,18 +412,18 @@
     if input_dtype not in [torch.float64, torch.complex128]:
         solve_dtype = _precision_mapping()[input_dtype]
     return _stable_solve(b.to(solve_dtype), a.to(solve_dtype)).to(input_dtype)
 
 
 def _stable_solve(b, a, eps=1e-6):
     try:
-        return torch.solve(b, a)[0]
+        return torch.linalg.solve(a, b)
     except RuntimeError:
         a = condition_scm(a, eps)
-        return torch.solve(b, a)[0]
+        return torch.linalg.solve(a, b)
 
 
 def stable_cholesky(input, upper=False, out=None, eps=1e-6):
     """Compute the Cholesky decomposition of ``input``.
     If ``input`` is only p.s.d, add a small jitter to the diagonal.
 
     Args:
@@ -438,18 +438,22 @@
     if input_dtype not in [torch.float64, torch.complex128]:
         solve_dtype = _precision_mapping()[input_dtype]
     return _stable_cholesky(input.to(solve_dtype), upper=upper, out=out, eps=eps).to(input_dtype)
 
 
 def _stable_cholesky(input, upper=False, out=None, eps=1e-6):
     try:
-        return torch.cholesky(input, upper=upper, out=out)
+        if upper:
+            return torch.linalg.cholesky(input, out=out).mH
+        return torch.linalg.cholesky(input, out=out)
     except RuntimeError:
         input = condition_scm(input, eps)
-        return torch.cholesky(input, upper=upper, out=out)
+        if upper:
+            return torch.linalg.cholesky(input, out=out).mH
+        return torch.linalg.cholesky(input, out=out)
 
 
 def generalized_eigenvalue_decomposition(a, b):
     """Solves the generalized eigenvalue decomposition through Cholesky decomposition.
     Returns eigen values and eigen vectors (ascending order).
     """
     # Only run it in double
```

### Comparing `asteroid-0.6.0rc0/asteroid/dsp/consistency.py` & `asteroid-0.6.1rc0/asteroid/dsp/consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """
     # If the source weights are not specified, the weights are the relative
     # power of each source to the sum. w_i = P_i / (P_all), P for power.
     if src_weights is None:
         all_dims: List[int] = torch.arange(est_sources.ndim).tolist()
         all_dims.pop(dim)  # Remove source axis
         all_dims.pop(0)  # Remove batch axis
-        src_weights = torch.mean(est_sources ** 2, dim=all_dims, keepdim=True)
+        src_weights = torch.mean(est_sources**2, dim=all_dims, keepdim=True)
     # Make sure that the weights sum up to 1
     norm_weights = torch.sum(src_weights, dim=dim, keepdim=True) + 1e-8
     src_weights = src_weights / norm_weights
 
     # Compute residual mix - sum(est_sources)
     if mixture.ndim == est_sources.ndim - 1:
         # mixture (batch, *), est_sources (batch, n_src, *)
```

### Comparing `asteroid-0.6.0rc0/asteroid/dsp/deltas.py` & `asteroid-0.6.1rc0/asteroid/dsp/deltas.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/dsp/overlap_add.py` & `asteroid-0.6.1rc0/asteroid/dsp/overlap_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def __init__(
         self,
         nnet,
         n_src,
         window_size,
         hop_size=None,
-        window="hanning",
+        window="hann",
         reorder_chunks=True,
         enable_grad=False,
     ):
         super().__init__()
         assert window_size % 2 == 0, "Window size must be even"
 
         self.nnet = nnet
```

### Comparing `asteroid-0.6.0rc0/asteroid/dsp/spatial.py` & `asteroid-0.6.1rc0/asteroid/dsp/spatial.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/dsp/vad.py` & `asteroid-0.6.1rc0/asteroid/dsp/vad.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/engine/optimizers.py` & `asteroid-0.6.1rc0/asteroid/engine/optimizers.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/engine/schedulers.py` & `asteroid-0.6.1rc0/asteroid/engine/schedulers.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 * self.d_model ** (-0.5)
                 * min(self.step_num ** (-0.5), self.step_num * self.warmup_steps ** (-1.5))
             )
         return lr
 
 
 def sinkpit_default_beta_schedule(epoch):
-    return min([1.02 ** epoch, 10])
+    return min([1.02**epoch, 10])
 
 
 class SinkPITBetaScheduler(pl.callbacks.Callback):
     r"""Scheduler of the beta value of SinkPITLossWrapper
     This module is used as a Callback function of `pytorch_lightning.Trainer`.
 
     Args:
```

### Comparing `asteroid-0.6.0rc0/asteroid/engine/system.py` & `asteroid-0.6.1rc0/asteroid/engine/system.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/__init__.py` & `asteroid-0.6.1rc0/asteroid/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/bark_matrix_16k.mat` & `asteroid-0.6.1rc0/asteroid/losses/bark_matrix_16k.mat`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/bark_matrix_8k.mat` & `asteroid-0.6.1rc0/asteroid/losses/bark_matrix_8k.mat`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/cluster.py` & `asteroid-0.6.1rc0/asteroid/losses/cluster.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/mixit_wrapper.py` & `asteroid-0.6.1rc0/asteroid/losses/mixit_wrapper.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/mse.py` & `asteroid-0.6.1rc0/asteroid/losses/mse.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/multi_scale_spectral.py` & `asteroid-0.6.1rc0/asteroid/losses/multi_scale_spectral.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/pit_wrapper.py` & `asteroid-0.6.1rc0/asteroid/losses/pit_wrapper.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/pmsqe.py` & `asteroid-0.6.1rc0/asteroid/losses/pmsqe.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         # Bounded computation of the per frame distortion metric
         wd_frame = torch.min(d_frame / weights, 45.0 * torch.ones_like(d_frame))
         wda_frame = torch.min(da_frame / weights, 45.0 * torch.ones_like(da_frame))
         return wd_frame, wda_frame
 
     @staticmethod
     def get_correction_factor(window_name):
-        """ Returns the power correction factor depending on the window. """
+        """Returns the power correction factor depending on the window."""
         if window_name == "rect":
             return 1.0
         elif window_name == "hann":
             return 2.666666666666754
         elif window_name == "sqrt_hann":
             return 2.0
         elif window_name == "hamming":
@@ -311,15 +311,15 @@
         elif sample_rate == 16000:
             self.register_16k_constants()
         # Mask SSL
         mask_sll = np.zeros(shape=[self.nbins // 2 + 1], dtype=np.float32)
         mask_sll[11] = 0.5 * 25.0 / 31.25
         mask_sll[12:104] = 1.0
         mask_sll[104] = 0.5
-        correction = self.pow_correc_factor * (self.nbins + 2.0) / self.nbins ** 2
+        correction = self.pow_correc_factor * (self.nbins + 2.0) / self.nbins**2
         mask_sll = mask_sll * correction
         self.mask_sll = nn.Parameter(tensor(mask_sll), requires_grad=False)
 
     def register_16k_constants(self):
         # Absolute threshold power
         abs_thresh_power = [
             51286152.00,
```

### Comparing `asteroid-0.6.0rc0/asteroid/losses/sdr.py` & `asteroid-0.6.1rc0/asteroid/losses/sdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,27 +58,27 @@
         s_target = torch.unsqueeze(targets, dim=1)
         s_estimate = torch.unsqueeze(est_targets, dim=2)
 
         if self.sdr_type in ["sisdr", "sdsdr"]:
             # [batch, n_src, n_src, 1]
             pair_wise_dot = torch.sum(s_estimate * s_target, dim=3, keepdim=True)
             # [batch, 1, n_src, 1]
-            s_target_energy = torch.sum(s_target ** 2, dim=3, keepdim=True) + self.EPS
+            s_target_energy = torch.sum(s_target**2, dim=3, keepdim=True) + self.EPS
             # [batch, n_src, n_src, time]
             pair_wise_proj = pair_wise_dot * s_target / s_target_energy
         else:
             # [batch, n_src, n_src, time]
             pair_wise_proj = s_target.repeat(1, s_target.shape[2], 1, 1)
         if self.sdr_type in ["sdsdr", "snr"]:
             e_noise = s_estimate - s_target
         else:
             e_noise = s_estimate - pair_wise_proj
         # [batch, n_src, n_src]
-        pair_wise_sdr = torch.sum(pair_wise_proj ** 2, dim=3) / (
-            torch.sum(e_noise ** 2, dim=3) + self.EPS
+        pair_wise_sdr = torch.sum(pair_wise_proj**2, dim=3) / (
+            torch.sum(e_noise**2, dim=3) + self.EPS
         )
         if self.take_log:
             pair_wise_sdr = 10 * torch.log10(pair_wise_sdr + self.EPS)
         return -pair_wise_sdr
 
 
 class SingleSrcNegSDR(_Loss):
@@ -141,26 +141,26 @@
             target = target - mean_source
             est_target = est_target - mean_estimate
         # Step 2. Pair-wise SI-SDR.
         if self.sdr_type in ["sisdr", "sdsdr"]:
             # [batch, 1]
             dot = torch.sum(est_target * target, dim=1, keepdim=True)
             # [batch, 1]
-            s_target_energy = torch.sum(target ** 2, dim=1, keepdim=True) + self.EPS
+            s_target_energy = torch.sum(target**2, dim=1, keepdim=True) + self.EPS
             # [batch, time]
             scaled_target = dot * target / s_target_energy
         else:
             # [batch, time]
             scaled_target = target
         if self.sdr_type in ["sdsdr", "snr"]:
             e_noise = est_target - target
         else:
             e_noise = est_target - scaled_target
         # [batch]
-        losses = torch.sum(scaled_target ** 2, dim=1) / (torch.sum(e_noise ** 2, dim=1) + self.EPS)
+        losses = torch.sum(scaled_target**2, dim=1) / (torch.sum(e_noise**2, dim=1) + self.EPS)
         if self.take_log:
             losses = 10 * torch.log10(losses + self.EPS)
         losses = losses.mean() if self.reduction == "mean" else losses
         return -losses
 
 
 class MultiSrcNegSDR(_Loss):
@@ -218,27 +218,27 @@
             targets = targets - mean_source
             est_targets = est_targets - mean_estimate
         # Step 2. Pair-wise SI-SDR.
         if self.sdr_type in ["sisdr", "sdsdr"]:
             # [batch, n_src]
             pair_wise_dot = torch.sum(est_targets * targets, dim=2, keepdim=True)
             # [batch, n_src]
-            s_target_energy = torch.sum(targets ** 2, dim=2, keepdim=True) + self.EPS
+            s_target_energy = torch.sum(targets**2, dim=2, keepdim=True) + self.EPS
             # [batch, n_src, time]
             scaled_targets = pair_wise_dot * targets / s_target_energy
         else:
             # [batch, n_src, time]
             scaled_targets = targets
         if self.sdr_type in ["sdsdr", "snr"]:
             e_noise = est_targets - targets
         else:
             e_noise = est_targets - scaled_targets
         # [batch, n_src]
-        pair_wise_sdr = torch.sum(scaled_targets ** 2, dim=2) / (
-            torch.sum(e_noise ** 2, dim=2) + self.EPS
+        pair_wise_sdr = torch.sum(scaled_targets**2, dim=2) / (
+            torch.sum(e_noise**2, dim=2) + self.EPS
         )
         if self.take_log:
             pair_wise_sdr = 10 * torch.log10(pair_wise_sdr + self.EPS)
         return -torch.mean(pair_wise_sdr, dim=-1)
 
 
 # aliases
```

### Comparing `asteroid-0.6.0rc0/asteroid/losses/sinkpit_wrapper.py` & `asteroid-0.6.1rc0/asteroid/losses/sinkpit_wrapper.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/soft_f1.py` & `asteroid-0.6.1rc0/asteroid/losses/soft_f1.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/losses/stoi.py` & `asteroid-0.6.1rc0/asteroid/losses/stoi.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/_dccrn_architectures.py` & `asteroid-0.6.1rc0/asteroid/masknn/_dccrn_architectures.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/_dcunet_architectures.py` & `asteroid-0.6.1rc0/asteroid/masknn/_dcunet_architectures.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/_local.py` & `asteroid-0.6.1rc0/asteroid/masknn/_local.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/activations.py` & `asteroid-0.6.1rc0/asteroid/masknn/activations.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/attention.py` & `asteroid-0.6.1rc0/asteroid/masknn/attention.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/base.py` & `asteroid-0.6.1rc0/asteroid/masknn/base.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/convolutional.py` & `asteroid-0.6.1rc0/asteroid/masknn/convolutional.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,25 +161,25 @@
         bottleneck_conv = nn.Conv1d(in_chan, bn_chan, 1)
         self.bottleneck = nn.Sequential(layer_norm, bottleneck_conv)
         # Succession of Conv1DBlock with exponentially increasing dilation.
         self.TCN = nn.ModuleList()
         for r in range(n_repeats):
             for x in range(n_blocks):
                 if not causal:
-                    padding = (conv_kernel_size - 1) * 2 ** x // 2
+                    padding = (conv_kernel_size - 1) * 2**x // 2
                 else:
-                    padding = (conv_kernel_size - 1) * 2 ** x
+                    padding = (conv_kernel_size - 1) * 2**x
                 self.TCN.append(
                     Conv1DBlock(
                         bn_chan,
                         hid_chan,
                         skip_chan,
                         conv_kernel_size,
                         padding=padding,
-                        dilation=2 ** x,
+                        dilation=2**x,
                         norm_type=norm_type,
                         causal=causal,
                     )
                 )
         mask_conv_inp = skip_chan if skip_chan else bn_chan
         mask_conv = nn.Conv1d(mask_conv_inp, n_src * out_chan, 1)
         self.mask_net = nn.Sequential(nn.PReLU(), mask_conv)
@@ -308,32 +308,32 @@
         layer_norm = norms.get(norm_type)(in_chan)
         bottleneck_conv = nn.Conv1d(in_chan, bn_chan, 1)
         self.bottleneck = nn.Sequential(layer_norm, bottleneck_conv)
         # Succession of Conv1DBlock with exponentially increasing dilation.
         self.TCN = nn.ModuleList()
         for r in range(n_repeats):
             for x in range(n_blocks):
-                padding = (conv_kernel_size - 1) * 2 ** x // 2
+                padding = (conv_kernel_size - 1) * 2**x // 2
                 self.TCN.append(
                     Conv1DBlock(
                         bn_chan,
                         hid_chan,
                         skip_chan,
                         conv_kernel_size,
                         padding=padding,
-                        dilation=2 ** x,
+                        dilation=2**x,
                         norm_type=norm_type,
                     )
                 )
         # Dense connection in TDCNpp
         self.dense_skip = nn.ModuleList()
         for r in range(n_repeats - 1):
             self.dense_skip.append(nn.Conv1d(bn_chan, bn_chan, 1))
 
-        scaling_param = torch.Tensor([0.9 ** l for l in range(1, n_blocks)])
+        scaling_param = torch.Tensor([0.9**l for l in range(1, n_blocks)])
         scaling_param = scaling_param.unsqueeze(0).expand(n_repeats, n_blocks - 1).clone()
         self.scaling_param = nn.Parameter(scaling_param, requires_grad=True)
 
         mask_conv_inp = skip_chan if skip_chan else bn_chan
         mask_conv = nn.Conv1d(mask_conv_inp, n_src * out_chan, 1)
         self.mask_net = nn.Sequential(nn.PReLU(), mask_conv)
         # Get activation function.
```

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/norms.py` & `asteroid-0.6.1rc0/asteroid/masknn/norms.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __init__(self, channel_size):
         super(_LayerNorm, self).__init__()
         self.channel_size = channel_size
         self.gamma = nn.Parameter(torch.ones(channel_size), requires_grad=True)
         self.beta = nn.Parameter(torch.zeros(channel_size), requires_grad=True)
 
     def apply_gain_and_bias(self, normed_x):
-        """ Assumes input of size `[batch, chanel, *]`. """
+        """Assumes input of size `[batch, chanel, *]`."""
         return (self.gamma * normed_x.transpose(1, -1) + self.beta).transpose(1, -1)
 
 
 class GlobLN(_LayerNorm):
     """Global Layer Normalization (globLN)."""
 
     def forward(self, x, EPS: float = 1e-8):
@@ -94,15 +94,15 @@
         batch, chan, spec_len = x.size()
         cum_sum = torch.cumsum(x.sum(1, keepdim=True), dim=-1)
         cum_pow_sum = torch.cumsum(x.pow(2).sum(1, keepdim=True), dim=-1)
         cnt = torch.arange(
             start=chan, end=chan * (spec_len + 1), step=chan, dtype=x.dtype, device=x.device
         ).view(1, 1, -1)
         cum_mean = cum_sum / cnt
-        cum_var = cum_pow_sum - cum_mean.pow(2)
+        cum_var = cum_pow_sum / cnt - cum_mean.pow(2)
         return self.apply_gain_and_bias((x - cum_mean) / (cum_var + EPS).sqrt())
 
 
 class FeatsGlobLN(_LayerNorm):
     """Feature-wise global Layer Normalization (FeatsGlobLN).
     Applies normalization over frames for each channel."""
```

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/recurrent.py` & `asteroid-0.6.1rc0/asteroid/masknn/recurrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         )
 
     @property
     def output_size(self):
         return self.hidden_size * (2 if self.bidirectional else 1)
 
     def forward(self, inp):
-        """ Input shape [batch, seq, feats] """
+        """Input shape [batch, seq, feats]"""
         self.rnn.flatten_parameters()  # Enables faster multi-GPU training.
         output = inp
         rnn_output, _ = self.rnn(output)
         return rnn_output
 
 
 class MulCatRNN(nn.Module):
@@ -111,15 +111,15 @@
         )
 
     @property
     def output_size(self):
         return self.hidden_size * (2 if self.bidirectional else 1) + self.input_size
 
     def forward(self, inp):
-        """ Input shape [batch, seq, feats] """
+        """Input shape [batch, seq, feats]"""
         self.rnn1.flatten_parameters()  # Enables faster multi-GPU training.
         self.rnn2.flatten_parameters()  # Enables faster multi-GPU training.
         rnn_output1, _ = self.rnn1(inp)
         rnn_output2, _ = self.rnn2(inp)
         return torch.cat((rnn_output1 * rnn_output2, inp), 2)
 
 
@@ -301,15 +301,15 @@
         self.intra_linear = nn.Linear(self.intra_RNN.output_size, in_chan)
         self.intra_norm = norms.get(norm_type)(in_chan)
 
         self.inter_linear = nn.Linear(self.inter_RNN.output_size, in_chan)
         self.inter_norm = norms.get(norm_type)(in_chan)
 
     def forward(self, x):
-        """ Input shape : [batch, feats, chunk_size, num_chunks] """
+        """Input shape : [batch, feats, chunk_size, num_chunks]"""
         B, N, K, L = x.size()
         output = x  # for skip connection
         # Intra-chunk processing
         x = x.transpose(1, -1).reshape(B * L, K, N)
         x = self.intra_RNN(x)
         x = self.intra_linear(x)
         x = x.reshape(B, L, K, N).transpose(1, -1)
```

### Comparing `asteroid-0.6.0rc0/asteroid/masknn/tac.py` & `asteroid-0.6.1rc0/asteroid/masknn/tac.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/metrics.py` & `asteroid-0.6.1rc0/asteroid/metrics.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/__init__.py` & `asteroid-0.6.1rc0/asteroid/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/base_models.py` & `asteroid-0.6.1rc0/asteroid/models/base_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             pytorch_lightning_version=pl.__version__,
             asteroid_version=asteroid_version,
         )
         model_conf["infos"] = infos
         return model_conf
 
     def get_state_dict(self):
-        """ In case the state dict needs to be modified before sharing the model."""
+        """In case the state dict needs to be modified before sharing the model."""
         return self.state_dict()
 
     def get_model_args(self):
         """Should return args to re-instantiate the class."""
         raise NotImplementedError
 
 
@@ -268,15 +268,15 @@
 
         Returns:
             torch.Tensor: Time-domain waveforms.
         """
         return self.decoder(masked_tf_rep)
 
     def get_model_args(self):
-        """ Arguments needed to re-instantiate the model. """
+        """Arguments needed to re-instantiate the model."""
         fb_config = self.encoder.filterbank.get_config()
         masknet_config = self.masker.get_config()
         # Assert both dict are disjoint
         if not all(k not in fb_config for k in masknet_config):
             raise AssertionError(
                 "Filterbank and Mask network config share common keys. Merging them is not safe."
             )
```

### Comparing `asteroid-0.6.0rc0/asteroid/models/conv_tasnet.py` & `asteroid-0.6.1rc0/asteroid/models/conv_tasnet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/dccrnet.py` & `asteroid-0.6.1rc0/asteroid/models/dccrnet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/dcunet.py` & `asteroid-0.6.1rc0/asteroid/models/dcunet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/demask.py` & `asteroid-0.6.1rc0/asteroid/models/demask.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             torch.Tensor: Masked time-frequency representations.
         """
         if self.output_type == "reim":
             tf_rep = tf_rep.unsqueeze(1)
         return est_masks * tf_rep
 
     def get_model_args(self):
-        """ Arguments needed to re-instantiate the model. """
+        """Arguments needed to re-instantiate the model."""
         model_args = {
             "input_type": self.input_type,
             "output_type": self.output_type,
             "hidden_dims": self.hidden_dims,
             "dropout": self.dropout,
             "activation": self.activation,
             "mask_act": self.mask_act,
```

### Comparing `asteroid-0.6.0rc0/asteroid/models/dprnn_tasnet.py` & `asteroid-0.6.1rc0/asteroid/models/dprnn_tasnet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/dptnet.py` & `asteroid-0.6.1rc0/asteroid/models/dptnet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/fasnet.py` & `asteroid-0.6.1rc0/asteroid/models/fasnet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/lstm_tasnet.py` & `asteroid-0.6.1rc0/asteroid/models/lstm_tasnet.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/models/publisher.py` & `asteroid-0.6.1rc0/asteroid/models/publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     model["infos"]["affiliation"] = affiliation if affiliation else "Unknown"
     model["infos"]["upload_name"] = upload_name
     model["infos"]["license_note"] = license_note
     return model
 
 
 def get_username():
-    """ Get git of FS username for upload. """
+    """Get git of FS username for upload."""
     username = subprocess.check_output(["git", "config", "user.name"])
     username = username.decode("utf-8")[:-1]
     if not username:  # Empty string
         import getpass
 
         username = getpass.getuser()
     return username
```

### Comparing `asteroid-0.6.0rc0/asteroid/models/sudormrf.py` & `asteroid-0.6.1rc0/asteroid/models/sudormrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
     def __init__(self, encoder, upsampling_depth=4, kernel_size=21):
         super().__init__()
         self.encoder = encoder
         self.upsampling_depth = upsampling_depth
         self.kernel_size = kernel_size
 
         # Appropriate padding is needed for arbitrary lengths
-        self.lcm = abs(self.kernel_size // 2 * 2 ** self.upsampling_depth) // math.gcd(
-            self.kernel_size // 2, 2 ** self.upsampling_depth
+        self.lcm = abs(self.kernel_size // 2 * 2**self.upsampling_depth) // math.gcd(
+            self.kernel_size // 2, 2**self.upsampling_depth
         )
 
         # For serialize
         self.filterbank = self.encoder.filterbank
         self.sample_rate = getattr(self.encoder.filterbank, "sample_rate", None)
 
     def forward(self, x):
```

### Comparing `asteroid-0.6.0rc0/asteroid/models/x_umx.py` & `asteroid-0.6.1rc0/asteroid/models/x_umx.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         return est_masks
 
     def apply_masks(self, mixture, est_masks):
         masked_tf_rep = torch.stack([mixture * est_masks[i] for i in range(len(self.sources))])
         return masked_tf_rep
 
     def get_model_args(self):
-        """ Arguments needed to re-instantiate the model. """
+        """Arguments needed to re-instantiate the model."""
         fb_config = {
             "window_length": self.window_length,
             "in_chan": self.in_chan,
             "n_hop": self.n_hop,
             "sample_rate": self.sample_rate,
         }
```

### Comparing `asteroid-0.6.0rc0/asteroid/models/zenodo.py` & `asteroid-0.6.1rc0/asteroid/models/zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,32 +135,32 @@
         r = requests.post(
             f"{self.zenodo_address}/api/deposit/depositions/{dep_id}/actions/publish",
             headers=self.headers,
         )
         return r
 
     def get_deposition(self, dep_id=-1):
-        """ Get deposition by deposition id. Get all dep_id is -1 (default)."""
+        """Get deposition by deposition id. Get all dep_id is -1 (default)."""
         if dep_id > -1:
             print(f"Get deposition {dep_id} from Zenodo")
             r = requests.get(
                 f"{self.zenodo_address}/api/deposit/depositions/{dep_id}", headers=self.headers
             )
         else:
             print("Get all depositions from Zenodo")
             r = requests.get(f"{self.zenodo_address}/api/deposit/depositions", headers=self.headers)
         print("Get Depositions: Status Code: {}".format(r.status_code))
         return r
 
     def remove_deposition(self, dep_id):
-        """ Remove deposition with deposition id `dep_id`"""
+        """Remove deposition with deposition id `dep_id`"""
         print(f"Delete deposition number {dep_id}")
         r = requests.delete(
             f"{self.zenodo_address}/api/deposit/depositions/{dep_id}", headers=self.auth_header
         )
         return r
 
     def remove_all_depositions(self):
-        """ Removes all unpublished deposition (not records)."""
+        """Removes all unpublished deposition (not records)."""
         all_depositions = self.get_deposition()
         for dep in all_depositions.json():
             self.remove_deposition(dep["id"])
```

### Comparing `asteroid-0.6.0rc0/asteroid/scripts/asteroid_cli.py` & `asteroid-0.6.1rc0/asteroid/scripts/asteroid_cli.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/scripts/asteroid_versions.py` & `asteroid-0.6.1rc0/asteroid/scripts/asteroid_versions.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/separate.py` & `asteroid-0.6.1rc0/asteroid/separate.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/utils/__init__.py` & `asteroid-0.6.1rc0/asteroid/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/utils/deprecation_utils.py` & `asteroid-0.6.1rc0/asteroid/utils/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/utils/generic_utils.py` & `asteroid-0.6.1rc0/asteroid/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/utils/hub_utils.py` & `asteroid-0.6.1rc0/asteroid/utils/hub_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "brijmohan/ConvTasNet_Libri1Mix_enhsingle": "https://zenodo.org/record/3970768/files/model.pth?download=1",
     "groadabike/ConvTasNet_DAMP-VSEP_enhboth": "https://zenodo.org/record/3994193/files/model.pth?download=1",
     "popcornell/DeMask_Surgical_mask_speech_enhancement_v1": "https://zenodo.org/record/3997047/files/model.pth?download=1",
     "popcornell/DPRNNTasNet_WHAM_enhancesingle": "https://zenodo.org/record/3998647/files/model.pth?download=1",
     "tmirzaev-dotcom/ConvTasNet_Libri3Mix_sepnoisy": "https://zenodo.org/record/4020529/files/model.pth?download=1",
     "mhu-coder/ConvTasNet_Libri1Mix_enhsingle": "https://zenodo.org/record/4301955/files/model.pth?download=1",
     "r-sawata/XUMX_MUSDB18_music_separation": "https://zenodo.org/record/4704231/files/pretrained_xumx.pth?download=1",
+    "r-sawata/XUMXL_MUSDB18_music_separation": "https://zenodo.org/record/7128659/files/pretrained_xumxl.pth?download=1",
 }
 
 SR_HASHTABLE = {k: 8000.0 if not "DeMask" in k else 16000.0 for k in MODELS_URLS_HASHTABLE}
 
 
 def cached_download(filename_or_url):
     """Download from URL and cache the result in ASTEROID_CACHE.
@@ -61,23 +62,23 @@
         # and  julien-c/DPRNNTasNet-ks16_WHAM_sepclean@main supports specifying a commit/branch/tag.
         if "@" in filename_or_url:
             model_id = filename_or_url.split("@")[0]
             revision = filename_or_url.split("@")[1]
         else:
             model_id = filename_or_url
             revision = None
-        url = huggingface_hub.hf_hub_url(
-            model_id, filename=huggingface_hub.PYTORCH_WEIGHTS_NAME, revision=revision
-        )
-        return huggingface_hub.cached_download(
-            url,
+        return huggingface_hub.hf_hub_download(
+            repo_id=model_id,
+            filename=huggingface_hub.PYTORCH_WEIGHTS_NAME,
             cache_dir=get_cache_dir(),
+            revision=revision,
             library_name="asteroid",
             library_version=asteroid_version,
         )
+
     cached_filename = url_to_filename(url)
     cached_dir = os.path.join(get_cache_dir(), cached_filename)
     cached_path = os.path.join(cached_dir, "model.pth")
 
     os.makedirs(cached_dir, exist_ok=True)
     if not os.path.isfile(cached_path):
         hub.download_url_to_file(url, cached_path)
```

### Comparing `asteroid-0.6.0rc0/asteroid/utils/parser_utils.py` & `asteroid-0.6.1rc0/asteroid/utils/parser_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import argparse
+import platform
+from packaging.version import parse as parse_version
 
 
 def prepare_parser_from_dict(dic, parser=None):
     """Prepare an argparser from a dictionary.
 
     Args:
         dic (dict): Two-level config dictionary with unique bottom-level keys.
@@ -49,27 +51,27 @@
     if isfloat(value):
         return float(value)
     elif isinstance(value, str):
         return value
 
 
 def str2bool(value):
-    """ Type to convert strings to Boolean (returns input if not boolean) """
+    """Type to convert strings to Boolean (returns input if not boolean)"""
     if not isinstance(value, str):
         return value
     if value.lower() in ("yes", "true", "y", "1"):
         return True
     elif value.lower() in ("no", "false", "n", "0"):
         return False
     else:
         return value
 
 
 def str2bool_arg(value):
-    """ Argparse type to convert strings to Boolean """
+    """Argparse type to convert strings to Boolean"""
     value = str2bool(value)
     if isinstance(value, bool):
         return value
     raise argparse.ArgumentTypeError("Boolean value expected.")
 
 
 def isfloat(value):
@@ -128,12 +130,17 @@
             direct output `parser.parse_args()`.
     """
     args = parser.parse_args(args=args)
     args_dic = {}
     for group in parser._action_groups:
         group_dict = {a.dest: getattr(args, a.dest, None) for a in group._group_actions}
         args_dic[group.title] = group_dict
-    args_dic["main_args"] = args_dic["optional arguments"]
-    del args_dic["optional arguments"]
+    opt_args_key = (
+        "optional arguments"
+        if parse_version(platform.python_version()) < parse_version("3.10")
+        else "options"
+    )
+    args_dic["main_args"] = args_dic[opt_args_key]
+    del args_dic[opt_args_key]
     if return_plain_args:
         return args_dic, args
     return args_dic
```

### Comparing `asteroid-0.6.0rc0/asteroid/utils/test_utils.py` & `asteroid-0.6.1rc0/asteroid/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid/utils/torch_utils.py` & `asteroid-0.6.1rc0/asteroid/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `asteroid-0.6.0rc0/asteroid.egg-info/PKG-INFO` & `asteroid-0.6.1rc0/asteroid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: asteroid
-Version: 0.6.0rc0
+Version: 0.6.1rc0
 Summary: PyTorch-based audio source separation toolkit
 Home-page: https://github.com/asteroid-team/asteroid
 Author: Manuel Pariente
 Author-email: manuel.pariente@loria.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -128,14 +127,15 @@
 * [x] [DualPathRNN](./egs/wham/DPRNN) ([Luo et al.](https://arxiv.org/abs/1910.06379))
 * [x] [Two step learning](./egs/wham/TwoStep)([Tzinis et al.](https://arxiv.org/abs/1910.09804))
 * [x] [SudoRMRFNet](./asteroid/models/sudormrf.py) ([Tzinis et al.](https://arxiv.org/abs/2007.06833))
 * [x] [DPTNet](./asteroid/models/dptnet.py) ([Chen et al.](https://arxiv.org/abs/2007.13975))
 * [x] [DCCRNet](./asteroid/models/dccrnet.py) ([Hu et al.](https://arxiv.org/abs/2008.00264))
 * [x] [DCUNet](./asteroid/models/dcunet.py) ([Choi et al.](https://arxiv.org/abs/1903.03107))
 * [x] [CrossNet-Open-Unmix](./asteroid/models/x_umx.py) ([Sawata et al.](https://arxiv.org/abs/2010.04228))
+* [x] [Multi-Decoder DPRNN](./egs/wsj0-mix-var/Multi-Decoder-DPRNN) ([Zhu et al.](http://www.isle.illinois.edu/speech_web_lg/pubs/2021/zhu2021multi.pdf))
 * [ ] Open-Unmix (coming) ([Stöter et al.](https://sigsep.github.io/open-unmix/))
 * [ ] Wavesplit (coming) ([Zeghidour et al.](https://arxiv.org/abs/2002.08933))
 
 ## Supported datasets
 ([↑up to contents](#contents))
 * [x] [WSJ0-2mix](./egs/wsj0-mix) / WSJ03mix ([Hershey et al.](https://arxiv.org/abs/1508.04306))
 * [x] [WHAM](./egs/wham) ([Wichern et al.](https://arxiv.org/abs/1907.01160))
@@ -225,9 +225,7 @@
 [codecov]: https://codecov.io/gh/asteroid-team/asteroid
 [slack-badge]: https://img.shields.io/badge/slack-chat-green.svg?logo=slack
 [slack-invite]: https://join.slack.com/t/asteroid-dev/shared_invite/zt-cn9y85t3-QNHXKD1Et7qoyzu1Ji5bcA
 
 [comment]: <> (Others)
 [issue]: https://github.com/asteroid-team/asteroid/issues/new
 [pr]: https://github.com/asteroid-team/asteroid/compare
-
-
```

### Comparing `asteroid-0.6.0rc0/asteroid.egg-info/SOURCES.txt` & `asteroid-0.6.1rc0/asteroid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,21 @@
 asteroid.egg-info/SOURCES.txt
 asteroid.egg-info/dependency_links.txt
 asteroid.egg-info/entry_points.txt
 asteroid.egg-info/requires.txt
 asteroid.egg-info/top_level.txt
 asteroid/data/__init__.py
 asteroid/data/avspeech_dataset.py
-asteroid/data/basic_design.py
 asteroid/data/dampvsep_dataset.py
 asteroid/data/dns_dataset.py
 asteroid/data/fuss_dataset.py
 asteroid/data/kinect_wsj.py
 asteroid/data/librimix_dataset.py
 asteroid/data/musdb18_dataset.py
-asteroid/data/scaler.py
 asteroid/data/sms_wsj_dataset.py
-asteroid/data/toy_data.py
 asteroid/data/utils.py
 asteroid/data/vad_dataset.py
 asteroid/data/wham_dataset.py
 asteroid/data/whamr_dataset.py
 asteroid/data/wsj0_mix.py
 asteroid/dsp/__init__.py
 asteroid/dsp/beamforming.py
```

### Comparing `asteroid-0.6.0rc0/setup.py` & `asteroid-0.6.1rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,29 +34,29 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     python_requires=">=3.6",
     install_requires=[
         # From requirements/torchhub.txt
         "numpy>=1.16.4",
-        "scipy>=1.1.0",
-        "torch>=1.8.0",
+        "scipy>=1.10.1",
+        "torch>=1.8.0,<2.0.0",
         "asteroid-filterbanks>=0.4.0",
         "SoundFile>=0.10.2",
         "huggingface_hub>=0.0.2",
         # From requirements/install.txt
         "PyYAML>=5.0",
         "pandas>=0.23.4",
-        "pytorch-lightning>=1.5.0",
+        "pytorch-lightning>=1.5.0,<=1.7.7",
+        "torchmetrics<=0.11.4",
         "torchaudio>=0.5.0",
         "pb_bss_eval>=0.0.2",
         "torch_stoi>=0.1.2",
         "torch_optimizer>=0.0.1a12,<0.2.0",
         "julius",
-        "torchmetrics<0.8.0",
     ],
     entry_points={
         "console_scripts": [
             "asteroid-upload=asteroid.scripts.asteroid_cli:upload",
             "asteroid-infer=asteroid.scripts.asteroid_cli:infer",
             "asteroid-register-sr=asteroid.scripts.asteroid_cli:register_sample_rate",
             "asteroid-versions=asteroid.scripts.asteroid_versions:print_versions",
```

