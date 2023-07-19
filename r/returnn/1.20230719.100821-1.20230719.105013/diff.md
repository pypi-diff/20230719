# Comparing `tmp/returnn-1.20230719.100821.tar.gz` & `tmp/returnn-1.20230719.105013.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230719.100821.tar", last modified: Wed Jul 19 08:45:23 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230719.105013.tar", last modified: Wed Jul 19 09:02:40 2023, max compression
```

## Comparing `returnn-1.20230719.100821.tar` & `returnn-1.20230719.105013.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 08:45:04.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-19 08:45:08.000000 returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40521 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   101803 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   158171 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   146879 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   302119 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    37372 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73572 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18501 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:45:23.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-19 08:45:01.000000 returnn-1.20230719.100821/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 09:02:16.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-19 09:02:20.000000 returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40521 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101797 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158171 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146879 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302119 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37372 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73572 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18501 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:40.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-19 09:02:14.000000 returnn-1.20230719.105013/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230719.100821/.gitignore` & `returnn-1.20230719.105013/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/.gitmodules` & `returnn-1.20230719.105013/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/CHANGELOG.md` & `returnn-1.20230719.105013/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/CODEOWNERS` & `returnn-1.20230719.105013/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/CONTRIBUTING.md` & `returnn-1.20230719.105013/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/LICENSE` & `returnn-1.20230719.105013/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/MANIFEST.in` & `returnn-1.20230719.105013/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/PKG-INFO` & `returnn-1.20230719.105013/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230719.100821
+Version: 1.20230719.105013
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230719.100821/README.rst` & `returnn-1.20230719.105013/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/__init__.py` & `returnn-1.20230719.105013/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/12AX.cluster_map` & `returnn-1.20230719.105013/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-fwd.config` & `returnn-1.20230719.105013/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-horovod-mpi.py` & `returnn-1.20230719.105013/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230719.105013/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-hyper-param-tuning.config` & `returnn-1.20230719.105013/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-iter-dataset.py` & `returnn-1.20230719.105013/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-list-devices.py` & `returnn-1.20230719.105013/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-lua-torch-layer.config` & `returnn-1.20230719.105013/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230719.105013/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-returnn-as-framework.py` & `returnn-1.20230719.105013/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-rf.config` & `returnn-1.20230719.105013/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-rhn-enwik8.config` & `returnn-1.20230719.105013/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-sprint-interface.py` & `returnn-1.20230719.105013/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-att-copy.config` & `returnn-1.20230719.105013/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-attention.config` & `returnn-1.20230719.105013/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-enc-dec.config` & `returnn-1.20230719.105013/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230719.105013/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230719.105013/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230719.105013/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230719.105013/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230719.105013/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-rec-self-att.config` & `returnn-1.20230719.105013/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230719.105013/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230719.105013/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230719.105013/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-torch.config` & `returnn-1.20230719.105013/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230719.105013/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/demo.sh` & `returnn-1.20230719.105013/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230719.105013/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/README.txt` & `returnn-1.20230719.105013/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/config_demo` & `returnn-1.20230719.105013/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230719.105013/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/config_real` & `returnn-1.20230719.105013/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230719.105013/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/decode.py` & `returnn-1.20230719.105013/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230719.105013/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230719.105013/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230719.105013/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230719.105013/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230719.105013/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230719.105013/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230719.105013/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230719.105013/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/__init__.py` & `returnn-1.20230719.105013/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/__main__.py` & `returnn-1.20230719.105013/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/__old_mod_loader__.py` & `returnn-1.20230719.105013/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/__setup__.py` & `returnn-1.20230719.105013/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/config.py` & `returnn-1.20230719.105013/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/audio.py` & `returnn-1.20230719.105013/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/basic.py` & `returnn-1.20230719.105013/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/bundle_file.py` & `returnn-1.20230719.105013/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/cached.py` & `returnn-1.20230719.105013/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/cached2.py` & `returnn-1.20230719.105013/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/generating.py` & `returnn-1.20230719.105013/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/hdf.py` & `returnn-1.20230719.105013/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/lm.py` & `returnn-1.20230719.105013/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/map.py` & `returnn-1.20230719.105013/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/meta.py` & `returnn-1.20230719.105013/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/multi_proc.py` & `returnn-1.20230719.105013/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/normalization_data.py` & `returnn-1.20230719.105013/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/numpy_dump.py` & `returnn-1.20230719.105013/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/raw_wav.py` & `returnn-1.20230719.105013/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/sprint.py` & `returnn-1.20230719.105013/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/stereo.py` & `returnn-1.20230719.105013/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230719.105013/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/datasets/util/vocabulary.py` & `returnn-1.20230719.105013/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/engine/base.py` & `returnn-1.20230719.105013/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/engine/batch.py` & `returnn-1.20230719.105013/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230719.105013/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/edit.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/select.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/transform.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/extern/graph_editor/util.py` & `returnn-1.20230719.105013/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/forward_iface.py` & `returnn-1.20230719.105013/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/__init__.py` & `returnn-1.20230719.105013/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/_backend.py` & `returnn-1.20230719.105013/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/_numpy_backend.py` & `returnn-1.20230719.105013/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/_utils.py` & `returnn-1.20230719.105013/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/array_.py` & `returnn-1.20230719.105013/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/attention.py` & `returnn-1.20230719.105013/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/cond.py` & `returnn-1.20230719.105013/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/const.py` & `returnn-1.20230719.105013/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/container.py` & `returnn-1.20230719.105013/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/conv.py` & `returnn-1.20230719.105013/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/device.py` & `returnn-1.20230719.105013/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/dims.py` & `returnn-1.20230719.105013/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/dropout.py` & `returnn-1.20230719.105013/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/dtype.py` & `returnn-1.20230719.105013/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/encoder/base.py` & `returnn-1.20230719.105013/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/encoder/conformer.py` & `returnn-1.20230719.105013/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/init.py` & `returnn-1.20230719.105013/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/linear.py` & `returnn-1.20230719.105013/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/loop.py` & `returnn-1.20230719.105013/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/loss.py` & `returnn-1.20230719.105013/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/math_.py` & `returnn-1.20230719.105013/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/matmul.py` & `returnn-1.20230719.105013/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/module.py` & `returnn-1.20230719.105013/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/normalization.py` & `returnn-1.20230719.105013/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/parameter.py` & `returnn-1.20230719.105013/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/rand.py` & `returnn-1.20230719.105013/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/rec.py` & `returnn-1.20230719.105013/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/reduce.py` & `returnn-1.20230719.105013/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/run_ctx.py` & `returnn-1.20230719.105013/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/signal.py` & `returnn-1.20230719.105013/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/state.py` & `returnn-1.20230719.105013/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/tensor_array.py` & `returnn-1.20230719.105013/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/frontend/types.py` & `returnn-1.20230719.105013/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/import_/common.py` & `returnn-1.20230719.105013/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/import_/git.py` & `returnn-1.20230719.105013/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/import_/import_.py` & `returnn-1.20230719.105013/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/learning_rate_control.py` & `returnn-1.20230719.105013/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/log.py` & `returnn-1.20230719.105013/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/native_op.cpp` & `returnn-1.20230719.105013/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/native_op.py` & `returnn-1.20230719.105013/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/pretrain.py` & `returnn-1.20230719.105013/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/sprint/cache.py` & `returnn-1.20230719.105013/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/sprint/control.py` & `returnn-1.20230719.105013/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/sprint/error_signals.py` & `returnn-1.20230719.105013/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/sprint/extern_interface.py` & `returnn-1.20230719.105013/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/sprint/interface.py` & `returnn-1.20230719.105013/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/_dim_extra.py` & `returnn-1.20230719.105013/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -988,5376 +988,5376 @@
 00003db0: 7261 6d20 626f 6f6c 2061 6c6c 6f77 5f6e  ram bool allow_n
 00003dc0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
 00003dd0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
 00003de0: 7365 6c66 2e63 616e 5f62 655f 7573 6564  self.can_be_used
 00003df0: 5f61 735f 6469 6d28 290a 2020 2020 2020  _as_dim().      
 00003e00: 2020 6966 2073 656c 662e 6261 7463 6820    if self.batch 
 00003e10: 3d3d 2062 6174 6368 2061 6e64 2073 656c  == batch and sel
-00003e20: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-00003e30: 7478 203d 3d20 6374 7820 616e 6420 7365  tx == ctx and se
-00003e40: 6c66 2e64 796e 5f73 697a 655f 6578 743a  lf.dyn_size_ext:
-00003e50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003e60: 662e 5f76 616c 6964 6174 655f 696e 5f63  f._validate_in_c
-00003e70: 7572 7265 6e74 5f67 7261 7068 2829 0a20  urrent_graph(). 
-00003e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003e90: 5f6d 6179 6265 5f75 7064 6174 6528 290a  _maybe_update().
-00003ea0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003eb0: 656c 662e 6261 7463 6820 3d3d 2062 6174  elf.batch == bat
-00003ec0: 6368 2061 6e64 2073 656c 662e 636f 6e74  ch and self.cont
-00003ed0: 726f 6c5f 666c 6f77 5f63 7478 203d 3d20  rol_flow_ctx == 
-00003ee0: 6374 7820 616e 6420 7365 6c66 2e64 796e  ctx and self.dyn
-00003ef0: 5f73 697a 655f 6578 743a 2020 2320 6368  _size_ext:  # ch
-00003f00: 6563 6b20 6167 6169 6e0a 2020 2020 2020  eck again.      
-00003f10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003f20: 2073 656c 660a 2020 2020 2020 2020 6966   self.        if
-00003f30: 2073 656c 662e 6973 5f62 6174 6368 5f64   self.is_batch_d
-00003f40: 696d 2829 3a0a 2020 2020 2020 2020 2020  im():.          
-00003f50: 2020 2320 5765 2069 676e 6f72 6520 7468    # We ignore th
-00003f60: 6520 6374 7820 666f 7220 7468 6520 6261  e ctx for the ba
-00003f70: 7463 6820 6469 6d20 6375 7272 656e 746c  tch dim currentl
-00003f80: 792e 0a20 2020 2020 2020 2020 2020 2069  y..            i
-00003f90: 6620 7365 6c66 2e62 6174 6368 203d 3d20  f self.batch == 
-00003fa0: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
-00003fb0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00003fc0: 6c66 0a20 2020 2020 2020 2020 2020 2069  lf.            i
-00003fd0: 6620 6261 7463 682e 6973 5f67 6c6f 6261  f batch.is_globa
-00003fe0: 6c5f 6261 7463 6828 293a 0a20 2020 2020  l_batch():.     
-00003ff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004000: 6e20 5f64 2e62 6174 6368 5f64 696d 2020  n _d.batch_dim  
-00004010: 2320 7265 7573 6520 676c 6f62 616c 2062  # reuse global b
-00004020: 6174 6368 2064 696d 2069 6620 706f 7373  atch dim if poss
-00004030: 6962 6c65 0a20 2020 2020 2020 2020 2020  ible.           
-00004040: 2072 6574 7572 6e20 5f64 2e44 696d 286b   return _d.Dim(k
-00004050: 696e 643d 4469 6d54 7970 6573 2e42 6174  ind=DimTypes.Bat
-00004060: 6368 2c20 6465 7363 7269 7074 696f 6e3d  ch, description=
-00004070: 2262 6174 6368 3a25 7322 2025 2062 6174  "batch:%s" % bat
-00004080: 6368 2e73 686f 7274 5f72 6570 7228 292c  ch.short_repr(),
-00004090: 2062 6174 6368 3d62 6174 6368 2c20 6469   batch=batch, di
-000040a0: 6d65 6e73 696f 6e3d 4e6f 6e65 290a 2020  mension=None).  
-000040b0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-000040c0: 662e 6973 5f64 796e 616d 6963 2829 3a0a  f.is_dynamic():.
-000040d0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-000040e0: 2073 7461 7469 6320 6469 6d2c 206e 6f20   static dim, no 
-000040f0: 6566 6665 6374 2e0a 2020 2020 2020 2020  effect..        
-00004100: 2020 2020 6173 7365 7274 206e 6f74 2073      assert not s
-00004110: 656c 662e 6261 7463 680a 2020 2020 2020  elf.batch.      
-00004120: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004130: 660a 2020 2020 2020 2020 6966 2062 6174  f.        if bat
-00004140: 6368 2e69 735f 6272 6f61 6463 6173 7428  ch.is_broadcast(
-00004150: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00004160: 6574 7572 6e20 7365 6c66 2020 2320 6a75  eturn self  # ju
-00004170: 7374 206c 6561 7665 2061 732d 6973 2e20  st leave as-is. 
-00004180: 7368 6f75 6c64 206e 6f74 206d 6174 7465  should not matte
-00004190: 722e 0a20 2020 2020 2020 2069 6620 7365  r..        if se
-000041a0: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
-000041b0: 2020 2020 2020 2073 616d 655f 6261 7365         same_base
-000041c0: 203d 2073 656c 662e 6765 745f 7361 6d65   = self.get_same
-000041d0: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
-000041e0: 2020 2020 7361 6d65 5f62 6173 652e 5f76      same_base._v
-000041f0: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
-00004200: 6e74 5f67 7261 7068 2829 0a20 2020 2020  nt_graph().     
-00004210: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-00004220: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-00004230: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-00004240: 2020 2020 6966 2073 616d 655f 6261 7365      if same_base
-00004250: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
-00004260: 2020 2020 2020 2020 2066 726f 6d20 7265           from re
-00004270: 7475 726e 6e2e 7466 2e75 7469 6c2e 6461  turnn.tf.util.da
-00004280: 7461 2069 6d70 6f72 7420 436f 6e74 726f  ta import Contro
-00004290: 6c46 6c6f 7743 6f6e 7465 7874 0a0a 2020  lFlowContext..  
-000042a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000042b0: 7220 6374 785f 2069 6e20 436f 6e74 726f  r ctx_ in Contro
-000042c0: 6c46 6c6f 7743 6f6e 7465 7874 2e61 6273  lFlowContext.abs
-000042d0: 5f63 7478 5f73 7461 636b 5f77 6974 685f  _ctx_stack_with_
-000042e0: 726f 6f74 2863 7478 293a 0a20 2020 2020  root(ctx):.     
-000042f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004300: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-00004310: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004330: 2020 2020 7461 6720 3d20 7361 6d65 5f62      tag = same_b
-00004340: 6173 652e 5f65 7874 7261 2e73 616d 655f  ase._extra.same_
-00004350: 666f 725f 6261 7463 685f 6374 782e 6765  for_batch_ctx.ge
-00004360: 7428 2862 6174 6368 2c20 6374 785f 292c  t((batch, ctx_),
-00004370: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
-00004380: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
-00004390: 6720 616e 6420 7461 672e 5f63 616e 5f75  g and tag._can_u
-000043a0: 7365 5f69 6e5f 6374 7828 6374 7829 2061  se_in_ctx(ctx) a
-000043b0: 6e64 2074 6167 2e5f 7661 6c69 6461 7465  nd tag._validate
-000043c0: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
-000043d0: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
-000043e0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-000043f0: 6572 7420 280a 2020 2020 2020 2020 2020  ert (.          
-00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2020 7461 672e 6261 7463 6820 3d3d 2062    tag.batch == b
-00004420: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-00004430: 2020 2020 2020 2020 2020 2020 2029 2020               )  
-00004440: 2320 736f 6d65 2063 6f64 6520 7570 6461  # some code upda
-00004450: 7465 6420 6261 7463 6820 6469 7265 6374  ted batch direct
-00004460: 6c79 2028 696e 636f 7272 6563 746c 7929  ly (incorrectly)
-00004470: 2061 6e64 2063 6f75 6c64 2074 7269 6767   and could trigg
-00004480: 6572 2074 6869 730a 2020 2020 2020 2020  er this.        
-00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044a0: 7265 7475 726e 2074 6167 0a20 2020 2020  return tag.     
-000044b0: 2020 2020 2020 2069 6620 7361 6d65 5f62         if same_b
-000044c0: 6173 652e 6261 7463 6820 3d3d 2062 6174  ase.batch == bat
-000044d0: 6368 2061 6e64 2073 616d 655f 6261 7365  ch and same_base
-000044e0: 2e5f 6361 6e5f 7573 655f 696e 5f63 7478  ._can_use_in_ctx
-000044f0: 2863 7478 2920 616e 6420 7361 6d65 5f62  (ctx) and same_b
-00004500: 6173 652e 6479 6e5f 7369 7a65 5f65 7874  ase.dyn_size_ext
-00004510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004520: 2020 7265 7475 726e 2073 616d 655f 6261    return same_ba
-00004530: 7365 0a20 2020 2020 2020 2065 6c73 653a  se.        else:
-00004540: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
-00004550: 655f 6261 7365 203d 2073 656c 660a 2020  e_base = self.  
-00004560: 2020 2020 2020 7361 6d65 5f62 6173 655f        same_base_
-00004570: 6578 7472 6120 3d20 7361 6d65 5f62 6173  extra = same_bas
-00004580: 652e 5f6d 616b 655f 6578 7472 6128 290a  e._make_extra().
-00004590: 2020 2020 2020 2020 2320 4f6b 2c20 6e6f          # Ok, no
-000045a0: 7468 696e 6720 6d61 7463 6869 6e67 2066  thing matching f
-000045b0: 6f75 6e64 2e0a 2020 2020 2020 2020 6966  ound..        if
-000045c0: 2063 7478 3a0a 2020 2020 2020 2020 2020   ctx:.          
-000045d0: 2020 2320 4368 6563 6b20 6966 2074 6865    # Check if the
-000045e0: 2063 7478 2069 7320 7265 616c 6c79 2072   ctx is really r
-000045f0: 656c 6576 616e 742c 2077 6865 6e20 7468  elevant, when th
-00004600: 6973 2069 7320 6465 7269 7665 6420 6672  is is derived fr
-00004610: 6f6d 206f 7468 6572 2074 6167 732e 0a20  om other tags.. 
-00004620: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-00004630: 6564 5f62 6173 6573 203d 2073 616d 655f  ed_bases = same_
-00004640: 6261 7365 2e67 6574 5f64 6572 6976 6564  base.get_derived
-00004650: 5f62 6173 6573 5f73 6574 2829 0a20 2020  _bases_set().   
-00004660: 2020 2020 2020 2020 2064 6572 6976 6564           derived
-00004670: 5f62 6173 6573 2e72 656d 6f76 6528 7361  _bases.remove(sa
-00004680: 6d65 5f62 6173 6529 0a20 2020 2020 2020  me_base).       
-00004690: 2020 2020 2069 6620 6465 7269 7665 645f       if derived_
-000046a0: 6261 7365 733a 0a20 2020 2020 2020 2020  bases:.         
-000046b0: 2020 2020 2020 2064 6572 6976 6564 5f63         derived_c
-000046c0: 7478 7320 3d20 7365 7428 290a 2020 2020  txs = set().    
-000046d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000046e0: 6420 696e 2064 6572 6976 6564 5f62 6173  d in derived_bas
-000046f0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00004700: 2020 2020 2020 2020 7769 7468 2075 7469          with uti
-00004710: 6c2e 6775 6172 645f 696e 6669 6e69 7465  l.guard_infinite
-00004720: 5f72 6563 7572 7369 6f6e 285f 642e 4469  _recursion(_d.Di
-00004730: 6d2e 6765 745f 666f 725f 6261 7463 685f  m.get_for_batch_
-00004740: 6374 782c 2064 293a 0a20 2020 2020 2020  ctx, d):.       
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2064 203d 2064 2e67 6574 5f66 6f72 5f62   d = d.get_for_b
-00004770: 6174 6368 5f63 7478 2862 6174 6368 3d62  atch_ctx(batch=b
-00004780: 6174 6368 2c20 6374 783d 6374 7829 0a20  atch, ctx=ctx). 
-00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047a0: 2020 2069 6620 642e 636f 6e74 726f 6c5f     if d.control_
-000047b0: 666c 6f77 5f63 7478 3a0a 2020 2020 2020  flow_ctx:.      
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2020 6465 7269 7665 645f 6374 7873 2e61    derived_ctxs.a
-000047e0: 6464 2864 2e63 6f6e 7472 6f6c 5f66 6c6f  dd(d.control_flo
-000047f0: 775f 6374 7829 0a20 2020 2020 2020 2020  w_ctx).         
-00004800: 2020 2020 2020 2069 6620 6e6f 7420 6465         if not de
-00004810: 7269 7665 645f 6374 7873 3a0a 2020 2020  rived_ctxs:.    
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 6374 7820 3d20 4e6f 6e65 0a20 2020 2020  ctx = None.     
-00004840: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00004850: 6c65 6e28 6465 7269 7665 645f 6374 7873  len(derived_ctxs
-00004860: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
-00004870: 2020 2020 2020 2020 2020 2020 6374 7820              ctx 
-00004880: 3d20 6465 7269 7665 645f 6374 7873 2e70  = derived_ctxs.p
-00004890: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
-000048a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000048c0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-000048d0: 7465 6445 7272 6f72 2822 6e6f 7420 7965  tedError("not ye
-000048e0: 7420 696d 706c 656d 656e 7465 643a 206d  t implemented: m
-000048f0: 756c 7469 706c 6520 6465 7269 7665 6420  ultiple derived 
-00004900: 6374 7873 3a20 2572 2220 2520 2864 6572  ctxs: %r" % (der
-00004910: 6976 6564 5f63 7478 732c 2929 0a20 2020  ived_ctxs,)).   
-00004920: 2020 2020 2064 796e 5f73 697a 655f 6578       dyn_size_ex
-00004930: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
-00004940: 2023 204d 6179 6265 2077 6520 6861 7665   # Maybe we have
-00004950: 2073 7468 2077 6974 6820 7468 6520 6261   sth with the ba
-00004960: 7365 2062 6174 6368 2077 6974 686f 7574  se batch without
-00004970: 2062 6561 6d20 6f72 2070 6164 6465 6420   beam or padded 
-00004980: 6261 7463 6820 7768 6963 6820 7765 2063  batch which we c
-00004990: 616e 2065 7874 656e 642e 0a20 2020 2020  an extend..     
-000049a0: 2020 2069 6620 6261 7463 6820 213d 2062     if batch != b
-000049b0: 6174 6368 2e67 6574 5f67 6c6f 6261 6c5f  atch.get_global_
-000049c0: 6261 7365 2829 3a0a 2020 2020 2020 2020  base():.        
-000049d0: 2020 2020 6261 7463 685f 6261 7365 203d      batch_base =
-000049e0: 2062 6174 6368 2e67 6574 5f67 6c6f 6261   batch.get_globa
-000049f0: 6c5f 6261 7365 2829 0a20 2020 2020 2020  l_base().       
-00004a00: 2020 2020 2062 6173 655f 6361 6e5f 7573       base_can_us
-00004a10: 655f 696e 5f63 7478 203d 204e 6f6e 6520  e_in_ctx = None 
-00004a20: 2023 2074 7970 653a 204f 7074 696f 6e61   # type: Optiona
-00004a30: 6c5b 5f64 2e44 696d 5d0a 2020 2020 2020  l[_d.Dim].      
-00004a40: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-00004a50: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-00004a60: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
-00004a70: 2020 2069 6620 7361 6d65 5f62 6173 652e     if same_base.
-00004a80: 6261 7463 6820 3d3d 2062 6174 6368 5f62  batch == batch_b
-00004a90: 6173 6520 616e 6420 7361 6d65 5f62 6173  ase and same_bas
-00004aa0: 652e 5f63 616e 5f75 7365 5f69 6e5f 6374  e._can_use_in_ct
-00004ab0: 7828 6374 7829 2061 6e64 2073 616d 655f  x(ctx) and same_
-00004ac0: 6261 7365 2e64 796e 5f73 697a 655f 6578  base.dyn_size_ex
-00004ad0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00004ae0: 2020 2062 6173 655f 6361 6e5f 7573 655f     base_can_use_
-00004af0: 696e 5f63 7478 203d 2073 616d 655f 6261  in_ctx = same_ba
-00004b00: 7365 0a20 2020 2020 2020 2020 2020 2065  se.            e
-00004b10: 6c69 6620 7361 6d65 5f62 6173 652e 5f65  lif same_base._e
-00004b20: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
-00004b30: 2020 2020 2020 6672 6f6d 2072 6574 7572        from retur
-00004b40: 6e6e 2e74 662e 7574 696c 2e64 6174 6120  nn.tf.util.data 
-00004b50: 696d 706f 7274 2043 6f6e 7472 6f6c 466c  import ControlFl
-00004b60: 6f77 436f 6e74 6578 740a 0a20 2020 2020  owContext..     
-00004b70: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00004b80: 7478 5f20 696e 2043 6f6e 7472 6f6c 466c  tx_ in ControlFl
-00004b90: 6f77 436f 6e74 6578 742e 6162 735f 6374  owContext.abs_ct
-00004ba0: 785f 7374 6163 6b5f 7769 7468 5f72 6f6f  x_stack_with_roo
-00004bb0: 7428 6374 7829 3a0a 2020 2020 2020 2020  t(ctx):.        
-00004bc0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-00004bd0: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
-00004be0: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2074 6167 203d 2073 616d 655f 6261 7365   tag = same_base
-00004c10: 2e5f 6578 7472 612e 7361 6d65 5f66 6f72  ._extra.same_for
-00004c20: 5f62 6174 6368 5f63 7478 2e67 6574 2828  _batch_ctx.get((
-00004c30: 6261 7463 685f 6261 7365 2c20 6374 785f  batch_base, ctx_
-00004c40: 292c 204e 6f6e 6529 0a20 2020 2020 2020  ), None).       
-00004c50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004c60: 7461 6720 616e 6420 7461 672e 5f63 616e  tag and tag._can
-00004c70: 5f75 7365 5f69 6e5f 6374 7828 6374 7829  _use_in_ctx(ctx)
-00004c80: 2061 6e64 2074 6167 2e5f 7661 6c69 6461   and tag._valida
-00004c90: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
-00004ca0: 6170 6828 2920 616e 6420 7461 672e 6479  aph() and tag.dy
-00004cb0: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2020 6261 7365 5f63 616e 5f75 7365      base_can_use
-00004ce0: 5f69 6e5f 6374 7820 3d20 7461 670a 2020  _in_ctx = tag.  
+00003e20: 662e 5f63 616e 5f75 7365 5f69 6e5f 6374  f._can_use_in_ct
+00003e30: 7828 6374 7829 2061 6e64 2073 656c 662e  x(ctx) and self.
+00003e40: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+00003e50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00003e60: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
+00003e70: 656e 745f 6772 6170 6828 290a 2020 2020  ent_graph().    
+00003e80: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
+00003e90: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
+00003ea0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00003eb0: 2e62 6174 6368 203d 3d20 6261 7463 6820  .batch == batch 
+00003ec0: 616e 6420 7365 6c66 2e5f 6361 6e5f 7573  and self._can_us
+00003ed0: 655f 696e 5f63 7478 2863 7478 2920 616e  e_in_ctx(ctx) an
+00003ee0: 6420 7365 6c66 2e64 796e 5f73 697a 655f  d self.dyn_size_
+00003ef0: 6578 743a 2020 2320 6368 6563 6b20 6167  ext:  # check ag
+00003f00: 6169 6e0a 2020 2020 2020 2020 2020 2020  ain.            
+00003f10: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00003f20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003f30: 6973 5f62 6174 6368 5f64 696d 2829 3a0a  is_batch_dim():.
+00003f40: 2020 2020 2020 2020 2020 2020 2320 5765              # We
+00003f50: 2069 676e 6f72 6520 7468 6520 6374 7820   ignore the ctx 
+00003f60: 666f 7220 7468 6520 6261 7463 6820 6469  for the batch di
+00003f70: 6d20 6375 7272 656e 746c 792e 0a20 2020  m currently..   
+00003f80: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00003f90: 2e62 6174 6368 203d 3d20 6261 7463 683a  .batch == batch:
+00003fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003fb0: 2072 6574 7572 6e20 7365 6c66 0a20 2020   return self.   
+00003fc0: 2020 2020 2020 2020 2069 6620 6261 7463           if batc
+00003fd0: 682e 6973 5f67 6c6f 6261 6c5f 6261 7463  h.is_global_batc
+00003fe0: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
+00003ff0: 2020 2020 2072 6574 7572 6e20 5f64 2e62       return _d.b
+00004000: 6174 6368 5f64 696d 2020 2320 7265 7573  atch_dim  # reus
+00004010: 6520 676c 6f62 616c 2062 6174 6368 2064  e global batch d
+00004020: 696d 2069 6620 706f 7373 6962 6c65 0a20  im if possible. 
+00004030: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00004040: 6e20 5f64 2e44 696d 286b 696e 643d 4469  n _d.Dim(kind=Di
+00004050: 6d54 7970 6573 2e42 6174 6368 2c20 6465  mTypes.Batch, de
+00004060: 7363 7269 7074 696f 6e3d 2262 6174 6368  scription="batch
+00004070: 3a25 7322 2025 2062 6174 6368 2e73 686f  :%s" % batch.sho
+00004080: 7274 5f72 6570 7228 292c 2062 6174 6368  rt_repr(), batch
+00004090: 3d62 6174 6368 2c20 6469 6d65 6e73 696f  =batch, dimensio
+000040a0: 6e3d 4e6f 6e65 290a 2020 2020 2020 2020  n=None).        
+000040b0: 6966 206e 6f74 2073 656c 662e 6973 5f64  if not self.is_d
+000040c0: 796e 616d 6963 2829 3a0a 2020 2020 2020  ynamic():.      
+000040d0: 2020 2020 2020 2320 4966 2073 7461 7469        # If stati
+000040e0: 6320 6469 6d2c 206e 6f20 6566 6665 6374  c dim, no effect
+000040f0: 2e0a 2020 2020 2020 2020 2020 2020 6173  ..            as
+00004100: 7365 7274 206e 6f74 2073 656c 662e 6261  sert not self.ba
+00004110: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
+00004120: 7265 7475 726e 2073 656c 660a 2020 2020  return self.    
+00004130: 2020 2020 6966 2062 6174 6368 2e69 735f      if batch.is_
+00004140: 6272 6f61 6463 6173 7428 293a 0a20 2020  broadcast():.   
+00004150: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004160: 7365 6c66 2020 2320 6a75 7374 206c 6561  self  # just lea
+00004170: 7665 2061 732d 6973 2e20 7368 6f75 6c64  ve as-is. should
+00004180: 206e 6f74 206d 6174 7465 722e 0a20 2020   not matter..   
+00004190: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
+000041a0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+000041b0: 2073 616d 655f 6261 7365 203d 2073 656c   same_base = sel
+000041c0: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
+000041d0: 290a 2020 2020 2020 2020 2020 2020 7361  ).            sa
+000041e0: 6d65 5f62 6173 652e 5f76 616c 6964 6174  me_base._validat
+000041f0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
+00004200: 7068 2829 0a20 2020 2020 2020 2020 2020  ph().           
+00004210: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+00004220: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+00004230: 720a 2020 2020 2020 2020 2020 2020 6966  r.            if
+00004240: 2073 616d 655f 6261 7365 2e5f 6578 7472   same_base._extr
+00004250: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
+00004260: 2020 2066 726f 6d20 7265 7475 726e 6e2e     from returnn.
+00004270: 7466 2e75 7469 6c2e 6461 7461 2069 6d70  tf.util.data imp
+00004280: 6f72 7420 436f 6e74 726f 6c46 6c6f 7743  ort ControlFlowC
+00004290: 6f6e 7465 7874 0a0a 2020 2020 2020 2020  ontext..        
+000042a0: 2020 2020 2020 2020 666f 7220 6374 785f          for ctx_
+000042b0: 2069 6e20 436f 6e74 726f 6c46 6c6f 7743   in ControlFlowC
+000042c0: 6f6e 7465 7874 2e61 6273 5f63 7478 5f73  ontext.abs_ctx_s
+000042d0: 7461 636b 5f77 6974 685f 726f 6f74 2863  tack_with_root(c
+000042e0: 7478 293a 0a20 2020 2020 2020 2020 2020  tx):.           
+000042f0: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
+00004300: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
+00004310: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
+00004320: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00004330: 6720 3d20 7361 6d65 5f62 6173 652e 5f65  g = same_base._e
+00004340: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
+00004350: 7463 685f 6374 782e 6765 7428 2862 6174  tch_ctx.get((bat
+00004360: 6368 2c20 6374 785f 292c 204e 6f6e 6529  ch, ctx_), None)
+00004370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004380: 2020 2020 2069 6620 7461 6720 616e 6420       if tag and 
+00004390: 7461 672e 5f63 616e 5f75 7365 5f69 6e5f  tag._can_use_in_
+000043a0: 6374 7828 6374 7829 2061 6e64 2074 6167  ctx(ctx) and tag
+000043b0: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+000043c0: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
+000043d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043e0: 2020 2020 2020 2061 7373 6572 7420 280a         assert (.
+000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004400: 2020 2020 2020 2020 2020 2020 7461 672e              tag.
+00004410: 6261 7463 6820 3d3d 2062 6174 6368 0a20  batch == batch. 
+00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004430: 2020 2020 2020 2029 2020 2320 736f 6d65         )  # some
+00004440: 2063 6f64 6520 7570 6461 7465 6420 6261   code updated ba
+00004450: 7463 6820 6469 7265 6374 6c79 2028 696e  tch directly (in
+00004460: 636f 7272 6563 746c 7929 2061 6e64 2063  correctly) and c
+00004470: 6f75 6c64 2074 7269 6767 6572 2074 6869  ould trigger thi
+00004480: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00004490: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000044a0: 2074 6167 0a20 2020 2020 2020 2020 2020   tag.           
+000044b0: 2069 6620 7361 6d65 5f62 6173 652e 6261   if same_base.ba
+000044c0: 7463 6820 3d3d 2062 6174 6368 2061 6e64  tch == batch and
+000044d0: 2073 616d 655f 6261 7365 2e5f 6361 6e5f   same_base._can_
+000044e0: 7573 655f 696e 5f63 7478 2863 7478 2920  use_in_ctx(ctx) 
+000044f0: 616e 6420 7361 6d65 5f62 6173 652e 6479  and same_base.dy
+00004500: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+00004510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004520: 726e 2073 616d 655f 6261 7365 0a20 2020  rn same_base.   
+00004530: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004540: 2020 2020 2020 2073 616d 655f 6261 7365         same_base
+00004550: 203d 2073 656c 660a 2020 2020 2020 2020   = self.        
+00004560: 7361 6d65 5f62 6173 655f 6578 7472 6120  same_base_extra 
+00004570: 3d20 7361 6d65 5f62 6173 652e 5f6d 616b  = same_base._mak
+00004580: 655f 6578 7472 6128 290a 2020 2020 2020  e_extra().      
+00004590: 2020 2320 4f6b 2c20 6e6f 7468 696e 6720    # Ok, nothing 
+000045a0: 6d61 7463 6869 6e67 2066 6f75 6e64 2e0a  matching found..
+000045b0: 2020 2020 2020 2020 6966 2063 7478 3a0a          if ctx:.
+000045c0: 2020 2020 2020 2020 2020 2020 2320 4368              # Ch
+000045d0: 6563 6b20 6966 2074 6865 2063 7478 2069  eck if the ctx i
+000045e0: 7320 7265 616c 6c79 2072 656c 6576 616e  s really relevan
+000045f0: 742c 2077 6865 6e20 7468 6973 2069 7320  t, when this is 
+00004600: 6465 7269 7665 6420 6672 6f6d 206f 7468  derived from oth
+00004610: 6572 2074 6167 732e 0a20 2020 2020 2020  er tags..       
+00004620: 2020 2020 2064 6572 6976 6564 5f62 6173       derived_bas
+00004630: 6573 203d 2073 616d 655f 6261 7365 2e67  es = same_base.g
+00004640: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
+00004650: 5f73 6574 2829 0a20 2020 2020 2020 2020  _set().         
+00004660: 2020 2064 6572 6976 6564 5f62 6173 6573     derived_bases
+00004670: 2e72 656d 6f76 6528 7361 6d65 5f62 6173  .remove(same_bas
+00004680: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00004690: 6620 6465 7269 7665 645f 6261 7365 733a  f derived_bases:
+000046a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000046b0: 2064 6572 6976 6564 5f63 7478 7320 3d20   derived_ctxs = 
+000046c0: 7365 7428 290a 2020 2020 2020 2020 2020  set().          
+000046d0: 2020 2020 2020 666f 7220 6420 696e 2064        for d in d
+000046e0: 6572 6976 6564 5f62 6173 6573 3a0a 2020  erived_bases:.  
+000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004700: 2020 7769 7468 2075 7469 6c2e 6775 6172    with util.guar
+00004710: 645f 696e 6669 6e69 7465 5f72 6563 7572  d_infinite_recur
+00004720: 7369 6f6e 285f 642e 4469 6d2e 6765 745f  sion(_d.Dim.get_
+00004730: 666f 725f 6261 7463 685f 6374 782c 2064  for_batch_ctx, d
+00004740: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00004750: 2020 2020 2020 2020 2020 2064 203d 2064             d = d
+00004760: 2e67 6574 5f66 6f72 5f62 6174 6368 5f63  .get_for_batch_c
+00004770: 7478 2862 6174 6368 3d62 6174 6368 2c20  tx(batch=batch, 
+00004780: 6374 783d 6374 7829 0a20 2020 2020 2020  ctx=ctx).       
+00004790: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000047a0: 642e 636f 6e74 726f 6c5f 666c 6f77 5f63  d.control_flow_c
+000047b0: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
+000047c0: 2020 2020 2020 2020 2020 2020 6465 7269              deri
+000047d0: 7665 645f 6374 7873 2e61 6464 2864 2e63  ved_ctxs.add(d.c
+000047e0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7829  ontrol_flow_ctx)
+000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004800: 2069 6620 6e6f 7420 6465 7269 7665 645f   if not derived_
+00004810: 6374 7873 3a0a 2020 2020 2020 2020 2020  ctxs:.          
+00004820: 2020 2020 2020 2020 2020 6374 7820 3d20            ctx = 
+00004830: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00004840: 2020 2020 2065 6c69 6620 6c65 6e28 6465       elif len(de
+00004850: 7269 7665 645f 6374 7873 2920 3d3d 2031  rived_ctxs) == 1
+00004860: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004870: 2020 2020 2020 6374 7820 3d20 6465 7269        ctx = deri
+00004880: 7665 645f 6374 7873 2e70 6f70 2829 0a20  ved_ctxs.pop(). 
+00004890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000048a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000048b0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+000048c0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+000048d0: 6f72 2822 6e6f 7420 7965 7420 696d 706c  or("not yet impl
+000048e0: 656d 656e 7465 643a 206d 756c 7469 706c  emented: multipl
+000048f0: 6520 6465 7269 7665 6420 6374 7873 3a20  e derived ctxs: 
+00004900: 2572 2220 2520 2864 6572 6976 6564 5f63  %r" % (derived_c
+00004910: 7478 732c 2929 0a20 2020 2020 2020 2064  txs,)).        d
+00004920: 796e 5f73 697a 655f 6578 7420 3d20 4e6f  yn_size_ext = No
+00004930: 6e65 0a20 2020 2020 2020 2023 204d 6179  ne.        # May
+00004940: 6265 2077 6520 6861 7665 2073 7468 2077  be we have sth w
+00004950: 6974 6820 7468 6520 6261 7365 2062 6174  ith the base bat
+00004960: 6368 2077 6974 686f 7574 2062 6561 6d20  ch without beam 
+00004970: 6f72 2070 6164 6465 6420 6261 7463 6820  or padded batch 
+00004980: 7768 6963 6820 7765 2063 616e 2065 7874  which we can ext
+00004990: 656e 642e 0a20 2020 2020 2020 2069 6620  end..        if 
+000049a0: 6261 7463 6820 213d 2062 6174 6368 2e67  batch != batch.g
+000049b0: 6574 5f67 6c6f 6261 6c5f 6261 7365 2829  et_global_base()
+000049c0: 3a0a 2020 2020 2020 2020 2020 2020 6261  :.            ba
+000049d0: 7463 685f 6261 7365 203d 2062 6174 6368  tch_base = batch
+000049e0: 2e67 6574 5f67 6c6f 6261 6c5f 6261 7365  .get_global_base
+000049f0: 2829 0a20 2020 2020 2020 2020 2020 2062  ().            b
+00004a00: 6173 655f 6361 6e5f 7573 655f 696e 5f63  ase_can_use_in_c
+00004a10: 7478 203d 204e 6f6e 6520 2023 2074 7970  tx = None  # typ
+00004a20: 653a 204f 7074 696f 6e61 6c5b 5f64 2e44  e: Optional[_d.D
+00004a30: 696d 5d0a 2020 2020 2020 2020 2020 2020  im].            
+00004a40: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+00004a50: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+00004a60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004a70: 7361 6d65 5f62 6173 652e 6261 7463 6820  same_base.batch 
+00004a80: 3d3d 2062 6174 6368 5f62 6173 6520 616e  == batch_base an
+00004a90: 6420 7361 6d65 5f62 6173 652e 5f63 616e  d same_base._can
+00004aa0: 5f75 7365 5f69 6e5f 6374 7828 6374 7829  _use_in_ctx(ctx)
+00004ab0: 2061 6e64 2073 616d 655f 6261 7365 2e64   and same_base.d
+00004ac0: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00004ad0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
+00004ae0: 655f 6361 6e5f 7573 655f 696e 5f63 7478  e_can_use_in_ctx
+00004af0: 203d 2073 616d 655f 6261 7365 0a20 2020   = same_base.   
+00004b00: 2020 2020 2020 2020 2065 6c69 6620 7361           elif sa
+00004b10: 6d65 5f62 6173 652e 5f65 7874 7261 3a0a  me_base._extra:.
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b30: 6672 6f6d 2072 6574 7572 6e6e 2e74 662e  from returnn.tf.
+00004b40: 7574 696c 2e64 6174 6120 696d 706f 7274  util.data import
+00004b50: 2043 6f6e 7472 6f6c 466c 6f77 436f 6e74   ControlFlowCont
+00004b60: 6578 740a 0a20 2020 2020 2020 2020 2020  ext..           
+00004b70: 2020 2020 2066 6f72 2063 7478 5f20 696e       for ctx_ in
+00004b80: 2043 6f6e 7472 6f6c 466c 6f77 436f 6e74   ControlFlowCont
+00004b90: 6578 742e 6162 735f 6374 785f 7374 6163  ext.abs_ctx_stac
+00004ba0: 6b5f 7769 7468 5f72 6f6f 7428 6374 7829  k_with_root(ctx)
+00004bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004bc0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+00004bd0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+00004be0: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
+00004bf0: 2020 2020 2020 2020 2020 2074 6167 203d             tag =
+00004c00: 2073 616d 655f 6261 7365 2e5f 6578 7472   same_base._extr
+00004c10: 612e 7361 6d65 5f66 6f72 5f62 6174 6368  a.same_for_batch
+00004c20: 5f63 7478 2e67 6574 2828 6261 7463 685f  _ctx.get((batch_
+00004c30: 6261 7365 2c20 6374 785f 292c 204e 6f6e  base, ctx_), Non
+00004c40: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00004c50: 2020 2020 2020 2069 6620 7461 6720 616e         if tag an
+00004c60: 6420 7461 672e 5f63 616e 5f75 7365 5f69  d tag._can_use_i
+00004c70: 6e5f 6374 7828 6374 7829 2061 6e64 2074  n_ctx(ctx) and t
+00004c80: 6167 2e5f 7661 6c69 6461 7465 5f69 6e5f  ag._validate_in_
+00004c90: 6375 7272 656e 745f 6772 6170 6828 2920  current_graph() 
+00004ca0: 616e 6420 7461 672e 6479 6e5f 7369 7a65  and tag.dyn_size
+00004cb0: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+00004cd0: 7365 5f63 616e 5f75 7365 5f69 6e5f 6374  se_can_use_in_ct
+00004ce0: 7820 3d20 7461 670a 2020 2020 2020 2020  x = tag.        
 00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d00: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00004d10: 2020 2020 2020 2020 6966 2062 6173 655f          if base_
-00004d20: 6361 6e5f 7573 655f 696e 5f63 7478 2061  can_use_in_ctx a
-00004d30: 6e64 2062 6173 655f 6361 6e5f 7573 655f  nd base_can_use_
-00004d40: 696e 5f63 7478 2e64 796e 5f73 697a 655f  in_ctx.dyn_size_
-00004d50: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-00004d60: 2020 2020 2069 6620 6261 7365 5f63 616e       if base_can
-00004d70: 5f75 7365 5f69 6e5f 6374 782e 6479 6e5f  _use_in_ctx.dyn_
-00004d80: 7369 7a65 5f65 7874 2e68 6176 655f 6261  size_ext.have_ba
-00004d90: 7463 685f 6178 6973 2829 3a0a 2020 2020  tch_axis():.    
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004db0: 2320 5468 6520 7361 6d65 5f62 6173 6520  # The same_base 
-00004dc0: 6861 7320 736f 6d65 2064 796e 2073 697a  has some dyn siz
-00004dd0: 6520 7769 7468 6f75 7420 616e 7920 6265  e without any be
-00004de0: 616d 206e 6f72 2063 6f6e 7472 6f6c 2066  am nor control f
-00004df0: 6c6f 7720 636f 6e74 6578 742e 0a20 2020  low context..   
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2023 2057 6520 6361 6e20 6578 7061 6e64   # We can expand
-00004e20: 2069 7420 746f 2074 6865 2063 7572 7265   it to the curre
-00004e30: 6e74 2062 6561 6d2c 206f 7220 6578 7465  nt beam, or exte
-00004e40: 6e64 2062 7920 7061 6464 6564 2062 6174  nd by padded bat
-00004e50: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
-00004e60: 2020 2020 2020 2020 6479 6e5f 7369 7a65          dyn_size
-00004e70: 5f65 7874 203d 2062 6173 655f 6361 6e5f  _ext = base_can_
-00004e80: 7573 655f 696e 5f63 7478 2e64 796e 5f73  use_in_ctx.dyn_s
-00004e90: 697a 655f 6578 742e 636f 7079 5f65 7874  ize_ext.copy_ext
-00004ea0: 656e 645f 6261 7463 6828 6261 7463 6829  end_batch(batch)
-00004eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ec0: 2020 2020 2069 6620 6261 7463 682e 6265       if batch.be
-00004ed0: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
-00004ee0: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
-00004ef0: 7369 7a65 5f65 7874 203d 2062 6173 655f  size_ext = base_
-00004f00: 6361 6e5f 7573 655f 696e 5f63 7478 2e64  can_use_in_ctx.d
-00004f10: 796e 5f73 697a 655f 6578 742e 636f 7079  yn_size_ext.copy
-00004f20: 5f65 7874 656e 645f 7769 7468 5f62 6561  _extend_with_bea
-00004f30: 6d28 6261 7463 682e 6265 616d 290a 2020  m(batch.beam).  
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 6173 7365 7274 2064 796e 5f73 697a    assert dyn_siz
-00004f60: 655f 6578 742e 6261 7463 6820 3d3d 2062  e_ext.batch == b
-00004f70: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-00004f80: 2020 2020 2020 2020 2069 6620 6479 6e5f           if dyn_
-00004f90: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
-00004fa0: 6c64 6572 2069 7320 6e6f 7420 4e6f 6e65  lder is not None
-00004fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004fc0: 2020 2020 2020 2020 2020 6265 616d 5f65            beam_e
-00004fd0: 7870 616e 6465 645f 6261 7365 5f64 6174  xpanded_base_dat
-00004fe0: 6120 3d20 6765 7461 7474 7228 0a20 2020  a = getattr(.   
+00004d00: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+00004d10: 2020 6966 2062 6173 655f 6361 6e5f 7573    if base_can_us
+00004d20: 655f 696e 5f63 7478 2061 6e64 2062 6173  e_in_ctx and bas
+00004d30: 655f 6361 6e5f 7573 655f 696e 5f63 7478  e_can_use_in_ctx
+00004d40: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
+00004d50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004d60: 6620 6261 7365 5f63 616e 5f75 7365 5f69  f base_can_use_i
+00004d70: 6e5f 6374 782e 6479 6e5f 7369 7a65 5f65  n_ctx.dyn_size_e
+00004d80: 7874 2e68 6176 655f 6261 7463 685f 6178  xt.have_batch_ax
+00004d90: 6973 2829 3a0a 2020 2020 2020 2020 2020  is():.          
+00004da0: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
+00004db0: 7361 6d65 5f62 6173 6520 6861 7320 736f  same_base has so
+00004dc0: 6d65 2064 796e 2073 697a 6520 7769 7468  me dyn size with
+00004dd0: 6f75 7420 616e 7920 6265 616d 206e 6f72  out any beam nor
+00004de0: 2063 6f6e 7472 6f6c 2066 6c6f 7720 636f   control flow co
+00004df0: 6e74 6578 742e 0a20 2020 2020 2020 2020  ntext..         
+00004e00: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+00004e10: 6361 6e20 6578 7061 6e64 2069 7420 746f  can expand it to
+00004e20: 2074 6865 2063 7572 7265 6e74 2062 6561   the current bea
+00004e30: 6d2c 206f 7220 6578 7465 6e64 2062 7920  m, or extend by 
+00004e40: 7061 6464 6564 2062 6174 6368 2e0a 2020  padded batch..  
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 6479 6e5f 7369 7a65 5f65 7874 203d    dyn_size_ext =
+00004e70: 2062 6173 655f 6361 6e5f 7573 655f 696e   base_can_use_in
+00004e80: 5f63 7478 2e64 796e 5f73 697a 655f 6578  _ctx.dyn_size_ex
+00004e90: 742e 636f 7079 5f65 7874 656e 645f 6261  t.copy_extend_ba
+00004ea0: 7463 6828 6261 7463 6829 0a20 2020 2020  tch(batch).     
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004ec0: 6620 6261 7463 682e 6265 616d 3a0a 2020  f batch.beam:.  
+00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ee0: 2020 2020 2020 6479 6e5f 7369 7a65 5f65        dyn_size_e
+00004ef0: 7874 203d 2062 6173 655f 6361 6e5f 7573  xt = base_can_us
+00004f00: 655f 696e 5f63 7478 2e64 796e 5f73 697a  e_in_ctx.dyn_siz
+00004f10: 655f 6578 742e 636f 7079 5f65 7874 656e  e_ext.copy_exten
+00004f20: 645f 7769 7468 5f62 6561 6d28 6261 7463  d_with_beam(batc
+00004f30: 682e 6265 616d 290a 2020 2020 2020 2020  h.beam).        
+00004f40: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00004f50: 7274 2064 796e 5f73 697a 655f 6578 742e  rt dyn_size_ext.
+00004f60: 6261 7463 6820 3d3d 2062 6174 6368 0a20  batch == batch. 
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2069 6620 6479 6e5f 7369 7a65 5f65     if dyn_size_e
+00004f90: 7874 2e70 6c61 6365 686f 6c64 6572 2069  xt.placeholder i
+00004fa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2020 2020 6265 616d 5f65 7870 616e 6465      beam_expande
+00004fd0: 645f 6261 7365 5f64 6174 6120 3d20 6765  d_base_data = ge
+00004fe0: 7461 7474 7228 0a20 2020 2020 2020 2020  tattr(.         
 00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 2020 2064 796e 5f73 697a           dyn_siz
-00005010: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-00005020: 722c 2022 5f52 4554 5552 4e4e 5f62 6561  r, "_RETURNN_bea
-00005030: 6d5f 6578 7061 6e64 6564 5f62 6173 655f  m_expanded_base_
-00005040: 6461 7461 222c 204e 6f6e 650a 2020 2020  data", None.    
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00005070: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005080: 2062 6174 6368 2e62 6561 6d3a 0a20 2020   batch.beam:.   
+00005000: 2020 2064 796e 5f73 697a 655f 6578 742e     dyn_size_ext.
+00005010: 706c 6163 6568 6f6c 6465 722c 2022 5f52  placeholder, "_R
+00005020: 4554 5552 4e4e 5f62 6561 6d5f 6578 7061  ETURNN_beam_expa
+00005030: 6e64 6564 5f62 6173 655f 6461 7461 222c  nded_base_data",
+00005040: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00005050: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2020 2020 2020 2020 6966 2062 6174 6368          if batch
+00005080: 2e62 6561 6d3a 0a20 2020 2020 2020 2020  .beam:.         
 00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050a0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000050b0: 6265 616d 5f65 7870 616e 6465 645f 6261  beam_expanded_ba
-000050c0: 7365 5f64 6174 610a 2020 2020 2020 2020  se_data.        
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2320 4e6f 7465 3a20 5468 6520 6265 616d  # Note: The beam
-000050f0: 2065 7870 616e 7369 6f6e 2075 7365 6420   expansion used 
-00005100: 7469 6c69 6e67 2c20 7768 6963 6820 6361  tiling, which ca
-00005110: 6e20 6265 2063 6163 6865 642e 0a20 2020  n be cached..   
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 2020 2023 2054 6869 7320 6d65 616e       # This mean
-00005140: 7320 7468 6174 2077 6520 636f 756c 6420  s that we could 
-00005150: 656e 6420 7570 2077 6974 6820 7468 6520  end up with the 
-00005160: 7361 6d65 2073 697a 6520 7465 6e73 6f72  same size tensor
-00005170: 2028 706c 6163 6568 6f6c 6465 7229 0a20   (placeholder). 
+000050a0: 2020 2061 7373 6572 7420 6265 616d 5f65     assert beam_e
+000050b0: 7870 616e 6465 645f 6261 7365 5f64 6174  xpanded_base_dat
+000050c0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+000050d0: 2020 2020 2020 2020 2020 2320 4e6f 7465            # Note
+000050e0: 3a20 5468 6520 6265 616d 2065 7870 616e  : The beam expan
+000050f0: 7369 6f6e 2075 7365 6420 7469 6c69 6e67  sion used tiling
+00005100: 2c20 7768 6963 6820 6361 6e20 6265 2063  , which can be c
+00005110: 6163 6865 642e 0a20 2020 2020 2020 2020  ached..         
+00005120: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005130: 2054 6869 7320 6d65 616e 7320 7468 6174   This means that
+00005140: 2077 6520 636f 756c 6420 656e 6420 7570   we could end up
+00005150: 2077 6974 6820 7468 6520 7361 6d65 2073   with the same s
+00005160: 697a 6520 7465 6e73 6f72 2028 706c 6163  ize tensor (plac
+00005170: 6568 6f6c 6465 7229 0a20 2020 2020 2020  eholder).       
 00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 2020 2023 2066 6f72 206d 756c         # for mul
-000051a0: 7469 706c 6520 6469 6666 6572 656e 7420  tiple different 
-000051b0: 6265 616d 732c 0a20 2020 2020 2020 2020  beams,.         
-000051c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000051d0: 2077 6865 6e20 7468 6572 6520 6172 6520   when there are 
-000051e0: 6469 6666 6572 656e 7420 6265 616d 7320  different beams 
-000051f0: 7769 7468 2073 616d 6520 6265 616d 2073  with same beam s
-00005200: 697a 6521 0a20 2020 2020 2020 2020 2020  ize!.           
-00005210: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-00005220: 6869 7320 6272 6561 6b73 2074 6865 2063  his breaks the c
-00005230: 7572 7265 6e74 206c 6f67 6963 2069 6e20  urrent logic in 
-00005240: 6765 745f 7461 675f 6672 6f6d 5f73 697a  get_tag_from_siz
-00005250: 655f 7465 6e73 6f72 2e0a 2020 2020 2020  e_tensor..      
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 2020 2320 4173 2061 2077 6f72 6b61 726f    # As a workaro
-00005280: 756e 642c 2077 6520 6d61 6b65 2061 6e20  und, we make an 
-00005290: 6578 706c 6963 6974 206e 6577 2074 656e  explicit new ten
-000052a0: 736f 7220 6865 7265 2e0a 2020 2020 2020  sor here..      
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 2020 696d 706f 7274 2074 656e 736f 7266    import tensorf
-000052d0: 6c6f 7720 6173 2074 660a 2020 2020 2020  low as tf.      
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 6672 6f6d 2072 6574 7572 6e6e 2e74    from returnn.t
-00005300: 662e 7574 696c 2e62 6173 6963 2069 6d70  f.util.basic imp
-00005310: 6f72 7420 6765 745f 7661 6c69 645f 7363  ort get_valid_sc
-00005320: 6f70 655f 6e61 6d65 5f66 726f 6d5f 7374  ope_name_from_st
-00005330: 722c 2073 616d 655f 636f 6e74 726f 6c5f  r, same_control_
-00005340: 666c 6f77 5f63 7478 0a0a 2020 2020 2020  flow_ctx..      
-00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005360: 2020 7769 7468 2073 616d 655f 636f 6e74    with same_cont
-00005370: 726f 6c5f 666c 6f77 5f63 7478 2864 796e  rol_flow_ctx(dyn
-00005380: 5f73 697a 655f 6578 742e 706c 6163 6568  _size_ext.placeh
-00005390: 6f6c 6465 7229 3a0a 2020 2020 2020 2020  older):.        
-000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053b0: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
-000053c0: 2e70 6c61 6365 686f 6c64 6572 203d 2074  .placeholder = t
-000053d0: 662e 6964 656e 7469 7479 280a 2020 2020  f.identity(.    
+00005190: 2023 2066 6f72 206d 756c 7469 706c 6520   # for multiple 
+000051a0: 6469 6666 6572 656e 7420 6265 616d 732c  different beams,
+000051b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051c0: 2020 2020 2020 2020 2023 2077 6865 6e20           # when 
+000051d0: 7468 6572 6520 6172 6520 6469 6666 6572  there are differ
+000051e0: 656e 7420 6265 616d 7320 7769 7468 2073  ent beams with s
+000051f0: 616d 6520 6265 616d 2073 697a 6521 0a20  ame beam size!. 
+00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005210: 2020 2020 2020 2023 2054 6869 7320 6272         # This br
+00005220: 6561 6b73 2074 6865 2063 7572 7265 6e74  eaks the current
+00005230: 206c 6f67 6963 2069 6e20 6765 745f 7461   logic in get_ta
+00005240: 675f 6672 6f6d 5f73 697a 655f 7465 6e73  g_from_size_tens
+00005250: 6f72 2e0a 2020 2020 2020 2020 2020 2020  or..            
+00005260: 2020 2020 2020 2020 2020 2020 2320 4173              # As
+00005270: 2061 2077 6f72 6b61 726f 756e 642c 2077   a workaround, w
+00005280: 6520 6d61 6b65 2061 6e20 6578 706c 6963  e make an explic
+00005290: 6974 206e 6577 2074 656e 736f 7220 6865  it new tensor he
+000052a0: 7265 2e0a 2020 2020 2020 2020 2020 2020  re..            
+000052b0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+000052c0: 7274 2074 656e 736f 7266 6c6f 7720 6173  rt tensorflow as
+000052d0: 2074 660a 2020 2020 2020 2020 2020 2020   tf.            
+000052e0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+000052f0: 2072 6574 7572 6e6e 2e74 662e 7574 696c   returnn.tf.util
+00005300: 2e62 6173 6963 2069 6d70 6f72 7420 6765  .basic import ge
+00005310: 745f 7661 6c69 645f 7363 6f70 655f 6e61  t_valid_scope_na
+00005320: 6d65 5f66 726f 6d5f 7374 722c 2073 616d  me_from_str, sam
+00005330: 655f 636f 6e74 726f 6c5f 666c 6f77 5f63  e_control_flow_c
+00005340: 7478 0a0a 2020 2020 2020 2020 2020 2020  tx..            
+00005350: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00005360: 2073 616d 655f 636f 6e74 726f 6c5f 666c   same_control_fl
+00005370: 6f77 5f63 7478 2864 796e 5f73 697a 655f  ow_ctx(dyn_size_
+00005380: 6578 742e 706c 6163 6568 6f6c 6465 7229  ext.placeholder)
+00005390: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000053a0: 2020 2020 2020 2020 2020 2020 2020 6479                dy
+000053b0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+000053c0: 686f 6c64 6572 203d 2074 662e 6964 656e  holder = tf.iden
+000053d0: 7469 7479 280a 2020 2020 2020 2020 2020  tity(.          
 000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053f0: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
-00005400: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
-00005410: 6c64 6572 2c0a 2020 2020 2020 2020 2020  lder,.          
+000053f0: 2020 2020 2020 6479 6e5f 7369 7a65 5f65        dyn_size_e
+00005400: 7874 2e70 6c61 6365 686f 6c64 6572 2c0a  xt.placeholder,.
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005430: 2020 2020 2020 6e61 6d65 3d67 6574 5f76        name=get_v
-00005440: 616c 6964 5f73 636f 7065 5f6e 616d 655f  alid_scope_name_
-00005450: 6672 6f6d 5f73 7472 280a 2020 2020 2020  from_str(.      
+00005430: 6e61 6d65 3d67 6574 5f76 616c 6964 5f73  name=get_valid_s
+00005440: 636f 7065 5f6e 616d 655f 6672 6f6d 5f73  cope_name_from_s
+00005450: 7472 280a 2020 2020 2020 2020 2020 2020  tr(.            
 00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005470: 2020 2020 2020 2020 2020 2020 2020 2225                "%
-00005480: 735f 6765 745f 666f 725f 6261 7463 685f  s_get_for_batch_
-00005490: 6374 785f 2573 2220 2520 2864 796e 5f73  ctx_%s" % (dyn_s
-000054a0: 697a 655f 6578 742e 6e61 6d65 2c20 6261  ize_ext.name, ba
-000054b0: 7463 682e 7368 6f72 745f 7265 7072 2829  tch.short_repr()
-000054c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005500: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00005510: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
-00005520: 7463 682e 6265 616d 3a0a 2020 2020 2020  tch.beam:.      
+00005470: 2020 2020 2020 2020 2225 735f 6765 745f          "%s_get_
+00005480: 666f 725f 6261 7463 685f 6374 785f 2573  for_batch_ctx_%s
+00005490: 2220 2520 2864 796e 5f73 697a 655f 6578  " % (dyn_size_ex
+000054a0: 742e 6e61 6d65 2c20 6261 7463 682e 7368  t.name, batch.sh
+000054b0: 6f72 745f 7265 7072 2829 290a 2020 2020  ort_repr()).    
+000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054d0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005510: 2020 2020 2069 6620 6261 7463 682e 6265       if batch.be
+00005520: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
 00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2020 2020 6479 6e5f 7369 7a65 5f65        dyn_size_e
-00005550: 7874 2e70 6c61 6365 686f 6c64 6572 2e5f  xt.placeholder._
-00005560: 5245 5455 524e 4e5f 6479 6e5f 7369 7a65  RETURNN_dyn_size
-00005570: 5f62 6561 6d20 3d20 6261 7463 682e 6265  _beam = batch.be
-00005580: 616d 0a20 2020 2020 2020 2020 2020 2020  am.             
-00005590: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000055a0: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
-000055b0: 6568 6f6c 6465 722e 5f52 4554 5552 4e4e  eholder._RETURNN
-000055c0: 5f62 6561 6d5f 6578 7061 6e64 6564 5f62  _beam_expanded_b
-000055d0: 6173 655f 6461 7461 203d 2062 6561 6d5f  ase_data = beam_
-000055e0: 6578 7061 6e64 6564 5f62 6173 655f 6461  expanded_base_da
-000055f0: 7461 0a20 2020 2020 2020 2069 6620 6e6f  ta.        if no
-00005600: 7420 6479 6e5f 7369 7a65 5f65 7874 2061  t dyn_size_ext a
-00005610: 6e64 2061 6c6c 6f77 5f6e 6f6e 6520 616e  nd allow_none an
-00005620: 6420 6e6f 7420 7361 6d65 5f62 6173 652e  d not same_base.
-00005630: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
-00005640: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005650: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-00005660: 2069 6620 6e6f 7420 6479 6e5f 7369 7a65   if not dyn_size
-00005670: 5f65 7874 2061 6e64 2073 616d 655f 6261  _ext and same_ba
-00005680: 7365 5f65 7874 7261 2e73 616d 655f 666f  se_extra.same_fo
-00005690: 725f 6261 7463 685f 6374 783a 0a20 2020  r_batch_ctx:.   
-000056a0: 2020 2020 2020 2020 2023 2054 6865 7265           # There
-000056b0: 2061 7265 2065 6172 6c69 6572 2065 6e74   are earlier ent
-000056c0: 7269 6573 2069 6e20 5f73 616d 655f 666f  ries in _same_fo
-000056d0: 725f 6261 7463 685f 6374 780a 2020 2020  r_batch_ctx.    
-000056e0: 2020 2020 2020 2020 2320 2d2d 206d 6179          # -- may
-000056f0: 6265 2077 6520 6361 6e20 696e 6665 7220  be we can infer 
-00005700: 6479 6e5f 7369 7a65 5f65 7874 2c20 6576  dyn_size_ext, ev
-00005710: 656e 2077 6974 6820 6469 6666 6572 656e  en with differen
-00005720: 7420 6261 7463 682e 0a20 2020 2020 2020  t batch..       
-00005730: 2020 2020 2066 6f72 2028 6261 7463 685f       for (batch_
-00005740: 2c20 6374 785f 292c 206f 7468 6572 2069  , ctx_), other i
-00005750: 6e20 7361 6d65 5f62 6173 655f 6578 7472  n same_base_extr
-00005760: 612e 7361 6d65 5f66 6f72 5f62 6174 6368  a.same_for_batch
-00005770: 5f63 7478 2e69 7465 6d73 2829 3a0a 2020  _ctx.items():.  
-00005780: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005790: 2063 7478 5f20 3d3d 2063 7478 2061 6e64   ctx_ == ctx and
-000057a0: 206f 7468 6572 2e64 796e 5f73 697a 655f   other.dyn_size_
-000057b0: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-000057c0: 2020 2020 2020 2020 2064 796e 5f73 697a           dyn_siz
-000057d0: 655f 6578 7420 3d20 6f74 6865 722e 6479  e_ext = other.dy
-000057e0: 6e5f 7369 7a65 5f65 7874 2e63 6f70 795f  n_size_ext.copy_
-000057f0: 7465 6d70 6c61 7465 2829 0a20 2020 2020  template().     
-00005800: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005810: 796e 5f73 697a 655f 6578 742e 6265 616d  yn_size_ext.beam
-00005820: 203d 2062 6174 6368 2e62 6561 6d0a 2020   = batch.beam.  
-00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 6479 6e5f 7369 7a65 5f65 7874 2e62    dyn_size_ext.b
-00005850: 6174 6368 203d 2062 6174 6368 0a20 2020  atch = batch.   
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2062 7265 616b 0a20 2020 2020 2020 2063   break.        c
-00005880: 7478 203d 2064 796e 5f73 697a 655f 6578  tx = dyn_size_ex
-00005890: 742e 636f 6e74 726f 6c5f 666c 6f77 5f63  t.control_flow_c
-000058a0: 7478 2069 6620 6479 6e5f 7369 7a65 5f65  tx if dyn_size_e
-000058b0: 7874 2065 6c73 6520 6374 780a 2020 2020  xt else ctx.    
-000058c0: 2020 2020 6469 6d5f 7461 6720 3d20 4e6f      dim_tag = No
-000058d0: 6e65 0a20 2020 2020 2020 2066 6f72 2063  ne.        for c
-000058e0: 616e 6469 6461 7465 2069 6e20 5b73 656c  andidate in [sel
-000058f0: 662c 2073 616d 655f 6261 7365 5d3a 0a20  f, same_base]:. 
-00005900: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2863 616e 6469 6461 7465 2e62 6174 6368  (candidate.batch
-00005930: 203d 3d20 6261 7463 6820 6f72 2028 6e6f   == batch or (no
-00005940: 7420 6361 6e64 6964 6174 652e 6261 7463  t candidate.batc
-00005950: 6820 616e 6420 6261 7463 682e 6973 5f67  h and batch.is_g
-00005960: 6c6f 6261 6c5f 6261 7463 6828 2929 290a  lobal_batch())).
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 616e 6420 6e6f 7420 6361 6e64 6964 6174  and not candidat
-00005990: 652e 636f 6e74 726f 6c5f 666c 6f77 5f63  e.control_flow_c
-000059a0: 7478 0a20 2020 2020 2020 2020 2020 2020  tx.             
-000059b0: 2020 2061 6e64 206e 6f74 2063 7478 0a20     and not ctx. 
-000059c0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000059e0: 5468 6520 7361 6d65 5f62 6173 6520 696e  The same_base in
-000059f0: 7374 616e 6365 2069 7320 6569 7468 6572  stance is either
-00005a00: 2075 6e64 6566 696e 6564 2028 6e6f 2062   undefined (no b
-00005a10: 6174 6368 2c20 6e6f 2063 7478 290a 2020  atch, no ctx).  
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00005a30: 6f72 2069 7420 6973 2064 6566 696e 6564  or it is defined
-00005a40: 2066 6f72 2074 6865 2073 616d 6520 6261   for the same ba
-00005a50: 7463 6820 616e 6420 6374 782e 0a20 2020  tch and ctx..   
-00005a60: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-00005a70: 6e20 616e 7920 6361 7365 2c20 7265 7573  n any case, reus
-00005a80: 6520 6974 2074 6865 6e2e 0a20 2020 2020  e it then..     
-00005a90: 2020 2020 2020 2020 2020 2063 616e 6469             candi
-00005aa0: 6461 7465 2e62 6174 6368 203d 2062 6174  date.batch = bat
-00005ab0: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
-00005ac0: 2020 2069 6620 6479 6e5f 7369 7a65 5f65     if dyn_size_e
-00005ad0: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-00005ae0: 2020 2020 2020 2020 6966 2063 616e 6469          if candi
-00005af0: 6461 7465 2e64 796e 5f73 697a 655f 6578  date.dyn_size_ex
-00005b00: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00005b10: 2020 2020 2020 2020 2020 2063 616e 6469             candi
-00005b20: 6461 7465 2e64 796e 5f73 697a 655f 6578  date.dyn_size_ex
-00005b30: 742e 6261 7463 6820 3d20 6261 7463 680a  t.batch = batch.
+00005540: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+00005550: 6365 686f 6c64 6572 2e5f 5245 5455 524e  ceholder._RETURN
+00005560: 4e5f 6479 6e5f 7369 7a65 5f62 6561 6d20  N_dyn_size_beam 
+00005570: 3d20 6261 7463 682e 6265 616d 0a20 2020  = batch.beam.   
+00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2020 2020 2020 2020 2064 796e 5f73 697a           dyn_siz
+000055a0: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
+000055b0: 722e 5f52 4554 5552 4e4e 5f62 6561 6d5f  r._RETURNN_beam_
+000055c0: 6578 7061 6e64 6564 5f62 6173 655f 6461  expanded_base_da
+000055d0: 7461 203d 2062 6561 6d5f 6578 7061 6e64  ta = beam_expand
+000055e0: 6564 5f62 6173 655f 6461 7461 0a20 2020  ed_base_data.   
+000055f0: 2020 2020 2069 6620 6e6f 7420 6479 6e5f       if not dyn_
+00005600: 7369 7a65 5f65 7874 2061 6e64 2061 6c6c  size_ext and all
+00005610: 6f77 5f6e 6f6e 6520 616e 6420 6e6f 7420  ow_none and not 
+00005620: 7361 6d65 5f62 6173 652e 6465 7269 7665  same_base.derive
+00005630: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
+00005640: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00005650: 6e65 0a20 2020 2020 2020 2069 6620 6e6f  ne.        if no
+00005660: 7420 6479 6e5f 7369 7a65 5f65 7874 2061  t dyn_size_ext a
+00005670: 6e64 2073 616d 655f 6261 7365 5f65 7874  nd same_base_ext
+00005680: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+00005690: 685f 6374 783a 0a20 2020 2020 2020 2020  h_ctx:.         
+000056a0: 2020 2023 2054 6865 7265 2061 7265 2065     # There are e
+000056b0: 6172 6c69 6572 2065 6e74 7269 6573 2069  arlier entries i
+000056c0: 6e20 5f73 616d 655f 666f 725f 6261 7463  n _same_for_batc
+000056d0: 685f 6374 780a 2020 2020 2020 2020 2020  h_ctx.          
+000056e0: 2020 2320 2d2d 206d 6179 6265 2077 6520    # -- maybe we 
+000056f0: 6361 6e20 696e 6665 7220 6479 6e5f 7369  can infer dyn_si
+00005700: 7a65 5f65 7874 2c20 6576 656e 2077 6974  ze_ext, even wit
+00005710: 6820 6469 6666 6572 656e 7420 6261 7463  h different batc
+00005720: 682e 0a20 2020 2020 2020 2020 2020 2066  h..            f
+00005730: 6f72 2028 6261 7463 685f 2c20 6374 785f  or (batch_, ctx_
+00005740: 292c 206f 7468 6572 2069 6e20 7361 6d65  ), other in same
+00005750: 5f62 6173 655f 6578 7472 612e 7361 6d65  _base_extra.same
+00005760: 5f66 6f72 5f62 6174 6368 5f63 7478 2e69  _for_batch_ctx.i
+00005770: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00005780: 2020 2020 2020 2020 6966 2063 7478 5f20          if ctx_ 
+00005790: 3d3d 2063 7478 2061 6e64 206f 7468 6572  == ctx and other
+000057a0: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2020 2064 796e 5f73 697a 655f 6578 7420     dyn_size_ext 
+000057d0: 3d20 6f74 6865 722e 6479 6e5f 7369 7a65  = other.dyn_size
+000057e0: 5f65 7874 2e63 6f70 795f 7465 6d70 6c61  _ext.copy_templa
+000057f0: 7465 2829 0a20 2020 2020 2020 2020 2020  te().           
+00005800: 2020 2020 2020 2020 2064 796e 5f73 697a           dyn_siz
+00005810: 655f 6578 742e 6265 616d 203d 2062 6174  e_ext.beam = bat
+00005820: 6368 2e62 6561 6d0a 2020 2020 2020 2020  ch.beam.        
+00005830: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
+00005840: 7369 7a65 5f65 7874 2e62 6174 6368 203d  size_ext.batch =
+00005850: 2062 6174 6368 0a20 2020 2020 2020 2020   batch.         
+00005860: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00005870: 0a20 2020 2020 2020 2063 7478 203d 2064  .        ctx = d
+00005880: 796e 5f73 697a 655f 6578 742e 636f 6e74  yn_size_ext.cont
+00005890: 726f 6c5f 666c 6f77 5f63 7478 2069 6620  rol_flow_ctx if 
+000058a0: 6479 6e5f 7369 7a65 5f65 7874 2065 6c73  dyn_size_ext els
+000058b0: 6520 6374 780a 2020 2020 2020 2020 6469  e ctx.        di
+000058c0: 6d5f 7461 6720 3d20 4e6f 6e65 0a20 2020  m_tag = None.   
+000058d0: 2020 2020 2066 6f72 2063 616e 6469 6461       for candida
+000058e0: 7465 2069 6e20 5b73 656c 662c 2073 616d  te in [self, sam
+000058f0: 655f 6261 7365 5d3a 0a20 2020 2020 2020  e_base]:.       
+00005900: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00005910: 2020 2020 2020 2020 2020 2863 616e 6469            (candi
+00005920: 6461 7465 2e62 6174 6368 203d 3d20 6261  date.batch == ba
+00005930: 7463 6820 6f72 2028 6e6f 7420 6361 6e64  tch or (not cand
+00005940: 6964 6174 652e 6261 7463 6820 616e 6420  idate.batch and 
+00005950: 6261 7463 682e 6973 5f67 6c6f 6261 6c5f  batch.is_global_
+00005960: 6261 7463 6828 2929 290a 2020 2020 2020  batch())).      
+00005970: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+00005980: 7420 6361 6e64 6964 6174 652e 636f 6e74  t candidate.cont
+00005990: 726f 6c5f 666c 6f77 5f63 7478 0a20 2020  rol_flow_ctx.   
+000059a0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000059b0: 206e 6f74 2063 7478 0a20 2020 2020 2020   not ctx.       
+000059c0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+000059d0: 2020 2020 2020 2020 2320 5468 6520 7361          # The sa
+000059e0: 6d65 5f62 6173 6520 696e 7374 616e 6365  me_base instance
+000059f0: 2069 7320 6569 7468 6572 2075 6e64 6566   is either undef
+00005a00: 696e 6564 2028 6e6f 2062 6174 6368 2c20  ined (no batch, 
+00005a10: 6e6f 2063 7478 290a 2020 2020 2020 2020  no ctx).        
+00005a20: 2020 2020 2020 2020 2320 6f72 2069 7420          # or it 
+00005a30: 6973 2064 6566 696e 6564 2066 6f72 2074  is defined for t
+00005a40: 6865 2073 616d 6520 6261 7463 6820 616e  he same batch an
+00005a50: 6420 6374 782e 0a20 2020 2020 2020 2020  d ctx..         
+00005a60: 2020 2020 2020 2023 2049 6e20 616e 7920         # In any 
+00005a70: 6361 7365 2c20 7265 7573 6520 6974 2074  case, reuse it t
+00005a80: 6865 6e2e 0a20 2020 2020 2020 2020 2020  hen..           
+00005a90: 2020 2020 2063 616e 6469 6461 7465 2e62       candidate.b
+00005aa0: 6174 6368 203d 2062 6174 6368 0a20 2020  atch = batch.   
+00005ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005ac0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2020 6966 2063 616e 6469 6461 7465 2e64    if candidate.d
+00005af0: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2020 2020 2063 616e 6469 6461 7465 2e64       candidate.d
+00005b20: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
+00005b30: 6820 3d20 6261 7463 680a 2020 2020 2020  h = batch.      
 00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
-00005b60: 616e 6469 6461 7465 2e64 796e 5f73 697a  andidate.dyn_siz
-00005b70: 655f 6578 742e 6469 6d5f 7461 6773 203d  e_ext.dim_tags =
-00005b80: 3d20 6479 6e5f 7369 7a65 5f65 7874 2e64  = dyn_size_ext.d
-00005b90: 696d 5f74 6167 730a 2020 2020 2020 2020  im_tags.        
-00005ba0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00005bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005bc0: 2020 2020 2020 2020 2020 6361 6e64 6964            candid
-00005bd0: 6174 652e 6479 6e5f 7369 7a65 5f65 7874  ate.dyn_size_ext
-00005be0: 203d 2064 796e 5f73 697a 655f 6578 740a   = dyn_size_ext.
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 2020 6173 7365 7274 206e 6f74 2063      assert not c
-00005c10: 616e 6469 6461 7465 2e64 796e 5f73 697a  andidate.dyn_siz
-00005c20: 655f 6578 742e 636f 6e74 726f 6c5f 666c  e_ext.control_fl
-00005c30: 6f77 5f63 7478 0a20 2020 2020 2020 2020  ow_ctx.         
-00005c40: 2020 2020 2020 2065 6c69 6620 6361 6e64         elif cand
-00005c50: 6964 6174 652e 6479 6e5f 7369 7a65 5f65  idate.dyn_size_e
-00005c60: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-00005c70: 2020 2020 2020 2020 6361 6e64 6964 6174          candidat
-00005c80: 652e 6479 6e5f 7369 7a65 5f65 7874 2e62  e.dyn_size_ext.b
-00005c90: 6174 6368 203d 2062 6174 6368 0a20 2020  atch = batch.   
-00005ca0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00005cb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00005cc0: 2020 2020 2020 2063 616e 6469 6461 7465         candidate
-00005cd0: 2e63 6f6d 706c 6574 655f 6479 6e5f 7369  .complete_dyn_si
-00005ce0: 7a65 2874 656d 706c 6174 655f 6f6e 6c79  ze(template_only
-00005cf0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00005d00: 2020 2020 2020 2064 696d 5f74 6167 203d         dim_tag =
-00005d10: 2063 616e 6469 6461 7465 0a20 2020 2020   candidate.     
-00005d20: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00005d30: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00005d40: 6469 6d5f 7461 673a 0a20 2020 2020 2020  dim_tag:.       
-00005d50: 2020 2020 2064 696d 5f74 6167 203d 205f       dim_tag = _
-00005d60: 642e 4469 6d28 0a20 2020 2020 2020 2020  d.Dim(.         
-00005d70: 2020 2020 2020 206b 696e 643d 7365 6c66         kind=self
-00005d80: 2e6b 696e 642c 0a20 2020 2020 2020 2020  .kind,.         
-00005d90: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00005da0: 6f6e 3d73 656c 662e 6465 7363 7269 7074  on=self.descript
-00005db0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00005dc0: 2020 2020 2064 696d 656e 7369 6f6e 3d73       dimension=s
-00005dd0: 656c 662e 6469 6d65 6e73 696f 6e2c 0a20  elf.dimension,. 
-00005de0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00005df0: 7574 6f5f 6765 6e65 7261 7465 643d 7365  uto_generated=se
-00005e00: 6c66 2e61 7574 6f5f 6765 6e65 7261 7465  lf.auto_generate
-00005e10: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00005e20: 2020 2062 6174 6368 3d62 6174 6368 2c0a     batch=batch,.
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-00005e50: 3d63 7478 2c0a 2020 2020 2020 2020 2020  =ctx,.          
-00005e60: 2020 2020 2020 6479 6e5f 7369 7a65 5f65        dyn_size_e
-00005e70: 7874 3d64 796e 5f73 697a 655f 6578 742c  xt=dyn_size_ext,
-00005e80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00005e90: 2020 2020 2020 2020 2020 2064 696d 5f74             dim_t
-00005ea0: 6167 2e73 616d 655f 6173 203d 2073 616d  ag.same_as = sam
-00005eb0: 655f 6261 7365 0a20 2020 2020 2020 2069  e_base.        i
-00005ec0: 6620 6479 6e5f 7369 7a65 5f65 7874 2061  f dyn_size_ext a
-00005ed0: 6e64 2064 796e 5f73 697a 655f 6578 742e  nd dyn_size_ext.
-00005ee0: 706c 6163 6568 6f6c 6465 7220 6973 206e  placeholder is n
-00005ef0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00005f00: 2020 2020 2069 6620 5f64 2e44 696d 2e67       if _d.Dim.g
-00005f10: 6574 5f74 6167 5f66 726f 6d5f 7369 7a65  et_tag_from_size
-00005f20: 5f74 656e 736f 7228 6479 6e5f 7369 7a65  _tensor(dyn_size
-00005f30: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
-00005f40: 2920 6973 204e 6f6e 653a 0a20 2020 2020  ) is None:.     
-00005f50: 2020 2020 2020 2020 2020 2064 696d 5f74             dim_t
-00005f60: 6167 2e73 6574 5f74 6167 5f6f 6e5f 7369  ag.set_tag_on_si
-00005f70: 7a65 5f74 656e 736f 7228 6479 6e5f 7369  ze_tensor(dyn_si
-00005f80: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
-00005f90: 6572 2c20 6261 7463 683d 6261 7463 6829  er, batch=batch)
-00005fa0: 0a20 2020 2020 2020 2073 616d 655f 6261  .        same_ba
-00005fb0: 7365 5f65 7874 7261 2e73 616d 655f 666f  se_extra.same_fo
-00005fc0: 725f 6261 7463 685f 6374 785b 2862 6174  r_batch_ctx[(bat
-00005fd0: 6368 2c20 6374 7829 5d20 3d20 6469 6d5f  ch, ctx)] = dim_
-00005fe0: 7461 670a 2020 2020 2020 2020 6469 6d5f  tag.        dim_
-00005ff0: 7461 672e 636f 6d70 6c65 7465 5f64 796e  tag.complete_dyn
-00006000: 5f73 697a 6528 7465 6d70 6c61 7465 5f6f  _size(template_o
-00006010: 6e6c 793d 5472 7565 290a 2020 2020 2020  nly=True).      
-00006020: 2020 7265 7475 726e 2064 696d 5f74 6167    return dim_tag
-00006030: 0a0a 2020 2020 6465 6620 7265 7365 745f  ..    def reset_
-00006040: 6261 7463 685f 6374 7828 7365 6c66 3a20  batch_ctx(self: 
-00006050: 4469 6d29 3a0a 2020 2020 2020 2020 2222  Dim):.        ""
-00006060: 220a 2020 2020 2020 2020 466f 7220 7468  ".        For th
-00006070: 6520 7365 6c66 2069 6e73 7461 6e63 652c  e self instance,
-00006080: 2072 6573 6574 2062 6174 6368 2061 6e64   reset batch and
-00006090: 2063 6f6e 7465 7874 2e0a 2020 2020 2020   context..      
-000060a0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000060b0: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
-000060c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000060d0: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
-000060e0: 6174 6368 5f63 7478 2e70 6f70 2828 7365  atch_ctx.pop((se
-000060f0: 6c66 2e62 6174 6368 2c20 7365 6c66 2e63  lf.batch, self.c
-00006100: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7829  ontrol_flow_ctx)
-00006110: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-00006120: 7365 6c66 2e62 6174 6368 203d 204e 6f6e  self.batch = Non
-00006130: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
-00006140: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7820  ontrol_flow_ctx 
-00006150: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-00006160: 6620 7365 6c66 2e64 796e 5f73 697a 655f  f self.dyn_size_
-00006170: 6578 7420 616e 6420 7365 6c66 2e64 796e  ext and self.dyn
-00006180: 5f73 697a 655f 6578 742e 6261 7463 683a  _size_ext.batch:
-00006190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000061a0: 662e 6479 6e5f 7369 7a65 5f65 7874 203d  f.dyn_size_ext =
-000061b0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-000061c0: 7874 2e63 6f70 795f 7465 6d70 6c61 7465  xt.copy_template
-000061d0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000061e0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-000061f0: 2e62 6174 6368 203d 204e 6f6e 650a 0a20  .batch = None.. 
-00006200: 2020 2064 6566 2073 6574 5f64 796e 5f73     def set_dyn_s
-00006210: 697a 655f 6578 745f 666f 725f 6261 7463  ize_ext_for_batc
-00006220: 685f 6374 7828 7365 6c66 2c20 6261 7463  h_ctx(self, batc
-00006230: 682c 2063 7478 2c20 6479 6e5f 7369 7a65  h, ctx, dyn_size
-00006240: 5f65 7874 293a 0a20 2020 2020 2020 2022  _ext):.        "
-00006250: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00006260: 6d20 4261 7463 6849 6e66 6f20 6261 7463  m BatchInfo batc
-00006270: 683a 0a20 2020 2020 2020 203a 7061 7261  h:.        :para
-00006280: 6d20 436f 6e74 726f 6c46 6c6f 7743 6f6e  m ControlFlowCon
-00006290: 7465 7874 7c4e 6f6e 6520 6374 783a 0a20  text|None ctx:. 
-000062a0: 2020 2020 2020 203a 7061 7261 6d20 4461         :param Da
-000062b0: 7461 2064 796e 5f73 697a 655f 6578 743a  ta dyn_size_ext:
-000062c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000062d0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-000062e0: 2e63 616e 5f62 655f 7573 6564 5f61 735f  .can_be_used_as_
-000062f0: 6469 6d28 290a 2020 2020 2020 2020 7361  dim().        sa
-00006300: 6d65 203d 2073 656c 662e 6765 745f 666f  me = self.get_fo
-00006310: 725f 6261 7463 685f 6374 7828 6261 7463  r_batch_ctx(batc
-00006320: 682c 2063 7478 290a 2020 2020 2020 2020  h, ctx).        
-00006330: 6173 7365 7274 2064 796e 5f73 697a 655f  assert dyn_size_
-00006340: 6578 742e 6261 7463 6820 3d3d 2062 6174  ext.batch == bat
-00006350: 6368 2061 6e64 2064 796e 5f73 697a 655f  ch and dyn_size_
-00006360: 6578 742e 636f 6e74 726f 6c5f 666c 6f77  ext.control_flow
-00006370: 5f63 7478 203d 3d20 6374 780a 2020 2020  _ctx == ctx.    
-00006380: 2020 2020 6966 2073 616d 652e 6479 6e5f      if same.dyn_
-00006390: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-000063a0: 2020 2020 2020 6173 7365 7274 2073 616d        assert sam
-000063b0: 652e 6479 6e5f 7369 7a65 5f65 7874 2e64  e.dyn_size_ext.d
-000063c0: 696d 5f74 6167 7320 3d3d 2064 796e 5f73  im_tags == dyn_s
-000063d0: 697a 655f 6578 742e 6469 6d5f 7461 6773  ize_ext.dim_tags
-000063e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000063f0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-00006400: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-00006410: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006420: 2020 2020 2020 7361 6d65 2e64 796e 5f73        same.dyn_s
-00006430: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
-00006440: 6465 7220 3d20 6479 6e5f 7369 7a65 5f65  der = dyn_size_e
-00006450: 7874 2e70 6c61 6365 686f 6c64 6572 0a20  xt.placeholder. 
-00006460: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006470: 2020 2020 2020 2020 2073 616d 652e 6479           same.dy
-00006480: 6e5f 7369 7a65 5f65 7874 203d 2064 796e  n_size_ext = dyn
-00006490: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
-000064a0: 2020 7365 6c66 2e5f 6d61 7962 655f 7570    self._maybe_up
-000064b0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-000064c0: 6765 745f 6479 6e5f 7369 7a65 5f65 7874  get_dyn_size_ext
-000064d0: 5f66 6f72 5f62 6174 6368 5f63 7478 2873  _for_batch_ctx(s
-000064e0: 656c 662c 2062 6174 6368 2c20 6374 782c  elf, batch, ctx,
-000064f0: 2074 656d 706c 6174 655f 6f6e 6c79 3d46   template_only=F
-00006500: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
-00006510: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00006520: 6d20 4261 7463 6849 6e66 6f7c 4e6f 6e65  m BatchInfo|None
-00006530: 2062 6174 6368 3a0a 2020 2020 2020 2020   batch:.        
-00006540: 3a70 6172 616d 2043 6f6e 7472 6f6c 466c  :param ControlFl
-00006550: 6f77 436f 6e74 6578 747c 4e6f 6e65 2063  owContext|None c
-00006560: 7478 3a0a 2020 2020 2020 2020 3a70 6172  tx:.        :par
-00006570: 616d 2062 6f6f 6c20 7465 6d70 6c61 7465  am bool template
-00006580: 5f6f 6e6c 793a 0a20 2020 2020 2020 203a  _only:.        :
-00006590: 7274 7970 653a 2044 6174 617c 4e6f 6e65  rtype: Data|None
-000065a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000065b0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-000065c0: 2e63 616e 5f62 655f 7573 6564 5f61 735f  .can_be_used_as_
-000065d0: 6469 6d28 290a 2020 2020 2020 2020 6966  dim().        if
-000065e0: 206e 6f74 2062 6174 6368 2061 6e64 2073   not batch and s
-000065f0: 656c 662e 6261 7463 683a 0a20 2020 2020  elf.batch:.     
-00006600: 2020 2020 2020 2023 2041 7373 756d 6520         # Assume 
-00006610: 676c 6f62 616c 2062 6174 6368 2e0a 2020  global batch..  
-00006620: 2020 2020 2020 2020 2020 6261 7463 6820            batch 
-00006630: 3d20 7365 6c66 2e62 6174 6368 2e67 6574  = self.batch.get
-00006640: 5f67 6c6f 6261 6c5f 6261 7365 2829 0a20  _global_base(). 
-00006650: 2020 2020 2020 2069 6620 6e6f 7420 6261         if not ba
-00006660: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
-00006670: 2023 2054 6869 7320 6973 2075 7375 616c   # This is usual
-00006680: 6c79 206e 6f74 2076 616c 6964 2e20 486f  ly not valid. Ho
-00006690: 7765 7665 722c 2074 6869 7320 6361 7365  wever, this case
-000066a0: 2063 616e 2068 6170 7065 6e20 6561 726c   can happen earl
-000066b0: 7920 6174 2069 6e69 7469 616c 697a 6174  y at initializat
-000066c0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-000066d0: 2061 7373 6572 7420 6261 7463 6820 3d3d   assert batch ==
-000066e0: 2073 656c 662e 6261 7463 6820 616e 6420   self.batch and 
-000066f0: 6374 7820 3d3d 2073 656c 662e 636f 6e74  ctx == self.cont
-00006700: 726f 6c5f 666c 6f77 5f63 7478 0a20 2020  rol_flow_ctx.   
-00006710: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006720: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00006730: 740a 2020 2020 2020 2020 7361 6d65 203d  t.        same =
-00006740: 2073 656c 662e 6765 745f 666f 725f 6261   self.get_for_ba
-00006750: 7463 685f 6374 7828 6261 7463 682c 2063  tch_ctx(batch, c
-00006760: 7478 2c20 616c 6c6f 775f 6e6f 6e65 3d54  tx, allow_none=T
-00006770: 7275 6529 0a20 2020 2020 2020 2069 6620  rue).        if 
-00006780: 6e6f 7420 7361 6d65 3a0a 2020 2020 2020  not same:.      
-00006790: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000067a0: 650a 2020 2020 2020 2020 7361 6d65 2e63  e.        same.c
-000067b0: 6f6d 706c 6574 655f 6479 6e5f 7369 7a65  omplete_dyn_size
-000067c0: 2874 656d 706c 6174 655f 6f6e 6c79 3d74  (template_only=t
-000067d0: 656d 706c 6174 655f 6f6e 6c79 290a 2020  emplate_only).  
-000067e0: 2020 2020 2020 7265 7475 726e 2073 616d        return sam
-000067f0: 652e 6479 6e5f 7369 7a65 5f65 7874 0a0a  e.dyn_size_ext..
-00006800: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00006810: 2020 6465 6620 6479 6e5f 7369 7a65 2873    def dyn_size(s
-00006820: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00006830: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
-00006840: 6e3a 2064 796e 2073 697a 6520 2f20 7365  n: dyn size / se
-00006850: 7120 6c65 6e20 2875 7375 616c 6c79 206f  q len (usually o
-00006860: 6620 7368 6170 6520 5b42 5d29 2c20 6f72  f shape [B]), or
-00006870: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00006880: 4966 2074 6865 2064 796e 2073 697a 6520  If the dyn size 
-00006890: 6361 6e20 706f 7465 6e74 6961 6c6c 7920  can potentially 
-000068a0: 6265 206f 6620 6120 6469 6666 6572 656e  be of a differen
-000068b0: 7420 7368 6170 652c 2064 6972 6563 746c  t shape, directl
-000068c0: 7920 6163 6365 7373 2064 796e 5f73 697a  y access dyn_siz
-000068d0: 655f 6578 742e 0a20 2020 2020 2020 203a  e_ext..        :
-000068e0: 7274 7970 653a 2074 662e 5465 6e73 6f72  rtype: tf.Tensor
-000068f0: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
-00006900: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00006910: 662e 6479 6e5f 7369 7a65 5f65 7874 3a0a  f.dyn_size_ext:.
-00006920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006930: 726e 2073 656c 662e 6479 6e5f 7369 7a65  rn self.dyn_size
-00006940: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
-00006950: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006960: 4e6f 6e65 0a0a 2020 2020 4064 796e 5f73  None..    @dyn_s
-00006970: 697a 652e 7365 7474 6572 0a20 2020 2064  ize.setter.    d
-00006980: 6566 2064 796e 5f73 697a 6528 7365 6c66  ef dyn_size(self
-00006990: 2c20 6479 6e5f 7369 7a65 293a 0a20 2020  , dyn_size):.   
-000069a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000069b0: 2041 6c73 6f20 7365 6520 3a66 756e 633a   Also see :func:
-000069c0: 6073 6574 5f64 796e 5f73 697a 655f 6578  `set_dyn_size_ex
-000069d0: 745f 666f 725f 6261 7463 685f 6374 7860  t_for_batch_ctx`
-000069e0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000069f0: 6d20 7466 2e54 656e 736f 7220 6479 6e5f  m tf.Tensor dyn_
-00006a00: 7369 7a65 3a0a 2020 2020 2020 2020 2222  size:.        ""
-00006a10: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00006a20: 662e 6479 6e5f 7369 7a65 5f65 7874 2061  f.dyn_size_ext a
-00006a30: 6e64 2073 656c 662e 6479 6e5f 7369 7a65  nd self.dyn_size
-00006a40: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
-00006a50: 2069 7320 6479 6e5f 7369 7a65 3a20 2023   is dyn_size:  #
-00006a60: 2066 6173 7420 7061 7468 2063 6865 636b   fast path check
-00006a70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006a80: 7572 6e0a 2020 2020 2020 2020 6173 7365  urn.        asse
-00006a90: 7274 2073 656c 662e 6361 6e5f 6265 5f75  rt self.can_be_u
-00006aa0: 7365 645f 6173 5f64 696d 2829 0a20 2020  sed_as_dim().   
-00006ab0: 2020 2020 206f 7468 6572 203d 205f 642e       other = _d.
-00006ac0: 4469 6d2e 6765 745f 7461 675f 6672 6f6d  Dim.get_tag_from
-00006ad0: 5f73 697a 655f 7465 6e73 6f72 2864 796e  _size_tensor(dyn
-00006ae0: 5f73 697a 6529 0a20 2020 2020 2020 2069  _size).        i
-00006af0: 6620 6f74 6865 723a 0a20 2020 2020 2020  f other:.       
-00006b00: 2020 2020 2073 656c 662e 6465 636c 6172       self.declar
-00006b10: 655f 7361 6d65 5f61 7328 6f74 6865 7229  e_same_as(other)
-00006b20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00006b30: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
-00006b40: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00006b50: 7274 2073 656c 662e 6261 7463 6820 3d3d  rt self.batch ==
-00006b60: 206f 7468 6572 2e62 6174 6368 2061 6e64   other.batch and
-00006b70: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
-00006b80: 6f77 5f63 7478 203d 3d20 6f74 6865 722e  ow_ctx == other.
-00006b90: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-00006ba0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00006bb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006bc0: 2020 2073 656c 662e 6261 7463 6820 3d20     self.batch = 
-00006bd0: 6f74 6865 722e 6261 7463 680a 2020 2020  other.batch.    
-00006be0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006bf0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-00006c00: 7820 3d20 6f74 6865 722e 636f 6e74 726f  x = other.contro
-00006c10: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
-00006c20: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
-00006c30: 7369 7a65 5f65 7874 203d 206f 7468 6572  size_ext = other
-00006c40: 2e64 796e 5f73 697a 655f 6578 740a 2020  .dyn_size_ext.  
-00006c50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006c60: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-00006c70: 6e69 745f 6465 6661 756c 745f 6479 6e5f  nit_default_dyn_
-00006c80: 7369 7a65 5f65 7874 2864 796e 5f73 697a  size_ext(dyn_siz
-00006c90: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00006ca0: 7365 745f 7461 675f 6f6e 5f73 697a 655f  set_tag_on_size_
-00006cb0: 7465 6e73 6f72 2864 796e 5f73 697a 6529  tensor(dyn_size)
-00006cc0: 0a0a 2020 2020 6465 6620 5f69 6e69 745f  ..    def _init_
-00006cd0: 6465 6661 756c 745f 6479 6e5f 7369 7a65  default_dyn_size
-00006ce0: 5f65 7874 2873 656c 662c 2064 796e 5f73  _ext(self, dyn_s
-00006cf0: 697a 6529 3a0a 2020 2020 2020 2020 2222  ize):.        ""
-00006d00: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00006d10: 2074 662e 5465 6e73 6f72 2064 796e 5f73   tf.Tensor dyn_s
-00006d20: 697a 653a 0a20 2020 2020 2020 2022 2222  ize:.        """
-00006d30: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006d40: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
-00006d50: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00006d60: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00006d70: 706c 6163 6568 6f6c 6465 7220 6973 206e  placeholder is n
-00006d80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00006d90: 2020 2020 2020 2020 2023 2044 6f20 6e6f           # Do no
-00006da0: 7420 616c 6c6f 7720 7265 7365 7474 696e  t allow resettin
-00006db0: 6720 6974 2074 6f20 7374 6820 6469 6666  g it to sth diff
-00006dc0: 6572 656e 742e 0a20 2020 2020 2020 2020  erent..         
-00006dd0: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-00006de0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00006df0: 706c 6163 6568 6f6c 6465 7220 6973 2064  placeholder is d
-00006e00: 796e 5f73 697a 650a 2020 2020 2020 2020  yn_size.        
-00006e10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00006e20: 2020 6265 616d 203d 2067 6574 6174 7472    beam = getattr
-00006e30: 2864 796e 5f73 697a 652c 2022 5f52 4554  (dyn_size, "_RET
-00006e40: 5552 4e4e 5f64 796e 5f73 697a 655f 6265  URNN_dyn_size_be
-00006e50: 616d 222c 204e 6f6e 6529 0a20 2020 2020  am", None).     
-00006e60: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
-00006e70: 7369 7a65 5f65 7874 203d 205f 742e 5465  size_ext = _t.Te
-00006e80: 6e73 6f72 280a 2020 2020 2020 2020 2020  nsor(.          
-00006e90: 2020 2020 2020 6e61 6d65 3d28 2225 733a        name=("%s:
-00006ea0: 6479 6e5f 7369 7a65 2220 2520 7365 6c66  dyn_size" % self
-00006eb0: 2e64 6573 6372 6970 7469 6f6e 2920 6966  .description) if
-00006ec0: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
-00006ed0: 6e20 656c 7365 2064 796e 5f73 697a 652e  n else dyn_size.
-00006ee0: 6f70 2e6e 616d 652c 0a20 2020 2020 2020  op.name,.       
-00006ef0: 2020 2020 2020 2020 2064 7479 7065 3d5f           dtype=_
-00006f00: 742e 5465 6e73 6f72 2e73 697a 655f 6474  t.Tensor.size_dt
-00006f10: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-00006f20: 2020 2020 2073 6861 7065 3d28 292c 0a20       shape=(),. 
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00006f40: 6174 6368 5f64 696d 5f61 7869 733d 302c  atch_dim_axis=0,
-00006f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f60: 2062 6174 6368 3d73 656c 662e 6261 7463   batch=self.batc
-00006f70: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-00006f80: 2020 2062 6561 6d3d 6265 616d 2c0a 2020     beam=beam,.  
-00006f90: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006fa0: 6e74 726f 6c5f 666c 6f77 5f63 7478 3d73  ntrol_flow_ctx=s
-00006fb0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-00006fc0: 5f63 7478 2c0a 2020 2020 2020 2020 2020  _ctx,.          
-00006fd0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00006fe0: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
-00006ff0: 6163 6568 6f6c 6465 7220 3d20 6479 6e5f  aceholder = dyn_
-00007000: 7369 7a65 0a0a 2020 2020 6465 6620 5f67  size..    def _g
-00007010: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
-00007020: 666f 725f 6465 7669 6365 2873 656c 663a  for_device(self:
-00007030: 2044 696d 2c20 6465 7669 6365 3a20 4f70   Dim, device: Op
-00007040: 7469 6f6e 616c 5b73 7472 5d29 202d 3e20  tional[str]) -> 
-00007050: 5f74 2e54 656e 736f 723a 0a20 2020 2020  _t.Tensor:.     
-00007060: 2020 2069 6620 6e6f 7420 6465 7669 6365     if not device
-00007070: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00007080: 7475 726e 2073 656c 662e 6479 6e5f 7369  turn self.dyn_si
-00007090: 7a65 5f65 7874 0a0a 2020 2020 2020 2020  ze_ext..        
-000070a0: 696d 706f 7274 2072 6574 7572 6e6e 2e66  import returnn.f
-000070b0: 726f 6e74 656e 6420 6173 2072 660a 0a20  rontend as rf.. 
-000070c0: 2020 2020 2020 2073 656c 662e 5f6d 616b         self._mak
-000070d0: 655f 6578 7472 6128 290a 2020 2020 2020  e_extra().      
-000070e0: 2020 6966 2064 6576 6963 6520 696e 2073    if device in s
-000070f0: 656c 662e 5f65 7874 7261 2e63 6163 6865  elf._extra.cache
-00007100: 5f64 796e 5f73 697a 655f 6578 745f 6465  _dyn_size_ext_de
-00007110: 763a 0a20 2020 2020 2020 2020 2020 2072  v:.            r
-00007120: 6574 7572 6e20 7365 6c66 2e5f 6578 7472  eturn self._extr
-00007130: 612e 6361 6368 655f 6479 6e5f 7369 7a65  a.cache_dyn_size
-00007140: 5f65 7874 5f64 6576 5b64 6576 6963 655d  _ext_dev[device]
-00007150: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-00007160: 7874 7261 2e63 6163 6865 5f64 796e 5f73  xtra.cache_dyn_s
-00007170: 697a 655f 6578 745f 6465 765b 6465 7669  ize_ext_dev[devi
-00007180: 6365 5d20 3d20 7266 2e63 6f70 795f 746f  ce] = rf.copy_to
-00007190: 5f64 6576 6963 6528 7365 6c66 2e64 796e  _device(self.dyn
-000071a0: 5f73 697a 655f 6578 742c 2064 6576 6963  _size_ext, devic
-000071b0: 653d 6465 7669 6365 290a 2020 2020 2020  e=device).      
-000071c0: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
-000071d0: 7874 7261 2e63 6163 6865 5f64 796e 5f73  xtra.cache_dyn_s
-000071e0: 697a 655f 6578 745f 6465 765b 6465 7669  ize_ext_dev[devi
-000071f0: 6365 5d0a 0a20 2020 2064 6566 2067 6574  ce]..    def get
-00007200: 5f6d 6173 6b28 7365 6c66 3a20 4469 6d2c  _mask(self: Dim,
-00007210: 202a 2c20 6469 6d5f 6f72 6465 723a 204f   *, dim_order: O
-00007220: 7074 696f 6e61 6c5b 5365 7175 656e 6365  ptional[Sequence
-00007230: 5b44 696d 5d5d 203d 204e 6f6e 652c 2064  [Dim]] = None, d
-00007240: 6576 6963 653a 204f 7074 696f 6e61 6c5b  evice: Optional[
-00007250: 7374 725d 203d 204e 6f6e 6529 202d 3e20  str] = None) -> 
-00007260: 5f74 2e54 656e 736f 723a 0a20 2020 2020  _t.Tensor:.     
-00007270: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00007280: 7061 7261 6d20 6469 6d5f 6f72 6465 723a  param dim_order:
-00007290: 2069 6620 6769 7665 6e2c 2074 6865 2064   if given, the d
-000072a0: 696d 7320 6f66 2074 6865 206d 6173 6b20  ims of the mask 
-000072b0: 7769 6c6c 2062 6520 696e 2074 6869 7320  will be in this 
-000072c0: 6f72 6465 722e 0a20 2020 2020 2020 2020  order..         
-000072d0: 2020 2054 6869 7320 6361 6e20 6265 2075     This can be u
-000072e0: 7365 6675 6c20 6966 2074 6865 206d 6173  seful if the mas
-000072f0: 6b20 6973 2062 726f 6164 6361 7374 6564  k is broadcasted
-00007300: 2061 6761 696e 7374 2073 6f6d 6520 6f74   against some ot
-00007310: 6865 7220 7465 6e73 6f72 2e0a 2020 2020  her tensor..    
-00007320: 2020 2020 3a70 6172 616d 2073 7472 7c4e      :param str|N
-00007330: 6f6e 6520 6465 7669 6365 3a20 6966 2067  one device: if g
-00007340: 6976 656e 2c20 7769 6c6c 206d 6f76 6520  iven, will move 
-00007350: 7468 6520 6d61 736b 2074 6f20 7468 6973  the mask to this
-00007360: 2064 6576 6963 650a 2020 2020 2020 2020   device.        
-00007370: 3a72 6574 7572 6e3a 2069 6620 6e65 6564  :return: if need
-00007380: 5f6d 6173 6b69 6e67 2829 2c20 7468 6520  _masking(), the 
-00007390: 636f 7272 6573 706f 6e64 696e 6720 6d61  corresponding ma
-000073a0: 736b 2e0a 2020 2020 2020 2020 2020 2020  sk..            
-000073b0: 4966 2074 6869 7320 6973 2065 2e67 2e20  If this is e.g. 
-000073c0: 7468 6520 7469 6d65 2d64 696d 2054 206f  the time-dim T o
-000073d0: 6620 7368 6170 6520 5b42 5d2c 2074 6865  f shape [B], the
-000073e0: 6e20 7468 6520 6d61 736b 2077 696c 6c20  n the mask will 
-000073f0: 6265 206f 6620 7368 6170 6520 5b42 2c54  be of shape [B,T
-00007400: 5d2e 0a20 2020 2020 2020 2020 2020 2054  ]..            T
-00007410: 6865 206d 6173 6b20 636f 756c 6420 6265  he mask could be
-00007420: 2075 7365 6420 7769 7468 203a 6675 6e63   used with :func
-00007430: 3a60 6d61 736b 6564 5f73 656c 6563 7460  :`masked_select`
-00007440: 2028 6060 626f 6f6c 6561 6e5f 6d61 736b   (``boolean_mask
-00007450: 6060 2920 6f72 2060 6077 6865 7265 6060  ``) or ``where``
-00007460: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00007470: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
-00007480: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
-00007490: 2072 660a 0a20 2020 2020 2020 2061 7373   rf..        ass
-000074a0: 6572 7420 7365 6c66 2e64 796e 5f73 697a  ert self.dyn_siz
-000074b0: 655f 6578 7420 616e 6420 7365 6c66 2e64  e_ext and self.d
-000074c0: 796e 5f73 697a 655f 6578 742e 7261 775f  yn_size_ext.raw_
-000074d0: 7465 6e73 6f72 2069 7320 6e6f 7420 4e6f  tensor is not No
-000074e0: 6e65 0a20 2020 2020 2020 2023 206e 6f69  ne.        # noi
-000074f0: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-00007500: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-00007510: 2020 2020 6261 636b 656e 6420 3d20 7365      backend = se
-00007520: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00007530: 5f72 6177 5f62 6163 6b65 6e64 0a0a 2020  _raw_backend..  
-00007540: 2020 2020 2020 6966 206e 6f74 2064 6576        if not dev
-00007550: 6963 653a 0a20 2020 2020 2020 2020 2020  ice:.           
-00007560: 2064 6576 6963 6520 3d20 7266 2e67 6574   device = rf.get
-00007570: 5f64 6566 6175 6c74 5f64 6576 6963 6528  _default_device(
-00007580: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00007590: 6c66 2e5f 6578 7472 6120 616e 6420 6465  lf._extra and de
-000075a0: 7669 6365 2069 6e20 7365 6c66 2e5f 6578  vice in self._ex
-000075b0: 7472 612e 6361 6368 655f 7365 715f 6d61  tra.cache_seq_ma
-000075c0: 736b 3a0a 2020 2020 2020 2020 2020 2020  sk:.            
-000075d0: 7265 7475 726e 2073 656c 662e 5f65 7874  return self._ext
-000075e0: 7261 2e63 6163 6865 5f73 6571 5f6d 6173  ra.cache_seq_mas
-000075f0: 6b5b 6465 7669 6365 5d0a 0a20 2020 2020  k[device]..     
-00007600: 2020 2073 697a 655f 6578 7420 3d20 7365     size_ext = se
-00007610: 6c66 2e5f 6765 745f 6479 6e5f 7369 7a65  lf._get_dyn_size
-00007620: 5f65 7874 5f66 6f72 5f64 6576 6963 6528  _ext_for_device(
-00007630: 6465 7669 6365 290a 0a20 2020 2020 2020  device)..       
-00007640: 206d 6178 5f69 6478 203d 2072 662e 7265   max_idx = rf.re
-00007650: 6475 6365 280a 2020 2020 2020 2020 2020  duce(.          
-00007660: 2020 7369 7a65 5f65 7874 2c0a 2020 2020    size_ext,.    
-00007670: 2020 2020 2020 2020 6178 6973 3d73 697a          axis=siz
-00007680: 655f 6578 742e 6469 6d73 2c0a 2020 2020  e_ext.dims,.    
-00007690: 2020 2020 2020 2020 6d6f 6465 3d22 6d61          mode="ma
-000076a0: 7822 2c0a 2020 2020 2020 2020 2020 2020  x",.            
-000076b0: 2320 4d61 736b 696e 6720 6865 7265 2069  # Masking here i
-000076c0: 7320 6e6f 7420 616c 7761 7973 2070 6f73  s not always pos
-000076d0: 7369 626c 652c 2065 2e67 2e20 6966 2077  sible, e.g. if w
-000076e0: 6520 6861 7665 0a20 2020 2020 2020 2020  e have.         
-000076f0: 2020 2023 2074 6167 203d 2044 696d 7b27     # tag = Dim{'
-00007700: 7365 6c66 2d61 7474 2d6b 6579 7327 5b27  self-att-keys'['
-00007710: 7469 6d65 3a76 6172 3a65 7874 6572 6e5f  time:var:extern_
-00007720: 6461 7461 3a63 6c61 7373 6573 275b 425d  data:classes'[B]
-00007730: 5d7d 0a20 2020 2020 2020 2020 2020 2075  ]}.            u
-00007740: 7365 5f6d 6173 6b3d 4661 6c73 652c 0a20  se_mask=False,. 
-00007750: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00007760: 2023 2057 6520 7573 6520 7468 6520 6173   # We use the as
-00007770: 7375 6d70 7469 6f6e 2074 6861 7420 7365  sumption that se
-00007780: 6c66 2e70 6c61 6365 686f 6c64 6572 2e73  lf.placeholder.s
-00007790: 6861 7065 5b61 7869 735d 203d 3d20 6d61  hape[axis] == ma
-000077a0: 785f 6964 782e 0a20 2020 2020 2020 2023  x_idx..        #
-000077b0: 2073 697a 655f 6578 7420 6d69 6768 7420   size_ext might 
-000077c0: 6861 7665 2069 6e76 616c 6964 2028 7a65  have invalid (ze
-000077d0: 726f 2920 7369 7a65 730a 2020 2020 2020  ro) sizes.      
-000077e0: 2020 2320 7768 656e 2069 7420 6974 7365    # when it itse
-000077f0: 6c66 2068 6173 2073 6f6d 6520 7061 6464  lf has some padd
-00007800: 696e 672c 2065 2e67 2e20 7768 656e 2069  ing, e.g. when i
-00007810: 7473 206f 776e 2073 6861 7065 2069 7320  ts own shape is 
-00007820: 6479 6e61 6d69 632e 0a20 2020 2020 2020  dynamic..       
-00007830: 2023 2041 207a 6572 6f20 7369 7a65 2063   # A zero size c
-00007840: 616e 206c 6561 6420 746f 2070 726f 626c  an lead to probl
-00007850: 656d 7320 696e 2073 6f6d 6520 6361 7365  ems in some case
-00007860: 732c 2065 2e67 2e20 696e 2053 6f66 746d  s, e.g. in Softm
-00007870: 6178 4f76 6572 5370 6174 6961 6c4c 6179  axOverSpatialLay
-00007880: 6572 2c0a 2020 2020 2020 2020 2320 7768  er,.        # wh
-00007890: 656e 2065 7665 7279 7468 696e 6720 6973  en everything is
-000078a0: 206d 6173 6b65 6420 746f 202d 696e 662c   masked to -inf,
-000078b0: 2069 7420 7265 7375 6c74 7320 696e 206e   it results in n
-000078c0: 616e 2c0a 2020 2020 2020 2020 2320 616e  an,.        # an
-000078d0: 6420 7468 6973 206c 696b 656c 7920 7072  d this likely pr
-000078e0: 6f64 7563 6573 206e 616e 2069 6e20 6261  oduces nan in ba
-000078f0: 636b 7072 6f70 206f 7220 656c 7365 7768  ckprop or elsewh
-00007900: 6572 652e 0a20 2020 2020 2020 2023 2054  ere..        # T
-00007910: 6875 732c 206d 6173 6b20 7369 7a65 5f65  hus, mask size_e
-00007920: 7874 2069 7473 656c 662c 2061 6e64 2073  xt itself, and s
-00007930: 6574 2074 6865 2070 6164 6465 6420 7661  et the padded va
-00007940: 6c75 6573 2074 6f20 312e 0a20 2020 2020  lues to 1..     
-00007950: 2020 2023 2054 6869 7320 6173 7375 6d65     # This assume
-00007960: 7320 7468 6174 206d 6178 5f69 6478 203e  s that max_idx >
-00007970: 3d20 312e 0a20 2020 2020 2020 2073 697a  = 1..        siz
-00007980: 655f 6578 7420 3d20 7369 7a65 5f65 7874  e_ext = size_ext
-00007990: 2e63 6f70 795f 6d61 736b 6564 286d 6178  .copy_masked(max
-000079a0: 5f69 6478 290a 2020 2020 2020 2020 7769  _idx).        wi
-000079b0: 7468 2072 662e 7365 745f 6465 6661 756c  th rf.set_defaul
-000079c0: 745f 6465 7669 6365 5f63 7478 2864 6576  t_device_ctx(dev
-000079d0: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
-000079e0: 2020 6964 785f 7261 6e67 6520 3d20 6261    idx_range = ba
-000079f0: 636b 656e 642e 7261 6e67 655f 6f76 6572  ckend.range_over
-00007a00: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00007a10: 2020 2073 6571 5f6d 6173 6b20 3d20 7266     seq_mask = rf
-00007a20: 2e63 6f6d 7061 7265 2869 6478 5f72 616e  .compare(idx_ran
-00007a30: 6765 2c20 223c 222c 2073 697a 655f 6578  ge, "<", size_ex
-00007a40: 742c 2061 6c6c 6f77 5f62 726f 6164 6361  t, allow_broadca
-00007a50: 7374 5f61 6c6c 5f73 6f75 7263 6573 3d54  st_all_sources=T
-00007a60: 7275 652c 2064 696d 5f6f 7264 6572 3d64  rue, dim_order=d
-00007a70: 696d 5f6f 7264 6572 290a 2020 2020 2020  im_order).      
-00007a80: 2020 7365 6c66 2e5f 6d61 6b65 5f65 7874    self._make_ext
-00007a90: 7261 2829 2e63 6163 6865 5f73 6571 5f6d  ra().cache_seq_m
-00007aa0: 6173 6b5b 6465 7669 6365 5d20 3d20 7365  ask[device] = se
-00007ab0: 715f 6d61 736b 0a20 2020 2020 2020 2072  q_mask.        r
-00007ac0: 6574 7572 6e20 7365 715f 6d61 736b 0a0a  eturn seq_mask..
-00007ad0: 2020 2020 6465 6620 6973 5f62 6174 6368      def is_batch
-00007ae0: 5f64 696d 2873 656c 6629 3a0a 2020 2020  _dim(self):.    
-00007af0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007b00: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
-00007b10: 2074 6869 7320 6469 6d20 7461 6720 6973   this dim tag is
-00007b20: 206f 6620 6b69 6e64 2062 6174 6368 0a20   of kind batch. 
-00007b30: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-00007b40: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-00007b50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00007b60: 656c 662e 6b69 6e64 203d 3d20 4469 6d54  elf.kind == DimT
-00007b70: 7970 6573 2e42 6174 6368 0a0a 2020 2020  ypes.Batch..    
-00007b80: 6465 6620 6973 5f66 6561 7475 7265 5f64  def is_feature_d
-00007b90: 696d 2873 656c 6629 3a0a 2020 2020 2020  im(self):.      
-00007ba0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-00007bb0: 6574 7572 6e3a 2077 6865 7468 6572 2074  eturn: whether t
-00007bc0: 6869 7320 6469 6d20 7461 6720 6973 206f  his dim tag is o
-00007bd0: 6620 6b69 6e64 2066 6561 7475 7265 0a20  f kind feature. 
-00007be0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-00007bf0: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-00007c00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00007c10: 656c 662e 6b69 6e64 203d 3d20 4469 6d54  elf.kind == DimT
-00007c20: 7970 6573 2e46 6561 7475 7265 0a0a 2020  ypes.Feature..  
-00007c30: 2020 6465 6620 6973 5f73 7061 7469 616c    def is_spatial
-00007c40: 5f64 696d 2873 656c 6629 3a0a 2020 2020  _dim(self):.    
-00007c50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007c60: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
-00007c70: 2074 6869 7320 6469 6d20 7461 6720 6973   this dim tag is
-00007c80: 206f 6620 6b69 6e64 2073 7061 7469 616c   of kind spatial
-00007c90: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00007ca0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-00007cb0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00007cc0: 2073 656c 662e 6b69 6e64 203d 3d20 4469   self.kind == Di
-00007cd0: 6d54 7970 6573 2e53 7061 7469 616c 0a0a  mTypes.Spatial..
-00007ce0: 2020 2020 6465 6620 6973 5f64 696d 5f6b      def is_dim_k
-00007cf0: 6e6f 776e 2873 656c 6629 3a0a 2020 2020  nown(self):.    
-00007d00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007d10: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
-00007d20: 2077 6520 6b6e 6f77 2074 6865 2064 696d   we know the dim
-00007d30: 656e 7369 6f6e 3b20 6261 7369 6361 6c6c  ension; basicall
-00007d40: 7920 7768 6574 6865 7220 7468 6973 2069  y whether this i
-00007d50: 7320 6465 6669 6e65 640a 2020 2020 2020  s defined.      
-00007d60: 2020 2020 2861 6c74 686f 7567 6820 606e      (although `n
-00007d70: 6f74 2073 656c 662e 756e 6465 6669 6e65  ot self.undefine
-00007d80: 6460 2069 7320 6465 6669 6e65 6420 736c  d` is defined sl
-00007d90: 6967 6874 6c79 2064 6966 6665 7265 6e74  ightly different
-00007da0: 6c79 290a 2020 2020 2020 2020 3a72 7479  ly).        :rty
-00007db0: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-00007dc0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00007dd0: 7365 6c66 2e69 735f 6261 7463 685f 6469  self.is_batch_di
-00007de0: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
-00007df0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00007e00: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00007e10: 2e69 735f 6479 6e61 6d69 6328 2920 616e  .is_dynamic() an
-00007e20: 6420 7365 6c66 2e64 696d 656e 7369 6f6e  d self.dimension
-00007e30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00007e40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007e50: 2054 7275 650a 2020 2020 2020 2020 6966   True.        if
-00007e60: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00007e70: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-00007e80: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00007e90: 2020 2020 6578 7472 6120 3d20 7365 6c66      extra = self
-00007ea0: 2e5f 6765 745f 7361 6d65 5f62 6173 655f  ._get_same_base_
-00007eb0: 6578 7472 6128 290a 2020 2020 2020 2020  extra().        
-00007ec0: 6966 2065 7874 7261 3a0a 2020 2020 2020  if extra:.      
-00007ed0: 2020 2020 2020 666f 7220 5f2c 206f 7468        for _, oth
-00007ee0: 6572 2069 6e20 6578 7472 612e 7361 6d65  er in extra.same
-00007ef0: 5f66 6f72 5f62 6174 6368 5f63 7478 2e69  _for_batch_ctx.i
-00007f00: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00007f10: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-00007f20: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00007f50: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00007f60: 6c73 650a 0a20 2020 2064 6566 2069 735f  lse..    def is_
-00007f70: 6479 6e61 6d69 6328 7365 6c66 2920 2d3e  dynamic(self) ->
-00007f80: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00007f90: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
-00007fa0: 726e 3a20 7768 6574 6865 7220 7468 6520  rn: whether the 
-00007fb0: 6469 6d20 6973 206e 6f74 2073 7461 7469  dim is not stati
-00007fc0: 632e 2075 7375 616c 6c79 206d 6561 6e73  c. usually means
-00007fd0: 2074 6861 7420 6974 2068 6173 2073 6571   that it has seq
-00007fe0: 206c 656e 6774 6873 0a20 2020 2020 2020   lengths.       
-00007ff0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00008000: 7572 6e20 7365 6c66 2e64 696d 656e 7369  urn self.dimensi
-00008010: 6f6e 2069 7320 4e6f 6e65 2061 6e64 206e  on is None and n
-00008020: 6f74 2073 656c 662e 6973 5f62 6174 6368  ot self.is_batch
-00008030: 5f64 696d 2829 0a0a 2020 2020 6465 6620  _dim()..    def 
-00008040: 6973 5f73 7461 7469 6328 7365 6c66 2920  is_static(self) 
-00008050: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00008060: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
-00008070: 7475 726e 3a20 7374 6174 6963 0a20 2020  turn: static.   
-00008080: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00008090: 2072 6574 7572 6e20 6e6f 7420 7365 6c66   return not self
-000080a0: 2e69 735f 6479 6e61 6d69 6328 290a 0a20  .is_dynamic().. 
-000080b0: 2020 2064 6566 206e 6565 645f 6d61 736b     def need_mask
-000080c0: 696e 6728 7365 6c66 293a 0a20 2020 2020  ing(self):.     
-000080d0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-000080e0: 7265 7475 726e 3a20 7768 6574 6865 7220  return: whether 
-000080f0: 6469 6d20 6973 2073 7461 7469 6320 6f72  dim is static or
-00008100: 2064 796e 616d 6963 2062 7574 2077 6974   dynamic but wit
-00008110: 6820 7363 616c 6172 2064 796e 5f73 697a  h scalar dyn_siz
-00008120: 655f 6578 740a 2020 2020 2020 2020 2222  e_ext.        ""
-00008130: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00008140: 662e 6973 5f73 7461 7469 6328 293a 0a20  f.is_static():. 
-00008150: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00008160: 6c66 2e63 6170 6163 6974 7920 6973 206e  lf.capacity is n
-00008170: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008190: 7365 6c66 2e73 697a 6520 3c20 7365 6c66  self.size < self
-000081a0: 2e63 6170 6163 6974 790a 2020 2020 2020  .capacity.      
-000081b0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000081c0: 7365 0a20 2020 2020 2020 2069 6620 7365  se.        if se
-000081d0: 6c66 2e63 6170 6163 6974 7920 6973 206e  lf.capacity is n
-000081e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000081f0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00008200: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00008210: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00008220: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00008230: 6574 7572 6e20 5472 7565 2020 2320 756e  eturn True  # un
-00008240: 6b6e 6f77 6e0a 2020 2020 2020 2020 7265  known.        re
-00008250: 7475 726e 2073 656c 662e 6479 6e5f 7369  turn self.dyn_si
-00008260: 7a65 5f65 7874 2e62 6174 6368 5f6e 6469  ze_ext.batch_ndi
-00008270: 6d20 3e20 300a 0a20 2020 2064 6566 2063  m > 0..    def c
-00008280: 616e 5f62 655f 7573 6564 5f61 735f 6469  an_be_used_as_di
-00008290: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
-000082a0: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
-000082b0: 7475 726e 3a20 7768 6574 6865 7220 7468  turn: whether th
-000082c0: 6973 2063 616e 2062 6520 7573 6564 2061  is can be used a
-000082d0: 7320 6120 6469 6d20 696e 203a 636c 6173  s a dim in :clas
-000082e0: 733a 6044 6174 6160 2c20 692e 652e 2069  s:`Data`, i.e. i
-000082f0: 7420 6973 206e 6f74 2073 7065 6369 616c  t is not special
-00008300: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00008310: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-00008320: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00008330: 206e 6f74 2073 656c 662e 7370 6563 6961   not self.specia
-00008340: 6c0a 0a20 2020 2064 6566 2069 735f 7361  l..    def is_sa
-00008350: 6d65 5f73 697a 655f 7465 6e73 6f72 2873  me_size_tensor(s
-00008360: 656c 662c 2078 293a 0a20 2020 2020 2020  elf, x):.       
-00008370: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00008380: 7261 6d20 7466 2e54 656e 736f 7220 783a  ram tf.Tensor x:
-00008390: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000083a0: 3a20 7768 6574 6865 7220 7468 6973 2064  : whether this d
-000083b0: 696d 2074 6167 2066 6f72 2074 6869 7320  im tag for this 
-000083c0: 7370 6563 6966 6963 2062 6174 6368 2028  specific batch (
-000083d0: 696e 636c 2062 6561 6d29 2069 7320 7468  incl beam) is th
-000083e0: 6520 7361 6d65 2061 7320 7468 6520 6769  e same as the gi
-000083f0: 7665 6e20 7369 7a65 0a20 2020 2020 2020  ven size.       
-00008400: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00008410: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00008420: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
-00008430: 7a65 5f65 7874 2061 6e64 2078 2069 7320  ze_ext and x is 
-00008440: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00008450: 742e 706c 6163 6568 6f6c 6465 723a 0a20  t.placeholder:. 
-00008460: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008470: 6e20 5472 7565 0a20 2020 2020 2020 2074  n True.        t
-00008480: 6167 203d 205f 4469 6d4d 6978 696e 2e67  ag = _DimMixin.g
-00008490: 6574 5f74 6167 5f66 726f 6d5f 7369 7a65  et_tag_from_size
-000084a0: 5f74 656e 736f 7228 7829 0a20 2020 2020  _tensor(x).     
-000084b0: 2020 2069 6620 7461 6720 616e 6420 7461     if tag and ta
-000084c0: 6720 3d3d 2073 656c 663a 0a20 2020 2020  g == self:.     
-000084d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000084e0: 7565 0a20 2020 2020 2020 2069 6620 6e6f  ue.        if no
-000084f0: 7420 7365 6c66 2e5f 6578 7472 613a 0a20  t self._extra:. 
-00008500: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008510: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00008520: 6966 2075 7469 6c2e 5265 6649 6445 7128  if util.RefIdEq(
-00008530: 7829 2069 6e20 7365 6c66 2e5f 6578 7472  x) in self._extr
-00008540: 612e 6479 6e5f 7369 7a65 5f73 616d 653a  a.dyn_size_same:
-00008550: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008560: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00008570: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00008580: 2020 2064 6566 2073 6574 5f74 6167 5f6f     def set_tag_o
-00008590: 6e5f 7369 7a65 5f74 656e 736f 7228 7365  n_size_tensor(se
-000085a0: 6c66 3a20 4469 6d2c 2078 2c20 6261 7463  lf: Dim, x, batc
-000085b0: 683d 4e6f 6e65 2c20 7361 6d65 5f61 735f  h=None, same_as_
-000085c0: 6265 666f 7265 3d46 616c 7365 2920 2d3e  before=False) ->
-000085d0: 2044 696d 3a0a 2020 2020 2020 2020 2222   Dim:.        ""
-000085e0: 220a 2020 2020 2020 2020 5468 6973 2066  ".        This f
-000085f0: 756e 6374 696f 6e20 6973 2075 7365 640a  unction is used.
-00008600: 2020 2020 2020 2020 746f 2063 6f75 706c          to coupl
-00008610: 6520 6120 7466 2e54 656e 736f 7220 696e  e a tf.Tensor in
-00008620: 7374 616e 6365 2072 6570 7265 7365 6e74  stance represent
-00008630: 696e 6720 7468 6520 6479 6e20 7369 7a65  ing the dyn size
-00008640: 0a20 2020 2020 2020 2077 6974 6820 7468  .        with th
-00008650: 6520 6469 6d20 7461 672e 0a0a 2020 2020  e dim tag...    
-00008660: 2020 2020 5468 6973 2069 7320 7573 7561      This is usua
-00008670: 6c6c 7920 6120 6e65 776c 7920 6372 6561  lly a newly crea
-00008680: 7465 6420 6469 6d20 7461 672c 0a20 2020  ted dim tag,.   
-00008690: 2020 2020 2077 6869 6368 2069 7320 7965       which is ye
-000086a0: 7420 756e 7365 742e 0a0a 2020 2020 2020  t unset...      
-000086b0: 2020 4974 2069 7320 616c 736f 2075 7365    It is also use
-000086c0: 6420 746f 2063 6f75 706c 6520 616e 2065  d to couple an e
-000086d0: 7869 7374 696e 6720 6469 6d20 7461 6720  xisting dim tag 
-000086e0: 7769 7468 206f 7468 6572 2064 796e 2073  with other dyn s
-000086f0: 697a 6573 0a20 2020 2020 2020 2077 6869  izes.        whi
-00008700: 6368 206a 7573 7420 6469 6666 6572 2062  ch just differ b
-00008710: 7920 616e 2065 7870 616e 7369 6f6e 206f  y an expansion o
-00008720: 6620 7468 6520 6261 7463 6820 2865 2e67  f the batch (e.g
-00008730: 2e20 7365 6172 6368 2062 6561 6d29 2e0a  . search beam)..
-00008740: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
-00008750: 6f20 3a66 756e 633a 6067 6574 5f74 6167  o :func:`get_tag
-00008760: 5f66 726f 6d5f 7369 7a65 5f74 656e 736f  _from_size_tenso
-00008770: 7260 2e0a 2020 2020 2020 2020 416c 736f  r`..        Also
-00008780: 2073 6565 203a 6675 6e63 3a60 7365 745f   see :func:`set_
-00008790: 6479 6e5f 7369 7a65 5f65 7874 5f66 6f72  dyn_size_ext_for
-000087a0: 5f62 6174 6368 5f63 7478 602e 0a0a 2020  _batch_ctx`...  
-000087b0: 2020 2020 2020 3a70 6172 616d 2078 3a20        :param x: 
-000087c0: 7261 7720 7465 6e73 6f72 2c20 666f 7220  raw tensor, for 
-000087d0: 6578 616d 706c 6520 7466 2e54 656e 736f  example tf.Tenso
-000087e0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-000087f0: 2042 6174 6368 496e 666f 7c4e 6f6e 6520   BatchInfo|None 
-00008800: 6261 7463 683a 0a20 2020 2020 2020 203a  batch:.        :
-00008810: 7061 7261 6d20 626f 6f6c 2073 616d 655f  param bool same_
-00008820: 6173 5f62 6566 6f72 653a 2069 6d70 6c69  as_before: impli
-00008830: 6573 2069 7420 7761 7320 7365 7420 6265  es it was set be
-00008840: 666f 7265 2c20 616e 6420 7468 6520 6e65  fore, and the ne
-00008850: 7720 7369 7a65 2069 7320 7468 6520 7361  w size is the sa
-00008860: 6d65 2e0a 2020 2020 2020 2020 2020 652e  me..          e.
-00008870: 672e 2069 7420 636f 756c 6420 6265 2073  g. it could be s
-00008880: 6f6d 6520 6964 656e 7469 7479 2077 6974  ome identity wit
-00008890: 6820 6164 6465 6420 6368 6563 6b73 2c20  h added checks, 
-000088a0: 6f72 206f 7468 6572 2063 6861 6e67 652e  or other change.
-000088b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000088c0: 3a20 7365 6c66 206f 7220 6e65 7720 6469  : self or new di
-000088d0: 6d20 7461 670a 2020 2020 2020 2020 2222  m tag.        ""
-000088e0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-000088f0: 2073 656c 662e 6361 6e5f 6265 5f75 7365   self.can_be_use
-00008900: 645f 6173 5f64 696d 2829 0a20 2020 2020  d_as_dim().     
-00008910: 2020 2023 2049 7427 7320 756e 7573 7561     # It's unusua
-00008920: 6c20 6966 2073 656c 662e 6469 6d65 6e73  l if self.dimens
-00008930: 696f 6e20 6973 206e 6f74 204e 6f6e 652c  ion is not None,
-00008940: 2062 7574 206c 6574 2773 2061 6363 6570   but let's accep
-00008950: 7420 7468 6174 2e0a 2020 2020 2020 2020  t that..        
-00008960: 6966 2068 6173 6174 7472 2878 2c20 225f  if hasattr(x, "_
-00008970: 6973 5f73 697a 655f 6f66 5f64 696d 5f74  is_size_of_dim_t
-00008980: 6167 2229 3a0a 2020 2020 2020 2020 2020  ag"):.          
-00008990: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
-000089a0: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
-000089b0: 6572 0a20 2020 2020 2020 2020 2020 2061  er.            a
-000089c0: 7373 6572 7420 782e 5f69 735f 7369 7a65  ssert x._is_size
-000089d0: 5f6f 665f 6469 6d5f 7461 6720 696e 2028  _of_dim_tag in (
-000089e0: 4e6f 6e65 2c20 7365 6c66 290a 2020 2020  None, self).    
-000089f0: 2020 2020 2320 4966 2077 6520 616c 7265      # If we alre
-00008a00: 6164 7920 6861 7665 2061 6e6f 7468 6572  ady have another
-00008a10: 2064 796e 2073 697a 6520 7365 7420 6f72   dyn size set or
-00008a20: 2064 6966 6665 7265 6e74 2062 6174 6368   different batch
-00008a30: 2c20 6372 6561 7465 2061 206e 6577 2044  , create a new D
-00008a40: 696d 2069 6e73 7461 6e63 652e 0a20 2020  im instance..   
-00008a50: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-00008a60: 6368 2061 6e64 2062 6174 6368 2061 6e64  ch and batch and
-00008a70: 2073 656c 662e 6261 7463 6820 213d 2062   self.batch != b
-00008a80: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-00008a90: 2020 6173 7365 7274 206e 6f74 2073 616d    assert not sam
-00008aa0: 655f 6173 5f62 6566 6f72 6520 2023 2069  e_as_before  # i
-00008ab0: 7420 6361 6e6e 6f74 2062 6520 7468 6520  t cannot be the 
-00008ac0: 7361 6d65 2077 6865 6e20 6974 2069 7320  same when it is 
-00008ad0: 616e 6f74 6865 7220 6261 7463 682e 2e2e  another batch...
-00008ae0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-00008af0: 5f64 696d 5f74 6167 203d 2073 656c 662e  _dim_tag = self.
-00008b00: 6765 745f 666f 725f 6261 7463 685f 6374  get_for_batch_ct
-00008b10: 7828 6261 7463 683d 6261 7463 682c 2063  x(batch=batch, c
-00008b20: 7478 3d73 656c 662e 636f 6e74 726f 6c5f  tx=self.control_
-00008b30: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
-00008b40: 2020 2020 2020 6e65 775f 6469 6d5f 7461        new_dim_ta
-00008b50: 672e 7365 745f 7461 675f 6f6e 5f73 697a  g.set_tag_on_siz
-00008b60: 655f 7465 6e73 6f72 2878 2c20 6261 7463  e_tensor(x, batc
-00008b70: 683d 6261 7463 6829 0a20 2020 2020 2020  h=batch).       
-00008b80: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
-00008b90: 6469 6d5f 7461 670a 2020 2020 2020 2020  dim_tag.        
-00008ba0: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-00008bb0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00008bc0: 2073 656c 662e 6479 6e5f 7369 7a65 2069   self.dyn_size i
-00008bd0: 7320 6e6f 7420 783a 0a20 2020 2020 2020  s not x:.       
-00008be0: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
-00008bf0: 7472 6120 616e 6420 7574 696c 2e52 6566  tra and util.Ref
-00008c00: 4964 4571 2878 2920 696e 2073 656c 662e  IdEq(x) in self.
-00008c10: 5f65 7874 7261 2e64 796e 5f73 697a 655f  _extra.dyn_size_
-00008c20: 7361 6d65 3a0a 2020 2020 2020 2020 2020  same:.          
-00008c30: 2020 2020 2020 7061 7373 2020 2320 6f6b        pass  # ok
-00008c40: 2c20 7061 7373 206f 6e0a 2020 2020 2020  , pass on.      
-00008c50: 2020 2020 2020 656c 6966 2073 616d 655f        elif same_
-00008c60: 6173 5f62 6566 6f72 653a 0a20 2020 2020  as_before:.     
-00008c70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008c80: 5f6d 616b 655f 6578 7472 6128 292e 6479  _make_extra().dy
-00008c90: 6e5f 7369 7a65 5f73 616d 652e 6164 6428  n_size_same.add(
-00008ca0: 7574 696c 2e52 6566 4964 4571 2878 2929  util.RefIdEq(x))
-00008cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008cc0: 2023 2041 6e64 206e 6f77 2070 6173 7320   # And now pass 
-00008cd0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00008ce0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008cf0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00008d00: 662e 6261 7463 6820 616e 6420 6261 7463  f.batch and batc
-00008d10: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-00008d20: 2020 2320 4974 2773 206e 6f74 2063 6c65    # It's not cle
-00008d30: 6172 2077 6861 7420 746f 2064 6f2e 2057  ar what to do. W
-00008d40: 6520 636f 756c 6420 6372 6561 7465 2061  e could create a
-00008d50: 206e 6577 2064 696d 2074 6167 2c20 6275   new dim tag, bu
-00008d60: 7420 7468 6520 7369 7a65 7320 6d69 6768  t the sizes migh
-00008d70: 7420 6265 2064 6966 6665 7265 6e74 2e0a  t be different..
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2320 5573 7561 6c6c 7920 7765 2073 686f  # Usually we sho
-00008da0: 756c 6420 6e6f 7420 6765 7420 6865 7265  uld not get here
-00008db0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008dc0: 2020 2320 536f 2066 6f72 206e 6f77 2c20    # So for now, 
-00008dd0: 6a75 7374 2065 7272 6f72 2e0a 2020 2020  just error..    
-00008de0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-00008df0: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
-00008e00: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
-00008e10: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-00008e20: 6d20 7265 7475 726e 6e2e 6672 6f6e 7465  m returnn.fronte
-00008e30: 6e64 2e5f 6261 636b 656e 6420 696d 706f  nd._backend impo
-00008e40: 7274 2067 6574 5f62 6163 6b65 6e64 5f62  rt get_backend_b
-00008e50: 795f 7261 775f 7465 6e73 6f72 5f74 7970  y_raw_tensor_typ
-00008e60: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-00008e70: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-00008e80: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00008e90: 2020 2020 2020 2020 225c 6e22 2e6a 6f69          "\n".joi
-00008ea0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00008eb0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00005b50: 2020 6173 7365 7274 2063 616e 6469 6461    assert candida
+00005b60: 7465 2e64 796e 5f73 697a 655f 6578 742e  te.dyn_size_ext.
+00005b70: 6469 6d5f 7461 6773 203d 3d20 6479 6e5f  dim_tags == dyn_
+00005b80: 7369 7a65 5f65 7874 2e64 696d 5f74 6167  size_ext.dim_tag
+00005b90: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00005ba0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bc0: 2020 2020 6361 6e64 6964 6174 652e 6479      candidate.dy
+00005bd0: 6e5f 7369 7a65 5f65 7874 203d 2064 796e  n_size_ext = dyn
+00005be0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
+00005bf0: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00005c00: 7365 7274 206e 6f74 2063 616e 6469 6461  sert not candida
+00005c10: 7465 2e64 796e 5f73 697a 655f 6578 742e  te.dyn_size_ext.
+00005c20: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00005c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c40: 2065 6c69 6620 6361 6e64 6964 6174 652e   elif candidate.
+00005c50: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 2020 6361 6e64 6964 6174 652e 6479 6e5f    candidate.dyn_
+00005c80: 7369 7a65 5f65 7874 2e62 6174 6368 203d  size_ext.batch =
+00005c90: 2062 6174 6368 0a20 2020 2020 2020 2020   batch.         
+00005ca0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2063 616e 6469 6461 7465 2e63 6f6d 706c   candidate.compl
+00005cd0: 6574 655f 6479 6e5f 7369 7a65 2874 656d  ete_dyn_size(tem
+00005ce0: 706c 6174 655f 6f6e 6c79 3d54 7275 6529  plate_only=True)
+00005cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d00: 2064 696d 5f74 6167 203d 2063 616e 6469   dim_tag = candi
+00005d10: 6461 7465 0a20 2020 2020 2020 2020 2020  date.           
+00005d20: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+00005d30: 2020 2069 6620 6e6f 7420 6469 6d5f 7461     if not dim_ta
+00005d40: 673a 0a20 2020 2020 2020 2020 2020 2064  g:.            d
+00005d50: 696d 5f74 6167 203d 205f 642e 4469 6d28  im_tag = _d.Dim(
+00005d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d70: 206b 696e 643d 7365 6c66 2e6b 696e 642c   kind=self.kind,
+00005d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d90: 2064 6573 6372 6970 7469 6f6e 3d73 656c   description=sel
+00005da0: 662e 6465 7363 7269 7074 696f 6e2c 0a20  f.description,. 
+00005db0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005dc0: 696d 656e 7369 6f6e 3d73 656c 662e 6469  imension=self.di
+00005dd0: 6d65 6e73 696f 6e2c 0a20 2020 2020 2020  mension,.       
+00005de0: 2020 2020 2020 2020 2061 7574 6f5f 6765           auto_ge
+00005df0: 6e65 7261 7465 643d 7365 6c66 2e61 7574  nerated=self.aut
+00005e00: 6f5f 6765 6e65 7261 7465 642c 0a20 2020  o_generated,.   
+00005e10: 2020 2020 2020 2020 2020 2020 2062 6174               bat
+00005e20: 6368 3d62 6174 6368 2c0a 2020 2020 2020  ch=batch,.      
+00005e30: 2020 2020 2020 2020 2020 636f 6e74 726f            contro
+00005e40: 6c5f 666c 6f77 5f63 7478 3d63 7478 2c0a  l_flow_ctx=ctx,.
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 6479 6e5f 7369 7a65 5f65 7874 3d64 796e  dyn_size_ext=dyn
+00005e70: 5f73 697a 655f 6578 742c 0a20 2020 2020  _size_ext,.     
+00005e80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005e90: 2020 2020 2064 696d 5f74 6167 2e73 616d       dim_tag.sam
+00005ea0: 655f 6173 203d 2073 616d 655f 6261 7365  e_as = same_base
+00005eb0: 0a20 2020 2020 2020 2069 6620 6479 6e5f  .        if dyn_
+00005ec0: 7369 7a65 5f65 7874 2061 6e64 2064 796e  size_ext and dyn
+00005ed0: 5f73 697a 655f 6578 742e 706c 6163 6568  _size_ext.placeh
+00005ee0: 6f6c 6465 7220 6973 206e 6f74 204e 6f6e  older is not Non
+00005ef0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00005f00: 6620 5f64 2e44 696d 2e67 6574 5f74 6167  f _d.Dim.get_tag
+00005f10: 5f66 726f 6d5f 7369 7a65 5f74 656e 736f  _from_size_tenso
+00005f20: 7228 6479 6e5f 7369 7a65 5f65 7874 2e70  r(dyn_size_ext.p
+00005f30: 6c61 6365 686f 6c64 6572 2920 6973 204e  laceholder) is N
+00005f40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00005f50: 2020 2020 2064 696d 5f74 6167 2e73 6574       dim_tag.set
+00005f60: 5f74 6167 5f6f 6e5f 7369 7a65 5f74 656e  _tag_on_size_ten
+00005f70: 736f 7228 6479 6e5f 7369 7a65 5f65 7874  sor(dyn_size_ext
+00005f80: 2e70 6c61 6365 686f 6c64 6572 2c20 6261  .placeholder, ba
+00005f90: 7463 683d 6261 7463 6829 0a20 2020 2020  tch=batch).     
+00005fa0: 2020 2073 616d 655f 6261 7365 5f65 7874     same_base_ext
+00005fb0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+00005fc0: 685f 6374 785b 2862 6174 6368 2c20 6374  h_ctx[(batch, ct
+00005fd0: 7829 5d20 3d20 6469 6d5f 7461 670a 2020  x)] = dim_tag.  
+00005fe0: 2020 2020 2020 6469 6d5f 7461 672e 636f        dim_tag.co
+00005ff0: 6d70 6c65 7465 5f64 796e 5f73 697a 6528  mplete_dyn_size(
+00006000: 7465 6d70 6c61 7465 5f6f 6e6c 793d 5472  template_only=Tr
+00006010: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
+00006020: 726e 2064 696d 5f74 6167 0a0a 2020 2020  rn dim_tag..    
+00006030: 6465 6620 7265 7365 745f 6261 7463 685f  def reset_batch_
+00006040: 6374 7828 7365 6c66 3a20 4469 6d29 3a0a  ctx(self: Dim):.
+00006050: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006060: 2020 2020 466f 7220 7468 6520 7365 6c66      For the self
+00006070: 2069 6e73 7461 6e63 652c 2072 6573 6574   instance, reset
+00006080: 2062 6174 6368 2061 6e64 2063 6f6e 7465   batch and conte
+00006090: 7874 2e0a 2020 2020 2020 2020 2222 220a  xt..        """.
+000060a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000060b0: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
+000060c0: 2020 2020 7365 6c66 2e5f 6578 7472 612e      self._extra.
+000060d0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
+000060e0: 7478 2e70 6f70 2828 7365 6c66 2e62 6174  tx.pop((self.bat
+000060f0: 6368 2c20 7365 6c66 2e63 6f6e 7472 6f6c  ch, self.control
+00006100: 5f66 6c6f 775f 6374 7829 2c20 4e6f 6e65  _flow_ctx), None
+00006110: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+00006120: 6174 6368 203d 204e 6f6e 650a 2020 2020  atch = None.    
+00006130: 2020 2020 7365 6c66 2e63 6f6e 7472 6f6c      self.control
+00006140: 5f66 6c6f 775f 6374 7820 3d20 4e6f 6e65  _flow_ctx = None
+00006150: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00006160: 2e64 796e 5f73 697a 655f 6578 7420 616e  .dyn_size_ext an
+00006170: 6420 7365 6c66 2e64 796e 5f73 697a 655f  d self.dyn_size_
+00006180: 6578 742e 6261 7463 683a 0a20 2020 2020  ext.batch:.     
+00006190: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
+000061a0: 7369 7a65 5f65 7874 203d 2073 656c 662e  size_ext = self.
+000061b0: 6479 6e5f 7369 7a65 5f65 7874 2e63 6f70  dyn_size_ext.cop
+000061c0: 795f 7465 6d70 6c61 7465 2829 0a20 2020  y_template().   
+000061d0: 2020 2020 2020 2020 2073 656c 662e 6479           self.dy
+000061e0: 6e5f 7369 7a65 5f65 7874 2e62 6174 6368  n_size_ext.batch
+000061f0: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
+00006200: 2073 6574 5f64 796e 5f73 697a 655f 6578   set_dyn_size_ex
+00006210: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
+00006220: 7365 6c66 2c20 6261 7463 682c 2063 7478  self, batch, ctx
+00006230: 2c20 6479 6e5f 7369 7a65 5f65 7874 293a  , dyn_size_ext):
+00006240: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006250: 2020 2020 203a 7061 7261 6d20 4261 7463       :param Batc
+00006260: 6849 6e66 6f20 6261 7463 683a 0a20 2020  hInfo batch:.   
+00006270: 2020 2020 203a 7061 7261 6d20 436f 6e74       :param Cont
+00006280: 726f 6c46 6c6f 7743 6f6e 7465 7874 7c4e  rolFlowContext|N
+00006290: 6f6e 6520 6374 783a 0a20 2020 2020 2020  one ctx:.       
+000062a0: 203a 7061 7261 6d20 4461 7461 2064 796e   :param Data dyn
+000062b0: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+000062c0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+000062d0: 7373 6572 7420 7365 6c66 2e63 616e 5f62  ssert self.can_b
+000062e0: 655f 7573 6564 5f61 735f 6469 6d28 290a  e_used_as_dim().
+000062f0: 2020 2020 2020 2020 7361 6d65 203d 2073          same = s
+00006300: 656c 662e 6765 745f 666f 725f 6261 7463  elf.get_for_batc
+00006310: 685f 6374 7828 6261 7463 682c 2063 7478  h_ctx(batch, ctx
+00006320: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00006330: 2064 796e 5f73 697a 655f 6578 742e 6261   dyn_size_ext.ba
+00006340: 7463 6820 3d3d 2062 6174 6368 2061 6e64  tch == batch and
+00006350: 2064 796e 5f73 697a 655f 6578 742e 636f   dyn_size_ext.co
+00006360: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
+00006370: 3d20 6374 780a 2020 2020 2020 2020 6966  = ctx.        if
+00006380: 2073 616d 652e 6479 6e5f 7369 7a65 5f65   same.dyn_size_e
+00006390: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+000063a0: 6173 7365 7274 2073 616d 652e 6479 6e5f  assert same.dyn_
+000063b0: 7369 7a65 5f65 7874 2e64 696d 5f74 6167  size_ext.dim_tag
+000063c0: 7320 3d3d 2064 796e 5f73 697a 655f 6578  s == dyn_size_ex
+000063d0: 742e 6469 6d5f 7461 6773 0a20 2020 2020  t.dim_tags.     
+000063e0: 2020 2020 2020 2069 6620 6479 6e5f 7369         if dyn_si
+000063f0: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
+00006400: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 7361 6d65 2e64 796e 5f73 697a 655f 6578  same.dyn_size_ex
+00006430: 742e 706c 6163 6568 6f6c 6465 7220 3d20  t.placeholder = 
+00006440: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+00006450: 6365 686f 6c64 6572 0a20 2020 2020 2020  ceholder.       
+00006460: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006470: 2020 2073 616d 652e 6479 6e5f 7369 7a65     same.dyn_size
+00006480: 5f65 7874 203d 2064 796e 5f73 697a 655f  _ext = dyn_size_
+00006490: 6578 740a 2020 2020 2020 2020 7365 6c66  ext.        self
+000064a0: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
+000064b0: 0a0a 2020 2020 6465 6620 6765 745f 6479  ..    def get_dy
+000064c0: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
+000064d0: 6174 6368 5f63 7478 2873 656c 662c 2062  atch_ctx(self, b
+000064e0: 6174 6368 2c20 6374 782c 2074 656d 706c  atch, ctx, templ
+000064f0: 6174 655f 6f6e 6c79 3d46 616c 7365 293a  ate_only=False):
+00006500: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006510: 2020 2020 203a 7061 7261 6d20 4261 7463       :param Batc
+00006520: 6849 6e66 6f7c 4e6f 6e65 2062 6174 6368  hInfo|None batch
+00006530: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00006540: 2043 6f6e 7472 6f6c 466c 6f77 436f 6e74   ControlFlowCont
+00006550: 6578 747c 4e6f 6e65 2063 7478 3a0a 2020  ext|None ctx:.  
+00006560: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
+00006570: 6c20 7465 6d70 6c61 7465 5f6f 6e6c 793a  l template_only:
+00006580: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00006590: 2044 6174 617c 4e6f 6e65 0a20 2020 2020   Data|None.     
+000065a0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+000065b0: 7373 6572 7420 7365 6c66 2e63 616e 5f62  ssert self.can_b
+000065c0: 655f 7573 6564 5f61 735f 6469 6d28 290a  e_used_as_dim().
+000065d0: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
+000065e0: 6174 6368 2061 6e64 2073 656c 662e 6261  atch and self.ba
+000065f0: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
+00006600: 2023 2041 7373 756d 6520 676c 6f62 616c   # Assume global
+00006610: 2062 6174 6368 2e0a 2020 2020 2020 2020   batch..        
+00006620: 2020 2020 6261 7463 6820 3d20 7365 6c66      batch = self
+00006630: 2e62 6174 6368 2e67 6574 5f67 6c6f 6261  .batch.get_globa
+00006640: 6c5f 6261 7365 2829 0a20 2020 2020 2020  l_base().       
+00006650: 2069 6620 6e6f 7420 6261 7463 683a 0a20   if not batch:. 
+00006660: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+00006670: 7320 6973 2075 7375 616c 6c79 206e 6f74  s is usually not
+00006680: 2076 616c 6964 2e20 486f 7765 7665 722c   valid. However,
+00006690: 2074 6869 7320 6361 7365 2063 616e 2068   this case can h
+000066a0: 6170 7065 6e20 6561 726c 7920 6174 2069  appen early at i
+000066b0: 6e69 7469 616c 697a 6174 696f 6e2e 0a20  nitialization.. 
+000066c0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000066d0: 7420 6261 7463 6820 3d3d 2073 656c 662e  t batch == self.
+000066e0: 6261 7463 6820 616e 6420 6374 7820 3d3d  batch and ctx ==
+000066f0: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
+00006700: 6f77 5f63 7478 0a20 2020 2020 2020 2020  ow_ctx.         
+00006710: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
+00006720: 796e 5f73 697a 655f 6578 740a 2020 2020  yn_size_ext.    
+00006730: 2020 2020 7361 6d65 203d 2073 656c 662e      same = self.
+00006740: 6765 745f 666f 725f 6261 7463 685f 6374  get_for_batch_ct
+00006750: 7828 6261 7463 682c 2063 7478 2c20 616c  x(batch, ctx, al
+00006760: 6c6f 775f 6e6f 6e65 3d54 7275 6529 0a20  low_none=True). 
+00006770: 2020 2020 2020 2069 6620 6e6f 7420 7361         if not sa
+00006780: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00006790: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+000067a0: 2020 2020 7361 6d65 2e63 6f6d 706c 6574      same.complet
+000067b0: 655f 6479 6e5f 7369 7a65 2874 656d 706c  e_dyn_size(templ
+000067c0: 6174 655f 6f6e 6c79 3d74 656d 706c 6174  ate_only=templat
+000067d0: 655f 6f6e 6c79 290a 2020 2020 2020 2020  e_only).        
+000067e0: 7265 7475 726e 2073 616d 652e 6479 6e5f  return same.dyn_
+000067f0: 7369 7a65 5f65 7874 0a0a 2020 2020 4070  size_ext..    @p
+00006800: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00006810: 6479 6e5f 7369 7a65 2873 656c 6629 3a0a  dyn_size(self):.
+00006820: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006830: 2020 2020 3a72 6574 7572 6e3a 2064 796e      :return: dyn
+00006840: 2073 697a 6520 2f20 7365 7120 6c65 6e20   size / seq len 
+00006850: 2875 7375 616c 6c79 206f 6620 7368 6170  (usually of shap
+00006860: 6520 5b42 5d29 2c20 6f72 204e 6f6e 650a  e [B]), or None.
+00006870: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+00006880: 2064 796e 2073 697a 6520 6361 6e20 706f   dyn size can po
+00006890: 7465 6e74 6961 6c6c 7920 6265 206f 6620  tentially be of 
+000068a0: 6120 6469 6666 6572 656e 7420 7368 6170  a different shap
+000068b0: 652c 2064 6972 6563 746c 7920 6163 6365  e, directly acce
+000068c0: 7373 2064 796e 5f73 697a 655f 6578 742e  ss dyn_size_ext.
+000068d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000068e0: 2074 662e 5465 6e73 6f72 7c4e 6f6e 650a   tf.Tensor|None.
+000068f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006900: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
+00006910: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
+00006920: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00006930: 662e 6479 6e5f 7369 7a65 5f65 7874 2e70  f.dyn_size_ext.p
+00006940: 6c61 6365 686f 6c64 6572 0a20 2020 2020  laceholder.     
+00006950: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00006960: 2020 2020 4064 796e 5f73 697a 652e 7365      @dyn_size.se
+00006970: 7474 6572 0a20 2020 2064 6566 2064 796e  tter.    def dyn
+00006980: 5f73 697a 6528 7365 6c66 2c20 6479 6e5f  _size(self, dyn_
+00006990: 7369 7a65 293a 0a20 2020 2020 2020 2022  size):.        "
+000069a0: 2222 0a20 2020 2020 2020 2041 6c73 6f20  "".        Also 
+000069b0: 7365 6520 3a66 756e 633a 6073 6574 5f64  see :func:`set_d
+000069c0: 796e 5f73 697a 655f 6578 745f 666f 725f  yn_size_ext_for_
+000069d0: 6261 7463 685f 6374 7860 2e0a 0a20 2020  batch_ctx`...   
+000069e0: 2020 2020 203a 7061 7261 6d20 7466 2e54       :param tf.T
+000069f0: 656e 736f 7220 6479 6e5f 7369 7a65 3a0a  ensor dyn_size:.
+00006a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006a10: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
+00006a20: 7369 7a65 5f65 7874 2061 6e64 2073 656c  size_ext and sel
+00006a30: 662e 6479 6e5f 7369 7a65 5f65 7874 2e70  f.dyn_size_ext.p
+00006a40: 6c61 6365 686f 6c64 6572 2069 7320 6479  laceholder is dy
+00006a50: 6e5f 7369 7a65 3a20 2023 2066 6173 7420  n_size:  # fast 
+00006a60: 7061 7468 2063 6865 636b 0a20 2020 2020  path check.     
+00006a70: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00006a80: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+00006a90: 662e 6361 6e5f 6265 5f75 7365 645f 6173  f.can_be_used_as
+00006aa0: 5f64 696d 2829 0a20 2020 2020 2020 206f  _dim().        o
+00006ab0: 7468 6572 203d 205f 642e 4469 6d2e 6765  ther = _d.Dim.ge
+00006ac0: 745f 7461 675f 6672 6f6d 5f73 697a 655f  t_tag_from_size_
+00006ad0: 7465 6e73 6f72 2864 796e 5f73 697a 6529  tensor(dyn_size)
+00006ae0: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+00006af0: 723a 0a20 2020 2020 2020 2020 2020 2073  r:.            s
+00006b00: 656c 662e 6465 636c 6172 655f 7361 6d65  elf.declare_same
+00006b10: 5f61 7328 6f74 6865 7229 0a20 2020 2020  _as(other).     
+00006b20: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00006b30: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+00006b40: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+00006b50: 662e 6261 7463 6820 3d3d 206f 7468 6572  f.batch == other
+00006b60: 2e62 6174 6368 2061 6e64 2073 656c 662e  .batch and self.
+00006b70: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00006b80: 203d 3d20 6f74 6865 722e 636f 6e74 726f   == other.contro
+00006b90: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
+00006ba0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006bb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006bc0: 662e 6261 7463 6820 3d20 6f74 6865 722e  f.batch = other.
+00006bd0: 6261 7463 680a 2020 2020 2020 2020 2020  batch.          
+00006be0: 2020 2020 2020 7365 6c66 2e63 6f6e 7472        self.contr
+00006bf0: 6f6c 5f66 6c6f 775f 6374 7820 3d20 6f74  ol_flow_ctx = ot
+00006c00: 6865 722e 636f 6e74 726f 6c5f 666c 6f77  her.control_flow
+00006c10: 5f63 7478 0a20 2020 2020 2020 2020 2020  _ctx.           
+00006c20: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00006c30: 7874 203d 206f 7468 6572 2e64 796e 5f73  xt = other.dyn_s
+00006c40: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+00006c50: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00006c60: 2020 2073 656c 662e 5f69 6e69 745f 6465     self._init_de
+00006c70: 6661 756c 745f 6479 6e5f 7369 7a65 5f65  fault_dyn_size_e
+00006c80: 7874 2864 796e 5f73 697a 6529 0a20 2020  xt(dyn_size).   
+00006c90: 2020 2020 2073 656c 662e 7365 745f 7461       self.set_ta
+00006ca0: 675f 6f6e 5f73 697a 655f 7465 6e73 6f72  g_on_size_tensor
+00006cb0: 2864 796e 5f73 697a 6529 0a0a 2020 2020  (dyn_size)..    
+00006cc0: 6465 6620 5f69 6e69 745f 6465 6661 756c  def _init_defaul
+00006cd0: 745f 6479 6e5f 7369 7a65 5f65 7874 2873  t_dyn_size_ext(s
+00006ce0: 656c 662c 2064 796e 5f73 697a 6529 3a0a  elf, dyn_size):.
+00006cf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006d00: 2020 2020 3a70 6172 616d 2074 662e 5465      :param tf.Te
+00006d10: 6e73 6f72 2064 796e 5f73 697a 653a 0a20  nsor dyn_size:. 
+00006d20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006d30: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
+00006d40: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
+00006d50: 2020 2020 2069 6620 7365 6c66 2e64 796e       if self.dyn
+00006d60: 5f73 697a 655f 6578 742e 706c 6163 6568  _size_ext.placeh
+00006d70: 6f6c 6465 7220 6973 206e 6f74 204e 6f6e  older is not Non
+00006d80: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006d90: 2020 2023 2044 6f20 6e6f 7420 616c 6c6f     # Do not allo
+00006da0: 7720 7265 7365 7474 696e 6720 6974 2074  w resetting it t
+00006db0: 6f20 7374 6820 6469 6666 6572 656e 742e  o sth different.
+00006dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006dd0: 2061 7373 6572 7420 7365 6c66 2e64 796e   assert self.dyn
+00006de0: 5f73 697a 655f 6578 742e 706c 6163 6568  _size_ext.placeh
+00006df0: 6f6c 6465 7220 6973 2064 796e 5f73 697a  older is dyn_siz
+00006e00: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
+00006e10: 2020 2020 2020 2020 2020 2020 6265 616d              beam
+00006e20: 203d 2067 6574 6174 7472 2864 796e 5f73   = getattr(dyn_s
+00006e30: 697a 652c 2022 5f52 4554 5552 4e4e 5f64  ize, "_RETURNN_d
+00006e40: 796e 5f73 697a 655f 6265 616d 222c 204e  yn_size_beam", N
+00006e50: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+00006e60: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00006e70: 7874 203d 205f 742e 5465 6e73 6f72 280a  xt = _t.Tensor(.
+00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e90: 6e61 6d65 3d28 2225 733a 6479 6e5f 7369  name=("%s:dyn_si
+00006ea0: 7a65 2220 2520 7365 6c66 2e64 6573 6372  ze" % self.descr
+00006eb0: 6970 7469 6f6e 2920 6966 2073 656c 662e  iption) if self.
+00006ec0: 6465 7363 7269 7074 696f 6e20 656c 7365  description else
+00006ed0: 2064 796e 5f73 697a 652e 6f70 2e6e 616d   dyn_size.op.nam
+00006ee0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00006ef0: 2020 2064 7479 7065 3d5f 742e 5465 6e73     dtype=_t.Tens
+00006f00: 6f72 2e73 697a 655f 6474 7970 652c 0a20  or.size_dtype,. 
+00006f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006f20: 6861 7065 3d28 292c 0a20 2020 2020 2020  hape=(),.       
+00006f30: 2020 2020 2020 2020 2062 6174 6368 5f64           batch_d
+00006f40: 696d 5f61 7869 733d 302c 0a20 2020 2020  im_axis=0,.     
+00006f50: 2020 2020 2020 2020 2020 2062 6174 6368             batch
+00006f60: 3d73 656c 662e 6261 7463 682c 0a20 2020  =self.batch,.   
+00006f70: 2020 2020 2020 2020 2020 2020 2062 6561               bea
+00006f80: 6d3d 6265 616d 2c0a 2020 2020 2020 2020  m=beam,.        
+00006f90: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
+00006fa0: 666c 6f77 5f63 7478 3d73 656c 662e 636f  flow_ctx=self.co
+00006fb0: 6e74 726f 6c5f 666c 6f77 5f63 7478 2c0a  ntrol_flow_ctx,.
+00006fc0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00006fd0: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
+00006fe0: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00006ff0: 6465 7220 3d20 6479 6e5f 7369 7a65 0a0a  der = dyn_size..
+00007000: 2020 2020 6465 6620 5f67 6574 5f64 796e      def _get_dyn
+00007010: 5f73 697a 655f 6578 745f 666f 725f 6465  _size_ext_for_de
+00007020: 7669 6365 2873 656c 663a 2044 696d 2c20  vice(self: Dim, 
+00007030: 6465 7669 6365 3a20 4f70 7469 6f6e 616c  device: Optional
+00007040: 5b73 7472 5d29 202d 3e20 5f74 2e54 656e  [str]) -> _t.Ten
+00007050: 736f 723a 0a20 2020 2020 2020 2069 6620  sor:.        if 
+00007060: 6e6f 7420 6465 7669 6365 3a0a 2020 2020  not device:.    
+00007070: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007080: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00007090: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+000070a0: 2072 6574 7572 6e6e 2e66 726f 6e74 656e   returnn.fronten
+000070b0: 6420 6173 2072 660a 0a20 2020 2020 2020  d as rf..       
+000070c0: 2073 656c 662e 5f6d 616b 655f 6578 7472   self._make_extr
+000070d0: 6128 290a 2020 2020 2020 2020 6966 2064  a().        if d
+000070e0: 6576 6963 6520 696e 2073 656c 662e 5f65  evice in self._e
+000070f0: 7874 7261 2e63 6163 6865 5f64 796e 5f73  xtra.cache_dyn_s
+00007100: 697a 655f 6578 745f 6465 763a 0a20 2020  ize_ext_dev:.   
+00007110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007120: 7365 6c66 2e5f 6578 7472 612e 6361 6368  self._extra.cach
+00007130: 655f 6479 6e5f 7369 7a65 5f65 7874 5f64  e_dyn_size_ext_d
+00007140: 6576 5b64 6576 6963 655d 0a20 2020 2020  ev[device].     
+00007150: 2020 2073 656c 662e 5f65 7874 7261 2e63     self._extra.c
+00007160: 6163 6865 5f64 796e 5f73 697a 655f 6578  ache_dyn_size_ex
+00007170: 745f 6465 765b 6465 7669 6365 5d20 3d20  t_dev[device] = 
+00007180: 7266 2e63 6f70 795f 746f 5f64 6576 6963  rf.copy_to_devic
+00007190: 6528 7365 6c66 2e64 796e 5f73 697a 655f  e(self.dyn_size_
+000071a0: 6578 742c 2064 6576 6963 653d 6465 7669  ext, device=devi
+000071b0: 6365 290a 2020 2020 2020 2020 7265 7475  ce).        retu
+000071c0: 726e 2073 656c 662e 5f65 7874 7261 2e63  rn self._extra.c
+000071d0: 6163 6865 5f64 796e 5f73 697a 655f 6578  ache_dyn_size_ex
+000071e0: 745f 6465 765b 6465 7669 6365 5d0a 0a20  t_dev[device].. 
+000071f0: 2020 2064 6566 2067 6574 5f6d 6173 6b28     def get_mask(
+00007200: 7365 6c66 3a20 4469 6d2c 202a 2c20 6469  self: Dim, *, di
+00007210: 6d5f 6f72 6465 723a 204f 7074 696f 6e61  m_order: Optiona
+00007220: 6c5b 5365 7175 656e 6365 5b44 696d 5d5d  l[Sequence[Dim]]
+00007230: 203d 204e 6f6e 652c 2064 6576 6963 653a   = None, device:
+00007240: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00007250: 204e 6f6e 6529 202d 3e20 5f74 2e54 656e   None) -> _t.Ten
+00007260: 736f 723a 0a20 2020 2020 2020 2022 2222  sor:.        """
+00007270: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00007280: 6469 6d5f 6f72 6465 723a 2069 6620 6769  dim_order: if gi
+00007290: 7665 6e2c 2074 6865 2064 696d 7320 6f66  ven, the dims of
+000072a0: 2074 6865 206d 6173 6b20 7769 6c6c 2062   the mask will b
+000072b0: 6520 696e 2074 6869 7320 6f72 6465 722e  e in this order.
+000072c0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+000072d0: 7320 6361 6e20 6265 2075 7365 6675 6c20  s can be useful 
+000072e0: 6966 2074 6865 206d 6173 6b20 6973 2062  if the mask is b
+000072f0: 726f 6164 6361 7374 6564 2061 6761 696e  roadcasted again
+00007300: 7374 2073 6f6d 6520 6f74 6865 7220 7465  st some other te
+00007310: 6e73 6f72 2e0a 2020 2020 2020 2020 3a70  nsor..        :p
+00007320: 6172 616d 2073 7472 7c4e 6f6e 6520 6465  aram str|None de
+00007330: 7669 6365 3a20 6966 2067 6976 656e 2c20  vice: if given, 
+00007340: 7769 6c6c 206d 6f76 6520 7468 6520 6d61  will move the ma
+00007350: 736b 2074 6f20 7468 6973 2064 6576 6963  sk to this devic
+00007360: 650a 2020 2020 2020 2020 3a72 6574 7572  e.        :retur
+00007370: 6e3a 2069 6620 6e65 6564 5f6d 6173 6b69  n: if need_maski
+00007380: 6e67 2829 2c20 7468 6520 636f 7272 6573  ng(), the corres
+00007390: 706f 6e64 696e 6720 6d61 736b 2e0a 2020  ponding mask..  
+000073a0: 2020 2020 2020 2020 2020 4966 2074 6869            If thi
+000073b0: 7320 6973 2065 2e67 2e20 7468 6520 7469  s is e.g. the ti
+000073c0: 6d65 2d64 696d 2054 206f 6620 7368 6170  me-dim T of shap
+000073d0: 6520 5b42 5d2c 2074 6865 6e20 7468 6520  e [B], then the 
+000073e0: 6d61 736b 2077 696c 6c20 6265 206f 6620  mask will be of 
+000073f0: 7368 6170 6520 5b42 2c54 5d2e 0a20 2020  shape [B,T]..   
+00007400: 2020 2020 2020 2020 2054 6865 206d 6173           The mas
+00007410: 6b20 636f 756c 6420 6265 2075 7365 6420  k could be used 
+00007420: 7769 7468 203a 6675 6e63 3a60 6d61 736b  with :func:`mask
+00007430: 6564 5f73 656c 6563 7460 2028 6060 626f  ed_select` (``bo
+00007440: 6f6c 6561 6e5f 6d61 736b 6060 2920 6f72  olean_mask``) or
+00007450: 2060 6077 6865 7265 6060 2e0a 2020 2020   ``where``..    
+00007460: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007470: 696d 706f 7274 2072 6574 7572 6e6e 2e66  import returnn.f
+00007480: 726f 6e74 656e 6420 6173 2072 660a 0a20  rontend as rf.. 
+00007490: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+000074a0: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
+000074b0: 616e 6420 7365 6c66 2e64 796e 5f73 697a  and self.dyn_siz
+000074c0: 655f 6578 742e 7261 775f 7465 6e73 6f72  e_ext.raw_tensor
+000074d0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+000074e0: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
+000074f0: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
+00007500: 656d 6265 720a 2020 2020 2020 2020 6261  ember.        ba
+00007510: 636b 656e 6420 3d20 7365 6c66 2e64 796e  ckend = self.dyn
+00007520: 5f73 697a 655f 6578 742e 5f72 6177 5f62  _size_ext._raw_b
+00007530: 6163 6b65 6e64 0a0a 2020 2020 2020 2020  ackend..        
+00007540: 6966 206e 6f74 2064 6576 6963 653a 0a20  if not device:. 
+00007550: 2020 2020 2020 2020 2020 2064 6576 6963             devic
+00007560: 6520 3d20 7266 2e67 6574 5f64 6566 6175  e = rf.get_defau
+00007570: 6c74 5f64 6576 6963 6528 290a 0a20 2020  lt_device()..   
+00007580: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
+00007590: 7472 6120 616e 6420 6465 7669 6365 2069  tra and device i
+000075a0: 6e20 7365 6c66 2e5f 6578 7472 612e 6361  n self._extra.ca
+000075b0: 6368 655f 7365 715f 6d61 736b 3a0a 2020  che_seq_mask:.  
+000075c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000075d0: 2073 656c 662e 5f65 7874 7261 2e63 6163   self._extra.cac
+000075e0: 6865 5f73 6571 5f6d 6173 6b5b 6465 7669  he_seq_mask[devi
+000075f0: 6365 5d0a 0a20 2020 2020 2020 2073 697a  ce]..        siz
+00007600: 655f 6578 7420 3d20 7365 6c66 2e5f 6765  e_ext = self._ge
+00007610: 745f 6479 6e5f 7369 7a65 5f65 7874 5f66  t_dyn_size_ext_f
+00007620: 6f72 5f64 6576 6963 6528 6465 7669 6365  or_device(device
+00007630: 290a 0a20 2020 2020 2020 206d 6178 5f69  )..        max_i
+00007640: 6478 203d 2072 662e 7265 6475 6365 280a  dx = rf.reduce(.
+00007650: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00007660: 5f65 7874 2c0a 2020 2020 2020 2020 2020  _ext,.          
+00007670: 2020 6178 6973 3d73 697a 655f 6578 742e    axis=size_ext.
+00007680: 6469 6d73 2c0a 2020 2020 2020 2020 2020  dims,.          
+00007690: 2020 6d6f 6465 3d22 6d61 7822 2c0a 2020    mode="max",.  
+000076a0: 2020 2020 2020 2020 2020 2320 4d61 736b            # Mask
+000076b0: 696e 6720 6865 7265 2069 7320 6e6f 7420  ing here is not 
+000076c0: 616c 7761 7973 2070 6f73 7369 626c 652c  always possible,
+000076d0: 2065 2e67 2e20 6966 2077 6520 6861 7665   e.g. if we have
+000076e0: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+000076f0: 6167 203d 2044 696d 7b27 7365 6c66 2d61  ag = Dim{'self-a
+00007700: 7474 2d6b 6579 7327 5b27 7469 6d65 3a76  tt-keys'['time:v
+00007710: 6172 3a65 7874 6572 6e5f 6461 7461 3a63  ar:extern_data:c
+00007720: 6c61 7373 6573 275b 425d 5d7d 0a20 2020  lasses'[B]]}.   
+00007730: 2020 2020 2020 2020 2075 7365 5f6d 6173           use_mas
+00007740: 6b3d 4661 6c73 652c 0a20 2020 2020 2020  k=False,.       
+00007750: 2029 0a20 2020 2020 2020 2023 2057 6520   ).        # We 
+00007760: 7573 6520 7468 6520 6173 7375 6d70 7469  use the assumpti
+00007770: 6f6e 2074 6861 7420 7365 6c66 2e70 6c61  on that self.pla
+00007780: 6365 686f 6c64 6572 2e73 6861 7065 5b61  ceholder.shape[a
+00007790: 7869 735d 203d 3d20 6d61 785f 6964 782e  xis] == max_idx.
+000077a0: 0a20 2020 2020 2020 2023 2073 697a 655f  .        # size_
+000077b0: 6578 7420 6d69 6768 7420 6861 7665 2069  ext might have i
+000077c0: 6e76 616c 6964 2028 7a65 726f 2920 7369  nvalid (zero) si
+000077d0: 7a65 730a 2020 2020 2020 2020 2320 7768  zes.        # wh
+000077e0: 656e 2069 7420 6974 7365 6c66 2068 6173  en it itself has
+000077f0: 2073 6f6d 6520 7061 6464 696e 672c 2065   some padding, e
+00007800: 2e67 2e20 7768 656e 2069 7473 206f 776e  .g. when its own
+00007810: 2073 6861 7065 2069 7320 6479 6e61 6d69   shape is dynami
+00007820: 632e 0a20 2020 2020 2020 2023 2041 207a  c..        # A z
+00007830: 6572 6f20 7369 7a65 2063 616e 206c 6561  ero size can lea
+00007840: 6420 746f 2070 726f 626c 656d 7320 696e  d to problems in
+00007850: 2073 6f6d 6520 6361 7365 732c 2065 2e67   some cases, e.g
+00007860: 2e20 696e 2053 6f66 746d 6178 4f76 6572  . in SoftmaxOver
+00007870: 5370 6174 6961 6c4c 6179 6572 2c0a 2020  SpatialLayer,.  
+00007880: 2020 2020 2020 2320 7768 656e 2065 7665        # when eve
+00007890: 7279 7468 696e 6720 6973 206d 6173 6b65  rything is maske
+000078a0: 6420 746f 202d 696e 662c 2069 7420 7265  d to -inf, it re
+000078b0: 7375 6c74 7320 696e 206e 616e 2c0a 2020  sults in nan,.  
+000078c0: 2020 2020 2020 2320 616e 6420 7468 6973        # and this
+000078d0: 206c 696b 656c 7920 7072 6f64 7563 6573   likely produces
+000078e0: 206e 616e 2069 6e20 6261 636b 7072 6f70   nan in backprop
+000078f0: 206f 7220 656c 7365 7768 6572 652e 0a20   or elsewhere.. 
+00007900: 2020 2020 2020 2023 2054 6875 732c 206d         # Thus, m
+00007910: 6173 6b20 7369 7a65 5f65 7874 2069 7473  ask size_ext its
+00007920: 656c 662c 2061 6e64 2073 6574 2074 6865  elf, and set the
+00007930: 2070 6164 6465 6420 7661 6c75 6573 2074   padded values t
+00007940: 6f20 312e 0a20 2020 2020 2020 2023 2054  o 1..        # T
+00007950: 6869 7320 6173 7375 6d65 7320 7468 6174  his assumes that
+00007960: 206d 6178 5f69 6478 203e 3d20 312e 0a20   max_idx >= 1.. 
+00007970: 2020 2020 2020 2073 697a 655f 6578 7420         size_ext 
+00007980: 3d20 7369 7a65 5f65 7874 2e63 6f70 795f  = size_ext.copy_
+00007990: 6d61 736b 6564 286d 6178 5f69 6478 290a  masked(max_idx).
+000079a0: 2020 2020 2020 2020 7769 7468 2072 662e          with rf.
+000079b0: 7365 745f 6465 6661 756c 745f 6465 7669  set_default_devi
+000079c0: 6365 5f63 7478 2864 6576 6963 6529 3a0a  ce_ctx(device):.
+000079d0: 2020 2020 2020 2020 2020 2020 6964 785f              idx_
+000079e0: 7261 6e67 6520 3d20 6261 636b 656e 642e  range = backend.
+000079f0: 7261 6e67 655f 6f76 6572 5f64 696d 2873  range_over_dim(s
+00007a00: 656c 6629 0a20 2020 2020 2020 2073 6571  elf).        seq
+00007a10: 5f6d 6173 6b20 3d20 7266 2e63 6f6d 7061  _mask = rf.compa
+00007a20: 7265 2869 6478 5f72 616e 6765 2c20 223c  re(idx_range, "<
+00007a30: 222c 2073 697a 655f 6578 742c 2061 6c6c  ", size_ext, all
+00007a40: 6f77 5f62 726f 6164 6361 7374 5f61 6c6c  ow_broadcast_all
+00007a50: 5f73 6f75 7263 6573 3d54 7275 652c 2064  _sources=True, d
+00007a60: 696d 5f6f 7264 6572 3d64 696d 5f6f 7264  im_order=dim_ord
+00007a70: 6572 290a 2020 2020 2020 2020 7365 6c66  er).        self
+00007a80: 2e5f 6d61 6b65 5f65 7874 7261 2829 2e63  ._make_extra().c
+00007a90: 6163 6865 5f73 6571 5f6d 6173 6b5b 6465  ache_seq_mask[de
+00007aa0: 7669 6365 5d20 3d20 7365 715f 6d61 736b  vice] = seq_mask
+00007ab0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007ac0: 7365 715f 6d61 736b 0a0a 2020 2020 6465  seq_mask..    de
+00007ad0: 6620 6973 5f62 6174 6368 5f64 696d 2873  f is_batch_dim(s
+00007ae0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00007af0: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
+00007b00: 6e3a 2077 6865 7468 6572 2074 6869 7320  n: whether this 
+00007b10: 6469 6d20 7461 6720 6973 206f 6620 6b69  dim tag is of ki
+00007b20: 6e64 2062 6174 6368 0a20 2020 2020 2020  nd batch.       
+00007b30: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+00007b40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007b50: 2020 7265 7475 726e 2073 656c 662e 6b69    return self.ki
+00007b60: 6e64 203d 3d20 4469 6d54 7970 6573 2e42  nd == DimTypes.B
+00007b70: 6174 6368 0a0a 2020 2020 6465 6620 6973  atch..    def is
+00007b80: 5f66 6561 7475 7265 5f64 696d 2873 656c  _feature_dim(sel
+00007b90: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00007ba0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00007bb0: 2077 6865 7468 6572 2074 6869 7320 6469   whether this di
+00007bc0: 6d20 7461 6720 6973 206f 6620 6b69 6e64  m tag is of kind
+00007bd0: 2066 6561 7475 7265 0a20 2020 2020 2020   feature.       
+00007be0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+00007bf0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007c00: 2020 7265 7475 726e 2073 656c 662e 6b69    return self.ki
+00007c10: 6e64 203d 3d20 4469 6d54 7970 6573 2e46  nd == DimTypes.F
+00007c20: 6561 7475 7265 0a0a 2020 2020 6465 6620  eature..    def 
+00007c30: 6973 5f73 7061 7469 616c 5f64 696d 2873  is_spatial_dim(s
+00007c40: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00007c50: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
+00007c60: 6e3a 2077 6865 7468 6572 2074 6869 7320  n: whether this 
+00007c70: 6469 6d20 7461 6720 6973 206f 6620 6b69  dim tag is of ki
+00007c80: 6e64 2073 7061 7469 616c 0a20 2020 2020  nd spatial.     
+00007c90: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+00007ca0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007cb0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00007cc0: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
+00007cd0: 2e53 7061 7469 616c 0a0a 2020 2020 6465  .Spatial..    de
+00007ce0: 6620 6973 5f64 696d 5f6b 6e6f 776e 2873  f is_dim_known(s
+00007cf0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00007d00: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
+00007d10: 6e3a 2077 6865 7468 6572 2077 6520 6b6e  n: whether we kn
+00007d20: 6f77 2074 6865 2064 696d 656e 7369 6f6e  ow the dimension
+00007d30: 3b20 6261 7369 6361 6c6c 7920 7768 6574  ; basically whet
+00007d40: 6865 7220 7468 6973 2069 7320 6465 6669  her this is defi
+00007d50: 6e65 640a 2020 2020 2020 2020 2020 2861  ned.          (a
+00007d60: 6c74 686f 7567 6820 606e 6f74 2073 656c  lthough `not sel
+00007d70: 662e 756e 6465 6669 6e65 6460 2069 7320  f.undefined` is 
+00007d80: 6465 6669 6e65 6420 736c 6967 6874 6c79  defined slightly
+00007d90: 2064 6966 6665 7265 6e74 6c79 290a 2020   differently).  
+00007da0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+00007db0: 6f6c 0a20 2020 2020 2020 2022 2222 0a20  ol.        """. 
+00007dc0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00007dd0: 735f 6261 7463 685f 6469 6d28 293a 0a20  s_batch_dim():. 
+00007de0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007df0: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
+00007e00: 6620 6e6f 7420 7365 6c66 2e69 735f 6479  f not self.is_dy
+00007e10: 6e61 6d69 6328 2920 616e 6420 7365 6c66  namic() and self
+00007e20: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+00007e30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00007e40: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00007e50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007e60: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+00007e70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007e80: 2054 7275 650a 2020 2020 2020 2020 6578   True.        ex
+00007e90: 7472 6120 3d20 7365 6c66 2e5f 6765 745f  tra = self._get_
+00007ea0: 7361 6d65 5f62 6173 655f 6578 7472 6128  same_base_extra(
+00007eb0: 290a 2020 2020 2020 2020 6966 2065 7874  ).        if ext
+00007ec0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+00007ed0: 666f 7220 5f2c 206f 7468 6572 2069 6e20  for _, other in 
+00007ee0: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
+00007ef0: 6174 6368 5f63 7478 2e69 7465 6d73 2829  atch_ctx.items()
+00007f00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007f10: 2020 6966 206f 7468 6572 2e64 796e 5f73    if other.dyn_s
+00007f20: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
+00007f30: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007f40: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00007f50: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+00007f60: 2020 2064 6566 2069 735f 6479 6e61 6d69     def is_dynami
+00007f70: 6328 7365 6c66 2920 2d3e 2062 6f6f 6c3a  c(self) -> bool:
+00007f80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007f90: 2020 2020 203a 7265 7475 726e 3a20 7768       :return: wh
+00007fa0: 6574 6865 7220 7468 6520 6469 6d20 6973  ether the dim is
+00007fb0: 206e 6f74 2073 7461 7469 632e 2075 7375   not static. usu
+00007fc0: 616c 6c79 206d 6561 6e73 2074 6861 7420  ally means that 
+00007fd0: 6974 2068 6173 2073 6571 206c 656e 6774  it has seq lengt
+00007fe0: 6873 0a20 2020 2020 2020 2022 2222 0a20  hs.        """. 
+00007ff0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00008000: 6c66 2e64 696d 656e 7369 6f6e 2069 7320  lf.dimension is 
+00008010: 4e6f 6e65 2061 6e64 206e 6f74 2073 656c  None and not sel
+00008020: 662e 6973 5f62 6174 6368 5f64 696d 2829  f.is_batch_dim()
+00008030: 0a0a 2020 2020 6465 6620 6973 5f73 7461  ..    def is_sta
+00008040: 7469 6328 7365 6c66 2920 2d3e 2062 6f6f  tic(self) -> boo
+00008050: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00008060: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00008070: 7374 6174 6963 0a20 2020 2020 2020 2022  static.        "
+00008080: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00008090: 6e20 6e6f 7420 7365 6c66 2e69 735f 6479  n not self.is_dy
+000080a0: 6e61 6d69 6328 290a 0a20 2020 2064 6566  namic()..    def
+000080b0: 206e 6565 645f 6d61 736b 696e 6728 7365   need_masking(se
+000080c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000080d0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000080e0: 3a20 7768 6574 6865 7220 6469 6d20 6973  : whether dim is
+000080f0: 2073 7461 7469 6320 6f72 2064 796e 616d   static or dynam
+00008100: 6963 2062 7574 2077 6974 6820 7363 616c  ic but with scal
+00008110: 6172 2064 796e 5f73 697a 655f 6578 740a  ar dyn_size_ext.
+00008120: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008130: 2020 2020 6966 2073 656c 662e 6973 5f73      if self.is_s
+00008140: 7461 7469 6328 293a 0a20 2020 2020 2020  tatic():.       
+00008150: 2020 2020 2069 6620 7365 6c66 2e63 6170       if self.cap
+00008160: 6163 6974 7920 6973 206e 6f74 204e 6f6e  acity is not Non
+00008170: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008180: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+00008190: 697a 6520 3c20 7365 6c66 2e63 6170 6163  ize < self.capac
+000081a0: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
+000081b0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+000081c0: 2020 2020 2069 6620 7365 6c66 2e63 6170       if self.cap
+000081d0: 6163 6974 7920 6973 206e 6f74 204e 6f6e  acity is not Non
+000081e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000081f0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00008200: 2020 2069 6620 6e6f 7420 7365 6c66 2e64     if not self.d
+00008210: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00008220: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008230: 5472 7565 2020 2320 756e 6b6e 6f77 6e0a  True  # unknown.
+00008240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008250: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00008260: 2e62 6174 6368 5f6e 6469 6d20 3e20 300a  .batch_ndim > 0.
+00008270: 0a20 2020 2064 6566 2063 616e 5f62 655f  .    def can_be_
+00008280: 7573 6564 5f61 735f 6469 6d28 7365 6c66  used_as_dim(self
+00008290: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000082a0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000082b0: 7768 6574 6865 7220 7468 6973 2063 616e  whether this can
+000082c0: 2062 6520 7573 6564 2061 7320 6120 6469   be used as a di
+000082d0: 6d20 696e 203a 636c 6173 733a 6044 6174  m in :class:`Dat
+000082e0: 6160 2c20 692e 652e 2069 7420 6973 206e  a`, i.e. it is n
+000082f0: 6f74 2073 7065 6369 616c 0a20 2020 2020  ot special.     
+00008300: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+00008310: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008320: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+00008330: 656c 662e 7370 6563 6961 6c0a 0a20 2020  elf.special..   
+00008340: 2064 6566 2069 735f 7361 6d65 5f73 697a   def is_same_siz
+00008350: 655f 7465 6e73 6f72 2873 656c 662c 2078  e_tensor(self, x
+00008360: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00008370: 2020 2020 2020 203a 7061 7261 6d20 7466         :param tf
+00008380: 2e54 656e 736f 7220 783a 0a20 2020 2020  .Tensor x:.     
+00008390: 2020 203a 7265 7475 726e 3a20 7768 6574     :return: whet
+000083a0: 6865 7220 7468 6973 2064 696d 2074 6167  her this dim tag
+000083b0: 2066 6f72 2074 6869 7320 7370 6563 6966   for this specif
+000083c0: 6963 2062 6174 6368 2028 696e 636c 2062  ic batch (incl b
+000083d0: 6561 6d29 2069 7320 7468 6520 7361 6d65  eam) is the same
+000083e0: 2061 7320 7468 6520 6769 7665 6e20 7369   as the given si
+000083f0: 7a65 0a20 2020 2020 2020 203a 7274 7970  ze.        :rtyp
+00008400: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00008410: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00008420: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00008430: 2061 6e64 2078 2069 7320 7365 6c66 2e64   and x is self.d
+00008440: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
+00008450: 6568 6f6c 6465 723a 0a20 2020 2020 2020  eholder:.       
+00008460: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00008470: 0a20 2020 2020 2020 2074 6167 203d 205f  .        tag = _
+00008480: 4469 6d4d 6978 696e 2e67 6574 5f74 6167  DimMixin.get_tag
+00008490: 5f66 726f 6d5f 7369 7a65 5f74 656e 736f  _from_size_tenso
+000084a0: 7228 7829 0a20 2020 2020 2020 2069 6620  r(x).        if 
+000084b0: 7461 6720 616e 6420 7461 6720 3d3d 2073  tag and tag == s
+000084c0: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
+000084d0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+000084e0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+000084f0: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+00008500: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00008510: 650a 2020 2020 2020 2020 6966 2075 7469  e.        if uti
+00008520: 6c2e 5265 6649 6445 7128 7829 2069 6e20  l.RefIdEq(x) in 
+00008530: 7365 6c66 2e5f 6578 7472 612e 6479 6e5f  self._extra.dyn_
+00008540: 7369 7a65 5f73 616d 653a 0a20 2020 2020  size_same:.     
+00008550: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00008560: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00008570: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00008580: 2073 6574 5f74 6167 5f6f 6e5f 7369 7a65   set_tag_on_size
+00008590: 5f74 656e 736f 7228 7365 6c66 3a20 4469  _tensor(self: Di
+000085a0: 6d2c 2078 2c20 6261 7463 683d 4e6f 6e65  m, x, batch=None
+000085b0: 2c20 7361 6d65 5f61 735f 6265 666f 7265  , same_as_before
+000085c0: 3d46 616c 7365 2920 2d3e 2044 696d 3a0a  =False) -> Dim:.
+000085d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000085e0: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+000085f0: 6e20 6973 2075 7365 640a 2020 2020 2020  n is used.      
+00008600: 2020 746f 2063 6f75 706c 6520 6120 7466    to couple a tf
+00008610: 2e54 656e 736f 7220 696e 7374 616e 6365  .Tensor instance
+00008620: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+00008630: 6520 6479 6e20 7369 7a65 0a20 2020 2020  e dyn size.     
+00008640: 2020 2077 6974 6820 7468 6520 6469 6d20     with the dim 
+00008650: 7461 672e 0a0a 2020 2020 2020 2020 5468  tag...        Th
+00008660: 6973 2069 7320 7573 7561 6c6c 7920 6120  is is usually a 
+00008670: 6e65 776c 7920 6372 6561 7465 6420 6469  newly created di
+00008680: 6d20 7461 672c 0a20 2020 2020 2020 2077  m tag,.        w
+00008690: 6869 6368 2069 7320 7965 7420 756e 7365  hich is yet unse
+000086a0: 742e 0a0a 2020 2020 2020 2020 4974 2069  t...        It i
+000086b0: 7320 616c 736f 2075 7365 6420 746f 2063  s also used to c
+000086c0: 6f75 706c 6520 616e 2065 7869 7374 696e  ouple an existin
+000086d0: 6720 6469 6d20 7461 6720 7769 7468 206f  g dim tag with o
+000086e0: 7468 6572 2064 796e 2073 697a 6573 0a20  ther dyn sizes. 
+000086f0: 2020 2020 2020 2077 6869 6368 206a 7573         which jus
+00008700: 7420 6469 6666 6572 2062 7920 616e 2065  t differ by an e
+00008710: 7870 616e 7369 6f6e 206f 6620 7468 6520  xpansion of the 
+00008720: 6261 7463 6820 2865 2e67 2e20 7365 6172  batch (e.g. sear
+00008730: 6368 2062 6561 6d29 2e0a 0a20 2020 2020  ch beam)...     
+00008740: 2020 2053 6565 2061 6c73 6f20 3a66 756e     See also :fun
+00008750: 633a 6067 6574 5f74 6167 5f66 726f 6d5f  c:`get_tag_from_
+00008760: 7369 7a65 5f74 656e 736f 7260 2e0a 2020  size_tensor`..  
+00008770: 2020 2020 2020 416c 736f 2073 6565 203a        Also see :
+00008780: 6675 6e63 3a60 7365 745f 6479 6e5f 7369  func:`set_dyn_si
+00008790: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
+000087a0: 5f63 7478 602e 0a0a 2020 2020 2020 2020  _ctx`...        
+000087b0: 3a70 6172 616d 2078 3a20 7261 7720 7465  :param x: raw te
+000087c0: 6e73 6f72 2c20 666f 7220 6578 616d 706c  nsor, for exampl
+000087d0: 6520 7466 2e54 656e 736f 720a 2020 2020  e tf.Tensor.    
+000087e0: 2020 2020 3a70 6172 616d 2042 6174 6368      :param Batch
+000087f0: 496e 666f 7c4e 6f6e 6520 6261 7463 683a  Info|None batch:
+00008800: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00008810: 626f 6f6c 2073 616d 655f 6173 5f62 6566  bool same_as_bef
+00008820: 6f72 653a 2069 6d70 6c69 6573 2069 7420  ore: implies it 
+00008830: 7761 7320 7365 7420 6265 666f 7265 2c20  was set before, 
+00008840: 616e 6420 7468 6520 6e65 7720 7369 7a65  and the new size
+00008850: 2069 7320 7468 6520 7361 6d65 2e0a 2020   is the same..  
+00008860: 2020 2020 2020 2020 652e 672e 2069 7420          e.g. it 
+00008870: 636f 756c 6420 6265 2073 6f6d 6520 6964  could be some id
+00008880: 656e 7469 7479 2077 6974 6820 6164 6465  entity with adde
+00008890: 6420 6368 6563 6b73 2c20 6f72 206f 7468  d checks, or oth
+000088a0: 6572 2063 6861 6e67 652e 0a20 2020 2020  er change..     
+000088b0: 2020 203a 7265 7475 726e 3a20 7365 6c66     :return: self
+000088c0: 206f 7220 6e65 7720 6469 6d20 7461 670a   or new dim tag.
+000088d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000088e0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+000088f0: 6361 6e5f 6265 5f75 7365 645f 6173 5f64  can_be_used_as_d
+00008900: 696d 2829 0a20 2020 2020 2020 2023 2049  im().        # I
+00008910: 7427 7320 756e 7573 7561 6c20 6966 2073  t's unusual if s
+00008920: 656c 662e 6469 6d65 6e73 696f 6e20 6973  elf.dimension is
+00008930: 206e 6f74 204e 6f6e 652c 2062 7574 206c   not None, but l
+00008940: 6574 2773 2061 6363 6570 7420 7468 6174  et's accept that
+00008950: 2e0a 2020 2020 2020 2020 6966 2068 6173  ..        if has
+00008960: 6174 7472 2878 2c20 225f 6973 5f73 697a  attr(x, "_is_siz
+00008970: 655f 6f66 5f64 696d 5f74 6167 2229 3a0a  e_of_dim_tag"):.
+00008980: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+00008990: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
+000089a0: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
+000089b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000089c0: 782e 5f69 735f 7369 7a65 5f6f 665f 6469  x._is_size_of_di
+000089d0: 6d5f 7461 6720 696e 2028 4e6f 6e65 2c20  m_tag in (None, 
+000089e0: 7365 6c66 290a 2020 2020 2020 2020 2320  self).        # 
+000089f0: 4966 2077 6520 616c 7265 6164 7920 6861  If we already ha
+00008a00: 7665 2061 6e6f 7468 6572 2064 796e 2073  ve another dyn s
+00008a10: 697a 6520 7365 7420 6f72 2064 6966 6665  ize set or diffe
+00008a20: 7265 6e74 2062 6174 6368 2c20 6372 6561  rent batch, crea
+00008a30: 7465 2061 206e 6577 2044 696d 2069 6e73  te a new Dim ins
+00008a40: 7461 6e63 652e 0a20 2020 2020 2020 2069  tance..        i
+00008a50: 6620 7365 6c66 2e62 6174 6368 2061 6e64  f self.batch and
+00008a60: 2062 6174 6368 2061 6e64 2073 656c 662e   batch and self.
+00008a70: 6261 7463 6820 213d 2062 6174 6368 3a0a  batch != batch:.
+00008a80: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00008a90: 7274 206e 6f74 2073 616d 655f 6173 5f62  rt not same_as_b
+00008aa0: 6566 6f72 6520 2023 2069 7420 6361 6e6e  efore  # it cann
+00008ab0: 6f74 2062 6520 7468 6520 7361 6d65 2077  ot be the same w
+00008ac0: 6865 6e20 6974 2069 7320 616e 6f74 6865  hen it is anothe
+00008ad0: 7220 6261 7463 682e 2e2e 0a20 2020 2020  r batch....     
+00008ae0: 2020 2020 2020 206e 6577 5f64 696d 5f74         new_dim_t
+00008af0: 6167 203d 2073 656c 662e 6765 745f 666f  ag = self.get_fo
+00008b00: 725f 6261 7463 685f 6374 7828 6261 7463  r_batch_ctx(batc
+00008b10: 683d 6261 7463 682c 2063 7478 3d73 656c  h=batch, ctx=sel
+00008b20: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+00008b30: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
+00008b40: 6e65 775f 6469 6d5f 7461 672e 7365 745f  new_dim_tag.set_
+00008b50: 7461 675f 6f6e 5f73 697a 655f 7465 6e73  tag_on_size_tens
+00008b60: 6f72 2878 2c20 6261 7463 683d 6261 7463  or(x, batch=batc
+00008b70: 6829 0a20 2020 2020 2020 2020 2020 2072  h).            r
+00008b80: 6574 7572 6e20 6e65 775f 6469 6d5f 7461  eturn new_dim_ta
+00008b90: 670a 2020 2020 2020 2020 6966 2073 656c  g.        if sel
+00008ba0: 662e 6479 6e5f 7369 7a65 2069 7320 6e6f  f.dyn_size is no
+00008bb0: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
+00008bc0: 6479 6e5f 7369 7a65 2069 7320 6e6f 7420  dyn_size is not 
+00008bd0: 783a 0a20 2020 2020 2020 2020 2020 2069  x:.            i
+00008be0: 6620 7365 6c66 2e5f 6578 7472 6120 616e  f self._extra an
+00008bf0: 6420 7574 696c 2e52 6566 4964 4571 2878  d util.RefIdEq(x
+00008c00: 2920 696e 2073 656c 662e 5f65 7874 7261  ) in self._extra
+00008c10: 2e64 796e 5f73 697a 655f 7361 6d65 3a0a  .dyn_size_same:.
+00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c30: 7061 7373 2020 2320 6f6b 2c20 7061 7373  pass  # ok, pass
+00008c40: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+00008c50: 656c 6966 2073 616d 655f 6173 5f62 6566  elif same_as_bef
+00008c60: 6f72 653a 0a20 2020 2020 2020 2020 2020  ore:.           
+00008c70: 2020 2020 2073 656c 662e 5f6d 616b 655f       self._make_
+00008c80: 6578 7472 6128 292e 6479 6e5f 7369 7a65  extra().dyn_size
+00008c90: 5f73 616d 652e 6164 6428 7574 696c 2e52  _same.add(util.R
+00008ca0: 6566 4964 4571 2878 2929 0a20 2020 2020  efIdEq(x)).     
+00008cb0: 2020 2020 2020 2020 2020 2023 2041 6e64             # And
+00008cc0: 206e 6f77 2070 6173 7320 6f6e 2e0a 2020   now pass on..  
+00008cd0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cf0: 6173 7365 7274 2073 656c 662e 6261 7463  assert self.batc
+00008d00: 6820 616e 6420 6261 7463 680a 2020 2020  h and batch.    
+00008d10: 2020 2020 2020 2020 2020 2020 2320 4974              # It
+00008d20: 2773 206e 6f74 2063 6c65 6172 2077 6861  's not clear wha
+00008d30: 7420 746f 2064 6f2e 2057 6520 636f 756c  t to do. We coul
+00008d40: 6420 6372 6561 7465 2061 206e 6577 2064  d create a new d
+00008d50: 696d 2074 6167 2c20 6275 7420 7468 6520  im tag, but the 
+00008d60: 7369 7a65 7320 6d69 6768 7420 6265 2064  sizes might be d
+00008d70: 6966 6665 7265 6e74 2e0a 2020 2020 2020  ifferent..      
+00008d80: 2020 2020 2020 2020 2020 2320 5573 7561            # Usua
+00008d90: 6c6c 7920 7765 2073 686f 756c 6420 6e6f  lly we should no
+00008da0: 7420 6765 7420 6865 7265 2e0a 2020 2020  t get here..    
+00008db0: 2020 2020 2020 2020 2020 2020 2320 536f              # So
+00008dc0: 2066 6f72 206e 6f77 2c20 6a75 7374 2065   for now, just e
+00008dd0: 7272 6f72 2e0a 2020 2020 2020 2020 2020  rror..          
+00008de0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+00008df0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+00008e00: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
+00008e10: 2020 2020 2020 2066 726f 6d20 7265 7475         from retu
+00008e20: 726e 6e2e 6672 6f6e 7465 6e64 2e5f 6261  rnn.frontend._ba
+00008e30: 636b 656e 6420 696d 706f 7274 2067 6574  ckend import get
+00008e40: 5f62 6163 6b65 6e64 5f62 795f 7261 775f  _backend_by_raw_
+00008e50: 7465 6e73 6f72 5f74 7970 650a 0a20 2020  tensor_type..   
+00008e60: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00008e70: 7365 2045 7863 6570 7469 6f6e 280a 2020  se Exception(.  
+00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e90: 2020 225c 6e22 2e6a 6f69 6e28 0a20 2020    "\n".join(.   
+00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008eb0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
 00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ed0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+00008ed0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
 00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ef0: 2020 2020 2020 2020 2020 2022 2572 2028             "%r (
-00008f00: 2572 2920 616c 7265 6164 7920 6861 7320  %r) already has 
-00008f10: 7369 7a65 2025 722c 220a 2020 2020 2020  size %r,".      
+00008ef0: 2020 2020 2022 2572 2028 2572 2920 616c       "%r (%r) al
+00008f00: 7265 6164 7920 6861 7320 7369 7a65 2025  ready has size %
+00008f10: 722c 220a 2020 2020 2020 2020 2020 2020  r,".            
 00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f30: 2020 2020 2020 2020 2020 2220 616e 6420            " and 
-00008f40: 616e 6f74 6865 7220 696e 636f 6d70 6174  another incompat
-00008f50: 6962 6c65 2073 697a 6520 2572 2028 6261  ible size %r (ba
-00008f60: 7463 6820 2572 2920 6973 2062 6569 6e67  tch %r) is being
-00008f70: 2061 7373 6967 6e65 642e 220a 2020 2020   assigned.".    
+00008f30: 2020 2020 2220 616e 6420 616e 6f74 6865      " and anothe
+00008f40: 7220 696e 636f 6d70 6174 6962 6c65 2073  r incompatible s
+00008f50: 697a 6520 2572 2028 6261 7463 6820 2572  ize %r (batch %r
+00008f60: 2920 6973 2062 6569 6e67 2061 7373 6967  ) is being assig
+00008f70: 6e65 642e 220a 2020 2020 2020 2020 2020  ned.".          
 00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00008f90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
 00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fb0: 2020 2020 2020 2520 2873 656c 662c 2073        % (self, s
-00008fc0: 656c 662e 6465 7363 7269 7074 696f 6e2c  elf.description,
-00008fd0: 2073 656c 662e 6479 6e5f 7369 7a65 2c20   self.dyn_size, 
-00008fe0: 782c 2062 6174 6368 292c 0a20 2020 2020  x, batch),.     
+00008fb0: 2520 2873 656c 662c 2073 656c 662e 6465  % (self, self.de
+00008fc0: 7363 7269 7074 696f 6e2c 2073 656c 662e  scription, self.
+00008fd0: 6479 6e5f 7369 7a65 2c20 782c 2062 6174  dyn_size, x, bat
+00008fe0: 6368 292c 0a20 2020 2020 2020 2020 2020  ch),.           
 00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009000: 2020 2020 2020 2022 5c6e 4e65 7720 7369         "\nNew si
-00009010: 7a65 2063 6f6d 7075 7461 7469 6f6e 2067  ze computation g
-00009020: 7261 7068 3a22 2c0a 2020 2020 2020 2020  raph:",.        
-00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 2020 2020 6765 745f 6261 636b 656e 645f      get_backend_
-00009050: 6279 5f72 6177 5f74 656e 736f 725f 7479  by_raw_tensor_ty
-00009060: 7065 2874 7970 6528 7829 292e 666f 726d  pe(type(x)).form
-00009070: 6174 5f67 7261 7068 5f6f 7574 7075 7428  at_graph_output(
-00009080: 782c 206d 6178 5f64 6570 7468 3d33 292c  x, max_depth=3),
-00009090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000090a0: 2020 2020 2020 2020 2020 2020 2022 5c6e               "\n
-000090b0: 5468 6973 2069 7320 6d61 7962 6520 7468  This is maybe th
-000090c0: 6520 7265 7375 6c74 206f 6620 616e 2069  e result of an i
-000090d0: 6e63 6f72 7265 6374 2064 6563 6c61 7265  ncorrect declare
-000090e0: 5f73 616d 655f 6173 2e20 222c 0a20 2020  _same_as. ",.   
+00009000: 2022 5c6e 4e65 7720 7369 7a65 2063 6f6d   "\nNew size com
+00009010: 7075 7461 7469 6f6e 2067 7261 7068 3a22  putation graph:"
+00009020: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009030: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00009040: 745f 6261 636b 656e 645f 6279 5f72 6177  t_backend_by_raw
+00009050: 5f74 656e 736f 725f 7479 7065 2874 7970  _tensor_type(typ
+00009060: 6528 7829 292e 666f 726d 6174 5f67 7261  e(x)).format_gra
+00009070: 7068 5f6f 7574 7075 7428 782c 206d 6178  ph_output(x, max
+00009080: 5f64 6570 7468 3d33 292c 0a20 2020 2020  _depth=3),.     
+00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090a0: 2020 2020 2020 2022 5c6e 5468 6973 2069         "\nThis i
+000090b0: 7320 6d61 7962 6520 7468 6520 7265 7375  s maybe the resu
+000090c0: 6c74 206f 6620 616e 2069 6e63 6f72 7265  lt of an incorre
+000090d0: 6374 2064 6563 6c61 7265 5f73 616d 655f  ct declare_same_
+000090e0: 6173 2e20 222c 0a20 2020 2020 2020 2020  as. ",.         
 000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009100: 2020 2020 2020 2020 2022 7361 6d65 5f61           "same_a
-00009110: 7320 3d20 2573 2220 2520 7365 6c66 2e73  s = %s" % self.s
-00009120: 616d 655f 6173 2c0a 2020 2020 2020 2020  ame_as,.        
-00009130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009140: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00009150: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009160: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009170: 2020 6966 2062 6174 6368 2061 6e64 2067    if batch and g
-00009180: 6574 6174 7472 2878 2c20 225f 5245 5455  etattr(x, "_RETU
-00009190: 524e 4e5f 6479 6e5f 7369 7a65 5f62 6561  RNN_dyn_size_bea
-000091a0: 6d22 2c20 4e6f 6e65 293a 0a20 2020 2020  m", None):.     
-000091b0: 2020 2020 2020 2061 7373 6572 7420 6261         assert ba
-000091c0: 7463 682e 6265 616d 203d 3d20 6765 7461  tch.beam == geta
-000091d0: 7474 7228 0a20 2020 2020 2020 2020 2020  ttr(.           
-000091e0: 2020 2020 2078 2c20 225f 5245 5455 524e       x, "_RETURN
-000091f0: 4e5f 6479 6e5f 7369 7a65 5f62 6561 6d22  N_dyn_size_beam"
-00009200: 0a20 2020 2020 2020 2020 2020 2029 2c20  .            ), 
-00009210: 2225 733a 2064 796e 2073 697a 6520 2573  "%s: dyn size %s
-00009220: 2068 6173 2075 6e65 7870 6563 7465 6420   has unexpected 
-00009230: 6261 7463 6820 2573 2c20 6578 7065 6374  batch %s, expect
-00009240: 6564 2025 7322 2025 2028 0a20 2020 2020  ed %s" % (.     
-00009250: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00009260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009270: 2078 2c0a 2020 2020 2020 2020 2020 2020   x,.            
-00009280: 2020 2020 6261 7463 682c 0a20 2020 2020      batch,.     
-00009290: 2020 2020 2020 2020 2020 2067 6574 6174             getat
-000092a0: 7472 2878 2c20 225f 5245 5455 524e 4e5f  tr(x, "_RETURNN_
-000092b0: 6479 6e5f 7369 7a65 5f62 6561 6d22 292c  dyn_size_beam"),
-000092c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000092d0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000092e0: 6174 6368 2061 6e64 2062 6174 6368 3a0a  atch and batch:.
-000092f0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00009300: 7274 2073 656c 662e 6261 7463 6820 3d3d  rt self.batch ==
-00009310: 2062 6174 6368 0a20 2020 2020 2020 2065   batch.        e
-00009320: 6c69 6620 6261 7463 6820 616e 6420 6e6f  lif batch and no
-00009330: 7420 7365 6c66 2e62 6174 6368 3a0a 2020  t self.batch:.  
-00009340: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00009350: 6174 6368 203d 2062 6174 6368 2020 2320  atch = batch  # 
-00009360: 6f76 6572 7461 6b65 0a20 2020 2020 2020  overtake.       
-00009370: 2069 6620 6e6f 7420 7365 6c66 2e69 735f   if not self.is_
-00009380: 6261 7463 685f 6469 6d28 2920 616e 6420  batch_dim() and 
-00009390: 7365 6c66 2e69 735f 6479 6e61 6d69 6328  self.is_dynamic(
-000093a0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-000093b0: 6620 7361 6d65 5f61 735f 6265 666f 7265  f same_as_before
-000093c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000093d0: 2020 6173 7365 7274 2073 656c 662e 6479    assert self.dy
-000093e0: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
-000093f0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00009400: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
-00009410: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-00009420: 2020 2020 2020 2020 2023 2044 6f20 6e6f           # Do no
-00009430: 7420 6f76 6572 7772 6974 6520 6974 2e0a  t overwrite it..
-00009440: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00009450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009460: 2020 7365 6c66 2e5f 696e 6974 5f64 6566    self._init_def
-00009470: 6175 6c74 5f64 796e 5f73 697a 655f 6578  ault_dyn_size_ex
-00009480: 7428 7829 0a20 2020 2020 2020 2069 6620  t(x).        if 
-00009490: 6765 7461 7474 7228 782c 2022 5f69 735f  getattr(x, "_is_
-000094a0: 7369 7a65 5f6f 665f 6469 6d5f 7461 6722  size_of_dim_tag"
-000094b0: 2c20 4e6f 6e65 2920 6973 204e 6f6e 653a  , None) is None:
-000094c0: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
-000094d0: 6174 7472 2878 2c20 225f 6973 5f73 697a  attr(x, "_is_siz
-000094e0: 655f 6f66 5f64 696d 5f74 6167 222c 2073  e_of_dim_tag", s
-000094f0: 656c 6629 0a20 2020 2020 2020 2072 6574  elf).        ret
-00009500: 7572 6e20 7365 6c66 0a0a 2020 2020 4063  urn self..    @c
-00009510: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00009520: 6566 2067 6574 5f74 6167 5f66 726f 6d5f  ef get_tag_from_
-00009530: 7369 7a65 5f74 656e 736f 7228 636c 732c  size_tensor(cls,
-00009540: 2078 2920 2d3e 204f 7074 696f 6e61 6c5b   x) -> Optional[
-00009550: 5f64 2e44 696d 5d3a 0a20 2020 2020 2020  _d.Dim]:.       
-00009560: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00009570: 7261 6d20 7466 2e54 656e 736f 7220 783a  ram tf.Tensor x:
-00009580: 2073 697a 6520 7465 6e73 6f72 2e20 6861   size tensor. ha
-00009590: 7320 6265 656e 2073 6574 2062 6566 6f72  s been set befor
-000095a0: 6520 7669 6120 3a66 756e 633a 6073 6574  e via :func:`set
-000095b0: 5f74 6167 5f6f 6e5f 7369 7a65 5f74 656e  _tag_on_size_ten
-000095c0: 736f 7260 0a20 2020 2020 2020 2022 2222  sor`.        """
-000095d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000095e0: 6765 7461 7474 7228 782c 2022 5f69 735f  getattr(x, "_is_
-000095f0: 7369 7a65 5f6f 665f 6469 6d5f 7461 6722  size_of_dim_tag"
-00009600: 2c20 4e6f 6e65 290a 0a20 2020 2064 6566  , None)..    def
-00009610: 2063 6f6d 706c 6574 655f 6479 6e5f 7369   complete_dyn_si
-00009620: 7a65 2873 656c 662c 2074 656d 706c 6174  ze(self, templat
-00009630: 655f 6f6e 6c79 3d46 616c 7365 293a 0a20  e_only=False):. 
-00009640: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009650: 2020 2049 6e20 6361 7365 2077 6520 6361     In case we ca
-00009660: 6e20 6361 6c63 756c 6174 6520 7468 6520  n calculate the 
-00009670: 6479 6e20 7369 7a65 2c20 646f 2074 6861  dyn size, do tha
-00009680: 7420 6e6f 772e 0a0a 2020 2020 2020 2020  t now...        
-00009690: 3a70 6172 616d 2062 6f6f 6c20 7465 6d70  :param bool temp
-000096a0: 6c61 7465 5f6f 6e6c 793a 0a20 2020 2020  late_only:.     
-000096b0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000096c0: 6620 6e6f 7420 7365 6c66 2e69 735f 6479  f not self.is_dy
-000096d0: 6e61 6d69 6328 293a 0a20 2020 2020 2020  namic():.       
-000096e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000096f0: 2020 2020 7365 6c66 2e5f 7661 6c69 6461      self._valida
-00009700: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
-00009710: 6170 6828 290a 2020 2020 2020 2020 6966  aph().        if
-00009720: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00009730: 7874 2061 6e64 2028 7365 6c66 2e64 796e  xt and (self.dyn
-00009740: 5f73 697a 655f 6578 742e 706c 6163 6568  _size_ext.placeh
-00009750: 6f6c 6465 7220 6973 206e 6f74 204e 6f6e  older is not Non
-00009760: 6520 6f72 2074 656d 706c 6174 655f 6f6e  e or template_on
-00009770: 6c79 293a 0a20 2020 2020 2020 2020 2020  ly):.           
-00009780: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00009790: 7361 6d65 5f62 6173 6520 3d20 7365 6c66  same_base = self
-000097a0: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
-000097b0: 0a20 2020 2020 2020 206f 7020 3d20 7365  .        op = se
-000097c0: 6c66 2e64 6572 6976 6564 5f66 726f 6d5f  lf.derived_from_
-000097d0: 6f70 206f 7220 7361 6d65 5f62 6173 652e  op or same_base.
-000097e0: 6465 7269 7665 645f 6672 6f6d 5f6f 700a  derived_from_op.
-000097f0: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
-00009800: 703a 0a20 2020 2020 2020 2020 2020 2072  p:.            r
-00009810: 6574 7572 6e0a 0a20 2020 2020 2020 2066  eturn..        f
-00009820: 6f72 2078 2069 6e20 6f70 2e69 6e70 7574  or x in op.input
-00009830: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00009840: 6620 7365 6c66 2e62 6174 6368 3a0a 2020  f self.batch:.  
-00009850: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-00009860: 3d20 782e 6765 745f 666f 725f 6261 7463  = x.get_for_batc
-00009870: 685f 6374 7828 7365 6c66 2e62 6174 6368  h_ctx(self.batch
-00009880: 2c20 7365 6c66 2e63 6f6e 7472 6f6c 5f66  , self.control_f
-00009890: 6c6f 775f 6374 7829 0a20 2020 2020 2020  low_ctx).       
-000098a0: 2020 2020 2078 2e63 6f6d 706c 6574 655f       x.complete_
-000098b0: 6479 6e5f 7369 7a65 2874 656d 706c 6174  dyn_size(templat
-000098c0: 655f 6f6e 6c79 3d74 656d 706c 6174 655f  e_only=template_
-000098d0: 6f6e 6c79 290a 0a20 2020 2020 2020 2062  only)..        b
-000098e0: 6163 6b65 6e64 203d 204e 6f6e 650a 2020  ackend = None.  
-000098f0: 2020 2020 2020 666f 7220 7820 696e 206f        for x in o
-00009900: 702e 696e 7075 7473 3a0a 2020 2020 2020  p.inputs:.      
-00009910: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-00009920: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
-00009930: 2020 2020 2078 203d 2078 2e67 6574 5f66       x = x.get_f
-00009940: 6f72 5f62 6174 6368 5f63 7478 2873 656c  or_batch_ctx(sel
-00009950: 662e 6261 7463 682c 2073 656c 662e 636f  f.batch, self.co
-00009960: 6e74 726f 6c5f 666c 6f77 5f63 7478 290a  ntrol_flow_ctx).
-00009970: 2020 2020 2020 2020 2020 2020 6966 2078              if x
-00009980: 2e64 796e 5f73 697a 655f 6578 7420 616e  .dyn_size_ext an
-00009990: 6420 782e 6479 6e5f 7369 7a65 5f65 7874  d x.dyn_size_ext
-000099a0: 2e72 6177 5f74 656e 736f 7220 6973 206e  .raw_tensor is n
-000099b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000099c0: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
-000099d0: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-000099e0: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
-000099f0: 2020 2020 2020 2020 2020 6261 636b 656e            backen
-00009a00: 6420 3d20 782e 6479 6e5f 7369 7a65 5f65  d = x.dyn_size_e
-00009a10: 7874 2e5f 7261 775f 6261 636b 656e 640a  xt._raw_backend.
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 6272 6561 6b0a 0a20 2020 2020 2020 2073  break..        s
-00009a40: 697a 655f 6474 7970 6520 3d20 4e6f 6e65  ize_dtype = None
-00009a50: 0a20 2020 2020 2020 2066 6f72 2078 2069  .        for x i
-00009a60: 6e20 6f70 2e69 6e70 7574 733a 0a20 2020  n op.inputs:.   
-00009a70: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00009a80: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
-00009a90: 2020 2020 2020 2020 7820 3d20 782e 6765          x = x.ge
-00009aa0: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-00009ab0: 7365 6c66 2e62 6174 6368 2c20 7365 6c66  self.batch, self
-00009ac0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-00009ad0: 7829 0a20 2020 2020 2020 2020 2020 2069  x).            i
-00009ae0: 6620 782e 6479 6e5f 7369 7a65 5f65 7874  f x.dyn_size_ext
-00009af0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009b00: 2020 7369 7a65 5f64 7479 7065 203d 2078    size_dtype = x
-00009b10: 2e64 796e 5f73 697a 655f 6578 742e 6474  .dyn_size_ext.dt
-00009b20: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
-00009b30: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00009b40: 2020 6966 206e 6f74 2073 697a 655f 6474    if not size_dt
-00009b50: 7970 653a 0a20 2020 2020 2020 2020 2020  ype:.           
-00009b60: 2073 697a 655f 6474 7970 6520 3d20 5f74   size_dtype = _t
-00009b70: 2e54 656e 736f 722e 7369 7a65 5f64 7479  .Tensor.size_dty
-00009b80: 7065 0a0a 2020 2020 2020 2020 696d 706f  pe..        impo
-00009b90: 7274 206e 756d 7079 0a20 2020 2020 2020  rt numpy.       
-00009ba0: 2069 6d70 6f72 7420 7265 7475 726e 6e2e   import returnn.
-00009bb0: 6672 6f6e 7465 6e64 2061 7320 7266 0a0a  frontend as rf..
-00009bc0: 2020 2020 2020 2020 7466 203d 2074 665f          tf = tf_
-00009bd0: 7574 696c 203d 2074 656e 736f 725f 7574  util = tensor_ut
-00009be0: 696c 203d 204e 6f6e 650a 2020 2020 2020  il = None.      
-00009bf0: 2020 6966 2062 6163 6b65 6e64 2061 6e64    if backend and
-00009c00: 2062 6163 6b65 6e64 2e69 735f 7465 6e73   backend.is_tens
-00009c10: 6f72 666c 6f77 3a0a 2020 2020 2020 2020  orflow:.        
-00009c20: 2020 2020 696d 706f 7274 2074 656e 736f      import tenso
-00009c30: 7266 6c6f 7720 6173 2074 660a 0a20 2020  rflow as tf..   
-00009c40: 2020 2020 2020 2020 2069 6620 6261 636b           if back
-00009c50: 656e 642e 5261 7754 656e 736f 7254 7970  end.RawTensorTyp
-00009c60: 6520 3d3d 2074 662e 5465 6e73 6f72 3a0a  e == tf.Tensor:.
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 6672 6f6d 2072 6574 7572 6e6e 2e74 662e  from returnn.tf.
-00009c90: 7574 696c 2069 6d70 6f72 7420 6261 7369  util import basi
-00009ca0: 6320 6173 2074 665f 7574 696c 0a20 2020  c as tf_util.   
-00009cb0: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-00009cc0: 6d20 7465 6e73 6f72 666c 6f77 2e70 7974  m tensorflow.pyt
-00009cd0: 686f 6e2e 6672 616d 6577 6f72 6b20 696d  hon.framework im
-00009ce0: 706f 7274 2074 656e 736f 725f 7574 696c  port tensor_util
-00009cf0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00009d00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009d10: 2020 2074 6620 3d20 4e6f 6e65 0a0a 2020     tf = None..  
-00009d20: 2020 2020 2020 6b69 6e64 203d 206f 702e        kind = op.
-00009d30: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
-00009d40: 6b69 6e64 2e65 6e64 7377 6974 6828 225f  kind.endswith("_
-00009d50: 7269 6768 7422 293a 0a20 2020 2020 2020  right"):.       
-00009d60: 2020 2020 206b 696e 6420 3d20 6b69 6e64       kind = kind
-00009d70: 5b3a 202d 6c65 6e28 225f 7269 6768 7422  [: -len("_right"
-00009d80: 295d 2020 2320 6f72 6465 7220 646f 6573  )]  # order does
-00009d90: 206e 6f74 206d 6174 7465 7220 6865 7265   not matter here
-00009da0: 0a20 2020 2020 2020 2069 6620 6b69 6e64  .        if kind
-00009db0: 2e65 6e64 7377 6974 6828 225f 6c65 6674  .endswith("_left
-00009dc0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00009dd0: 6b69 6e64 203d 206b 696e 645b 3a20 2d6c  kind = kind[: -l
-00009de0: 656e 2822 5f6c 6566 7422 295d 0a0a 2020  en("_left")]..  
-00009df0: 2020 2020 2020 6465 6620 5f69 735f 6e65        def _is_ne
-00009e00: 6761 7469 7665 2878 5f5f 293a 0a20 2020  gative(x__):.   
-00009e10: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00009e20: 7374 616e 6365 2878 5f5f 2c20 6e75 6d70  stance(x__, nump
-00009e30: 792e 6e64 6172 7261 7929 3a0a 2020 2020  y.ndarray):.    
-00009e40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009e50: 726e 2028 785f 5f20 3c20 3029 2e61 6e79  rn (x__ < 0).any
-00009e60: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-00009e70: 6620 6973 696e 7374 616e 6365 2878 5f5f  f isinstance(x__
-00009e80: 2c20 2869 6e74 2c20 666c 6f61 742c 206e  , (int, float, n
-00009e90: 756d 7079 2e6e 756d 6265 7229 293a 0a20  umpy.number)):. 
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009eb0: 6574 7572 6e20 785f 5f20 3c20 300a 2020  eturn x__ < 0.  
-00009ec0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00009ed0: 2074 663a 0a20 2020 2020 2020 2020 2020   tf:.           
-00009ee0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00009ef0: 650a 2020 2020 2020 2020 2020 2020 6173  e.            as
-00009f00: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
-00009f10: 785f 5f2c 2074 662e 5465 6e73 6f72 290a  x__, tf.Tensor).
-00009f20: 2020 2020 2020 2020 2020 2020 785f 5f20              x__ 
-00009f30: 3d20 7465 6e73 6f72 5f75 7469 6c2e 636f  = tensor_util.co
-00009f40: 6e73 7461 6e74 5f76 616c 7565 2878 5f5f  nstant_value(x__
-00009f50: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00009f60: 2078 5f5f 2069 7320 6e6f 7420 4e6f 6e65   x__ is not None
-00009f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009f80: 2020 7265 7475 726e 205f 6973 5f6e 6567    return _is_neg
-00009f90: 6174 6976 6528 785f 5f29 0a20 2020 2020  ative(x__).     
-00009fa0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00009fb0: 6c73 650a 0a20 2020 2020 2020 2064 6566  lse..        def
-00009fc0: 205f 6269 6e5f 6f70 5f74 6628 612c 2062   _bin_op_tf(a, b
-00009fd0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00009fe0: 6620 7465 6d70 6c61 7465 5f6f 6e6c 793a  f template_only:
-00009ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a000: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
-0000a010: 2020 2020 2020 2020 2069 6620 6120 6973           if a is
-0000a020: 204e 6f6e 6520 6f72 2062 2069 7320 4e6f   None or b is No
-0000a030: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a040: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0000a050: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000a060: 7274 2069 7369 6e73 7461 6e63 6528 612c  rt isinstance(a,
-0000a070: 2074 662e 5465 6e73 6f72 2920 616e 6420   tf.Tensor) and 
-0000a080: 6973 696e 7374 616e 6365 2862 2c20 2869  isinstance(b, (i
-0000a090: 6e74 2c20 7466 2e54 656e 736f 7229 290a  nt, tf.Tensor)).
-0000a0a0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000a0b0: 2074 665f 7574 696c 2e73 616d 655f 636f   tf_util.same_co
-0000a0c0: 6e74 726f 6c5f 666c 6f77 5f63 7478 285b  ntrol_flow_ctx([
-0000a0d0: 612c 2062 5d29 3a0a 2020 2020 2020 2020  a, b]):.        
-0000a0e0: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
-0000a0f0: 3d3d 2022 6164 6422 3a0a 2020 2020 2020  == "add":.      
-0000a100: 2020 2020 2020 2020 2020 2020 2020 7573                us
-0000a110: 655f 7265 6c75 203d 205f 6973 5f6e 6567  e_relu = _is_neg
-0000a120: 6174 6976 6528 6129 206f 7220 5f69 735f  ative(a) or _is_
-0000a130: 6e65 6761 7469 7665 2862 2920 2023 2066  negative(b)  # f
-0000a140: 6f72 2064 796e 616d 6963 2074 656e 736f  or dynamic tenso
-0000a150: 7273 2c20 6173 7375 6d65 2061 6c6c 2070  rs, assume all p
-0000a160: 6f73 6974 6976 650a 2020 2020 2020 2020  ositive.        
-0000a170: 2020 2020 2020 2020 2020 2020 6966 2075              if u
-0000a180: 7365 5f72 656c 753a 0a20 2020 2020 2020  se_relu:.       
-0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1a0: 2072 6574 7572 6e20 7466 2e63 6f6e 7665   return tf.conve
-0000a1b0: 7274 5f74 6f5f 7465 6e73 6f72 2874 665f  rt_to_tensor(tf_
-0000a1c0: 7574 696c 2e73 696d 706c 6966 795f 6e6f  util.simplify_no
-0000a1d0: 6e5f 6e65 6761 7469 7665 5f73 6571 5f6c  n_negative_seq_l
-0000a1e0: 656e 6774 6828 6120 2b20 6229 290a 2020  ength(a + b)).  
-0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a200: 2020 7265 7475 726e 2061 202b 2062 0a20    return a + b. 
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a220: 6c69 6620 6b69 6e64 203d 3d20 2273 7562  lif kind == "sub
-0000a230: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0000a240: 2020 2020 2020 2072 6574 7572 6e20 7466         return tf
-0000a250: 2e63 6f6e 7665 7274 5f74 6f5f 7465 6e73  .convert_to_tens
-0000a260: 6f72 2874 665f 7574 696c 2e73 696d 706c  or(tf_util.simpl
-0000a270: 6966 795f 6e6f 6e5f 6e65 6761 7469 7665  ify_non_negative
-0000a280: 5f73 6571 5f6c 656e 6774 6828 6120 2d20  _seq_length(a - 
-0000a290: 6229 290a 2020 2020 2020 2020 2020 2020  b)).            
-0000a2a0: 2020 2020 656c 6966 206b 696e 6420 3d3d      elif kind ==
-0000a2b0: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
-0000a2c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a2d0: 726e 2061 202a 2062 0a20 2020 2020 2020  rn a * b.       
-0000a2e0: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
-0000a2f0: 6e64 2069 6e20 2822 666c 6f6f 7264 6976  nd in ("floordiv
-0000a300: 222c 2022 7472 7565 6469 7622 293a 2020  ", "truediv"):  
-0000a310: 2320 7472 7565 6469 7620 6173 7375 6d65  # truediv assume
-0000a320: 7320 7468 6572 6520 6973 206e 6f20 7265  s there is no re
-0000a330: 6d61 696e 6465 720a 2020 2020 2020 2020  mainder.        
-0000a340: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a350: 726e 2061 202f 2f20 620a 2020 2020 2020  rn a // b.      
-0000a360: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-0000a370: 696e 6420 3d3d 2022 6365 696c 6469 7622  ind == "ceildiv"
-0000a380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a390: 2020 2020 2020 7265 7475 726e 202d 282d        return -(-
-0000a3a0: 6120 2f2f 2062 290a 2020 2020 2020 2020  a // b).        
-0000a3b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000a3e0: 6f72 2822 756e 6b6e 6f77 6e20 6f70 206b  or("unknown op k
-0000a3f0: 696e 6420 2572 2220 2520 6f70 2e6b 696e  ind %r" % op.kin
-0000a400: 6429 0a0a 2020 2020 2020 2020 6465 6620  d)..        def 
-0000a410: 5f62 696e 5f6f 7028 612c 2062 293a 0a20  _bin_op(a, b):. 
-0000a420: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-0000a430: 6d70 6c61 7465 5f6f 6e6c 7920 6f72 206e  mplate_only or n
-0000a440: 6f74 2062 6163 6b65 6e64 3a0a 2020 2020  ot backend:.    
-0000a450: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000a460: 7369 6e73 7461 6e63 6528 612c 205f 742e  sinstance(a, _t.
-0000a470: 5465 6e73 6f72 2920 616e 6420 6973 696e  Tensor) and isin
-0000a480: 7374 616e 6365 2862 2c20 5f74 2e54 656e  stance(b, _t.Ten
-0000a490: 736f 7229 3a0a 2020 2020 2020 2020 2020  sor):.          
-0000a4a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000a4b0: 205f 742e 5465 6e73 6f72 2e67 6574 5f63   _t.Tensor.get_c
-0000a4c0: 6f6d 6d6f 6e5f 6461 7461 285b 612c 2062  ommon_data([a, b
-0000a4d0: 5d2c 2061 6c6c 6f77 5f62 726f 6164 6361  ], allow_broadca
-0000a4e0: 7374 5f61 6c6c 5f73 6f75 7263 6573 3d54  st_all_sources=T
-0000a4f0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0000a500: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000a510: 6365 2861 2c20 5f74 2e54 656e 736f 7229  ce(a, _t.Tensor)
-0000a520: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a530: 2020 2020 2020 7265 7475 726e 2061 0a20        return a. 
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a550: 6620 6973 696e 7374 616e 6365 2862 2c20  f isinstance(b, 
-0000a560: 5f74 2e54 656e 736f 7229 3a0a 2020 2020  _t.Tensor):.    
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 7265 7475 726e 2062 0a20 2020 2020 2020  return b.       
-0000a590: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
-0000a5a0: 2261 6464 223a 0a20 2020 2020 2020 2020  "add":.         
-0000a5b0: 2020 2020 2020 2072 6574 7572 6e20 5f72         return _r
-0000a5c0: 656c 7528 6120 2b20 6229 0a20 2020 2020  elu(a + b).     
-0000a5d0: 2020 2020 2020 2065 6c69 6620 6b69 6e64         elif kind
-0000a5e0: 203d 3d20 2273 7562 223a 0a20 2020 2020   == "sub":.     
-0000a5f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a600: 6e20 5f72 656c 7528 6120 2d20 6229 0a20  n _relu(a - b). 
-0000a610: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000a620: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a640: 6574 7572 6e20 6120 2a20 620a 2020 2020  eturn a * b.    
-0000a650: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-0000a660: 6420 696e 2028 2266 6c6f 6f72 6469 7622  d in ("floordiv"
-0000a670: 2c20 2274 7275 6564 6976 2229 3a20 2023  , "truediv"):  #
-0000a680: 2074 7275 6564 6976 2061 7373 756d 6573   truediv assumes
-0000a690: 2074 6865 7265 2069 7320 6e6f 2072 656d   there is no rem
-0000a6a0: 6169 6e64 6572 0a20 2020 2020 2020 2020  ainder.         
-0000a6b0: 2020 2020 2020 2072 6574 7572 6e20 6120         return a 
-0000a6c0: 2f2f 2062 0a20 2020 2020 2020 2020 2020  // b.           
-0000a6d0: 2065 6c69 6620 6b69 6e64 203d 3d20 2263   elif kind == "c
-0000a6e0: 6569 6c64 6976 223a 0a20 2020 2020 2020  eildiv":.       
-0000a6f0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000a700: 7374 616e 6365 2861 2c20 5f74 2e54 656e  stance(a, _t.Ten
-0000a710: 736f 7229 3a0a 2020 2020 2020 2020 2020  sor):.          
-0000a720: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000a730: 2072 662e 6365 696c 5f64 6976 6964 6528   rf.ceil_divide(
-0000a740: 612c 2062 290a 2020 2020 2020 2020 2020  a, b).          
-0000a750: 2020 2020 2020 7265 7475 726e 202d 282d        return -(-
-0000a760: 6120 2f2f 2062 290a 2020 2020 2020 2020  a // b).        
-0000a770: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a780: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000a790: 5661 6c75 6545 7272 6f72 2822 756e 6b6e  ValueError("unkn
-0000a7a0: 6f77 6e20 6f70 206b 696e 6420 2572 2220  own op kind %r" 
-0000a7b0: 2520 6f70 2e6b 696e 6429 0a0a 2020 2020  % op.kind)..    
-0000a7c0: 2020 2020 6465 6620 5f72 656c 7528 6129      def _relu(a)
-0000a7d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000a7e0: 2069 7369 6e73 7461 6e63 6528 612c 205f   isinstance(a, _
-0000a7f0: 742e 5465 6e73 6f72 293a 0a20 2020 2020  t.Tensor):.     
-0000a800: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a810: 6e20 7266 2e72 656c 7528 6129 0a20 2020  n rf.relu(a).   
-0000a820: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-0000a830: 696e 7374 616e 6365 2861 2c20 696e 7429  instance(a, int)
-0000a840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a850: 2020 7265 7475 726e 206d 6178 2861 2c20    return max(a, 
-0000a860: 3029 0a20 2020 2020 2020 2020 2020 2065  0).            e
-0000a870: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000a880: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-0000a890: 7272 6f72 2866 2263 6f6d 706c 6574 655f  rror(f"complete_
-0000a8a0: 6479 6e5f 7369 7a65 3a20 5f72 656c 753a  dyn_size: _relu:
-0000a8b0: 2075 6e65 7870 6563 7465 6420 7479 7065   unexpected type
-0000a8c0: 207b 7479 7065 2861 297d 2229 0a0a 2020   {type(a)}")..  
-0000a8d0: 2020 2020 2020 795f 6e61 6d65 203d 2073        y_name = s
-0000a8e0: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-0000a8f0: 2b20 223a 7365 712d 6c65 6e67 7468 220a  + ":seq-length".
-0000a900: 2020 2020 2020 2020 793a 204f 7074 696f          y: Optio
-0000a910: 6e61 6c5b 5f74 2e54 656e 736f 725d 203d  nal[_t.Tensor] =
-0000a920: 204e 6f6e 6520 2023 2072 6573 756c 7469   None  # resulti
-0000a930: 6e67 2064 796e 2073 697a 650a 2020 2020  ng dyn size.    
-0000a940: 2020 2020 696e 7075 7473 203d 206c 6973      inputs = lis
-0000a950: 7428 6f70 2e69 6e70 7574 7329 0a20 2020  t(op.inputs).   
-0000a960: 2020 2020 2061 7373 6572 7420 696e 7075       assert inpu
-0000a970: 7473 0a20 2020 2020 2020 2077 6869 6c65  ts.        while
-0000a980: 2069 6e70 7574 733a 0a20 2020 2020 2020   inputs:.       
-0000a990: 2020 2020 2078 203d 2069 6e70 7574 732e       x = inputs.
-0000a9a0: 706f 7028 3029 0a20 2020 2020 2020 2020  pop(0).         
-0000a9b0: 2020 2069 6620 6e6f 7420 782e 6973 5f64     if not x.is_d
-0000a9c0: 796e 616d 6963 2829 3a20 2023 2073 7461  ynamic():  # sta
-0000a9d0: 7469 630a 2020 2020 2020 2020 2020 2020  tic.            
-0000a9e0: 2020 2020 6173 7365 7274 2078 2e64 696d      assert x.dim
-0000a9f0: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
-0000aa00: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000aa10: 2020 2069 6620 7920 6973 204e 6f6e 653a     if y is None:
-0000aa20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aa30: 2020 2020 2069 6620 6e6f 7420 7465 6d70       if not temp
-0000aa40: 6c61 7465 5f6f 6e6c 7920 616e 6420 6261  late_only and ba
-0000aa50: 636b 656e 6420 616e 6420 6e6f 7420 7466  ckend and not tf
-0000aa60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000aa70: 2020 2020 2020 2020 2020 7769 7468 2072            with r
-0000aa80: 662e 7365 745f 6465 6661 756c 745f 6465  f.set_default_de
-0000aa90: 7669 6365 5f63 7478 284e 6f6e 6529 3a0a  vice_ctx(None):.
+00009100: 2020 2022 7361 6d65 5f61 7320 3d20 2573     "same_as = %s
+00009110: 2220 2520 7365 6c66 2e73 616d 655f 6173  " % self.same_as
+00009120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009130: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00009140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009150: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009160: 2020 290a 2020 2020 2020 2020 6966 2062    ).        if b
+00009170: 6174 6368 2061 6e64 2067 6574 6174 7472  atch and getattr
+00009180: 2878 2c20 225f 5245 5455 524e 4e5f 6479  (x, "_RETURNN_dy
+00009190: 6e5f 7369 7a65 5f62 6561 6d22 2c20 4e6f  n_size_beam", No
+000091a0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+000091b0: 2061 7373 6572 7420 6261 7463 682e 6265   assert batch.be
+000091c0: 616d 203d 3d20 6765 7461 7474 7228 0a20  am == getattr(. 
+000091d0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+000091e0: 2c20 225f 5245 5455 524e 4e5f 6479 6e5f  , "_RETURNN_dyn_
+000091f0: 7369 7a65 5f62 6561 6d22 0a20 2020 2020  size_beam".     
+00009200: 2020 2020 2020 2029 2c20 2225 733a 2064         ), "%s: d
+00009210: 796e 2073 697a 6520 2573 2068 6173 2075  yn size %s has u
+00009220: 6e65 7870 6563 7465 6420 6261 7463 6820  nexpected batch 
+00009230: 2573 2c20 6578 7065 6374 6564 2025 7322  %s, expected %s"
+00009240: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
+00009250: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00009260: 2020 2020 2020 2020 2020 2078 2c0a 2020             x,.  
+00009270: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+00009280: 7463 682c 0a20 2020 2020 2020 2020 2020  tch,.           
+00009290: 2020 2020 2067 6574 6174 7472 2878 2c20       getattr(x, 
+000092a0: 225f 5245 5455 524e 4e5f 6479 6e5f 7369  "_RETURNN_dyn_si
+000092b0: 7a65 5f62 6561 6d22 292c 0a20 2020 2020  ze_beam"),.     
+000092c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000092d0: 2069 6620 7365 6c66 2e62 6174 6368 2061   if self.batch a
+000092e0: 6e64 2062 6174 6368 3a0a 2020 2020 2020  nd batch:.      
+000092f0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+00009300: 662e 6261 7463 6820 3d3d 2062 6174 6368  f.batch == batch
+00009310: 0a20 2020 2020 2020 2065 6c69 6620 6261  .        elif ba
+00009320: 7463 6820 616e 6420 6e6f 7420 7365 6c66  tch and not self
+00009330: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
+00009340: 2020 2020 7365 6c66 2e62 6174 6368 203d      self.batch =
+00009350: 2062 6174 6368 2020 2320 6f76 6572 7461   batch  # overta
+00009360: 6b65 0a20 2020 2020 2020 2069 6620 6e6f  ke.        if no
+00009370: 7420 7365 6c66 2e69 735f 6261 7463 685f  t self.is_batch_
+00009380: 6469 6d28 2920 616e 6420 7365 6c66 2e69  dim() and self.i
+00009390: 735f 6479 6e61 6d69 6328 293a 0a20 2020  s_dynamic():.   
+000093a0: 2020 2020 2020 2020 2069 6620 7361 6d65           if same
+000093b0: 5f61 735f 6265 666f 7265 3a0a 2020 2020  _as_before:.    
+000093c0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+000093d0: 7274 2073 656c 662e 6479 6e5f 7369 7a65  rt self.dyn_size
+000093e0: 5f65 7874 2061 6e64 2073 656c 662e 6479  _ext and self.dy
+000093f0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+00009400: 686f 6c64 6572 2069 7320 6e6f 7420 4e6f  holder is not No
+00009410: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00009420: 2020 2023 2044 6f20 6e6f 7420 6f76 6572     # Do not over
+00009430: 7772 6974 6520 6974 2e0a 2020 2020 2020  write it..      
+00009440: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009460: 2e5f 696e 6974 5f64 6566 6175 6c74 5f64  ._init_default_d
+00009470: 796e 5f73 697a 655f 6578 7428 7829 0a20  yn_size_ext(x). 
+00009480: 2020 2020 2020 2069 6620 6765 7461 7474         if getatt
+00009490: 7228 782c 2022 5f69 735f 7369 7a65 5f6f  r(x, "_is_size_o
+000094a0: 665f 6469 6d5f 7461 6722 2c20 4e6f 6e65  f_dim_tag", None
+000094b0: 2920 6973 204e 6f6e 653a 0a20 2020 2020  ) is None:.     
+000094c0: 2020 2020 2020 2073 6574 6174 7472 2878         setattr(x
+000094d0: 2c20 225f 6973 5f73 697a 655f 6f66 5f64  , "_is_size_of_d
+000094e0: 696d 5f74 6167 222c 2073 656c 6629 0a20  im_tag", self). 
+000094f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009500: 6c66 0a0a 2020 2020 4063 6c61 7373 6d65  lf..    @classme
+00009510: 7468 6f64 0a20 2020 2064 6566 2067 6574  thod.    def get
+00009520: 5f74 6167 5f66 726f 6d5f 7369 7a65 5f74  _tag_from_size_t
+00009530: 656e 736f 7228 636c 732c 2078 2920 2d3e  ensor(cls, x) ->
+00009540: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
+00009550: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+00009560: 2020 2020 2020 203a 7061 7261 6d20 7466         :param tf
+00009570: 2e54 656e 736f 7220 783a 2073 697a 6520  .Tensor x: size 
+00009580: 7465 6e73 6f72 2e20 6861 7320 6265 656e  tensor. has been
+00009590: 2073 6574 2062 6566 6f72 6520 7669 6120   set before via 
+000095a0: 3a66 756e 633a 6073 6574 5f74 6167 5f6f  :func:`set_tag_o
+000095b0: 6e5f 7369 7a65 5f74 656e 736f 7260 0a20  n_size_tensor`. 
+000095c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000095d0: 2020 2072 6574 7572 6e20 6765 7461 7474     return getatt
+000095e0: 7228 782c 2022 5f69 735f 7369 7a65 5f6f  r(x, "_is_size_o
+000095f0: 665f 6469 6d5f 7461 6722 2c20 4e6f 6e65  f_dim_tag", None
+00009600: 290a 0a20 2020 2064 6566 2063 6f6d 706c  )..    def compl
+00009610: 6574 655f 6479 6e5f 7369 7a65 2873 656c  ete_dyn_size(sel
+00009620: 662c 2074 656d 706c 6174 655f 6f6e 6c79  f, template_only
+00009630: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
+00009640: 2022 2222 0a20 2020 2020 2020 2049 6e20   """.        In 
+00009650: 6361 7365 2077 6520 6361 6e20 6361 6c63  case we can calc
+00009660: 756c 6174 6520 7468 6520 6479 6e20 7369  ulate the dyn si
+00009670: 7a65 2c20 646f 2074 6861 7420 6e6f 772e  ze, do that now.
+00009680: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00009690: 2062 6f6f 6c20 7465 6d70 6c61 7465 5f6f   bool template_o
+000096a0: 6e6c 793a 0a20 2020 2020 2020 2022 2222  nly:.        """
+000096b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000096c0: 7365 6c66 2e69 735f 6479 6e61 6d69 6328  self.is_dynamic(
+000096d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000096e0: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
+000096f0: 6c66 2e5f 7661 6c69 6461 7465 5f69 6e5f  lf._validate_in_
+00009700: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
+00009710: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009720: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+00009730: 2028 7365 6c66 2e64 796e 5f73 697a 655f   (self.dyn_size_
+00009740: 6578 742e 706c 6163 6568 6f6c 6465 7220  ext.placeholder 
+00009750: 6973 206e 6f74 204e 6f6e 6520 6f72 2074  is not None or t
+00009760: 656d 706c 6174 655f 6f6e 6c79 293a 0a20  emplate_only):. 
+00009770: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009780: 6e0a 2020 2020 2020 2020 7361 6d65 5f62  n.        same_b
+00009790: 6173 6520 3d20 7365 6c66 2e67 6574 5f73  ase = self.get_s
+000097a0: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
+000097b0: 2020 206f 7020 3d20 7365 6c66 2e64 6572     op = self.der
+000097c0: 6976 6564 5f66 726f 6d5f 6f70 206f 7220  ived_from_op or 
+000097d0: 7361 6d65 5f62 6173 652e 6465 7269 7665  same_base.derive
+000097e0: 645f 6672 6f6d 5f6f 700a 2020 2020 2020  d_from_op.      
+000097f0: 2020 6966 206e 6f74 206f 703a 0a20 2020    if not op:.   
+00009800: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00009810: 0a20 2020 2020 2020 2066 6f72 2078 2069  .        for x i
+00009820: 6e20 6f70 2e69 6e70 7574 733a 0a20 2020  n op.inputs:.   
+00009830: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00009840: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
+00009850: 2020 2020 2020 2020 7820 3d20 782e 6765          x = x.ge
+00009860: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
+00009870: 7365 6c66 2e62 6174 6368 2c20 7365 6c66  self.batch, self
+00009880: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+00009890: 7829 0a20 2020 2020 2020 2020 2020 2078  x).            x
+000098a0: 2e63 6f6d 706c 6574 655f 6479 6e5f 7369  .complete_dyn_si
+000098b0: 7a65 2874 656d 706c 6174 655f 6f6e 6c79  ze(template_only
+000098c0: 3d74 656d 706c 6174 655f 6f6e 6c79 290a  =template_only).
+000098d0: 0a20 2020 2020 2020 2062 6163 6b65 6e64  .        backend
+000098e0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000098f0: 666f 7220 7820 696e 206f 702e 696e 7075  for x in op.inpu
+00009900: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00009910: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
+00009920: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00009930: 203d 2078 2e67 6574 5f66 6f72 5f62 6174   = x.get_for_bat
+00009940: 6368 5f63 7478 2873 656c 662e 6261 7463  ch_ctx(self.batc
+00009950: 682c 2073 656c 662e 636f 6e74 726f 6c5f  h, self.control_
+00009960: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
+00009970: 2020 2020 2020 6966 2078 2e64 796e 5f73        if x.dyn_s
+00009980: 697a 655f 6578 7420 616e 6420 782e 6479  ize_ext and x.dy
+00009990: 6e5f 7369 7a65 5f65 7874 2e72 6177 5f74  n_size_ext.raw_t
+000099a0: 656e 736f 7220 6973 206e 6f74 204e 6f6e  ensor is not Non
+000099b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000099c0: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
+000099d0: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
+000099e0: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
+000099f0: 2020 2020 6261 636b 656e 6420 3d20 782e      backend = x.
+00009a00: 6479 6e5f 7369 7a65 5f65 7874 2e5f 7261  dyn_size_ext._ra
+00009a10: 775f 6261 636b 656e 640a 2020 2020 2020  w_backend.      
+00009a20: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00009a30: 0a20 2020 2020 2020 2073 697a 655f 6474  .        size_dt
+00009a40: 7970 6520 3d20 4e6f 6e65 0a20 2020 2020  ype = None.     
+00009a50: 2020 2066 6f72 2078 2069 6e20 6f70 2e69     for x in op.i
+00009a60: 6e70 7574 733a 0a20 2020 2020 2020 2020  nputs:.         
+00009a70: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+00009a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009a90: 2020 7820 3d20 782e 6765 745f 666f 725f    x = x.get_for_
+00009aa0: 6261 7463 685f 6374 7828 7365 6c66 2e62  batch_ctx(self.b
+00009ab0: 6174 6368 2c20 7365 6c66 2e63 6f6e 7472  atch, self.contr
+00009ac0: 6f6c 5f66 6c6f 775f 6374 7829 0a20 2020  ol_flow_ctx).   
+00009ad0: 2020 2020 2020 2020 2069 6620 782e 6479           if x.dy
+00009ae0: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+00009af0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00009b00: 5f64 7479 7065 203d 2078 2e64 796e 5f73  _dtype = x.dyn_s
+00009b10: 697a 655f 6578 742e 6474 7970 650a 2020  ize_ext.dtype.  
+00009b20: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00009b30: 6561 6b0a 2020 2020 2020 2020 6966 206e  eak.        if n
+00009b40: 6f74 2073 697a 655f 6474 7970 653a 0a20  ot size_dtype:. 
+00009b50: 2020 2020 2020 2020 2020 2073 697a 655f             size_
+00009b60: 6474 7970 6520 3d20 5f74 2e54 656e 736f  dtype = _t.Tenso
+00009b70: 722e 7369 7a65 5f64 7479 7065 0a0a 2020  r.size_dtype..  
+00009b80: 2020 2020 2020 696d 706f 7274 206e 756d        import num
+00009b90: 7079 0a20 2020 2020 2020 2069 6d70 6f72  py.        impor
+00009ba0: 7420 7265 7475 726e 6e2e 6672 6f6e 7465  t returnn.fronte
+00009bb0: 6e64 2061 7320 7266 0a0a 2020 2020 2020  nd as rf..      
+00009bc0: 2020 7466 203d 2074 665f 7574 696c 203d    tf = tf_util =
+00009bd0: 2074 656e 736f 725f 7574 696c 203d 204e   tensor_util = N
+00009be0: 6f6e 650a 2020 2020 2020 2020 6966 2062  one.        if b
+00009bf0: 6163 6b65 6e64 2061 6e64 2062 6163 6b65  ackend and backe
+00009c00: 6e64 2e69 735f 7465 6e73 6f72 666c 6f77  nd.is_tensorflow
+00009c10: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
+00009c20: 706f 7274 2074 656e 736f 7266 6c6f 7720  port tensorflow 
+00009c30: 6173 2074 660a 0a20 2020 2020 2020 2020  as tf..         
+00009c40: 2020 2069 6620 6261 636b 656e 642e 5261     if backend.Ra
+00009c50: 7754 656e 736f 7254 7970 6520 3d3d 2074  wTensorType == t
+00009c60: 662e 5465 6e73 6f72 3a0a 2020 2020 2020  f.Tensor:.      
+00009c70: 2020 2020 2020 2020 2020 6672 6f6d 2072            from r
+00009c80: 6574 7572 6e6e 2e74 662e 7574 696c 2069  eturnn.tf.util i
+00009c90: 6d70 6f72 7420 6261 7369 6320 6173 2074  mport basic as t
+00009ca0: 665f 7574 696c 0a20 2020 2020 2020 2020  f_util.         
+00009cb0: 2020 2020 2020 2066 726f 6d20 7465 6e73         from tens
+00009cc0: 6f72 666c 6f77 2e70 7974 686f 6e2e 6672  orflow.python.fr
+00009cd0: 616d 6577 6f72 6b20 696d 706f 7274 2074  amework import t
+00009ce0: 656e 736f 725f 7574 696c 0a20 2020 2020  ensor_util.     
+00009cf0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009d00: 2020 2020 2020 2020 2020 2020 2074 6620               tf 
+00009d10: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+00009d20: 6b69 6e64 203d 206f 702e 6b69 6e64 0a20  kind = op.kind. 
+00009d30: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
+00009d40: 6e64 7377 6974 6828 225f 7269 6768 7422  ndswith("_right"
+00009d50: 293a 0a20 2020 2020 2020 2020 2020 206b  ):.            k
+00009d60: 696e 6420 3d20 6b69 6e64 5b3a 202d 6c65  ind = kind[: -le
+00009d70: 6e28 225f 7269 6768 7422 295d 2020 2320  n("_right")]  # 
+00009d80: 6f72 6465 7220 646f 6573 206e 6f74 206d  order does not m
+00009d90: 6174 7465 7220 6865 7265 0a20 2020 2020  atter here.     
+00009da0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
+00009db0: 6974 6828 225f 6c65 6674 2229 3a0a 2020  ith("_left"):.  
+00009dc0: 2020 2020 2020 2020 2020 6b69 6e64 203d            kind =
+00009dd0: 206b 696e 645b 3a20 2d6c 656e 2822 5f6c   kind[: -len("_l
+00009de0: 6566 7422 295d 0a0a 2020 2020 2020 2020  eft")]..        
+00009df0: 6465 6620 5f69 735f 6e65 6761 7469 7665  def _is_negative
+00009e00: 2878 5f5f 293a 0a20 2020 2020 2020 2020  (x__):.         
+00009e10: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00009e20: 2878 5f5f 2c20 6e75 6d70 792e 6e64 6172  (x__, numpy.ndar
+00009e30: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
+00009e40: 2020 2020 2020 7265 7475 726e 2028 785f        return (x_
+00009e50: 5f20 3c20 3029 2e61 6e79 2829 0a20 2020  _ < 0).any().   
+00009e60: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00009e70: 7374 616e 6365 2878 5f5f 2c20 2869 6e74  stance(x__, (int
+00009e80: 2c20 666c 6f61 742c 206e 756d 7079 2e6e  , float, numpy.n
+00009e90: 756d 6265 7229 293a 0a20 2020 2020 2020  umber)):.       
+00009ea0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009eb0: 785f 5f20 3c20 300a 2020 2020 2020 2020  x__ < 0.        
+00009ec0: 2020 2020 6966 206e 6f74 2074 663a 0a20      if not tf:. 
+00009ed0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009ee0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00009ef0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00009f00: 7369 6e73 7461 6e63 6528 785f 5f2c 2074  sinstance(x__, t
+00009f10: 662e 5465 6e73 6f72 290a 2020 2020 2020  f.Tensor).      
+00009f20: 2020 2020 2020 785f 5f20 3d20 7465 6e73        x__ = tens
+00009f30: 6f72 5f75 7469 6c2e 636f 6e73 7461 6e74  or_util.constant
+00009f40: 5f76 616c 7565 2878 5f5f 290a 2020 2020  _value(x__).    
+00009f50: 2020 2020 2020 2020 6966 2078 5f5f 2069          if x__ i
+00009f60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00009f70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009f80: 726e 205f 6973 5f6e 6567 6174 6976 6528  rn _is_negative(
+00009f90: 785f 5f29 0a20 2020 2020 2020 2020 2020  x__).           
+00009fa0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+00009fb0: 2020 2020 2020 2064 6566 205f 6269 6e5f         def _bin_
+00009fc0: 6f70 5f74 6628 612c 2062 293a 0a20 2020  op_tf(a, b):.   
+00009fd0: 2020 2020 2020 2020 2069 6620 7465 6d70           if temp
+00009fe0: 6c61 7465 5f6f 6e6c 793a 0a20 2020 2020  late_only:.     
+00009ff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a000: 6e20 4e6f 6e65 0a20 2020 2020 2020 2020  n None.         
+0000a010: 2020 2069 6620 6120 6973 204e 6f6e 6520     if a is None 
+0000a020: 6f72 2062 2069 7320 4e6f 6e65 3a0a 2020  or b is None:.  
+0000a030: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000a040: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+0000a050: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+0000a060: 6e73 7461 6e63 6528 612c 2074 662e 5465  nstance(a, tf.Te
+0000a070: 6e73 6f72 2920 616e 6420 6973 696e 7374  nsor) and isinst
+0000a080: 616e 6365 2862 2c20 2869 6e74 2c20 7466  ance(b, (int, tf
+0000a090: 2e54 656e 736f 7229 290a 2020 2020 2020  .Tensor)).      
+0000a0a0: 2020 2020 2020 7769 7468 2074 665f 7574        with tf_ut
+0000a0b0: 696c 2e73 616d 655f 636f 6e74 726f 6c5f  il.same_control_
+0000a0c0: 666c 6f77 5f63 7478 285b 612c 2062 5d29  flow_ctx([a, b])
+0000a0d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a0e0: 2020 6966 206b 696e 6420 3d3d 2022 6164    if kind == "ad
+0000a0f0: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
+0000a100: 2020 2020 2020 2020 7573 655f 7265 6c75          use_relu
+0000a110: 203d 205f 6973 5f6e 6567 6174 6976 6528   = _is_negative(
+0000a120: 6129 206f 7220 5f69 735f 6e65 6761 7469  a) or _is_negati
+0000a130: 7665 2862 2920 2023 2066 6f72 2064 796e  ve(b)  # for dyn
+0000a140: 616d 6963 2074 656e 736f 7273 2c20 6173  amic tensors, as
+0000a150: 7375 6d65 2061 6c6c 2070 6f73 6974 6976  sume all positiv
+0000a160: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000a170: 2020 2020 2020 6966 2075 7365 5f72 656c        if use_rel
+0000a180: 753a 0a20 2020 2020 2020 2020 2020 2020  u:.             
+0000a190: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a1a0: 6e20 7466 2e63 6f6e 7665 7274 5f74 6f5f  n tf.convert_to_
+0000a1b0: 7465 6e73 6f72 2874 665f 7574 696c 2e73  tensor(tf_util.s
+0000a1c0: 696d 706c 6966 795f 6e6f 6e5f 6e65 6761  implify_non_nega
+0000a1d0: 7469 7665 5f73 6571 5f6c 656e 6774 6828  tive_seq_length(
+0000a1e0: 6120 2b20 6229 290a 2020 2020 2020 2020  a + b)).        
+0000a1f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a200: 726e 2061 202b 2062 0a20 2020 2020 2020  rn a + b.       
+0000a210: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
+0000a220: 6e64 203d 3d20 2273 7562 223a 0a20 2020  nd == "sub":.   
+0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 2072 6574 7572 6e20 7466 2e63 6f6e 7665   return tf.conve
+0000a250: 7274 5f74 6f5f 7465 6e73 6f72 2874 665f  rt_to_tensor(tf_
+0000a260: 7574 696c 2e73 696d 706c 6966 795f 6e6f  util.simplify_no
+0000a270: 6e5f 6e65 6761 7469 7665 5f73 6571 5f6c  n_negative_seq_l
+0000a280: 656e 6774 6828 6120 2d20 6229 290a 2020  ength(a - b)).  
+0000a290: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000a2a0: 6966 206b 696e 6420 3d3d 2022 6d75 6c22  if kind == "mul"
+0000a2b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a2c0: 2020 2020 2020 7265 7475 726e 2061 202a        return a *
+0000a2d0: 2062 0a20 2020 2020 2020 2020 2020 2020   b.             
+0000a2e0: 2020 2065 6c69 6620 6b69 6e64 2069 6e20     elif kind in 
+0000a2f0: 2822 666c 6f6f 7264 6976 222c 2022 7472  ("floordiv", "tr
+0000a300: 7565 6469 7622 293a 2020 2320 7472 7565  uediv"):  # true
+0000a310: 6469 7620 6173 7375 6d65 7320 7468 6572  div assumes ther
+0000a320: 6520 6973 206e 6f20 7265 6d61 696e 6465  e is no remainde
+0000a330: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000a340: 2020 2020 2020 7265 7475 726e 2061 202f        return a /
+0000a350: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
+0000a360: 2020 2020 656c 6966 206b 696e 6420 3d3d      elif kind ==
+0000a370: 2022 6365 696c 6469 7622 3a0a 2020 2020   "ceildiv":.    
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 7265 7475 726e 202d 282d 6120 2f2f 2062  return -(-a // b
+0000a3a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a3b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a3c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000a3d0: 6520 5661 6c75 6545 7272 6f72 2822 756e  e ValueError("un
+0000a3e0: 6b6e 6f77 6e20 6f70 206b 696e 6420 2572  known op kind %r
+0000a3f0: 2220 2520 6f70 2e6b 696e 6429 0a0a 2020  " % op.kind)..  
+0000a400: 2020 2020 2020 6465 6620 5f62 696e 5f6f        def _bin_o
+0000a410: 7028 612c 2062 293a 0a20 2020 2020 2020  p(a, b):.       
+0000a420: 2020 2020 2069 6620 7465 6d70 6c61 7465       if template
+0000a430: 5f6f 6e6c 7920 6f72 206e 6f74 2062 6163  _only or not bac
+0000a440: 6b65 6e64 3a0a 2020 2020 2020 2020 2020  kend:.          
+0000a450: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000a460: 6e63 6528 612c 205f 742e 5465 6e73 6f72  nce(a, _t.Tensor
+0000a470: 2920 616e 6420 6973 696e 7374 616e 6365  ) and isinstance
+0000a480: 2862 2c20 5f74 2e54 656e 736f 7229 3a0a  (b, _t.Tensor):.
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 7265 7475 726e 205f 742e 5465      return _t.Te
+0000a4b0: 6e73 6f72 2e67 6574 5f63 6f6d 6d6f 6e5f  nsor.get_common_
+0000a4c0: 6461 7461 285b 612c 2062 5d2c 2061 6c6c  data([a, b], all
+0000a4d0: 6f77 5f62 726f 6164 6361 7374 5f61 6c6c  ow_broadcast_all
+0000a4e0: 5f73 6f75 7263 6573 3d54 7275 6529 0a20  _sources=True). 
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a500: 6620 6973 696e 7374 616e 6365 2861 2c20  f isinstance(a, 
+0000a510: 5f74 2e54 656e 736f 7229 3a0a 2020 2020  _t.Tensor):.    
+0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a530: 7265 7475 726e 2061 0a20 2020 2020 2020  return a.       
+0000a540: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000a550: 7374 616e 6365 2862 2c20 5f74 2e54 656e  stance(b, _t.Ten
+0000a560: 736f 7229 3a0a 2020 2020 2020 2020 2020  sor):.          
+0000a570: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a580: 2062 0a20 2020 2020 2020 2020 2020 2069   b.            i
+0000a590: 6620 6b69 6e64 203d 3d20 2261 6464 223a  f kind == "add":
+0000a5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a5b0: 2072 6574 7572 6e20 5f72 656c 7528 6120   return _relu(a 
+0000a5c0: 2b20 6229 0a20 2020 2020 2020 2020 2020  + b).           
+0000a5d0: 2065 6c69 6620 6b69 6e64 203d 3d20 2273   elif kind == "s
+0000a5e0: 7562 223a 0a20 2020 2020 2020 2020 2020  ub":.           
+0000a5f0: 2020 2020 2072 6574 7572 6e20 5f72 656c       return _rel
+0000a600: 7528 6120 2d20 6229 0a20 2020 2020 2020  u(a - b).       
+0000a610: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+0000a620: 3d20 226d 756c 223a 0a20 2020 2020 2020  = "mul":.       
+0000a630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a640: 6120 2a20 620a 2020 2020 2020 2020 2020  a * b.          
+0000a650: 2020 656c 6966 206b 696e 6420 696e 2028    elif kind in (
+0000a660: 2266 6c6f 6f72 6469 7622 2c20 2274 7275  "floordiv", "tru
+0000a670: 6564 6976 2229 3a20 2023 2074 7275 6564  ediv"):  # trued
+0000a680: 6976 2061 7373 756d 6573 2074 6865 7265  iv assumes there
+0000a690: 2069 7320 6e6f 2072 656d 6169 6e64 6572   is no remainder
+0000a6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a6b0: 2072 6574 7572 6e20 6120 2f2f 2062 0a20   return a // b. 
+0000a6c0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000a6d0: 6b69 6e64 203d 3d20 2263 6569 6c64 6976  kind == "ceildiv
+0000a6e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000a6f0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000a700: 2861 2c20 5f74 2e54 656e 736f 7229 3a0a  (a, _t.Tensor):.
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a720: 2020 2020 7265 7475 726e 2072 662e 6365      return rf.ce
+0000a730: 696c 5f64 6976 6964 6528 612c 2062 290a  il_divide(a, b).
+0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 7265 7475 726e 202d 282d 6120 2f2f 2062  return -(-a // b
+0000a760: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000a770: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000a780: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000a790: 7272 6f72 2822 756e 6b6e 6f77 6e20 6f70  rror("unknown op
+0000a7a0: 206b 696e 6420 2572 2220 2520 6f70 2e6b   kind %r" % op.k
+0000a7b0: 696e 6429 0a0a 2020 2020 2020 2020 6465  ind)..        de
+0000a7c0: 6620 5f72 656c 7528 6129 3a0a 2020 2020  f _relu(a):.    
+0000a7d0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000a7e0: 7461 6e63 6528 612c 205f 742e 5465 6e73  tance(a, _t.Tens
+0000a7f0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0000a800: 2020 2020 2072 6574 7572 6e20 7266 2e72       return rf.r
+0000a810: 656c 7528 6129 0a20 2020 2020 2020 2020  elu(a).         
+0000a820: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+0000a830: 6365 2861 2c20 696e 7429 3a0a 2020 2020  ce(a, int):.    
+0000a840: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a850: 726e 206d 6178 2861 2c20 3029 0a20 2020  rn max(a, 0).   
+0000a860: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a880: 6169 7365 2054 7970 6545 7272 6f72 2866  aise TypeError(f
+0000a890: 2263 6f6d 706c 6574 655f 6479 6e5f 7369  "complete_dyn_si
+0000a8a0: 7a65 3a20 5f72 656c 753a 2075 6e65 7870  ze: _relu: unexp
+0000a8b0: 6563 7465 6420 7479 7065 207b 7479 7065  ected type {type
+0000a8c0: 2861 297d 2229 0a0a 2020 2020 2020 2020  (a)}")..        
+0000a8d0: 795f 6e61 6d65 203d 2073 656c 662e 6465  y_name = self.de
+0000a8e0: 7363 7269 7074 696f 6e20 2b20 223a 7365  scription + ":se
+0000a8f0: 712d 6c65 6e67 7468 220a 2020 2020 2020  q-length".      
+0000a900: 2020 793a 204f 7074 696f 6e61 6c5b 5f74    y: Optional[_t
+0000a910: 2e54 656e 736f 725d 203d 204e 6f6e 6520  .Tensor] = None 
+0000a920: 2023 2072 6573 756c 7469 6e67 2064 796e   # resulting dyn
+0000a930: 2073 697a 650a 2020 2020 2020 2020 696e   size.        in
+0000a940: 7075 7473 203d 206c 6973 7428 6f70 2e69  puts = list(op.i
+0000a950: 6e70 7574 7329 0a20 2020 2020 2020 2061  nputs).        a
+0000a960: 7373 6572 7420 696e 7075 7473 0a20 2020  ssert inputs.   
+0000a970: 2020 2020 2077 6869 6c65 2069 6e70 7574       while input
+0000a980: 733a 0a20 2020 2020 2020 2020 2020 2078  s:.            x
+0000a990: 203d 2069 6e70 7574 732e 706f 7028 3029   = inputs.pop(0)
+0000a9a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a9b0: 6e6f 7420 782e 6973 5f64 796e 616d 6963  not x.is_dynamic
+0000a9c0: 2829 3a20 2023 2073 7461 7469 630a 2020  ():  # static.  
+0000a9d0: 2020 2020 2020 2020 2020 2020 2020 6173                as
+0000a9e0: 7365 7274 2078 2e64 696d 656e 7369 6f6e  sert x.dimension
+0000a9f0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+0000aa00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000aa10: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000aa30: 6620 6e6f 7420 7465 6d70 6c61 7465 5f6f  f not template_o
+0000aa40: 6e6c 7920 616e 6420 6261 636b 656e 6420  nly and backend 
+0000aa50: 616e 6420 6e6f 7420 7466 3a0a 2020 2020  and not tf:.    
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2020 2020 7769 7468 2072 662e 7365 745f      with rf.set_
+0000aa80: 6465 6661 756c 745f 6465 7669 6365 5f63  default_device_c
+0000aa90: 7478 284e 6f6e 6529 3a0a 2020 2020 2020  tx(None):.      
 0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aab0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
-0000aac0: 6261 636b 656e 642e 636f 6e76 6572 745f  backend.convert_
-0000aad0: 746f 5f74 656e 736f 7228 782e 6469 6d65  to_tensor(x.dime
-0000aae0: 6e73 696f 6e2c 2064 696d 733d 5b5d 2c20  nsion, dims=[], 
-0000aaf0: 6474 7970 653d 7369 7a65 5f64 7479 7065  dtype=size_dtype
-0000ab00: 2c20 6e61 6d65 3d79 5f6e 616d 6529 0a20  , name=y_name). 
-0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2079 203d 205f 742e 5465 6e73 6f72 280a   y = _t.Tensor(.
+0000aab0: 2020 2020 2020 7920 3d20 6261 636b 656e        y = backen
+0000aac0: 642e 636f 6e76 6572 745f 746f 5f74 656e  d.convert_to_ten
+0000aad0: 736f 7228 782e 6469 6d65 6e73 696f 6e2c  sor(x.dimension,
+0000aae0: 2064 696d 733d 5b5d 2c20 6474 7970 653d   dims=[], dtype=
+0000aaf0: 7369 7a65 5f64 7479 7065 2c20 6e61 6d65  size_dtype, name
+0000ab00: 3d79 5f6e 616d 6529 0a20 2020 2020 2020  =y_name).       
+0000ab10: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000ab20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000ab30: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
+0000ab40: 742e 5465 6e73 6f72 280a 2020 2020 2020  t.Tensor(.      
 0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab60: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000ab70: 3d79 5f6e 616d 652c 0a20 2020 2020 2020  =y_name,.       
-0000ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab90: 2020 2020 2064 696d 5f74 6167 733d 5b5d       dim_tags=[]
-0000aba0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 6474                dt
-0000abc0: 7970 653d 7369 7a65 5f64 7479 7065 2c0a  ype=size_dtype,.
+0000ab60: 2020 2020 2020 6e61 6d65 3d79 5f6e 616d        name=y_nam
+0000ab70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000ab80: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000ab90: 696d 5f74 6167 733d 5b5d 2c0a 2020 2020  im_tags=[],.    
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abb0: 2020 2020 2020 2020 6474 7970 653d 7369          dtype=si
+0000abc0: 7a65 5f64 7479 7065 2c0a 2020 2020 2020  ze_dtype,.      
 0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abe0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 6966 206e 6f74 2074 656d 706c 6174    if not templat
-0000ac10: 655f 6f6e 6c79 2061 6e64 2074 663a 0a20  e_only and tf:. 
+0000abe0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000abf0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000ac00: 6f74 2074 656d 706c 6174 655f 6f6e 6c79  ot template_only
+0000ac10: 2061 6e64 2074 663a 0a20 2020 2020 2020   and tf:.       
 0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000ac40: 7466 2e63 6f6e 7472 6f6c 5f64 6570 656e  tf.control_depen
-0000ac50: 6465 6e63 6965 7328 4e6f 6e65 293a 2020  dencies(None):  
-0000ac60: 2320 7468 6973 2077 696c 6c20 7265 7365  # this will rese
-0000ac70: 7420 7468 6520 636f 6e74 6578 740a 2020  t the context.  
+0000ac30: 2020 2020 2077 6974 6820 7466 2e63 6f6e       with tf.con
+0000ac40: 7472 6f6c 5f64 6570 656e 6465 6e63 6965  trol_dependencie
+0000ac50: 7328 4e6f 6e65 293a 2020 2320 7468 6973  s(None):  # this
+0000ac60: 2077 696c 6c20 7265 7365 7420 7468 6520   will reset the 
+0000ac70: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
 0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 792e                y.
-0000aca0: 7261 775f 7465 6e73 6f72 203d 2074 662e  raw_tensor = tf.
-0000acb0: 636f 6e73 7461 6e74 2878 2e64 696d 656e  constant(x.dimen
-0000acc0: 7369 6f6e 290a 2020 2020 2020 2020 2020  sion).          
-0000acd0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0000ace0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-0000acf0: 2020 2069 6620 7466 3a0a 2020 2020 2020     if tf:.      
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 792e                y.
-0000ad10: 706c 6163 6568 6f6c 6465 7220 3d20 5f62  placeholder = _b
-0000ad20: 696e 5f6f 705f 7466 2879 2e70 6c61 6365  in_op_tf(y.place
-0000ad30: 686f 6c64 6572 2c20 782e 6469 6d65 6e73  holder, x.dimens
-0000ad40: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-0000ad50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0000ad70: 203d 205f 6269 6e5f 6f70 2879 2c20 782e   = _bin_op(y, x.
-0000ad80: 6469 6d65 6e73 696f 6e29 0a20 2020 2020  dimension).     
-0000ad90: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000ada0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-0000adb0: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0000add0: 203d 2078 2e67 6574 5f66 6f72 5f62 6174   = x.get_for_bat
-0000ade0: 6368 5f63 7478 2873 656c 662e 6261 7463  ch_ctx(self.batc
-0000adf0: 682c 2073 656c 662e 636f 6e74 726f 6c5f  h, self.control_
-0000ae00: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
-0000ae10: 2020 2020 2020 782e 636f 6d70 6c65 7465        x.complete
-0000ae20: 5f64 796e 5f73 697a 6528 7465 6d70 6c61  _dyn_size(templa
-0000ae30: 7465 5f6f 6e6c 793d 7465 6d70 6c61 7465  te_only=template
-0000ae40: 5f6f 6e6c 7929 0a20 2020 2020 2020 2020  _only).         
-0000ae50: 2020 2069 6620 6e6f 7420 782e 6479 6e5f     if not x.dyn_
-0000ae60: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-0000ae70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000ae80: 0a20 2020 2020 2020 2020 2020 2078 203d  .            x =
-0000ae90: 2078 2e64 796e 5f73 697a 655f 6578 740a   x.dyn_size_ext.
-0000aea0: 2020 2020 2020 2020 2020 2020 6966 2079              if y
-0000aeb0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000aec0: 2020 2020 2020 2020 2020 7920 3d20 782e            y = x.
-0000aed0: 636f 7079 286e 616d 653d 795f 6e61 6d65  copy(name=y_name
-0000aee0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000aef0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-0000af00: 2020 2020 2020 2069 6620 782e 6469 6d5f         if x.dim_
-0000af10: 7461 6773 2021 3d20 792e 6469 6d5f 7461  tags != y.dim_ta
-0000af20: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000af30: 2020 2020 636f 6d6d 6f6e 203d 205f 742e      common = _t.
-0000af40: 5465 6e73 6f72 2e67 6574 5f63 6f6d 6d6f  Tensor.get_commo
-0000af50: 6e5f 6461 7461 285b 782c 2079 5d2c 2061  n_data([x, y], a
-0000af60: 6c6c 6f77 5f62 726f 6164 6361 7374 5f61  llow_broadcast_a
-0000af70: 6c6c 5f73 6f75 7263 6573 3d54 7275 6529  ll_sources=True)
-0000af80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000af90: 2078 5f20 3d20 782e 636f 7079 5f63 6f6d   x_ = x.copy_com
-0000afa0: 7061 7469 626c 655f 746f 2863 6f6d 6d6f  patible_to(commo
-0000afb0: 6e29 2069 6620 782e 6469 6d5f 7461 6773  n) if x.dim_tags
-0000afc0: 2065 6c73 6520 780a 2020 2020 2020 2020   else x.        
-0000afd0: 2020 2020 2020 2020 795f 203d 2079 2e63          y_ = y.c
-0000afe0: 6f70 795f 636f 6d70 6174 6962 6c65 5f74  opy_compatible_t
-0000aff0: 6f28 636f 6d6d 6f6e 2920 6966 2079 2e64  o(common) if y.d
-0000b000: 696d 5f74 6167 7320 656c 7365 2079 0a20  im_tags else y. 
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0000b020: 203d 2063 6f6d 6d6f 6e0a 2020 2020 2020   = common.      
-0000b030: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000b040: 2020 2020 2020 2020 2020 2020 785f 2c20              x_, 
-0000b050: 795f 203d 2078 2c20 790a 2020 2020 2020  y_ = x, y.      
-0000b060: 2020 2020 2020 6966 2074 663a 0a20 2020        if tf:.   
-0000b070: 2020 2020 2020 2020 2020 2020 2079 2e70               y.p
-0000b080: 6c61 6365 686f 6c64 6572 203d 205f 6269  laceholder = _bi
-0000b090: 6e5f 6f70 5f74 6628 795f 2e70 6c61 6365  n_op_tf(y_.place
-0000b0a0: 686f 6c64 6572 2c20 785f 2e70 6c61 6365  holder, x_.place
-0000b0b0: 686f 6c64 6572 290a 2020 2020 2020 2020  holder).        
-0000b0c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000b0d0: 2020 2020 2020 2020 2020 7920 3d20 5f62            y = _b
-0000b0e0: 696e 5f6f 7028 795f 2c20 785f 290a 2020  in_op(y_, x_).  
-0000b0f0: 2020 2020 2020 6173 7365 7274 2079 2c20        assert y, 
-0000b100: 6622 6f70 207b 6f70 7d3f 220a 2020 2020  f"op {op}?".    
-0000b110: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
-0000b120: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-0000b130: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-0000b140: 662e 6479 6e5f 7369 7a65 5f65 7874 2e64  f.dyn_size_ext.d
-0000b150: 696d 5f74 6167 7320 3d3d 2079 2e64 696d  im_tags == y.dim
-0000b160: 5f74 6167 730a 2020 2020 2020 2020 6966  _tags.        if
-0000b170: 2079 2e62 6174 6368 3a0a 2020 2020 2020   y.batch:.      
-0000b180: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-0000b190: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
-0000b1a0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0000b1b0: 2e62 6174 6368 203d 3d20 792e 6261 7463  .batch == y.batc
-0000b1c0: 680a 2020 2020 2020 2020 2020 2020 656c  h.            el
-0000b1d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000b1e0: 2020 2020 7365 6c66 2e62 6174 6368 203d      self.batch =
-0000b1f0: 2079 2e62 6174 6368 0a20 2020 2020 2020   y.batch.       
-0000b200: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-0000b210: 7874 203d 2079 0a20 2020 2020 2020 2069  xt = y.        i
-0000b220: 6620 7466 2061 6e64 2079 2e70 6c61 6365  f tf and y.place
-0000b230: 686f 6c64 6572 2069 7320 6e6f 7420 4e6f  holder is not No
-0000b240: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b250: 7365 6c66 2e73 6574 5f74 6167 5f6f 6e5f  self.set_tag_on_
-0000b260: 7369 7a65 5f74 656e 736f 7228 792e 706c  size_tensor(y.pl
-0000b270: 6163 6568 6f6c 6465 7229 0a0a 2020 2020  aceholder)..    
-0000b280: 6465 6620 6973 5f65 7175 616c 280a 2020  def is_equal(.  
-0000b290: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000b2a0: 2020 2020 6f74 6865 722c 0a20 2020 2020      other,.     
-0000b2b0: 2020 2069 676e 6f72 655f 6665 6174 7572     ignore_featur
-0000b2c0: 655f 6469 6d3d 4661 6c73 652c 0a20 2020  e_dim=False,.   
-0000b2d0: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
-0000b2e0: 6665 6174 7572 655f 6469 6d3d 4661 6c73  feature_dim=Fals
-0000b2f0: 652c 0a20 2020 2020 2020 2061 6c6c 6f77  e,.        allow
-0000b300: 5f73 616d 655f 7370 6174 6961 6c5f 6469  _same_spatial_di
-0000b310: 6d3d 4e6f 6e65 2c0a 2020 2020 2020 2020  m=None,.        
-0000b320: 7472 6561 745f 6665 6174 7572 655f 6173  treat_feature_as
-0000b330: 5f73 7061 7469 616c 3d46 616c 7365 2c0a  _spatial=False,.
-0000b340: 2020 2020 2020 2020 6272 6f61 6463 6173          broadcas
-0000b350: 745f 6d61 7463 6865 733d 4661 6c73 652c  t_matches=False,
-0000b360: 0a20 2020 2020 2020 2075 6e6b 6e6f 776e  .        unknown
-0000b370: 5f73 7061 7469 616c 5f6d 6174 6368 6573  _spatial_matches
-0000b380: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000b390: 756e 6465 6669 6e65 645f 6d61 7463 6865  undefined_matche
-0000b3a0: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-0000b3b0: 2064 6572 6976 6564 5f6d 6174 6368 6573   derived_matches
-0000b3c0: 3d46 616c 7365 2c0a 2020 2020 293a 0a20  =False,.    ):. 
-0000b3d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000b3e0: 2020 2043 6f6d 7061 7265 7320 7365 6c66     Compares self
-0000b3f0: 2074 6f20 6f74 6865 7220 666f 7220 6571   to other for eq
-0000b400: 7561 6c69 7479 2e0a 0a20 2020 2020 2020  uality...       
-0000b410: 204e 6f74 6520 7468 6174 2074 6865 2064   Note that the d
-0000b420: 6566 6175 6c74 2062 6568 6176 696f 7220  efault behavior 
-0000b430: 6973 2076 6572 7920 7265 7374 7269 6374  is very restrict
-0000b440: 6976 652e 0a20 2020 2020 2020 2055 7365  ive..        Use
-0000b450: 2066 756e 6374 696f 6e73 2073 7563 6820   functions such 
-0000b460: 6173 203a 6675 6e63 3a60 6765 745f 616c  as :func:`get_al
-0000b470: 6c5f 6469 6d65 6e73 696f 6e5f 7461 6773  l_dimension_tags
-0000b480: 6020 6f72 203a 6675 6e63 3a60 6765 745f  ` or :func:`get_
-0000b490: 6578 6973 7469 6e67 5f74 6167 5f66 726f  existing_tag_fro
-0000b4a0: 6d5f 636f 6c6c 6563 7469 6f6e 600a 2020  m_collection`.  
-0000b4b0: 2020 2020 2020 746f 2065 7870 6c69 6369        to explici
-0000b4c0: 746c 7920 7370 6563 6966 7920 7468 6520  tly specify the 
-0000b4d0: 6265 6861 7669 6f72 2066 6f72 2074 6865  behavior for the
-0000b4e0: 2063 6f6d 7061 7269 736f 6e2e 0a0a 2020   comparison...  
-0000b4f0: 2020 2020 2020 416c 736f 206e 6f74 6520        Also note 
-0000b500: 7468 6174 2074 6865 2064 6566 696e 6974  that the definit
-0000b510: 696f 6e20 6973 2073 6c69 6768 746c 7920  ion is slightly 
-0000b520: 6164 2d68 6f63 2066 6f72 2073 6f6d 6520  ad-hoc for some 
-0000b530: 6361 7365 732c 0a20 2020 2020 2020 2061  cases,.        a
-0000b540: 6e64 206d 6967 6874 2070 6f74 656e 7469  nd might potenti
-0000b550: 616c 6c79 2063 6861 6e67 6520 696e 2074  ally change in t
-0000b560: 6865 2066 7574 7572 652e 0a20 2020 2020  he future..     
-0000b570: 2020 2020 2068 7474 7073 3a2f 2f67 6974       https://git
-0000b580: 6875 622e 636f 6d2f 7277 7468 2d69 362f  hub.com/rwth-i6/
-0000b590: 7265 7475 726e 6e2f 6973 7375 6573 2f36  returnn/issues/6
-0000b5a0: 3334 0a0a 2020 2020 2020 2020 3a70 6172  34..        :par
-0000b5b0: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
-0000b5c0: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
-0000b5d0: 6c20 6967 6e6f 7265 5f66 6561 7475 7265  l ignore_feature
-0000b5e0: 5f64 696d 3a0a 2020 2020 2020 2020 3a70  _dim:.        :p
-0000b5f0: 6172 616d 2062 6f6f 6c20 616c 6c6f 775f  aram bool allow_
-0000b600: 7361 6d65 5f66 6561 7475 7265 5f64 696d  same_feature_dim
-0000b610: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-0000b620: 2062 6f6f 6c7c 4e6f 6e65 2061 6c6c 6f77   bool|None allow
-0000b630: 5f73 616d 655f 7370 6174 6961 6c5f 6469  _same_spatial_di
-0000b640: 6d3a 0a20 2020 2020 2020 203a 7061 7261  m:.        :para
-0000b650: 6d20 626f 6f6c 2074 7265 6174 5f66 6561  m bool treat_fea
-0000b660: 7475 7265 5f61 735f 7370 6174 6961 6c3a  ture_as_spatial:
-0000b670: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000b680: 626f 6f6c 2062 726f 6164 6361 7374 5f6d  bool broadcast_m
-0000b690: 6174 6368 6573 3a0a 2020 2020 2020 2020  atches:.        
-0000b6a0: 3a70 6172 616d 2062 6f6f 6c20 756e 6b6e  :param bool unkn
-0000b6b0: 6f77 6e5f 7370 6174 6961 6c5f 6d61 7463  own_spatial_matc
-0000b6c0: 6865 733a 0a20 2020 2020 2020 203a 7061  hes:.        :pa
-0000b6d0: 7261 6d20 626f 6f6c 2075 6e64 6566 696e  ram bool undefin
-0000b6e0: 6564 5f6d 6174 6368 6573 3a0a 2020 2020  ed_matches:.    
-0000b6f0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-0000b700: 6465 7269 7665 645f 6d61 7463 6865 733a  derived_matches:
-0000b710: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-0000b720: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-0000b730: 220a 2020 2020 2020 2020 6672 6f6d 2072  ".        from r
-0000b740: 6574 7572 6e6e 2e75 7469 6c20 696d 706f  eturnn.util impo
-0000b750: 7274 2042 6568 6176 696f 7256 6572 7369  rt BehaviorVersi
-0000b760: 6f6e 0a0a 2020 2020 2020 2020 6966 2073  on..        if s
-0000b770: 656c 6620 6973 206f 7468 6572 3a20 2023  elf is other:  #
-0000b780: 2066 6972 7374 2073 6f6d 6520 6661 7374   first some fast
-0000b790: 2070 6174 6820 6368 6563 6b0a 2020 2020   path check.    
-0000b7a0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000b7b0: 7275 650a 2020 2020 2020 2020 6966 2073  rue.        if s
-0000b7c0: 656c 662e 7370 6563 6961 6c20 6f72 206f  elf.special or o
-0000b7d0: 7468 6572 2e73 7065 6369 616c 3a0a 2020  ther.special:.  
-0000b7e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000b7f0: 2046 616c 7365 2020 2320 6f6e 6c79 2074   False  # only t
-0000b800: 7275 6520 6966 2073 616d 6520 696e 7374  rue if same inst
-0000b810: 616e 6365 2c20 6368 6563 6b20 6162 6f76  ance, check abov
-0000b820: 650a 2020 2020 2020 2020 6966 2061 6c6c  e.        if all
-0000b830: 6f77 5f73 616d 655f 7370 6174 6961 6c5f  ow_same_spatial_
-0000b840: 6469 6d20 6973 204e 6f6e 653a 0a20 2020  dim is None:.   
-0000b850: 2020 2020 2020 2020 2061 6c6c 6f77 5f73           allow_s
-0000b860: 616d 655f 7370 6174 6961 6c5f 6469 6d20  ame_spatial_dim 
-0000b870: 3d20 616c 6c6f 775f 7361 6d65 5f66 6561  = allow_same_fea
-0000b880: 7475 7265 5f64 696d 0a20 2020 2020 2020  ture_dim.       
-0000b890: 2073 656c 665f 6261 7365 203d 2073 656c   self_base = sel
-0000b8a0: 662e 6765 745f 7361 6d65 5f64 6572 6976  f.get_same_deriv
-0000b8b0: 6564 5f62 6173 6528 7361 6d65 5f64 696d  ed_base(same_dim
-0000b8c0: 3d54 7275 6529 2069 6620 6465 7269 7665  =True) if derive
-0000b8d0: 645f 6d61 7463 6865 7320 656c 7365 2073  d_matches else s
-0000b8e0: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
-0000b8f0: 6528 290a 2020 2020 2020 2020 6f74 6865  e().        othe
-0000b900: 725f 6261 7365 203d 206f 7468 6572 2e67  r_base = other.g
-0000b910: 6574 5f73 616d 655f 6465 7269 7665 645f  et_same_derived_
-0000b920: 6261 7365 2873 616d 655f 6469 6d3d 5472  base(same_dim=Tr
-0000b930: 7565 2920 6966 2064 6572 6976 6564 5f6d  ue) if derived_m
-0000b940: 6174 6368 6573 2065 6c73 6520 6f74 6865  atches else othe
-0000b950: 722e 6765 745f 7361 6d65 5f62 6173 6528  r.get_same_base(
-0000b960: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000b970: 665f 6261 7365 2069 7320 6f74 6865 725f  f_base is other_
-0000b980: 6261 7365 3a0a 2020 2020 2020 2020 2020  base:.          
-0000b990: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000b9a0: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
-0000b9b0: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000b9c0: 6f70 2061 6e64 206f 7468 6572 5f62 6173  op and other_bas
-0000b9d0: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
-0000b9e0: 703a 0a20 2020 2020 2020 2020 2020 2069  p:.            i
-0000b9f0: 6620 7365 6c66 5f62 6173 652e 6465 7269  f self_base.deri
-0000ba00: 7665 645f 6672 6f6d 5f6f 7020 3d3d 206f  ved_from_op == o
-0000ba10: 7468 6572 5f62 6173 652e 6465 7269 7665  ther_base.derive
-0000ba20: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
-0000ba30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ba40: 6e20 5472 7565 0a20 2020 2020 2020 2073  n True.        s
-0000ba50: 656c 665f 6b69 6e64 203d 2073 656c 662e  elf_kind = self.
-0000ba60: 6b69 6e64 0a20 2020 2020 2020 206f 7468  kind.        oth
-0000ba70: 6572 5f6b 696e 6420 3d20 6f74 6865 722e  er_kind = other.
-0000ba80: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
-0000ba90: 7365 6c66 5f6b 696e 6420 3d3d 206f 7468  self_kind == oth
-0000baa0: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
-0000bab0: 7065 732e 4665 6174 7572 6520 616e 6420  pes.Feature and 
-0000bac0: 6967 6e6f 7265 5f66 6561 7475 7265 5f64  ignore_feature_d
-0000bad0: 696d 3a0a 2020 2020 2020 2020 2020 2020  im:.            
-0000bae0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000baf0: 2020 2020 6966 2074 7265 6174 5f66 6561      if treat_fea
-0000bb00: 7475 7265 5f61 735f 7370 6174 6961 6c3a  ture_as_spatial:
-0000bb10: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
-0000bb20: 6f74 653a 204e 6f20 6b69 6e64 2061 7420  ote: No kind at 
-0000bb30: 616c 6c3a 2052 6569 6e74 6572 7072 6574  all: Reinterpret
-0000bb40: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
-0000bb50: 735f 7370 6174 6961 6c20 6120 6269 743a  s_spatial a bit:
-0000bb60: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-0000bb70: 7373 756d 6520 7468 6174 2077 6520 7761  ssume that we wa
-0000bb80: 6e74 2074 6865 6d20 616c 6c20 746f 2062  nt them all to b
-0000bb90: 6520 6861 6e64 6c65 6420 7468 6520 7361  e handled the sa
-0000bba0: 6d65 2c20 6e6f 206d 6174 7465 7220 7468  me, no matter th
-0000bbb0: 6520 6b69 6e64 2e0a 2020 2020 2020 2020  e kind..        
-0000bbc0: 2020 2020 2320 2845 7863 6570 7420 6f66      # (Except of
-0000bbd0: 2062 6174 6368 2064 696d 206b 696e 642c   batch dim kind,
-0000bbe0: 2077 6869 6368 2069 7320 7374 696c 6c20   which is still 
-0000bbf0: 6578 636c 7564 6564 2068 6572 652e 290a  excluded here.).
-0000bc00: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000bc10: 656c 665f 6b69 6e64 203d 3d20 4469 6d54  elf_kind == DimT
-0000bc20: 7970 6573 2e46 6561 7475 7265 206f 7220  ypes.Feature or 
-0000bc30: 6e6f 7420 7365 6c66 5f6b 696e 643a 0a20  not self_kind:. 
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bc50: 656c 665f 6b69 6e64 203d 2044 696d 5479  elf_kind = DimTy
-0000bc60: 7065 732e 5370 6174 6961 6c0a 2020 2020  pes.Spatial.    
-0000bc70: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-0000bc80: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
-0000bc90: 732e 4665 6174 7572 6520 6f72 206e 6f74  s.Feature or not
-0000bca0: 206f 7468 6572 5f6b 696e 643a 0a20 2020   other_kind:.   
-0000bcb0: 2020 2020 2020 2020 2020 2020 206f 7468               oth
-0000bcc0: 6572 5f6b 696e 6420 3d20 4469 6d54 7970  er_kind = DimTyp
-0000bcd0: 6573 2e53 7061 7469 616c 0a20 2020 2020  es.Spatial.     
-0000bce0: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
-0000bcf0: 7369 6f6e 2021 3d20 6f74 6865 722e 6469  sion != other.di
-0000bd00: 6d65 6e73 696f 6e3a 0a20 2020 2020 2020  mension:.       
-0000bd10: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
-0000bd20: 745f 6d61 7463 6865 7320 616e 6420 2873  t_matches and (s
-0000bd30: 656c 662e 6469 6d65 6e73 696f 6e20 3d3d  elf.dimension ==
-0000bd40: 2031 206f 7220 6f74 6865 722e 6469 6d65   1 or other.dime
-0000bd50: 6e73 696f 6e20 3d3d 2031 293a 0a20 2020  nsion == 1):.   
-0000bd60: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-0000bd70: 7320 2023 2070 6173 7320 6f6e 0a20 2020  s  # pass on.   
-0000bd80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000bd90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bda0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0000bdb0: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
-0000bdc0: 2021 3d20 6f74 6865 725f 6b69 6e64 3a0a   != other_kind:.
-0000bdd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000bde0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0000bdf0: 2069 6620 7365 6c66 5f6b 696e 6420 3d3d   if self_kind ==
-0000be00: 206f 7468 6572 5f6b 696e 6420 3d3d 2044   other_kind == D
-0000be10: 696d 5479 7065 732e 4261 7463 683a 0a20  imTypes.Batch:. 
-0000be20: 2020 2020 2020 2020 2020 2023 204e 6f74             # Not
-0000be30: 653a 2054 6869 7320 6d69 6768 7420 6265  e: This might be
-0000be40: 2069 6e63 6f72 7265 6374 2069 6e20 736f   incorrect in so
-0000be50: 6d65 2063 6173 6573 2c0a 2020 2020 2020  me cases,.      
-0000be60: 2020 2020 2020 2320 652e 672e 2066 6f72        # e.g. for
-0000be70: 2062 6561 6d20 7365 6172 6368 2077 6865   beam search whe
-0000be80: 6e20 7765 2068 6176 6520 7468 6520 6265  n we have the be
-0000be90: 616d 2068 6964 6465 6e20 696e 2074 6865  am hidden in the
-0000bea0: 2062 6174 6368 2064 696d 2c0a 2020 2020   batch dim,.    
-0000beb0: 2020 2020 2020 2020 2320 6f72 2077 6865          # or whe
-0000bec0: 6e20 7765 2075 7365 6420 4d65 7267 6544  n we used MergeD
-0000bed0: 696d 734c 6179 6572 206f 6e20 7468 6520  imsLayer on the 
-0000bee0: 6261 7463 6820 6178 6973 2c20 6f72 2073  batch axis, or s
-0000bef0: 6f2e 0a20 2020 2020 2020 2020 2020 2023  o..            #
-0000bf00: 2057 6520 6d69 6768 7420 6e65 6564 2074   We might need t
-0000bf10: 6f20 6578 7465 6e64 2074 6865 206c 6f67  o extend the log
-0000bf20: 6963 2068 6572 6520 6c61 7465 722e 0a20  ic here later.. 
-0000bf30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000bf40: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
-0000bf50: 6620 4265 6861 7669 6f72 5665 7273 696f  f BehaviorVersio
-0000bf60: 6e2e 6765 7428 2920 3e3d 2031 363a 0a20  n.get() >= 16:. 
-0000bf70: 2020 2020 2020 2020 2020 2023 2045 6974             # Eit
-0000bf80: 6865 7220 7365 6c66 206f 7220 6f74 6865  her self or othe
-0000bf90: 7220 6973 2073 6f6d 6520 6469 6d20 7461  r is some dim ta
-0000bfa0: 6720 6578 706c 6963 6974 6c79 2063 7265  g explicitly cre
-0000bfb0: 6174 6564 2062 7920 7468 6520 7573 6572  ated by the user
-0000bfc0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-0000bfd0: 616e 6420 7468 6579 2061 7265 206e 6f74  and they are not
-0000bfe0: 2074 6865 2073 616d 652c 2073 6f20 7765   the same, so we
-0000bff0: 206e 6576 6572 2074 7265 6174 2074 6865   never treat the
-0000c000: 6d20 6173 2065 7175 616c 2e0a 2020 2020  m as equal..    
-0000c010: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000c020: 656c 662e 6175 746f 5f67 656e 6572 6174  elf.auto_generat
-0000c030: 6564 206f 7220 6e6f 7420 6f74 6865 722e  ed or not other.
-0000c040: 6175 746f 5f67 656e 6572 6174 6564 3a0a  auto_generated:.
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 6966 2062 726f 6164 6361 7374 5f6d 6174  if broadcast_mat
-0000c070: 6368 6573 2061 6e64 2028 0a20 2020 2020  ches and (.     
-0000c080: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000c090: 7365 6c66 2e64 696d 656e 7369 6f6e 203d  self.dimension =
-0000c0a0: 3d20 3120 616e 6420 7365 6c66 2e61 7574  = 1 and self.aut
-0000c0b0: 6f5f 6765 6e65 7261 7465 6429 206f 7220  o_generated) or 
-0000c0c0: 286f 7468 6572 2e64 696d 656e 7369 6f6e  (other.dimension
-0000c0d0: 203d 3d20 3120 616e 6420 6f74 6865 722e   == 1 and other.
-0000c0e0: 6175 746f 5f67 656e 6572 6174 6564 290a  auto_generated).
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c110: 2020 2020 2020 2070 6173 7320 2023 2065         pass  # e
-0000c120: 7863 6570 7469 6f6e 2c20 616c 6c6f 7720  xception, allow 
-0000c130: 6272 6f61 6463 6173 7420 6c6f 6769 630a  broadcast logic.
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000c160: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c170: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
-0000c180: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
-0000c190: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
-0000c1a0: 5479 7065 732e 4665 6174 7572 653a 0a20  Types.Feature:. 
-0000c1b0: 2020 2020 2020 2020 2020 2069 6620 616c             if al
-0000c1c0: 6c6f 775f 7361 6d65 5f66 6561 7475 7265  low_same_feature
-0000c1d0: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
-0000c1e0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000c1f0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000c200: 665f 6b69 6e64 203d 3d20 6f74 6865 725f  f_kind == other_
-0000c210: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
-0000c220: 2e53 7061 7469 616c 3a0a 2020 2020 2020  .Spatial:.      
-0000c230: 2020 2020 2020 6966 2061 6c6c 6f77 5f73        if allow_s
-0000c240: 616d 655f 7370 6174 6961 6c5f 6469 6d3a  ame_spatial_dim:
-0000c250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c260: 2069 6620 7365 6c66 2e64 696d 656e 7369   if self.dimensi
-0000c270: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-0000c280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c290: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2b0: 6966 2062 726f 6164 6361 7374 5f6d 6174  if broadcast_mat
-0000c2c0: 6368 6573 2061 6e64 2028 7365 6c66 2e64  ches and (self.d
-0000c2d0: 696d 656e 7369 6f6e 203d 3d20 3120 6f72  imension == 1 or
-0000c2e0: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-0000c2f0: 203d 3d20 3129 3a0a 2020 2020 2020 2020   == 1):.        
-0000c300: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c310: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000c320: 2020 2020 6966 2075 6e6b 6e6f 776e 5f73      if unknown_s
-0000c330: 7061 7469 616c 5f6d 6174 6368 6573 2061  patial_matches a
-0000c340: 6e64 2028 2873 656c 662e 6479 6e5f 7369  nd ((self.dyn_si
-0000c350: 7a65 2069 7320 4e6f 6e65 2920 6f72 2028  ze is None) or (
-0000c360: 6f74 6865 722e 6479 6e5f 7369 7a65 2069  other.dyn_size i
-0000c370: 7320 4e6f 6e65 2929 3a0a 2020 2020 2020  s None)):.      
-0000c380: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c390: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000c3a0: 2020 6966 2075 6e64 6566 696e 6564 5f6d    if undefined_m
-0000c3b0: 6174 6368 6573 2061 6e64 2028 7365 6c66  atches and (self
-0000c3c0: 2e75 6e64 6566 696e 6564 206f 7220 6f74  .undefined or ot
-0000c3d0: 6865 722e 756e 6465 6669 6e65 6429 3a0a  her.undefined):.
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000c400: 2020 2020 2320 496e 2070 7269 6e63 6970      # In princip
-0000c410: 6c65 2c20 7765 2077 6f75 6c64 2077 616e  le, we would wan
-0000c420: 7420 746f 2063 6865 636b 2066 6f72 2069  t to check for i
-0000c430: 6465 6e74 6974 7920 2873 656c 6620 6973  dentity (self is
-0000c440: 206f 7468 6572 292e 0a20 2020 2020 2020   other)..       
-0000c450: 2023 2057 6520 6375 7272 656e 746c 7920   # We currently 
-0000c460: 7573 6520 7468 6520 6465 7363 7269 7074  use the descript
-0000c470: 696f 6e20 6265 6361 7573 6520 7468 6520  ion because the 
-0000c480: 6964 656e 7469 7479 2077 6f75 6c64 206e  identity would n
-0000c490: 6f74 2062 6520 7468 6520 7361 6d65 0a20  ot be the same. 
-0000c4a0: 2020 2020 2020 2023 2069 6e20 6361 7365         # in case
-0000c4b0: 206f 6620 7465 6d70 6c61 7465 2063 6f6e   of template con
-0000c4c0: 7374 7275 6374 696f 6e20 7768 6572 6520  struction where 
-0000c4d0: 6120 6469 6d20 7461 6720 6973 206f 6e63  a dim tag is onc
-0000c4e0: 6520 6372 6561 7465 6420 666f 7220 6120  e created for a 
-0000c4f0: 7465 6d70 6c61 7465 206c 6179 6572 2c0a  template layer,.
-0000c500: 2020 2020 2020 2020 2320 616e 6420 7468          # and th
-0000c510: 656e 206c 6174 6572 2061 6761 696e 2066  en later again f
-0000c520: 6f72 2074 6865 2072 6561 6c20 6c61 7965  or the real laye
-0000c530: 722e 0a20 2020 2020 2020 2069 6620 7365  r..        if se
-0000c540: 6c66 2e61 7574 6f5f 6765 6e65 7261 7465  lf.auto_generate
-0000c550: 6420 616e 6420 6f74 6865 722e 6175 746f  d and other.auto
-0000c560: 5f67 656e 6572 6174 6564 2061 6e64 2073  _generated and s
-0000c570: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-0000c580: 3d3d 206f 7468 6572 2e64 6573 6372 6970  == other.descrip
-0000c590: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-0000c5a0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000c5b0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000c5c0: 7365 0a0a 2020 2020 6465 6620 5f5f 6571  se..    def __eq
-0000c5d0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-0000c5e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c5f0: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-0000c600: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-0000c610: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-0000c620: 2020 2020 3a72 6574 7572 6e3a 203a 6675      :return: :fu
-0000c630: 6e63 3a60 6973 5f65 7175 616c 6020 7769  nc:`is_equal` wi
-0000c640: 7468 2064 6566 6175 6c74 206f 7074 696f  th default optio
-0000c650: 6e73 0a20 2020 2020 2020 2022 2222 0a20  ns.        """. 
-0000c660: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0000c670: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
-0000c680: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
-0000c690: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0000c6a0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000c6b0: 2073 656c 662e 6973 5f65 7175 616c 286f   self.is_equal(o
-0000c6c0: 7468 6572 290a 0a20 2020 2064 6566 205f  ther)..    def _
-0000c6d0: 5f6e 655f 5f28 7365 6c66 3a20 4469 6d2c  _ne__(self: Dim,
-0000c6e0: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
-0000c6f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c700: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
-0000c710: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
-0000c720: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-0000c730: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000c740: 7572 6e20 6e6f 7420 2873 656c 6620 3d3d  urn not (self ==
-0000c750: 206f 7468 6572 290a 0a20 2020 2064 6566   other)..    def
-0000c760: 205f 5f68 6173 685f 5f28 7365 6c66 293a   __hash__(self):
-0000c770: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c780: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-0000c790: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000c7a0: 3a20 6861 7368 2c20 6d61 7463 6869 6e67  : hash, matching
-0000c7b0: 2074 6f20 3a66 756e 633a 605f 5f65 715f   to :func:`__eq_
-0000c7c0: 5f60 0a20 2020 2020 2020 2022 2222 0a20  _`.        """. 
-0000c7d0: 2020 2020 2020 2023 2054 6869 7320 6d75         # This mu
-0000c7e0: 7374 206d 6174 6368 2074 6865 2062 6568  st match the beh
-0000c7f0: 6176 696f 7220 696e 205f 5f65 715f 5f2c  avior in __eq__,
-0000c800: 2077 6869 6368 2069 7320 6973 5f65 7175   which is is_equ
-0000c810: 616c 2077 6974 6820 6465 6661 756c 7420  al with default 
-0000c820: 6f70 7469 6f6e 732e 0a20 2020 2020 2020  options..       
-0000c830: 2023 2049 2e65 2e20 6469 6666 6572 656e   # I.e. differen
-0000c840: 7420 6861 7368 2069 6d70 6c69 6573 206e  t hash implies n
-0000c850: 6f74 2065 7175 616c 2028 6275 7420 7361  ot equal (but sa
-0000c860: 6d65 2068 6173 6820 6e6f 7420 6e65 6365  me hash not nece
-0000c870: 7373 6172 696c 7920 6571 7561 6c29 2e0a  ssarily equal)..
-0000c880: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c890: 7370 6563 6961 6c3a 0a20 2020 2020 2020  special:.       
-0000c8a0: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
-0000c8b0: 2869 6428 7365 6c66 2929 0a20 2020 2020  (id(self)).     
-0000c8c0: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
-0000c8d0: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
-0000c8e0: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
-0000c8f0: 7368 2828 2929 0a20 2020 2020 2020 2077  sh(()).        w
-0000c900: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
-0000c910: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
-0000c920: 6e28 5f64 2e44 696d 2e5f 5f68 6173 685f  n(_d.Dim.__hash_
-0000c930: 5f2c 2073 656c 6629 3a0a 2020 2020 2020  _, self):.      
-0000c940: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
-0000c950: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
-0000c960: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000c970: 2062 6173 6520 6973 206e 6f74 2073 656c   base is not sel
-0000c980: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-0000c990: 2020 2072 6574 7572 6e20 6861 7368 2862     return hash(b
-0000c9a0: 6173 6529 0a20 2020 2020 2020 2020 2020  ase).           
-0000c9b0: 2069 6620 7365 6c66 2e64 6572 6976 6564   if self.derived
-0000c9c0: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-0000c9d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c9e0: 2068 6173 6828 7365 6c66 2e64 6572 6976   hash(self.deriv
-0000c9f0: 6564 5f66 726f 6d5f 6f70 290a 2020 2020  ed_from_op).    
-0000ca00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ca10: 6175 746f 5f67 656e 6572 6174 6564 3a0a  auto_generated:.
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 7265 7475 726e 2068 6173 6828 2862 6173  return hash((bas
-0000ca40: 652e 6b69 6e64 2c20 6261 7365 2e64 696d  e.kind, base.dim
-0000ca50: 656e 7369 6f6e 2c20 6261 7365 2e64 6573  ension, base.des
-0000ca60: 6372 6970 7469 6f6e 2929 0a20 2020 2020  cription)).     
-0000ca70: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
-0000ca80: 7368 2869 6428 6261 7365 2929 0a0a 2020  sh(id(base))..  
-0000ca90: 2020 6465 6620 5f5f 6c74 5f5f 2873 656c    def __lt__(sel
-0000caa0: 663a 2044 696d 2c20 6f74 6865 723a 2044  f: Dim, other: D
-0000cab0: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
-0000cac0: 0a20 2020 2020 2020 2044 6566 696e 6520  .        Define 
-0000cad0: 736f 6d65 206f 7264 6572 2e20 5468 6973  some order. This
-0000cae0: 2069 7320 6a75 7374 2073 7563 6820 7468   is just such th
-0000caf0: 6174 2060 736f 7274 6564 6020 776f 726b  at `sorted` work
-0000cb00: 732c 206f 7220 736f 6d65 2064 6966 6620  s, or some diff 
-0000cb10: 7265 706f 7274 696e 672c 206f 7220 736f  reporting, or so
-0000cb20: 2e0a 2020 2020 2020 2020 4974 2069 7320  ..        It is 
-0000cb30: 6f6e 2073 796d 626f 6c69 6320 6c65 7665  on symbolic leve
-0000cb40: 6c2c 2069 2e65 2e20 6974 2064 6f65 7320  l, i.e. it does 
-0000cb50: 6e6f 7420 636f 6e73 6964 6572 2074 6865  not consider the
-0000cb60: 2061 6374 7561 6c20 6469 6d65 6e73 696f   actual dimensio
-0000cb70: 6e20 7661 6c75 652e 0a20 2020 2020 2020  n value..       
-0000cb80: 2054 6865 2064 6566 696e 6564 206f 7264   The defined ord
-0000cb90: 6572 2073 6f6d 6577 6861 7420 6172 6269  er somewhat arbi
-0000cba0: 7472 6172 792c 2073 6f20 646f 206e 6f74  trary, so do not
-0000cbb0: 2072 656c 7920 6f6e 2074 6865 2065 7861   rely on the exa
-0000cbc0: 6374 2062 6568 6176 696f 722c 0a20 2020  ct behavior,.   
-0000cbd0: 2020 2020 2061 7320 7468 6973 206d 6967       as this mig
-0000cbe0: 6874 2063 6861 6e67 6520 6174 2073 6f6d  ht change at som
-0000cbf0: 6520 6c61 7465 7220 706f 696e 742e 0a20  e later point.. 
-0000cc00: 2020 2020 2020 2043 7572 7265 6e74 6c79         Currently
-0000cc10: 2c20 6974 2064 6570 656e 6473 206f 6e20  , it depends on 
-0000cc20: 7468 6520 6372 6561 7469 6f6e 2069 6e64  the creation ind
-0000cc30: 6578 2e0a 0a20 2020 2020 2020 203a 7061  ex...        :pa
-0000cc40: 7261 6d20 4469 6d20 6f74 6865 723a 0a20  ram Dim other:. 
-0000cc50: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-0000cc60: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-0000cc70: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0000cc80: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-0000cc90: 2028 5f64 2e44 696d 2c20 5f6d 2e4d 6172   (_d.Dim, _m.Mar
-0000cca0: 6b65 6444 696d 2929 3a0a 2020 2020 2020  kedDim)):.      
-0000ccb0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-0000ccc0: 4572 726f 7228 2263 616e 6e6f 7420 636f  Error("cannot co
-0000ccd0: 6d70 6172 6520 2572 2077 6974 6820 2572  mpare %r with %r
-0000cce0: 2220 2520 2873 656c 662c 206f 7468 6572  " % (self, other
-0000ccf0: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
-0000cd00: 6c66 203d 3d20 6f74 6865 723a 0a20 2020  lf == other:.   
-0000cd10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000cd20: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
-0000cd30: 7475 726e 2064 696d 5f63 6d70 5f76 616c  turn dim_cmp_val
-0000cd40: 7565 2873 656c 6629 203c 2064 696d 5f63  ue(self) < dim_c
-0000cd50: 6d70 5f76 616c 7565 286f 7468 6572 290a  mp_value(other).
-0000cd60: 0a20 2020 2064 6566 205f 5f67 745f 5f28  .    def __gt__(
-0000cd70: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-0000cd80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000cd90: 2020 5365 6520 3a66 756e 633a 605f 5f6c    See :func:`__l
-0000cda0: 745f 5f60 2e0a 0a20 2020 2020 2020 203a  t__`...        :
-0000cdb0: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
-0000cdc0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-0000cdd0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-0000cde0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000cdf0: 206f 7468 6572 203c 2073 656c 660a 0a20   other < self.. 
-0000ce00: 2020 2064 6566 205f 5f67 655f 5f28 7365     def __ge__(se
-0000ce10: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-0000ce20: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
-0000ce30: 656c 6620 3c20 6f74 6865 720a 0a20 2020  elf < other..   
-0000ce40: 2064 6566 205f 5f6c 655f 5f28 7365 6c66   def __le__(self
-0000ce50: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-0000ce60: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
-0000ce70: 6620 3e20 6f74 6865 720a 0a20 2020 2064  f > other..    d
-0000ce80: 6566 2067 6574 5f73 616d 655f 6261 7365  ef get_same_base
-0000ce90: 2873 656c 663a 205f 642e 4469 6d29 202d  (self: _d.Dim) -
-0000cea0: 3e20 5f64 2e44 696d 3a0a 2020 2020 2020  > _d.Dim:.      
-0000ceb0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-0000cec0: 6574 7572 6e3a 2073 616d 6520 6261 7365  eturn: same base
-0000ced0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000cee0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0000cef0: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
-0000cf00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000cf10: 0a20 2020 2020 2020 2062 6173 6520 3d20  .        base = 
-0000cf20: 7365 6c66 0a20 2020 2020 2020 2077 6869  self.        whi
-0000cf30: 6c65 2062 6173 652e 7361 6d65 5f61 733a  le base.same_as:
-0000cf40: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-0000cf50: 6520 3d20 6261 7365 2e73 616d 655f 6173  e = base.same_as
-0000cf60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cf70: 6261 7365 0a0a 2020 2020 6465 6620 6765  base..    def ge
-0000cf80: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
-0000cf90: 6173 6528 7365 6c66 3a20 5f64 2e44 696d  ase(self: _d.Dim
-0000cfa0: 2c20 2a2c 2073 616d 655f 6469 6d3a 2062  , *, same_dim: b
-0000cfb0: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
-0000cfc0: 5f64 2e44 696d 3a0a 2020 2020 2020 2020  _d.Dim:.        
-0000cfd0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-0000cfe0: 616d 2073 616d 655f 6469 6d3a 2069 6620  am same_dim: if 
-0000cff0: 5472 7565 2c20 7265 7475 726e 2074 6865  True, return the
-0000d000: 206c 6173 7420 6261 7365 2077 6869 6368   last base which
-0000d010: 2068 6173 2074 6865 2073 616d 6520 6469   has the same di
-0000d020: 6d65 6e73 696f 6e2e 0a20 2020 2020 2020  mension..       
-0000d030: 2020 2020 2054 6865 2064 6572 6976 6564       The derived
-0000d040: 2062 6173 6520 6d69 6768 7420 6861 7665   base might have
-0000d050: 2061 2064 6966 6665 7265 6e74 2064 696d   a different dim
-0000d060: 656e 7369 6f6e 2e0a 2020 2020 2020 2020  ension..        
-0000d070: 2020 2020 496e 2063 6173 6520 6974 2069      In case it i
-0000d080: 7320 6479 6e61 6d69 632c 2074 6865 2064  s dynamic, the d
-0000d090: 696d 656e 7369 6f6e 2069 7320 4e6f 6e65  imension is None
-0000d0a0: 2c20 736f 2069 7420 6973 2061 6c77 6179  , so it is alway
-0000d0b0: 7320 7468 6520 7361 6d65 2e0a 2020 2020  s the same..    
-0000d0c0: 2020 2020 2020 2020 496e 2063 6173 6520          In case 
-0000d0d0: 6974 2069 7320 7374 6174 6963 2c20 7468  it is static, th
-0000d0e0: 6572 6520 6d69 6768 7420 6265 2061 2064  ere might be a d
-0000d0f0: 6966 6665 7265 6e74 2064 696d 656e 7369  ifferent dimensi
-0000d100: 6f6e 2e0a 2020 2020 2020 2020 3a72 6574  on..        :ret
-0000d110: 7572 6e3a 2073 616d 6520 6261 7365 2c20  urn: same base, 
-0000d120: 6275 7420 616c 736f 2063 6f6e 7369 6465  but also conside
-0000d130: 7220 6465 7269 7665 645f 6672 6f6d 5f2e  r derived_from_.
-0000d140: 2e2e 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-0000d150: 2020 2020 2020 206c 6173 745f 6261 7365         last_base
-0000d160: 5f73 656c 665f 6469 6d20 3d20 7365 6c66  _self_dim = self
-0000d170: 0a20 2020 2020 2020 2062 6173 6520 3d20  .        base = 
-0000d180: 7365 6c66 0a20 2020 2020 2020 2076 6973  self.        vis
-0000d190: 6974 6564 203d 207b 7d0a 2020 2020 2020  ited = {}.      
-0000d1a0: 2020 7768 696c 6520 6261 7365 2e73 616d    while base.sam
-0000d1b0: 655f 6173 206f 7220 6261 7365 2e64 6572  e_as or base.der
-0000d1c0: 6976 6564 5f66 726f 6d5f 7461 673a 0a20  ived_from_tag:. 
-0000d1d0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000d1e0: 7420 6964 2862 6173 6529 206e 6f74 2069  t id(base) not i
-0000d1f0: 6e20 7669 7369 7465 6420 2023 2073 686f  n visited  # sho
-0000d200: 756c 6420 6e6f 7420 6861 7665 2063 7963  uld not have cyc
-0000d210: 6c65 732e 206e 6f72 6d61 6c6c 7920 7468  les. normally th
-0000d220: 6973 2073 686f 756c 6420 6e65 7665 7220  is should never 
-0000d230: 6265 2074 7269 6767 6572 6564 0a20 2020  be triggered.   
-0000d240: 2020 2020 2020 2020 2076 6973 6974 6564           visited
-0000d250: 5b69 6428 6261 7365 295d 203d 2062 6173  [id(base)] = bas
-0000d260: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-0000d270: 2062 6173 652e 7361 6d65 5f61 733a 0a20   base.same_as:. 
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000d290: 6173 6520 3d20 6261 7365 2e73 616d 655f  ase = base.same_
-0000d2a0: 6173 0a20 2020 2020 2020 2020 2020 2020  as.             
-0000d2b0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000d2c0: 2020 2020 2020 2020 6261 7365 203d 2062          base = b
-0000d2d0: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-0000d2e0: 5f74 6167 0a20 2020 2020 2020 2020 2020  _tag.           
-0000d2f0: 2061 7373 6572 7420 6261 7365 0a20 2020   assert base.   
-0000d300: 2020 2020 2020 2020 2069 6620 6261 7365           if base
-0000d310: 2e64 696d 656e 7369 6f6e 203d 3d20 7365  .dimension == se
-0000d320: 6c66 2e64 696d 656e 7369 6f6e 3a0a 2020  lf.dimension:.  
-0000d330: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0000d340: 7374 5f62 6173 655f 7365 6c66 5f64 696d  st_base_self_dim
-0000d350: 203d 2062 6173 650a 2020 2020 2020 2020   = base.        
-0000d360: 7265 7475 726e 206c 6173 745f 6261 7365  return last_base
-0000d370: 5f73 656c 665f 6469 6d20 6966 2073 616d  _self_dim if sam
-0000d380: 655f 6469 6d20 656c 7365 2062 6173 650a  e_dim else base.
-0000d390: 0a20 2020 2064 6566 2067 6574 5f64 6572  .    def get_der
-0000d3a0: 6976 6564 5f62 6173 6573 5f73 6574 2873  ived_bases_set(s
-0000d3b0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000d3c0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-0000d3d0: 3a20 7365 745b 4469 6d5d 0a20 2020 2020  : set[Dim].     
-0000d3e0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000d3f0: 6573 203d 2073 6574 2829 0a20 2020 2020  es = set().     
-0000d400: 2020 2071 7565 7565 203d 205b 7365 6c66     queue = [self
-0000d410: 5d0a 2020 2020 2020 2020 7669 7369 7465  ].        visite
-0000d420: 6420 3d20 7b7d 2020 2320 7479 7065 3a20  d = {}  # type: 
-0000d430: 4469 6374 5b69 6e74 2c5f 642e 4469 6d5d  Dict[int,_d.Dim]
-0000d440: 2020 2320 6279 2069 640a 2020 2020 2020    # by id.      
-0000d450: 2020 7768 696c 6520 7175 6575 653a 0a20    while queue:. 
-0000d460: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0000d470: 3d20 7175 6575 652e 706f 7028 2d31 290a  = queue.pop(-1).
-0000d480: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000d490: 6173 652e 7361 6d65 5f61 733a 0a20 2020  ase.same_as:.   
-0000d4a0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-0000d4b0: 6520 3d20 6261 7365 2e73 616d 655f 6173  e = base.same_as
-0000d4c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d4d0: 6964 2862 6173 6529 2069 6e20 7669 7369  id(base) in visi
-0000d4e0: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-0000d4f0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-0000d500: 2020 2020 2020 2020 2020 7669 7369 7465            visite
-0000d510: 645b 6964 2862 6173 6529 5d20 3d20 6261  d[id(base)] = ba
-0000d520: 7365 0a20 2020 2020 2020 2020 2020 2072  se.            r
-0000d530: 6573 2e61 6464 2862 6173 6529 0a20 2020  es.add(base).   
-0000d540: 2020 2020 2020 2020 2069 6620 6261 7365           if base
-0000d550: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-0000d560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d570: 2020 7175 6575 652e 6578 7465 6e64 2862    queue.extend(b
-0000d580: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-0000d590: 5f6f 702e 696e 7075 7473 290a 2020 2020  _op.inputs).    
-0000d5a0: 2020 2020 2020 2020 656c 6966 2062 6173          elif bas
-0000d5b0: 652e 6465 7269 7665 645f 6672 6f6d 5f74  e.derived_from_t
-0000d5c0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
-0000d5d0: 2020 2020 7175 6575 652e 6170 7065 6e64      queue.append
-0000d5e0: 2862 6173 652e 6465 7269 7665 645f 6672  (base.derived_fr
-0000d5f0: 6f6d 5f74 6167 290a 2020 2020 2020 2020  om_tag).        
-0000d600: 7265 7475 726e 2072 6573 0a0a 2020 2020  return res..    
-0000d610: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000d620: 6620 756e 6465 6669 6e65 6428 7365 6c66  f undefined(self
-0000d630: 3a20 5f64 2e44 696d 2920 2d3e 2062 6f6f  : _d.Dim) -> boo
-0000d640: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-0000d650: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-0000d660: 7768 6574 6865 7220 7468 6520 756e 6465  whether the unde
-0000d670: 6669 6e65 6420 666c 6167 2069 7320 7365  fined flag is se
-0000d680: 742c 2069 6e20 7365 6c66 2c20 6261 7365  t, in self, base
-0000d690: 732c 206f 7220 616e 7920 6465 7269 7665  s, or any derive
-0000d6a0: 6420 6261 7365 732e 2061 6c73 6f20 7365  d bases. also se
-0000d6b0: 6520 3a66 756e 633a 6069 735f 6469 6d5f  e :func:`is_dim_
-0000d6c0: 6b6e 6f77 6e60 0a20 2020 2020 2020 2022  known`.        "
-0000d6d0: 2222 0a20 2020 2020 2020 2062 6173 6520  "".        base 
-0000d6e0: 3d20 7365 6c66 0a20 2020 2020 2020 2076  = self.        v
-0000d6f0: 6973 6974 6564 203d 207b 7d0a 2020 2020  isited = {}.    
-0000d700: 2020 2020 7768 696c 6520 6261 7365 2e73      while base.s
-0000d710: 616d 655f 6173 206f 7220 6261 7365 2e64  ame_as or base.d
-0000d720: 6572 6976 6564 5f66 726f 6d5f 7461 673a  erived_from_tag:
-0000d730: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000d740: 6572 7420 6964 2862 6173 6529 206e 6f74  ert id(base) not
-0000d750: 2069 6e20 7669 7369 7465 6420 2023 2073   in visited  # s
-0000d760: 686f 756c 6420 6e6f 7420 6861 7665 2063  hould not have c
-0000d770: 7963 6c65 732e 206e 6f72 6d61 6c6c 7920  ycles. normally 
-0000d780: 7468 6973 2073 686f 756c 6420 6e65 7665  this should neve
-0000d790: 7220 6265 2074 7269 6767 6572 6564 0a20  r be triggered. 
-0000d7a0: 2020 2020 2020 2020 2020 2076 6973 6974             visit
-0000d7b0: 6564 5b69 6428 6261 7365 295d 203d 2062  ed[id(base)] = b
-0000d7c0: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
-0000d7d0: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-0000d7e0: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-0000d7f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d800: 6261 7365 2e5f 6578 7472 6120 616e 6420  base._extra and 
-0000d810: 6261 7365 2e5f 6578 7472 612e 756e 6465  base._extra.unde
-0000d820: 6669 6e65 643a 0a20 2020 2020 2020 2020  fined:.         
-0000d830: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000d840: 7565 0a20 2020 2020 2020 2020 2020 2069  ue.            i
-0000d850: 6620 6261 7365 2e73 616d 655f 6173 3a0a  f base.same_as:.
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 6261 7365 203d 2062 6173 652e 7361 6d65  base = base.same
-0000d880: 5f61 730a 2020 2020 2020 2020 2020 2020  _as.            
-0000d890: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-0000d8a0: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000d8b0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
-0000d8c0: 6d5f 7461 670a 2020 2020 2020 2020 2020  m_tag.          
-0000d8d0: 2020 6173 7365 7274 2062 6173 650a 2020    assert base.  
-0000d8e0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000d8f0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000d900: 4d65 6d62 6572 0a20 2020 2020 2020 2072  Member.        r
-0000d910: 6574 7572 6e20 6261 7365 2e5f 6578 7472  eturn base._extr
-0000d920: 6120 616e 6420 6261 7365 2e5f 6578 7472  a and base._extr
-0000d930: 612e 756e 6465 6669 6e65 640a 0a20 2020  a.undefined..   
-0000d940: 2064 6566 2064 6563 6c61 7265 5f73 616d   def declare_sam
-0000d950: 655f 6173 2873 656c 663a 205f 642e 4469  e_as(self: _d.Di
-0000d960: 6d2c 206f 7468 6572 3a20 5f64 2e44 696d  m, other: _d.Dim
-0000d970: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000d980: 2020 2020 2020 203a 7061 7261 6d20 6f74         :param ot
-0000d990: 6865 723a 0a20 2020 2020 2020 2022 2222  her:.        """
-0000d9a0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000d9b0: 7365 6c66 2e63 616e 5f62 655f 7573 6564  self.can_be_used
-0000d9c0: 5f61 735f 6469 6d28 2920 616e 6420 6f74  _as_dim() and ot
-0000d9d0: 6865 722e 6361 6e5f 6265 5f75 7365 645f  her.can_be_used_
-0000d9e0: 6173 5f64 696d 2829 2020 2320 6465 636c  as_dim()  # decl
-0000d9f0: 6172 655f 7361 6d65 5f61 7320 646f 6573  are_same_as does
-0000da00: 206e 6f74 206d 616b 6520 7365 6e73 6520   not make sense 
-0000da10: 6f74 6865 7277 6973 650a 2020 2020 2020  otherwise.      
-0000da20: 2020 2320 4e6f 7465 3a20 4368 6563 6b20    # Note: Check 
-0000da30: 6069 7360 2c20 6e6f 7420 603d 3d60 2e20  `is`, not `==`. 
-0000da40: 603d 3d60 2063 616e 2062 6520 7472 7565  `==` can be true
-0000da50: 2065 7665 6e20 7468 6f75 6768 2073 616d   even though sam
-0000da60: 655f 6173 2061 7265 206e 6f74 2074 6865  e_as are not the
-0000da70: 2073 616d 6520 696e 7374 616e 6365 2c0a   same instance,.
-0000da80: 2020 2020 2020 2020 2320 652e 672e 2076          # e.g. v
-0000da90: 6961 2061 7574 6f5f 6765 6e65 7261 7465  ia auto_generate
-0000daa0: 642e 0a20 2020 2020 2020 2069 6620 7365  d..        if se
-0000dab0: 6c66 2069 7320 6f74 6865 723a 0a20 2020  lf is other:.   
-0000dac0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000dad0: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
-0000dae0: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
-0000daf0: 2020 2020 2073 656c 662e 5f76 616c 6964       self._valid
-0000db00: 6174 655f 696e 5f63 7572 7265 6e74 5f67  ate_in_current_g
-0000db10: 7261 7068 2829 0a20 2020 2020 2020 206f  raph().        o
-0000db20: 7468 6572 2e5f 7661 6c69 6461 7465 5f69  ther._validate_i
-0000db30: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
-0000db40: 290a 2020 2020 2020 2020 6f74 6865 725f  ).        other_
-0000db50: 7361 6d65 5f62 6173 6520 3d20 6f74 6865  same_base = othe
-0000db60: 722e 6765 745f 7361 6d65 5f62 6173 6528  r.get_same_base(
-0000db70: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000db80: 6620 6973 206f 7468 6572 5f73 616d 655f  f is other_same_
-0000db90: 6261 7365 206f 7220 7365 6c66 2e73 616d  base or self.sam
-0000dba0: 655f 6173 2069 7320 6f74 6865 725f 7361  e_as is other_sa
-0000dbb0: 6d65 5f62 6173 653a 0a20 2020 2020 2020  me_base:.       
-0000dbc0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000dbd0: 2020 2020 7365 6c66 5f73 616d 655f 6173      self_same_as
-0000dbe0: 203d 2073 656c 662e 6765 745f 7361 6d65   = self.get_same
-0000dbf0: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
-0000dc00: 6966 2073 656c 665f 7361 6d65 5f61 7320  if self_same_as 
-0000dc10: 6973 206f 7468 6572 5f73 616d 655f 6261  is other_same_ba
-0000dc20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000dc30: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000dc40: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
-0000dc50: 652e 6765 745f 7361 6d65 5f64 6572 6976  e.get_same_deriv
-0000dc60: 6564 5f62 6173 6528 2920 6973 2073 656c  ed_base() is sel
-0000dc70: 665f 7361 6d65 5f61 733a 0a20 2020 2020  f_same_as:.     
-0000dc80: 2020 2020 2020 2023 2057 6520 6163 7475         # We actu
-0000dc90: 616c 6c79 2077 616e 7420 6974 2074 6f20  ally want it to 
-0000dca0: 6265 2074 6865 206f 7468 6572 2077 6179  be the other way
-0000dcb0: 2061 726f 756e 642e 0a20 2020 2020 2020   around..       
-0000dcc0: 2020 2020 2077 6974 6820 7574 696c 2e67       with util.g
-0000dcd0: 7561 7264 5f69 6e66 696e 6974 655f 7265  uard_infinite_re
-0000dce0: 6375 7273 696f 6e28 5f64 2e44 696d 2e64  cursion(_d.Dim.d
-0000dcf0: 6563 6c61 7265 5f73 616d 655f 6173 2c20  eclare_same_as, 
-0000dd00: 6f74 6865 722c 2073 656c 6629 3a0a 2020  other, self):.  
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000dd20: 7475 726e 206f 7468 6572 2e64 6563 6c61  turn other.decla
-0000dd30: 7265 5f73 616d 655f 6173 2873 656c 6629  re_same_as(self)
-0000dd40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000dd50: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
-0000dd60: 2020 2020 2320 4966 2073 656c 6620 6973      # If self is
-0000dd70: 2064 6566 696e 6564 2028 7365 6c66 2e69   defined (self.i
-0000dd80: 735f 6469 6d5f 6b6e 6f77 6e29 2c20 6265  s_dim_known), be
-0000dd90: 2066 6169 7220 746f 206f 7468 6572 2c20   fair to other, 
-0000dda0: 616e 6420 6164 6170 7420 6974 2074 6f20  and adapt it to 
-0000ddb0: 7468 6520 7269 6768 7420 6261 7463 682c  the right batch,
-0000ddc0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-0000ddd0: 7563 6820 7468 6174 206f 7468 6572 2e69  uch that other.i
-0000dde0: 735f 6469 6d5f 6b6e 6f77 6e20 6973 2063  s_dim_known is c
-0000ddf0: 6f72 7265 6374 2c20 6279 2070 6f74 656e  orrect, by poten
-0000de00: 7469 616c 6c79 2063 6f6d 706c 6574 696e  tially completin
-0000de10: 6720 6974 2e0a 2020 2020 2020 2020 2020  g it..          
-0000de20: 2020 6f74 6865 725f 203d 206f 7468 6572    other_ = other
-0000de30: 2e67 6574 5f66 6f72 5f62 6174 6368 5f63  .get_for_batch_c
-0000de40: 7478 2873 656c 662e 6261 7463 682c 2063  tx(self.batch, c
-0000de50: 7478 3d73 656c 662e 636f 6e74 726f 6c5f  tx=self.control_
-0000de60: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
-0000de70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000de80: 2020 2020 6f74 6865 725f 203d 206f 7468      other_ = oth
-0000de90: 6572 0a20 2020 2020 2020 2069 6620 280a  er.        if (.
-0000dea0: 2020 2020 2020 2020 2020 2020 2873 656c              (sel
-0000deb0: 662e 6973 5f64 696d 5f6b 6e6f 776e 2829  f.is_dim_known()
-0000dec0: 2061 6e64 206e 6f74 206f 7468 6572 5f2e   and not other_.
-0000ded0: 6973 5f64 696d 5f6b 6e6f 776e 2829 290a  is_dim_known()).
-0000dee0: 2020 2020 2020 2020 2020 2020 6f72 0a20              or. 
-0000def0: 2020 2020 2020 2020 2020 2023 204c 696b             # Lik
-0000df00: 6520 6973 5f64 696d 5f6b 6e6f 776e 2062  e is_dim_known b
-0000df10: 7574 2066 6f72 2073 7461 7469 6320 6469  ut for static di
-0000df20: 6d73 2c20 7765 206d 6967 6874 206b 6e6f  ms, we might kno
-0000df30: 7720 626f 7468 2c0a 2020 2020 2020 2020  w both,.        
-0000df40: 2020 2020 2320 6275 7420 7468 6520 6465      # but the de
-0000df50: 7269 7665 645f 6672 6f6d 5f6f 7020 7374  rived_from_op st
-0000df60: 696c 6c20 776f 756c 6420 7072 6f76 6964  ill would provid
-0000df70: 6520 6d6f 7265 2069 6e66 6f72 6d61 7469  e more informati
-0000df80: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000df90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000dfa0: 2020 7365 6c66 5f73 616d 655f 6173 2e64    self_same_as.d
-0000dfb0: 6572 6976 6564 5f66 726f 6d5f 6f70 0a20  erived_from_op. 
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000dfd0: 6e64 206e 6f74 206f 7468 6572 5f73 616d  nd not other_sam
-0000dfe0: 655f 6261 7365 2e64 6572 6976 6564 5f66  e_base.derived_f
-0000dff0: 726f 6d5f 6f70 0a20 2020 2020 2020 2020  rom_op.         
-0000e000: 2020 2020 2020 2061 6e64 206f 7468 6572         and other
-0000e010: 206e 6f74 2069 6e20 7365 6c66 2e67 6574   not in self.get
-0000e020: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
-0000e030: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
-0000e040: 2029 0a20 2020 2020 2020 2020 2020 206f   ).            o
-0000e050: 7220 286e 6f74 2073 656c 662e 756e 6465  r (not self.unde
-0000e060: 6669 6e65 6420 616e 6420 6f74 6865 725f  fined and other_
-0000e070: 2e75 6e64 6566 696e 6564 290a 2020 2020  .undefined).    
-0000e080: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-0000e090: 2020 2077 6974 6820 7574 696c 2e67 7561     with util.gua
-0000e0a0: 7264 5f69 6e66 696e 6974 655f 7265 6375  rd_infinite_recu
-0000e0b0: 7273 696f 6e28 5f64 2e44 696d 2e64 6563  rsion(_d.Dim.dec
-0000e0c0: 6c61 7265 5f73 616d 655f 6173 2c20 6f74  lare_same_as, ot
-0000e0d0: 6865 722c 2073 656c 6629 3a0a 2020 2020  her, self):.    
-0000e0e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e0f0: 726e 206f 7468 6572 2e64 6563 6c61 7265  rn other.declare
-0000e100: 5f73 616d 655f 6173 2873 656c 6629 0a20  _same_as(self). 
-0000e110: 2020 2020 2020 206f 7468 6572 5f64 6572         other_der
-0000e120: 6976 6564 5f62 6173 6573 203d 206f 7468  ived_bases = oth
-0000e130: 6572 2e67 6574 5f64 6572 6976 6564 5f62  er.get_derived_b
-0000e140: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
-0000e150: 2020 2073 656c 665f 6465 7269 7665 645f     self_derived_
-0000e160: 6261 7365 7320 3d20 7365 6c66 2e67 6574  bases = self.get
-0000e170: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
-0000e180: 6574 2829 0a20 2020 2020 2020 2069 6620  et().        if 
-0000e190: 6f74 6865 725f 6465 7269 7665 645f 6261  other_derived_ba
-0000e1a0: 7365 7320 213d 2073 656c 665f 6465 7269  ses != self_deri
-0000e1b0: 7665 645f 6261 7365 7320 616e 6420 7365  ved_bases and se
-0000e1c0: 6c66 5f64 6572 6976 6564 5f62 6173 6573  lf_derived_bases
-0000e1d0: 2e69 7373 7562 7365 7428 6f74 6865 725f  .issubset(other_
-0000e1e0: 6465 7269 7665 645f 6261 7365 7329 3a0a  derived_bases):.
-0000e1f0: 2020 2020 2020 2020 2020 2020 2320 4176              # Av
-0000e200: 6f69 6420 6379 636c 6573 206f 6e20 6465  oid cycles on de
-0000e210: 7269 7665 645f 6672 6f6d 5f74 6167 2e20  rived_from_tag. 
-0000e220: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000e230: 6f6d 2f72 7774 682d 6936 2f72 6574 7572  om/rwth-i6/retur
-0000e240: 6e6e 2f69 7373 7565 732f 3130 3534 0a20  nn/issues/1054. 
-0000e250: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000e260: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
-0000e270: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
-0000e280: 2e44 696d 2e64 6563 6c61 7265 5f73 616d  .Dim.declare_sam
-0000e290: 655f 6173 2c20 6f74 6865 722c 2073 656c  e_as, other, sel
-0000e2a0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-0000e2b0: 2020 2020 7265 7475 726e 206f 7468 6572      return other
-0000e2c0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
-0000e2d0: 2873 656c 6629 0a20 2020 2020 2020 2069  (self).        i
-0000e2e0: 6620 7365 6c66 2e5f 6578 7472 613a 0a20  f self._extra:. 
-0000e2f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e300: 5f65 7874 7261 2e64 6572 6976 6564 5f66  _extra.derived_f
-0000e310: 726f 6d5f 6f70 203d 204e 6f6e 650a 2020  rom_op = None.  
-0000e320: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e330: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
-0000e340: 6f6d 5f74 6167 203d 204e 6f6e 650a 2020  om_tag = None.  
-0000e350: 2020 2020 2020 6966 2073 656c 665f 7361        if self_sa
-0000e360: 6d65 5f61 7320 6973 206e 6f74 2073 656c  me_as is not sel
-0000e370: 663a 0a20 2020 2020 2020 2020 2020 2061  f:.            a
-0000e380: 7373 6572 7420 6e6f 7420 7365 6c66 5f73  ssert not self_s
-0000e390: 616d 655f 6173 2e73 616d 655f 6173 0a20  ame_as.same_as. 
-0000e3a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e3b0: 6c66 5f73 616d 655f 6173 2069 7320 6f74  lf_same_as is ot
-0000e3c0: 6865 725f 7361 6d65 5f62 6173 653a 0a20  her_same_base:. 
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e3e0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000e3f0: 2020 7769 7468 2075 7469 6c2e 6775 6172    with util.guar
-0000e400: 645f 696e 6669 6e69 7465 5f72 6563 7572  d_infinite_recur
-0000e410: 7369 6f6e 285f 642e 4469 6d2e 6465 636c  sion(_d.Dim.decl
-0000e420: 6172 655f 7361 6d65 5f61 732c 2073 656c  are_same_as, sel
-0000e430: 665f 7361 6d65 5f61 732c 206f 7468 6572  f_same_as, other
-0000e440: 5f73 616d 655f 6261 7365 293a 0a20 2020  _same_base):.   
-0000e450: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e460: 665f 7361 6d65 5f61 732e 6465 636c 6172  f_same_as.declar
-0000e470: 655f 7361 6d65 5f61 7328 6f74 6865 725f  e_same_as(other_
-0000e480: 7361 6d65 5f62 6173 6529 0a20 2020 2020  same_base).     
-0000e490: 2020 2020 2020 2069 6620 2873 656c 662e         if (self.
-0000e4a0: 6479 6e5f 7369 7a65 5f65 7874 2069 7320  dyn_size_ext is 
-0000e4b0: 4e6f 6e65 206f 7220 6e6f 7420 7365 6c66  None or not self
-0000e4c0: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
-0000e4d0: 7272 656e 745f 6772 6170 6828 2929 2061  rrent_graph()) a
-0000e4e0: 6e64 2073 656c 665f 7361 6d65 5f61 732e  nd self_same_as.
-0000e4f0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-0000e500: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e510: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
-0000e520: 3d20 7365 6c66 5f73 616d 655f 6173 2e67  = self_same_as.g
-0000e530: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
-0000e540: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e560: 2020 2073 656c 662e 6261 7463 682c 2073     self.batch, s
-0000e570: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000e580: 5f63 7478 2c20 7465 6d70 6c61 7465 5f6f  _ctx, template_o
-0000e590: 6e6c 793d 5472 7565 0a20 2020 2020 2020  nly=True.       
-0000e5a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e5b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e5c0: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
-0000e5d0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
-0000e5e0: 2020 2020 2066 6f72 2064 696d 5f20 696e       for dim_ in
-0000e5f0: 2073 656c 662e 5f65 7874 7261 2e73 616d   self._extra.sam
-0000e600: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
-0000e610: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000e630: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-0000e640: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 2020 2069 6620 6469 6d5f 2e5f 6578 7472     if dim_._extr
-0000e670: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-0000e680: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
-0000e690: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-0000e6a0: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6c0: 2020 2020 6469 6d5f 2e5f 6578 7472 612e      dim_._extra.
-0000e6d0: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000e6e0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000e700: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-0000e710: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+0000ac90: 2020 2020 2020 2020 792e 7261 775f 7465          y.raw_te
+0000aca0: 6e73 6f72 203d 2074 662e 636f 6e73 7461  nsor = tf.consta
+0000acb0: 6e74 2878 2e64 696d 656e 7369 6f6e 290a  nt(x.dimension).
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acd0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+0000ace0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000acf0: 7466 3a0a 2020 2020 2020 2020 2020 2020  tf:.            
+0000ad00: 2020 2020 2020 2020 792e 706c 6163 6568          y.placeh
+0000ad10: 6f6c 6465 7220 3d20 5f62 696e 5f6f 705f  older = _bin_op_
+0000ad20: 7466 2879 2e70 6c61 6365 686f 6c64 6572  tf(y.placeholder
+0000ad30: 2c20 782e 6469 6d65 6e73 696f 6e29 0a20  , x.dimension). 
+0000ad40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000ad50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000ad60: 2020 2020 2020 2020 2079 203d 205f 6269           y = _bi
+0000ad70: 6e5f 6f70 2879 2c20 782e 6469 6d65 6e73  n_op(y, x.dimens
+0000ad80: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+0000ad90: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+0000ada0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000adb0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
+0000adc0: 2020 2020 2020 2020 2078 203d 2078 2e67           x = x.g
+0000add0: 6574 5f66 6f72 5f62 6174 6368 5f63 7478  et_for_batch_ctx
+0000ade0: 2873 656c 662e 6261 7463 682c 2073 656c  (self.batch, sel
+0000adf0: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+0000ae00: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
+0000ae10: 782e 636f 6d70 6c65 7465 5f64 796e 5f73  x.complete_dyn_s
+0000ae20: 697a 6528 7465 6d70 6c61 7465 5f6f 6e6c  ize(template_onl
+0000ae30: 793d 7465 6d70 6c61 7465 5f6f 6e6c 7929  y=template_only)
+0000ae40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000ae50: 6e6f 7420 782e 6479 6e5f 7369 7a65 5f65  not x.dyn_size_e
+0000ae60: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000ae70: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000ae80: 2020 2020 2020 2078 203d 2078 2e64 796e         x = x.dyn
+0000ae90: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
+0000aea0: 2020 2020 2020 6966 2079 2069 7320 4e6f        if y is No
+0000aeb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000aec0: 2020 2020 7920 3d20 782e 636f 7079 286e      y = x.copy(n
+0000aed0: 616d 653d 795f 6e61 6d65 290a 2020 2020  ame=y_name).    
+0000aee0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000aef0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000af00: 2069 6620 782e 6469 6d5f 7461 6773 2021   if x.dim_tags !
+0000af10: 3d20 792e 6469 6d5f 7461 6773 3a0a 2020  = y.dim_tags:.  
+0000af20: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000af30: 6d6d 6f6e 203d 205f 742e 5465 6e73 6f72  mmon = _t.Tensor
+0000af40: 2e67 6574 5f63 6f6d 6d6f 6e5f 6461 7461  .get_common_data
+0000af50: 285b 782c 2079 5d2c 2061 6c6c 6f77 5f62  ([x, y], allow_b
+0000af60: 726f 6164 6361 7374 5f61 6c6c 5f73 6f75  roadcast_all_sou
+0000af70: 7263 6573 3d54 7275 6529 0a20 2020 2020  rces=True).     
+0000af80: 2020 2020 2020 2020 2020 2078 5f20 3d20             x_ = 
+0000af90: 782e 636f 7079 5f63 6f6d 7061 7469 626c  x.copy_compatibl
+0000afa0: 655f 746f 2863 6f6d 6d6f 6e29 2069 6620  e_to(common) if 
+0000afb0: 782e 6469 6d5f 7461 6773 2065 6c73 6520  x.dim_tags else 
+0000afc0: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+0000afd0: 2020 795f 203d 2079 2e63 6f70 795f 636f    y_ = y.copy_co
+0000afe0: 6d70 6174 6962 6c65 5f74 6f28 636f 6d6d  mpatible_to(comm
+0000aff0: 6f6e 2920 6966 2079 2e64 696d 5f74 6167  on) if y.dim_tag
+0000b000: 7320 656c 7365 2079 0a20 2020 2020 2020  s else y.       
+0000b010: 2020 2020 2020 2020 2079 203d 2063 6f6d           y = com
+0000b020: 6d6f 6e0a 2020 2020 2020 2020 2020 2020  mon.            
+0000b030: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b040: 2020 2020 2020 785f 2c20 795f 203d 2078        x_, y_ = x
+0000b050: 2c20 790a 2020 2020 2020 2020 2020 2020  , y.            
+0000b060: 6966 2074 663a 0a20 2020 2020 2020 2020  if tf:.         
+0000b070: 2020 2020 2020 2079 2e70 6c61 6365 686f         y.placeho
+0000b080: 6c64 6572 203d 205f 6269 6e5f 6f70 5f74  lder = _bin_op_t
+0000b090: 6628 795f 2e70 6c61 6365 686f 6c64 6572  f(y_.placeholder
+0000b0a0: 2c20 785f 2e70 6c61 6365 686f 6c64 6572  , x_.placeholder
+0000b0b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000b0c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000b0d0: 2020 2020 7920 3d20 5f62 696e 5f6f 7028      y = _bin_op(
+0000b0e0: 795f 2c20 785f 290a 2020 2020 2020 2020  y_, x_).        
+0000b0f0: 6173 7365 7274 2079 2c20 6622 6f70 207b  assert y, f"op {
+0000b100: 6f70 7d3f 220a 2020 2020 2020 2020 6966  op}?".        if
+0000b110: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+0000b120: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000b130: 6173 7365 7274 2073 656c 662e 6479 6e5f  assert self.dyn_
+0000b140: 7369 7a65 5f65 7874 2e64 696d 5f74 6167  size_ext.dim_tag
+0000b150: 7320 3d3d 2079 2e64 696d 5f74 6167 730a  s == y.dim_tags.
+0000b160: 2020 2020 2020 2020 6966 2079 2e62 6174          if y.bat
+0000b170: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+0000b180: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000b1a0: 7373 6572 7420 7365 6c66 2e62 6174 6368  ssert self.batch
+0000b1b0: 203d 3d20 792e 6261 7463 680a 2020 2020   == y.batch.    
+0000b1c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b1e0: 6c66 2e62 6174 6368 203d 2079 2e62 6174  lf.batch = y.bat
+0000b1f0: 6368 0a20 2020 2020 2020 2073 656c 662e  ch.        self.
+0000b200: 6479 6e5f 7369 7a65 5f65 7874 203d 2079  dyn_size_ext = y
+0000b210: 0a20 2020 2020 2020 2069 6620 7466 2061  .        if tf a
+0000b220: 6e64 2079 2e70 6c61 6365 686f 6c64 6572  nd y.placeholder
+0000b230: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000b240: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000b250: 6574 5f74 6167 5f6f 6e5f 7369 7a65 5f74  et_tag_on_size_t
+0000b260: 656e 736f 7228 792e 706c 6163 6568 6f6c  ensor(y.placehol
+0000b270: 6465 7229 0a0a 2020 2020 6465 6620 6973  der)..    def is
+0000b280: 5f65 7175 616c 280a 2020 2020 2020 2020  _equal(.        
+0000b290: 7365 6c66 2c0a 2020 2020 2020 2020 6f74  self,.        ot
+0000b2a0: 6865 722c 0a20 2020 2020 2020 2069 676e  her,.        ign
+0000b2b0: 6f72 655f 6665 6174 7572 655f 6469 6d3d  ore_feature_dim=
+0000b2c0: 4661 6c73 652c 0a20 2020 2020 2020 2061  False,.        a
+0000b2d0: 6c6c 6f77 5f73 616d 655f 6665 6174 7572  llow_same_featur
+0000b2e0: 655f 6469 6d3d 4661 6c73 652c 0a20 2020  e_dim=False,.   
+0000b2f0: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
+0000b300: 7370 6174 6961 6c5f 6469 6d3d 4e6f 6e65  spatial_dim=None
+0000b310: 2c0a 2020 2020 2020 2020 7472 6561 745f  ,.        treat_
+0000b320: 6665 6174 7572 655f 6173 5f73 7061 7469  feature_as_spati
+0000b330: 616c 3d46 616c 7365 2c0a 2020 2020 2020  al=False,.      
+0000b340: 2020 6272 6f61 6463 6173 745f 6d61 7463    broadcast_matc
+0000b350: 6865 733d 4661 6c73 652c 0a20 2020 2020  hes=False,.     
+0000b360: 2020 2075 6e6b 6e6f 776e 5f73 7061 7469     unknown_spati
+0000b370: 616c 5f6d 6174 6368 6573 3d46 616c 7365  al_matches=False
+0000b380: 2c0a 2020 2020 2020 2020 756e 6465 6669  ,.        undefi
+0000b390: 6e65 645f 6d61 7463 6865 733d 4661 6c73  ned_matches=Fals
+0000b3a0: 652c 0a20 2020 2020 2020 2064 6572 6976  e,.        deriv
+0000b3b0: 6564 5f6d 6174 6368 6573 3d46 616c 7365  ed_matches=False
+0000b3c0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0000b3d0: 2022 2222 0a20 2020 2020 2020 2043 6f6d   """.        Com
+0000b3e0: 7061 7265 7320 7365 6c66 2074 6f20 6f74  pares self to ot
+0000b3f0: 6865 7220 666f 7220 6571 7561 6c69 7479  her for equality
+0000b400: 2e0a 0a20 2020 2020 2020 204e 6f74 6520  ...        Note 
+0000b410: 7468 6174 2074 6865 2064 6566 6175 6c74  that the default
+0000b420: 2062 6568 6176 696f 7220 6973 2076 6572   behavior is ver
+0000b430: 7920 7265 7374 7269 6374 6976 652e 0a20  y restrictive.. 
+0000b440: 2020 2020 2020 2055 7365 2066 756e 6374         Use funct
+0000b450: 696f 6e73 2073 7563 6820 6173 203a 6675  ions such as :fu
+0000b460: 6e63 3a60 6765 745f 616c 6c5f 6469 6d65  nc:`get_all_dime
+0000b470: 6e73 696f 6e5f 7461 6773 6020 6f72 203a  nsion_tags` or :
+0000b480: 6675 6e63 3a60 6765 745f 6578 6973 7469  func:`get_existi
+0000b490: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
+0000b4a0: 6563 7469 6f6e 600a 2020 2020 2020 2020  ection`.        
+0000b4b0: 746f 2065 7870 6c69 6369 746c 7920 7370  to explicitly sp
+0000b4c0: 6563 6966 7920 7468 6520 6265 6861 7669  ecify the behavi
+0000b4d0: 6f72 2066 6f72 2074 6865 2063 6f6d 7061  or for the compa
+0000b4e0: 7269 736f 6e2e 0a0a 2020 2020 2020 2020  rison...        
+0000b4f0: 416c 736f 206e 6f74 6520 7468 6174 2074  Also note that t
+0000b500: 6865 2064 6566 696e 6974 696f 6e20 6973  he definition is
+0000b510: 2073 6c69 6768 746c 7920 6164 2d68 6f63   slightly ad-hoc
+0000b520: 2066 6f72 2073 6f6d 6520 6361 7365 732c   for some cases,
+0000b530: 0a20 2020 2020 2020 2061 6e64 206d 6967  .        and mig
+0000b540: 6874 2070 6f74 656e 7469 616c 6c79 2063  ht potentially c
+0000b550: 6861 6e67 6520 696e 2074 6865 2066 7574  hange in the fut
+0000b560: 7572 652e 0a20 2020 2020 2020 2020 2068  ure..          h
+0000b570: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000b580: 6d2f 7277 7468 2d69 362f 7265 7475 726e  m/rwth-i6/return
+0000b590: 6e2f 6973 7375 6573 2f36 3334 0a0a 2020  n/issues/634..  
+0000b5a0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+0000b5b0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+0000b5c0: 3a70 6172 616d 2062 6f6f 6c20 6967 6e6f  :param bool igno
+0000b5d0: 7265 5f66 6561 7475 7265 5f64 696d 3a0a  re_feature_dim:.
+0000b5e0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+0000b5f0: 6f6f 6c20 616c 6c6f 775f 7361 6d65 5f66  ool allow_same_f
+0000b600: 6561 7475 7265 5f64 696d 3a0a 2020 2020  eature_dim:.    
+0000b610: 2020 2020 3a70 6172 616d 2062 6f6f 6c7c      :param bool|
+0000b620: 4e6f 6e65 2061 6c6c 6f77 5f73 616d 655f  None allow_same_
+0000b630: 7370 6174 6961 6c5f 6469 6d3a 0a20 2020  spatial_dim:.   
+0000b640: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+0000b650: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
+0000b660: 735f 7370 6174 6961 6c3a 0a20 2020 2020  s_spatial:.     
+0000b670: 2020 203a 7061 7261 6d20 626f 6f6c 2062     :param bool b
+0000b680: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
+0000b690: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+0000b6a0: 2062 6f6f 6c20 756e 6b6e 6f77 6e5f 7370   bool unknown_sp
+0000b6b0: 6174 6961 6c5f 6d61 7463 6865 733a 0a20  atial_matches:. 
+0000b6c0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+0000b6d0: 6f6c 2075 6e64 6566 696e 6564 5f6d 6174  ol undefined_mat
+0000b6e0: 6368 6573 3a0a 2020 2020 2020 2020 3a70  ches:.        :p
+0000b6f0: 6172 616d 2062 6f6f 6c20 6465 7269 7665  aram bool derive
+0000b700: 645f 6d61 7463 6865 733a 0a20 2020 2020  d_matches:.     
+0000b710: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+0000b720: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b730: 2020 2020 6672 6f6d 2072 6574 7572 6e6e      from returnn
+0000b740: 2e75 7469 6c20 696d 706f 7274 2042 6568  .util import Beh
+0000b750: 6176 696f 7256 6572 7369 6f6e 0a0a 2020  aviorVersion..  
+0000b760: 2020 2020 2020 6966 2073 656c 6620 6973        if self is
+0000b770: 206f 7468 6572 3a20 2023 2066 6972 7374   other:  # first
+0000b780: 2073 6f6d 6520 6661 7374 2070 6174 6820   some fast path 
+0000b790: 6368 6563 6b0a 2020 2020 2020 2020 2020  check.          
+0000b7a0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b7b0: 2020 2020 2020 6966 2073 656c 662e 7370        if self.sp
+0000b7c0: 6563 6961 6c20 6f72 206f 7468 6572 2e73  ecial or other.s
+0000b7d0: 7065 6369 616c 3a0a 2020 2020 2020 2020  pecial:.        
+0000b7e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0000b7f0: 2020 2320 6f6e 6c79 2074 7275 6520 6966    # only true if
+0000b800: 2073 616d 6520 696e 7374 616e 6365 2c20   same instance, 
+0000b810: 6368 6563 6b20 6162 6f76 650a 2020 2020  check above.    
+0000b820: 2020 2020 6966 2061 6c6c 6f77 5f73 616d      if allow_sam
+0000b830: 655f 7370 6174 6961 6c5f 6469 6d20 6973  e_spatial_dim is
+0000b840: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000b850: 2020 2061 6c6c 6f77 5f73 616d 655f 7370     allow_same_sp
+0000b860: 6174 6961 6c5f 6469 6d20 3d20 616c 6c6f  atial_dim = allo
+0000b870: 775f 7361 6d65 5f66 6561 7475 7265 5f64  w_same_feature_d
+0000b880: 696d 0a20 2020 2020 2020 2073 656c 665f  im.        self_
+0000b890: 6261 7365 203d 2073 656c 662e 6765 745f  base = self.get_
+0000b8a0: 7361 6d65 5f64 6572 6976 6564 5f62 6173  same_derived_bas
+0000b8b0: 6528 7361 6d65 5f64 696d 3d54 7275 6529  e(same_dim=True)
+0000b8c0: 2069 6620 6465 7269 7665 645f 6d61 7463   if derived_matc
+0000b8d0: 6865 7320 656c 7365 2073 656c 662e 6765  hes else self.ge
+0000b8e0: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
+0000b8f0: 2020 2020 2020 6f74 6865 725f 6261 7365        other_base
+0000b900: 203d 206f 7468 6572 2e67 6574 5f73 616d   = other.get_sam
+0000b910: 655f 6465 7269 7665 645f 6261 7365 2873  e_derived_base(s
+0000b920: 616d 655f 6469 6d3d 5472 7565 2920 6966  ame_dim=True) if
+0000b930: 2064 6572 6976 6564 5f6d 6174 6368 6573   derived_matches
+0000b940: 2065 6c73 6520 6f74 6865 722e 6765 745f   else other.get_
+0000b950: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
+0000b960: 2020 2020 6966 2073 656c 665f 6261 7365      if self_base
+0000b970: 2069 7320 6f74 6865 725f 6261 7365 3a0a   is other_base:.
+0000b980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b990: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000b9a0: 6966 2073 656c 665f 6261 7365 2e64 6572  if self_base.der
+0000b9b0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
+0000b9c0: 206f 7468 6572 5f62 6173 652e 6465 7269   other_base.deri
+0000b9d0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+0000b9e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b9f0: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
+0000ba00: 6f6d 5f6f 7020 3d3d 206f 7468 6572 5f62  om_op == other_b
+0000ba10: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+0000ba20: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
+0000ba30: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0000ba40: 0a20 2020 2020 2020 2073 656c 665f 6b69  .        self_ki
+0000ba50: 6e64 203d 2073 656c 662e 6b69 6e64 0a20  nd = self.kind. 
+0000ba60: 2020 2020 2020 206f 7468 6572 5f6b 696e         other_kin
+0000ba70: 6420 3d20 6f74 6865 722e 6b69 6e64 0a20  d = other.kind. 
+0000ba80: 2020 2020 2020 2069 6620 7365 6c66 5f6b         if self_k
+0000ba90: 696e 6420 3d3d 206f 7468 6572 5f6b 696e  ind == other_kin
+0000baa0: 6420 3d3d 2044 696d 5479 7065 732e 4665  d == DimTypes.Fe
+0000bab0: 6174 7572 6520 616e 6420 6967 6e6f 7265  ature and ignore
+0000bac0: 5f66 6561 7475 7265 5f64 696d 3a0a 2020  _feature_dim:.  
+0000bad0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000bae0: 2054 7275 650a 2020 2020 2020 2020 6966   True.        if
+0000baf0: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
+0000bb00: 735f 7370 6174 6961 6c3a 0a20 2020 2020  s_spatial:.     
+0000bb10: 2020 2020 2020 2023 204e 6f74 653a 204e         # Note: N
+0000bb20: 6f20 6b69 6e64 2061 7420 616c 6c3a 2052  o kind at all: R
+0000bb30: 6569 6e74 6572 7072 6574 2074 7265 6174  einterpret treat
+0000bb40: 5f66 6561 7475 7265 5f61 735f 7370 6174  _feature_as_spat
+0000bb50: 6961 6c20 6120 6269 743a 0a20 2020 2020  ial a bit:.     
+0000bb60: 2020 2020 2020 2023 2041 7373 756d 6520         # Assume 
+0000bb70: 7468 6174 2077 6520 7761 6e74 2074 6865  that we want the
+0000bb80: 6d20 616c 6c20 746f 2062 6520 6861 6e64  m all to be hand
+0000bb90: 6c65 6420 7468 6520 7361 6d65 2c20 6e6f  led the same, no
+0000bba0: 206d 6174 7465 7220 7468 6520 6b69 6e64   matter the kind
+0000bbb0: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000bbc0: 2845 7863 6570 7420 6f66 2062 6174 6368  (Except of batch
+0000bbd0: 2064 696d 206b 696e 642c 2077 6869 6368   dim kind, which
+0000bbe0: 2069 7320 7374 696c 6c20 6578 636c 7564   is still exclud
+0000bbf0: 6564 2068 6572 652e 290a 2020 2020 2020  ed here.).      
+0000bc00: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
+0000bc10: 6e64 203d 3d20 4469 6d54 7970 6573 2e46  nd == DimTypes.F
+0000bc20: 6561 7475 7265 206f 7220 6e6f 7420 7365  eature or not se
+0000bc30: 6c66 5f6b 696e 643a 0a20 2020 2020 2020  lf_kind:.       
+0000bc40: 2020 2020 2020 2020 2073 656c 665f 6b69           self_ki
+0000bc50: 6e64 203d 2044 696d 5479 7065 732e 5370  nd = DimTypes.Sp
+0000bc60: 6174 6961 6c0a 2020 2020 2020 2020 2020  atial.          
+0000bc70: 2020 6966 206f 7468 6572 5f6b 696e 6420    if other_kind 
+0000bc80: 3d3d 2044 696d 5479 7065 732e 4665 6174  == DimTypes.Feat
+0000bc90: 7572 6520 6f72 206e 6f74 206f 7468 6572  ure or not other
+0000bca0: 5f6b 696e 643a 0a20 2020 2020 2020 2020  _kind:.         
+0000bcb0: 2020 2020 2020 206f 7468 6572 5f6b 696e         other_kin
+0000bcc0: 6420 3d20 4469 6d54 7970 6573 2e53 7061  d = DimTypes.Spa
+0000bcd0: 7469 616c 0a20 2020 2020 2020 2069 6620  tial.        if 
+0000bce0: 7365 6c66 2e64 696d 656e 7369 6f6e 2021  self.dimension !
+0000bcf0: 3d20 6f74 6865 722e 6469 6d65 6e73 696f  = other.dimensio
+0000bd00: 6e3a 0a20 2020 2020 2020 2020 2020 2069  n:.            i
+0000bd10: 6620 6272 6f61 6463 6173 745f 6d61 7463  f broadcast_matc
+0000bd20: 6865 7320 616e 6420 2873 656c 662e 6469  hes and (self.di
+0000bd30: 6d65 6e73 696f 6e20 3d3d 2031 206f 7220  mension == 1 or 
+0000bd40: 6f74 6865 722e 6469 6d65 6e73 696f 6e20  other.dimension 
+0000bd50: 3d3d 2031 293a 0a20 2020 2020 2020 2020  == 1):.         
+0000bd60: 2020 2020 2020 2070 6173 7320 2023 2070         pass  # p
+0000bd70: 6173 7320 6f6e 0a20 2020 2020 2020 2020  ass on.         
+0000bd80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000bd90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000bda0: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
+0000bdb0: 2073 656c 665f 6b69 6e64 2021 3d20 6f74   self_kind != ot
+0000bdc0: 6865 725f 6b69 6e64 3a0a 2020 2020 2020  her_kind:.      
+0000bdd0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000bde0: 7365 0a20 2020 2020 2020 2069 6620 7365  se.        if se
+0000bdf0: 6c66 5f6b 696e 6420 3d3d 206f 7468 6572  lf_kind == other
+0000be00: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
+0000be10: 732e 4261 7463 683a 0a20 2020 2020 2020  s.Batch:.       
+0000be20: 2020 2020 2023 204e 6f74 653a 2054 6869       # Note: Thi
+0000be30: 7320 6d69 6768 7420 6265 2069 6e63 6f72  s might be incor
+0000be40: 7265 6374 2069 6e20 736f 6d65 2063 6173  rect in some cas
+0000be50: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0000be60: 2320 652e 672e 2066 6f72 2062 6561 6d20  # e.g. for beam 
+0000be70: 7365 6172 6368 2077 6865 6e20 7765 2068  search when we h
+0000be80: 6176 6520 7468 6520 6265 616d 2068 6964  ave the beam hid
+0000be90: 6465 6e20 696e 2074 6865 2062 6174 6368  den in the batch
+0000bea0: 2064 696d 2c0a 2020 2020 2020 2020 2020   dim,.          
+0000beb0: 2020 2320 6f72 2077 6865 6e20 7765 2075    # or when we u
+0000bec0: 7365 6420 4d65 7267 6544 696d 734c 6179  sed MergeDimsLay
+0000bed0: 6572 206f 6e20 7468 6520 6261 7463 6820  er on the batch 
+0000bee0: 6178 6973 2c20 6f72 2073 6f2e 0a20 2020  axis, or so..   
+0000bef0: 2020 2020 2020 2020 2023 2057 6520 6d69           # We mi
+0000bf00: 6768 7420 6e65 6564 2074 6f20 6578 7465  ght need to exte
+0000bf10: 6e64 2074 6865 206c 6f67 6963 2068 6572  nd the logic her
+0000bf20: 6520 6c61 7465 722e 0a20 2020 2020 2020  e later..       
+0000bf30: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0000bf40: 0a20 2020 2020 2020 2069 6620 4265 6861  .        if Beha
+0000bf50: 7669 6f72 5665 7273 696f 6e2e 6765 7428  viorVersion.get(
+0000bf60: 2920 3e3d 2031 363a 0a20 2020 2020 2020  ) >= 16:.       
+0000bf70: 2020 2020 2023 2045 6974 6865 7220 7365       # Either se
+0000bf80: 6c66 206f 7220 6f74 6865 7220 6973 2073  lf or other is s
+0000bf90: 6f6d 6520 6469 6d20 7461 6720 6578 706c  ome dim tag expl
+0000bfa0: 6963 6974 6c79 2063 7265 6174 6564 2062  icitly created b
+0000bfb0: 7920 7468 6520 7573 6572 2c0a 2020 2020  y the user,.    
+0000bfc0: 2020 2020 2020 2020 2320 616e 6420 7468          # and th
+0000bfd0: 6579 2061 7265 206e 6f74 2074 6865 2073  ey are not the s
+0000bfe0: 616d 652c 2073 6f20 7765 206e 6576 6572  ame, so we never
+0000bff0: 2074 7265 6174 2074 6865 6d20 6173 2065   treat them as e
+0000c000: 7175 616c 2e0a 2020 2020 2020 2020 2020  qual..          
+0000c010: 2020 6966 206e 6f74 2073 656c 662e 6175    if not self.au
+0000c020: 746f 5f67 656e 6572 6174 6564 206f 7220  to_generated or 
+0000c030: 6e6f 7420 6f74 6865 722e 6175 746f 5f67  not other.auto_g
+0000c040: 656e 6572 6174 6564 3a0a 2020 2020 2020  enerated:.      
+0000c050: 2020 2020 2020 2020 2020 6966 2062 726f            if bro
+0000c060: 6164 6361 7374 5f6d 6174 6368 6573 2061  adcast_matches a
+0000c070: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
+0000c080: 2020 2020 2020 2020 2028 7365 6c66 2e64           (self.d
+0000c090: 696d 656e 7369 6f6e 203d 3d20 3120 616e  imension == 1 an
+0000c0a0: 6420 7365 6c66 2e61 7574 6f5f 6765 6e65  d self.auto_gene
+0000c0b0: 7261 7465 6429 206f 7220 286f 7468 6572  rated) or (other
+0000c0c0: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
+0000c0d0: 616e 6420 6f74 6865 722e 6175 746f 5f67  and other.auto_g
+0000c0e0: 656e 6572 6174 6564 290a 2020 2020 2020  enerated).      
+0000c0f0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 2070 6173 7320 2023 2065 7863 6570 7469   pass  # excepti
+0000c120: 6f6e 2c20 616c 6c6f 7720 6272 6f61 6463  on, allow broadc
+0000c130: 6173 7420 6c6f 6769 630a 2020 2020 2020  ast logic.      
+0000c140: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c160: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0000c170: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000c180: 5f6b 696e 6420 3d3d 206f 7468 6572 5f6b  _kind == other_k
+0000c190: 696e 6420 3d3d 2044 696d 5479 7065 732e  ind == DimTypes.
+0000c1a0: 4665 6174 7572 653a 0a20 2020 2020 2020  Feature:.       
+0000c1b0: 2020 2020 2069 6620 616c 6c6f 775f 7361       if allow_sa
+0000c1c0: 6d65 5f66 6561 7475 7265 5f64 696d 3a0a  me_feature_dim:.
+0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1e0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+0000c1f0: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
+0000c200: 203d 3d20 6f74 6865 725f 6b69 6e64 203d   == other_kind =
+0000c210: 3d20 4469 6d54 7970 6573 2e53 7061 7469  = DimTypes.Spati
+0000c220: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
+0000c230: 6966 2061 6c6c 6f77 5f73 616d 655f 7370  if allow_same_sp
+0000c240: 6174 6961 6c5f 6469 6d3a 0a20 2020 2020  atial_dim:.     
+0000c250: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c260: 6c66 2e64 696d 656e 7369 6f6e 2069 7320  lf.dimension is 
+0000c270: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000c280: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000c290: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+0000c2a0: 2020 2020 2020 2020 2020 6966 2062 726f            if bro
+0000c2b0: 6164 6361 7374 5f6d 6174 6368 6573 2061  adcast_matches a
+0000c2c0: 6e64 2028 7365 6c66 2e64 696d 656e 7369  nd (self.dimensi
+0000c2d0: 6f6e 203d 3d20 3120 6f72 206f 7468 6572  on == 1 or other
+0000c2e0: 2e64 696d 656e 7369 6f6e 203d 3d20 3129  .dimension == 1)
+0000c2f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c300: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000c310: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+0000c320: 2075 6e6b 6e6f 776e 5f73 7061 7469 616c   unknown_spatial
+0000c330: 5f6d 6174 6368 6573 2061 6e64 2028 2873  _matches and ((s
+0000c340: 656c 662e 6479 6e5f 7369 7a65 2069 7320  elf.dyn_size is 
+0000c350: 4e6f 6e65 2920 6f72 2028 6f74 6865 722e  None) or (other.
+0000c360: 6479 6e5f 7369 7a65 2069 7320 4e6f 6e65  dyn_size is None
+0000c370: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000c380: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000c390: 2020 2020 2020 2020 2020 2020 6966 2075              if u
+0000c3a0: 6e64 6566 696e 6564 5f6d 6174 6368 6573  ndefined_matches
+0000c3b0: 2061 6e64 2028 7365 6c66 2e75 6e64 6566   and (self.undef
+0000c3c0: 696e 6564 206f 7220 6f74 6865 722e 756e  ined or other.un
+0000c3d0: 6465 6669 6e65 6429 3a0a 2020 2020 2020  defined):.      
+0000c3e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c3f0: 2054 7275 650a 2020 2020 2020 2020 2320   True.        # 
+0000c400: 496e 2070 7269 6e63 6970 6c65 2c20 7765  In principle, we
+0000c410: 2077 6f75 6c64 2077 616e 7420 746f 2063   would want to c
+0000c420: 6865 636b 2066 6f72 2069 6465 6e74 6974  heck for identit
+0000c430: 7920 2873 656c 6620 6973 206f 7468 6572  y (self is other
+0000c440: 292e 0a20 2020 2020 2020 2023 2057 6520  )..        # We 
+0000c450: 6375 7272 656e 746c 7920 7573 6520 7468  currently use th
+0000c460: 6520 6465 7363 7269 7074 696f 6e20 6265  e description be
+0000c470: 6361 7573 6520 7468 6520 6964 656e 7469  cause the identi
+0000c480: 7479 2077 6f75 6c64 206e 6f74 2062 6520  ty would not be 
+0000c490: 7468 6520 7361 6d65 0a20 2020 2020 2020  the same.       
+0000c4a0: 2023 2069 6e20 6361 7365 206f 6620 7465   # in case of te
+0000c4b0: 6d70 6c61 7465 2063 6f6e 7374 7275 6374  mplate construct
+0000c4c0: 696f 6e20 7768 6572 6520 6120 6469 6d20  ion where a dim 
+0000c4d0: 7461 6720 6973 206f 6e63 6520 6372 6561  tag is once crea
+0000c4e0: 7465 6420 666f 7220 6120 7465 6d70 6c61  ted for a templa
+0000c4f0: 7465 206c 6179 6572 2c0a 2020 2020 2020  te layer,.      
+0000c500: 2020 2320 616e 6420 7468 656e 206c 6174    # and then lat
+0000c510: 6572 2061 6761 696e 2066 6f72 2074 6865  er again for the
+0000c520: 2072 6561 6c20 6c61 7965 722e 0a20 2020   real layer..   
+0000c530: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
+0000c540: 6f5f 6765 6e65 7261 7465 6420 616e 6420  o_generated and 
+0000c550: 6f74 6865 722e 6175 746f 5f67 656e 6572  other.auto_gener
+0000c560: 6174 6564 2061 6e64 2073 656c 662e 6465  ated and self.de
+0000c570: 7363 7269 7074 696f 6e20 3d3d 206f 7468  scription == oth
+0000c580: 6572 2e64 6573 6372 6970 7469 6f6e 3a0a  er.description:.
+0000c590: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c5a0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000c5b0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
+0000c5c0: 2020 6465 6620 5f5f 6571 5f5f 2873 656c    def __eq__(sel
+0000c5d0: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+0000c5e0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+0000c5f0: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+0000c600: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000c610: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
+0000c620: 6574 7572 6e3a 203a 6675 6e63 3a60 6973  eturn: :func:`is
+0000c630: 5f65 7175 616c 6020 7769 7468 2064 6566  _equal` with def
+0000c640: 6175 6c74 206f 7074 696f 6e73 0a20 2020  ault options.   
+0000c650: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c660: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000c670: 6365 286f 7468 6572 2c20 5f64 2e44 696d  ce(other, _d.Dim
+0000c680: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000c690: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0000c6a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000c6b0: 6973 5f65 7175 616c 286f 7468 6572 290a  is_equal(other).
+0000c6c0: 0a20 2020 2064 6566 205f 5f6e 655f 5f28  .    def __ne__(
+0000c6d0: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+0000c6e0: 3a20 4469 6d29 3a0a 2020 2020 2020 2020  : Dim):.        
+0000c6f0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+0000c700: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
+0000c710: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+0000c720: 6f6c 0a20 2020 2020 2020 2022 2222 0a20  ol.        """. 
+0000c730: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+0000c740: 7420 2873 656c 6620 3d3d 206f 7468 6572  t (self == other
+0000c750: 290a 0a20 2020 2064 6566 205f 5f68 6173  )..    def __has
+0000c760: 685f 5f28 7365 6c66 293a 0a20 2020 2020  h__(self):.     
+0000c770: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+0000c780: 7274 7970 653a 2069 6e74 0a20 2020 2020  rtype: int.     
+0000c790: 2020 203a 7265 7475 726e 3a20 6861 7368     :return: hash
+0000c7a0: 2c20 6d61 7463 6869 6e67 2074 6f20 3a66  , matching to :f
+0000c7b0: 756e 633a 605f 5f65 715f 5f60 0a20 2020  unc:`__eq__`.   
+0000c7c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c7d0: 2023 2054 6869 7320 6d75 7374 206d 6174   # This must mat
+0000c7e0: 6368 2074 6865 2062 6568 6176 696f 7220  ch the behavior 
+0000c7f0: 696e 205f 5f65 715f 5f2c 2077 6869 6368  in __eq__, which
+0000c800: 2069 7320 6973 5f65 7175 616c 2077 6974   is is_equal wit
+0000c810: 6820 6465 6661 756c 7420 6f70 7469 6f6e  h default option
+0000c820: 732e 0a20 2020 2020 2020 2023 2049 2e65  s..        # I.e
+0000c830: 2e20 6469 6666 6572 656e 7420 6861 7368  . different hash
+0000c840: 2069 6d70 6c69 6573 206e 6f74 2065 7175   implies not equ
+0000c850: 616c 2028 6275 7420 7361 6d65 2068 6173  al (but same has
+0000c860: 6820 6e6f 7420 6e65 6365 7373 6172 696c  h not necessaril
+0000c870: 7920 6571 7561 6c29 2e0a 2020 2020 2020  y equal)..      
+0000c880: 2020 6966 2073 656c 662e 7370 6563 6961    if self.specia
+0000c890: 6c3a 0a20 2020 2020 2020 2020 2020 2072  l:.            r
+0000c8a0: 6574 7572 6e20 6861 7368 2869 6428 7365  eturn hash(id(se
+0000c8b0: 6c66 2929 0a20 2020 2020 2020 2069 6620  lf)).        if 
+0000c8c0: 7365 6c66 2e69 735f 6261 7463 685f 6469  self.is_batch_di
+0000c8d0: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
+0000c8e0: 2072 6574 7572 6e20 6861 7368 2828 2929   return hash(())
+0000c8f0: 0a20 2020 2020 2020 2077 6974 6820 7574  .        with ut
+0000c900: 696c 2e67 7561 7264 5f69 6e66 696e 6974  il.guard_infinit
+0000c910: 655f 7265 6375 7273 696f 6e28 5f64 2e44  e_recursion(_d.D
+0000c920: 696d 2e5f 5f68 6173 685f 5f2c 2073 656c  im.__hash__, sel
+0000c930: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+0000c940: 6261 7365 203d 2073 656c 662e 6765 745f  base = self.get_
+0000c950: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
+0000c960: 2020 2020 2020 2020 6966 2062 6173 6520          if base 
+0000c970: 6973 206e 6f74 2073 656c 663a 0a20 2020  is not self:.   
+0000c980: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000c990: 7572 6e20 6861 7368 2862 6173 6529 0a20  urn hash(base). 
+0000c9a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c9b0: 6c66 2e64 6572 6976 6564 5f66 726f 6d5f  lf.derived_from_
+0000c9c0: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+0000c9d0: 2020 2020 7265 7475 726e 2068 6173 6828      return hash(
+0000c9e0: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
+0000c9f0: 6d5f 6f70 290a 2020 2020 2020 2020 2020  m_op).          
+0000ca00: 2020 6966 2073 656c 662e 6175 746f 5f67    if self.auto_g
+0000ca10: 656e 6572 6174 6564 3a0a 2020 2020 2020  enerated:.      
+0000ca20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ca30: 2068 6173 6828 2862 6173 652e 6b69 6e64   hash((base.kind
+0000ca40: 2c20 6261 7365 2e64 696d 656e 7369 6f6e  , base.dimension
+0000ca50: 2c20 6261 7365 2e64 6573 6372 6970 7469  , base.descripti
+0000ca60: 6f6e 2929 0a20 2020 2020 2020 2020 2020  on)).           
+0000ca70: 2072 6574 7572 6e20 6861 7368 2869 6428   return hash(id(
+0000ca80: 6261 7365 2929 0a0a 2020 2020 6465 6620  base))..    def 
+0000ca90: 5f5f 6c74 5f5f 2873 656c 663a 2044 696d  __lt__(self: Dim
+0000caa0: 2c20 6f74 6865 723a 2044 696d 293a 0a20  , other: Dim):. 
+0000cab0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000cac0: 2020 2044 6566 696e 6520 736f 6d65 206f     Define some o
+0000cad0: 7264 6572 2e20 5468 6973 2069 7320 6a75  rder. This is ju
+0000cae0: 7374 2073 7563 6820 7468 6174 2060 736f  st such that `so
+0000caf0: 7274 6564 6020 776f 726b 732c 206f 7220  rted` works, or 
+0000cb00: 736f 6d65 2064 6966 6620 7265 706f 7274  some diff report
+0000cb10: 696e 672c 206f 7220 736f 2e0a 2020 2020  ing, or so..    
+0000cb20: 2020 2020 4974 2069 7320 6f6e 2073 796d      It is on sym
+0000cb30: 626f 6c69 6320 6c65 7665 6c2c 2069 2e65  bolic level, i.e
+0000cb40: 2e20 6974 2064 6f65 7320 6e6f 7420 636f  . it does not co
+0000cb50: 6e73 6964 6572 2074 6865 2061 6374 7561  nsider the actua
+0000cb60: 6c20 6469 6d65 6e73 696f 6e20 7661 6c75  l dimension valu
+0000cb70: 652e 0a20 2020 2020 2020 2054 6865 2064  e..        The d
+0000cb80: 6566 696e 6564 206f 7264 6572 2073 6f6d  efined order som
+0000cb90: 6577 6861 7420 6172 6269 7472 6172 792c  ewhat arbitrary,
+0000cba0: 2073 6f20 646f 206e 6f74 2072 656c 7920   so do not rely 
+0000cbb0: 6f6e 2074 6865 2065 7861 6374 2062 6568  on the exact beh
+0000cbc0: 6176 696f 722c 0a20 2020 2020 2020 2061  avior,.        a
+0000cbd0: 7320 7468 6973 206d 6967 6874 2063 6861  s this might cha
+0000cbe0: 6e67 6520 6174 2073 6f6d 6520 6c61 7465  nge at some late
+0000cbf0: 7220 706f 696e 742e 0a20 2020 2020 2020  r point..       
+0000cc00: 2043 7572 7265 6e74 6c79 2c20 6974 2064   Currently, it d
+0000cc10: 6570 656e 6473 206f 6e20 7468 6520 6372  epends on the cr
+0000cc20: 6561 7469 6f6e 2069 6e64 6578 2e0a 0a20  eation index... 
+0000cc30: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+0000cc40: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+0000cc50: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+0000cc60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000cc70: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+0000cc80: 6e63 6528 6f74 6865 722c 2028 5f64 2e44  nce(other, (_d.D
+0000cc90: 696d 2c20 5f6d 2e4d 6172 6b65 6444 696d  im, _m.MarkedDim
+0000cca0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000ccb0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+0000ccc0: 2263 616e 6e6f 7420 636f 6d70 6172 6520  "cannot compare 
+0000ccd0: 2572 2077 6974 6820 2572 2220 2520 2873  %r with %r" % (s
+0000cce0: 656c 662c 206f 7468 6572 2929 0a20 2020  elf, other)).   
+0000ccf0: 2020 2020 2069 6620 7365 6c66 203d 3d20       if self == 
+0000cd00: 6f74 6865 723a 0a20 2020 2020 2020 2020  other:.         
+0000cd10: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000cd20: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0000cd30: 696d 5f63 6d70 5f76 616c 7565 2873 656c  im_cmp_value(sel
+0000cd40: 6629 203c 2064 696d 5f63 6d70 5f76 616c  f) < dim_cmp_val
+0000cd50: 7565 286f 7468 6572 290a 0a20 2020 2064  ue(other)..    d
+0000cd60: 6566 205f 5f67 745f 5f28 7365 6c66 2c20  ef __gt__(self, 
+0000cd70: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+0000cd80: 2222 220a 2020 2020 2020 2020 5365 6520  """.        See 
+0000cd90: 3a66 756e 633a 605f 5f6c 745f 5f60 2e0a  :func:`__lt__`..
+0000cda0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000cdb0: 4469 6d20 6f74 6865 723a 0a20 2020 2020  Dim other:.     
+0000cdc0: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+0000cdd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000cde0: 2020 2020 7265 7475 726e 206f 7468 6572      return other
+0000cdf0: 203c 2073 656c 660a 0a20 2020 2064 6566   < self..    def
+0000ce00: 205f 5f67 655f 5f28 7365 6c66 2c20 6f74   __ge__(self, ot
+0000ce10: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
+0000ce20: 7475 726e 206e 6f74 2073 656c 6620 3c20  turn not self < 
+0000ce30: 6f74 6865 720a 0a20 2020 2064 6566 205f  other..    def _
+0000ce40: 5f6c 655f 5f28 7365 6c66 2c20 6f74 6865  _le__(self, othe
+0000ce50: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
+0000ce60: 726e 206e 6f74 2073 656c 6620 3e20 6f74  rn not self > ot
+0000ce70: 6865 720a 0a20 2020 2064 6566 2067 6574  her..    def get
+0000ce80: 5f73 616d 655f 6261 7365 2873 656c 663a  _same_base(self:
+0000ce90: 205f 642e 4469 6d29 202d 3e20 5f64 2e44   _d.Dim) -> _d.D
+0000cea0: 696d 3a0a 2020 2020 2020 2020 2222 220a  im:.        """.
+0000ceb0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+0000cec0: 2073 616d 6520 6261 7365 0a20 2020 2020   same base.     
+0000ced0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000cee0: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
+0000cef0: 613a 0a20 2020 2020 2020 2020 2020 2072  a:.            r
+0000cf00: 6574 7572 6e20 7365 6c66 0a20 2020 2020  eturn self.     
+0000cf10: 2020 2062 6173 6520 3d20 7365 6c66 0a20     base = self. 
+0000cf20: 2020 2020 2020 2077 6869 6c65 2062 6173         while bas
+0000cf30: 652e 7361 6d65 5f61 733a 0a20 2020 2020  e.same_as:.     
+0000cf40: 2020 2020 2020 2062 6173 6520 3d20 6261         base = ba
+0000cf50: 7365 2e73 616d 655f 6173 0a20 2020 2020  se.same_as.     
+0000cf60: 2020 2072 6574 7572 6e20 6261 7365 0a0a     return base..
+0000cf70: 2020 2020 6465 6620 6765 745f 7361 6d65      def get_same
+0000cf80: 5f64 6572 6976 6564 5f62 6173 6528 7365  _derived_base(se
+0000cf90: 6c66 3a20 5f64 2e44 696d 2c20 2a2c 2073  lf: _d.Dim, *, s
+0000cfa0: 616d 655f 6469 6d3a 2062 6f6f 6c20 3d20  ame_dim: bool = 
+0000cfb0: 4661 6c73 6529 202d 3e20 5f64 2e44 696d  False) -> _d.Dim
+0000cfc0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000cfd0: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
+0000cfe0: 655f 6469 6d3a 2069 6620 5472 7565 2c20  e_dim: if True, 
+0000cff0: 7265 7475 726e 2074 6865 206c 6173 7420  return the last 
+0000d000: 6261 7365 2077 6869 6368 2068 6173 2074  base which has t
+0000d010: 6865 2073 616d 6520 6469 6d65 6e73 696f  he same dimensio
+0000d020: 6e2e 0a20 2020 2020 2020 2020 2020 2054  n..            T
+0000d030: 6865 2064 6572 6976 6564 2062 6173 6520  he derived base 
+0000d040: 6d69 6768 7420 6861 7665 2061 2064 6966  might have a dif
+0000d050: 6665 7265 6e74 2064 696d 656e 7369 6f6e  ferent dimension
+0000d060: 2e0a 2020 2020 2020 2020 2020 2020 496e  ..            In
+0000d070: 2063 6173 6520 6974 2069 7320 6479 6e61   case it is dyna
+0000d080: 6d69 632c 2074 6865 2064 696d 656e 7369  mic, the dimensi
+0000d090: 6f6e 2069 7320 4e6f 6e65 2c20 736f 2069  on is None, so i
+0000d0a0: 7420 6973 2061 6c77 6179 7320 7468 6520  t is always the 
+0000d0b0: 7361 6d65 2e0a 2020 2020 2020 2020 2020  same..          
+0000d0c0: 2020 496e 2063 6173 6520 6974 2069 7320    In case it is 
+0000d0d0: 7374 6174 6963 2c20 7468 6572 6520 6d69  static, there mi
+0000d0e0: 6768 7420 6265 2061 2064 6966 6665 7265  ght be a differe
+0000d0f0: 6e74 2064 696d 656e 7369 6f6e 2e0a 2020  nt dimension..  
+0000d100: 2020 2020 2020 3a72 6574 7572 6e3a 2073        :return: s
+0000d110: 616d 6520 6261 7365 2c20 6275 7420 616c  ame base, but al
+0000d120: 736f 2063 6f6e 7369 6465 7220 6465 7269  so consider deri
+0000d130: 7665 645f 6672 6f6d 5f2e 2e2e 0a20 2020  ved_from_....   
+0000d140: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d150: 206c 6173 745f 6261 7365 5f73 656c 665f   last_base_self_
+0000d160: 6469 6d20 3d20 7365 6c66 0a20 2020 2020  dim = self.     
+0000d170: 2020 2062 6173 6520 3d20 7365 6c66 0a20     base = self. 
+0000d180: 2020 2020 2020 2076 6973 6974 6564 203d         visited =
+0000d190: 207b 7d0a 2020 2020 2020 2020 7768 696c   {}.        whil
+0000d1a0: 6520 6261 7365 2e73 616d 655f 6173 206f  e base.same_as o
+0000d1b0: 7220 6261 7365 2e64 6572 6976 6564 5f66  r base.derived_f
+0000d1c0: 726f 6d5f 7461 673a 0a20 2020 2020 2020  rom_tag:.       
+0000d1d0: 2020 2020 2061 7373 6572 7420 6964 2862       assert id(b
+0000d1e0: 6173 6529 206e 6f74 2069 6e20 7669 7369  ase) not in visi
+0000d1f0: 7465 6420 2023 2073 686f 756c 6420 6e6f  ted  # should no
+0000d200: 7420 6861 7665 2063 7963 6c65 732e 206e  t have cycles. n
+0000d210: 6f72 6d61 6c6c 7920 7468 6973 2073 686f  ormally this sho
+0000d220: 756c 6420 6e65 7665 7220 6265 2074 7269  uld never be tri
+0000d230: 6767 6572 6564 0a20 2020 2020 2020 2020  ggered.         
+0000d240: 2020 2076 6973 6974 6564 5b69 6428 6261     visited[id(ba
+0000d250: 7365 295d 203d 2062 6173 650a 2020 2020  se)] = base.    
+0000d260: 2020 2020 2020 2020 6966 2062 6173 652e          if base.
+0000d270: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
+0000d280: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
+0000d290: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
+0000d2a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000d2b0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+0000d2c0: 2020 6261 7365 203d 2062 6173 652e 6465    base = base.de
+0000d2d0: 7269 7665 645f 6672 6f6d 5f74 6167 0a20  rived_from_tag. 
+0000d2e0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000d2f0: 7420 6261 7365 0a20 2020 2020 2020 2020  t base.         
+0000d300: 2020 2069 6620 6261 7365 2e64 696d 656e     if base.dimen
+0000d310: 7369 6f6e 203d 3d20 7365 6c66 2e64 696d  sion == self.dim
+0000d320: 656e 7369 6f6e 3a0a 2020 2020 2020 2020  ension:.        
+0000d330: 2020 2020 2020 2020 6c61 7374 5f62 6173          last_bas
+0000d340: 655f 7365 6c66 5f64 696d 203d 2062 6173  e_self_dim = bas
+0000d350: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000d360: 206c 6173 745f 6261 7365 5f73 656c 665f   last_base_self_
+0000d370: 6469 6d20 6966 2073 616d 655f 6469 6d20  dim if same_dim 
+0000d380: 656c 7365 2062 6173 650a 0a20 2020 2064  else base..    d
+0000d390: 6566 2067 6574 5f64 6572 6976 6564 5f62  ef get_derived_b
+0000d3a0: 6173 6573 5f73 6574 2873 656c 6629 3a0a  ases_set(self):.
+0000d3b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d3c0: 2020 2020 3a72 7479 7065 3a20 7365 745b      :rtype: set[
+0000d3d0: 4469 6d5d 0a20 2020 2020 2020 2022 2222  Dim].        """
+0000d3e0: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
+0000d3f0: 6574 2829 0a20 2020 2020 2020 2071 7565  et().        que
+0000d400: 7565 203d 205b 7365 6c66 5d0a 2020 2020  ue = [self].    
+0000d410: 2020 2020 7669 7369 7465 6420 3d20 7b7d      visited = {}
+0000d420: 2020 2320 7479 7065 3a20 4469 6374 5b69    # type: Dict[i
+0000d430: 6e74 2c5f 642e 4469 6d5d 2020 2320 6279  nt,_d.Dim]  # by
+0000d440: 2069 640a 2020 2020 2020 2020 7768 696c   id.        whil
+0000d450: 6520 7175 6575 653a 0a20 2020 2020 2020  e queue:.       
+0000d460: 2020 2020 2062 6173 6520 3d20 7175 6575       base = queu
+0000d470: 652e 706f 7028 2d31 290a 2020 2020 2020  e.pop(-1).      
+0000d480: 2020 2020 2020 6966 2062 6173 652e 7361        if base.sa
+0000d490: 6d65 5f61 733a 0a20 2020 2020 2020 2020  me_as:.         
+0000d4a0: 2020 2020 2020 2062 6173 6520 3d20 6261         base = ba
+0000d4b0: 7365 2e73 616d 655f 6173 0a20 2020 2020  se.same_as.     
+0000d4c0: 2020 2020 2020 2069 6620 6964 2862 6173         if id(bas
+0000d4d0: 6529 2069 6e20 7669 7369 7465 643a 0a20  e) in visited:. 
+0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d4f0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+0000d500: 2020 2020 7669 7369 7465 645b 6964 2862      visited[id(b
+0000d510: 6173 6529 5d20 3d20 6261 7365 0a20 2020  ase)] = base.   
+0000d520: 2020 2020 2020 2020 2072 6573 2e61 6464           res.add
+0000d530: 2862 6173 6529 0a20 2020 2020 2020 2020  (base).         
+0000d540: 2020 2069 6620 6261 7365 2e64 6572 6976     if base.deriv
+0000d550: 6564 5f66 726f 6d5f 6f70 3a0a 2020 2020  ed_from_op:.    
+0000d560: 2020 2020 2020 2020 2020 2020 7175 6575              queu
+0000d570: 652e 6578 7465 6e64 2862 6173 652e 6465  e.extend(base.de
+0000d580: 7269 7665 645f 6672 6f6d 5f6f 702e 696e  rived_from_op.in
+0000d590: 7075 7473 290a 2020 2020 2020 2020 2020  puts).          
+0000d5a0: 2020 656c 6966 2062 6173 652e 6465 7269    elif base.deri
+0000d5b0: 7665 645f 6672 6f6d 5f74 6167 3a0a 2020  ved_from_tag:.  
+0000d5c0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
+0000d5d0: 6575 652e 6170 7065 6e64 2862 6173 652e  eue.append(base.
+0000d5e0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+0000d5f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d600: 2072 6573 0a0a 2020 2020 4070 726f 7065   res..    @prope
+0000d610: 7274 790a 2020 2020 6465 6620 756e 6465  rty.    def unde
+0000d620: 6669 6e65 6428 7365 6c66 3a20 5f64 2e44  fined(self: _d.D
+0000d630: 696d 2920 2d3e 2062 6f6f 6c3a 0a20 2020  im) -> bool:.   
+0000d640: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d650: 203a 7265 7475 726e 3a20 7768 6574 6865   :return: whethe
+0000d660: 7220 7468 6520 756e 6465 6669 6e65 6420  r the undefined 
+0000d670: 666c 6167 2069 7320 7365 742c 2069 6e20  flag is set, in 
+0000d680: 7365 6c66 2c20 6261 7365 732c 206f 7220  self, bases, or 
+0000d690: 616e 7920 6465 7269 7665 6420 6261 7365  any derived base
+0000d6a0: 732e 2061 6c73 6f20 7365 6520 3a66 756e  s. also see :fun
+0000d6b0: 633a 6069 735f 6469 6d5f 6b6e 6f77 6e60  c:`is_dim_known`
+0000d6c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d6d0: 2020 2020 2062 6173 6520 3d20 7365 6c66       base = self
+0000d6e0: 0a20 2020 2020 2020 2076 6973 6974 6564  .        visited
+0000d6f0: 203d 207b 7d0a 2020 2020 2020 2020 7768   = {}.        wh
+0000d700: 696c 6520 6261 7365 2e73 616d 655f 6173  ile base.same_as
+0000d710: 206f 7220 6261 7365 2e64 6572 6976 6564   or base.derived
+0000d720: 5f66 726f 6d5f 7461 673a 0a20 2020 2020  _from_tag:.     
+0000d730: 2020 2020 2020 2061 7373 6572 7420 6964         assert id
+0000d740: 2862 6173 6529 206e 6f74 2069 6e20 7669  (base) not in vi
+0000d750: 7369 7465 6420 2023 2073 686f 756c 6420  sited  # should 
+0000d760: 6e6f 7420 6861 7665 2063 7963 6c65 732e  not have cycles.
+0000d770: 206e 6f72 6d61 6c6c 7920 7468 6973 2073   normally this s
+0000d780: 686f 756c 6420 6e65 7665 7220 6265 2074  hould never be t
+0000d790: 7269 6767 6572 6564 0a20 2020 2020 2020  riggered.       
+0000d7a0: 2020 2020 2076 6973 6974 6564 5b69 6428       visited[id(
+0000d7b0: 6261 7365 295d 203d 2062 6173 650a 2020  base)] = base.  
+0000d7c0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
+0000d7d0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+0000d7e0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+0000d7f0: 2020 2020 2020 2069 6620 6261 7365 2e5f         if base._
+0000d800: 6578 7472 6120 616e 6420 6261 7365 2e5f  extra and base._
+0000d810: 6578 7472 612e 756e 6465 6669 6e65 643a  extra.undefined:
+0000d820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d830: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+0000d840: 2020 2020 2020 2020 2069 6620 6261 7365           if base
+0000d850: 2e73 616d 655f 6173 3a0a 2020 2020 2020  .same_as:.      
+0000d860: 2020 2020 2020 2020 2020 6261 7365 203d            base =
+0000d870: 2062 6173 652e 7361 6d65 5f61 730a 2020   base.same_as.  
+0000d880: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000d890: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+0000d8a0: 2020 2062 6173 6520 3d20 6261 7365 2e64     base = base.d
+0000d8b0: 6572 6976 6564 5f66 726f 6d5f 7461 670a  erived_from_tag.
+0000d8c0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000d8d0: 7274 2062 6173 650a 2020 2020 2020 2020  rt base.        
+0000d8e0: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+0000d8f0: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+0000d900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d910: 6261 7365 2e5f 6578 7472 6120 616e 6420  base._extra and 
+0000d920: 6261 7365 2e5f 6578 7472 612e 756e 6465  base._extra.unde
+0000d930: 6669 6e65 640a 0a20 2020 2064 6566 2064  fined..    def d
+0000d940: 6563 6c61 7265 5f73 616d 655f 6173 2873  eclare_same_as(s
+0000d950: 656c 663a 205f 642e 4469 6d2c 206f 7468  elf: _d.Dim, oth
+0000d960: 6572 3a20 5f64 2e44 696d 293a 0a20 2020  er: _d.Dim):.   
+0000d970: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d980: 203a 7061 7261 6d20 6f74 6865 723a 0a20   :param other:. 
+0000d990: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d9a0: 2020 2061 7373 6572 7420 7365 6c66 2e63     assert self.c
+0000d9b0: 616e 5f62 655f 7573 6564 5f61 735f 6469  an_be_used_as_di
+0000d9c0: 6d28 2920 616e 6420 6f74 6865 722e 6361  m() and other.ca
+0000d9d0: 6e5f 6265 5f75 7365 645f 6173 5f64 696d  n_be_used_as_dim
+0000d9e0: 2829 2020 2320 6465 636c 6172 655f 7361  ()  # declare_sa
+0000d9f0: 6d65 5f61 7320 646f 6573 206e 6f74 206d  me_as does not m
+0000da00: 616b 6520 7365 6e73 6520 6f74 6865 7277  ake sense otherw
+0000da10: 6973 650a 2020 2020 2020 2020 2320 4e6f  ise.        # No
+0000da20: 7465 3a20 4368 6563 6b20 6069 7360 2c20  te: Check `is`, 
+0000da30: 6e6f 7420 603d 3d60 2e20 603d 3d60 2063  not `==`. `==` c
+0000da40: 616e 2062 6520 7472 7565 2065 7665 6e20  an be true even 
+0000da50: 7468 6f75 6768 2073 616d 655f 6173 2061  though same_as a
+0000da60: 7265 206e 6f74 2074 6865 2073 616d 6520  re not the same 
+0000da70: 696e 7374 616e 6365 2c0a 2020 2020 2020  instance,.      
+0000da80: 2020 2320 652e 672e 2076 6961 2061 7574    # e.g. via aut
+0000da90: 6f5f 6765 6e65 7261 7465 642e 0a20 2020  o_generated..   
+0000daa0: 2020 2020 2069 6620 7365 6c66 2069 7320       if self is 
+0000dab0: 6f74 6865 723a 0a20 2020 2020 2020 2020  other:.         
+0000dac0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000dad0: 2020 7365 6c66 2e5f 6d61 7962 655f 7570    self._maybe_up
+0000dae0: 6461 7465 2829 0a20 2020 2020 2020 2073  date().        s
+0000daf0: 656c 662e 5f76 616c 6964 6174 655f 696e  elf._validate_in
+0000db00: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
+0000db10: 0a20 2020 2020 2020 206f 7468 6572 2e5f  .        other._
+0000db20: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
+0000db30: 656e 745f 6772 6170 6828 290a 2020 2020  ent_graph().    
+0000db40: 2020 2020 6f74 6865 725f 7361 6d65 5f62      other_same_b
+0000db50: 6173 6520 3d20 6f74 6865 722e 6765 745f  ase = other.get_
+0000db60: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
+0000db70: 2020 2020 6966 2073 656c 6620 6973 206f      if self is o
+0000db80: 7468 6572 5f73 616d 655f 6261 7365 206f  ther_same_base o
+0000db90: 7220 7365 6c66 2e73 616d 655f 6173 2069  r self.same_as i
+0000dba0: 7320 6f74 6865 725f 7361 6d65 5f62 6173  s other_same_bas
+0000dbb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000dbc0: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
+0000dbd0: 6c66 5f73 616d 655f 6173 203d 2073 656c  lf_same_as = sel
+0000dbe0: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
+0000dbf0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000dc00: 665f 7361 6d65 5f61 7320 6973 206f 7468  f_same_as is oth
+0000dc10: 6572 5f73 616d 655f 6261 7365 3a0a 2020  er_same_base:.  
+0000dc20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000dc30: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+0000dc40: 725f 7361 6d65 5f62 6173 652e 6765 745f  r_same_base.get_
+0000dc50: 7361 6d65 5f64 6572 6976 6564 5f62 6173  same_derived_bas
+0000dc60: 6528 2920 6973 2073 656c 665f 7361 6d65  e() is self_same
+0000dc70: 5f61 733a 0a20 2020 2020 2020 2020 2020  _as:.           
+0000dc80: 2023 2057 6520 6163 7475 616c 6c79 2077   # We actually w
+0000dc90: 616e 7420 6974 2074 6f20 6265 2074 6865  ant it to be the
+0000dca0: 206f 7468 6572 2077 6179 2061 726f 756e   other way aroun
+0000dcb0: 642e 0a20 2020 2020 2020 2020 2020 2077  d..            w
+0000dcc0: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
+0000dcd0: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
+0000dce0: 6e28 5f64 2e44 696d 2e64 6563 6c61 7265  n(_d.Dim.declare
+0000dcf0: 5f73 616d 655f 6173 2c20 6f74 6865 722c  _same_as, other,
+0000dd00: 2073 656c 6629 3a0a 2020 2020 2020 2020   self):.        
+0000dd10: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+0000dd20: 7468 6572 2e64 6563 6c61 7265 5f73 616d  ther.declare_sam
+0000dd30: 655f 6173 2873 656c 6629 0a20 2020 2020  e_as(self).     
+0000dd40: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+0000dd50: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000dd60: 4966 2073 656c 6620 6973 2064 6566 696e  If self is defin
+0000dd70: 6564 2028 7365 6c66 2e69 735f 6469 6d5f  ed (self.is_dim_
+0000dd80: 6b6e 6f77 6e29 2c20 6265 2066 6169 7220  known), be fair 
+0000dd90: 746f 206f 7468 6572 2c20 616e 6420 6164  to other, and ad
+0000dda0: 6170 7420 6974 2074 6f20 7468 6520 7269  apt it to the ri
+0000ddb0: 6768 7420 6261 7463 682c 0a20 2020 2020  ght batch,.     
+0000ddc0: 2020 2020 2020 2023 2073 7563 6820 7468         # such th
+0000ddd0: 6174 206f 7468 6572 2e69 735f 6469 6d5f  at other.is_dim_
+0000dde0: 6b6e 6f77 6e20 6973 2063 6f72 7265 6374  known is correct
+0000ddf0: 2c20 6279 2070 6f74 656e 7469 616c 6c79  , by potentially
+0000de00: 2063 6f6d 706c 6574 696e 6720 6974 2e0a   completing it..
+0000de10: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000de20: 725f 203d 206f 7468 6572 2e67 6574 5f66  r_ = other.get_f
+0000de30: 6f72 5f62 6174 6368 5f63 7478 2873 656c  or_batch_ctx(sel
+0000de40: 662e 6261 7463 682c 2063 7478 3d73 656c  f.batch, ctx=sel
+0000de50: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+0000de60: 7478 290a 2020 2020 2020 2020 656c 7365  tx).        else
+0000de70: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
+0000de80: 6865 725f 203d 206f 7468 6572 0a20 2020  her_ = other.   
+0000de90: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+0000dea0: 2020 2020 2020 2873 656c 662e 6973 5f64        (self.is_d
+0000deb0: 696d 5f6b 6e6f 776e 2829 2061 6e64 206e  im_known() and n
+0000dec0: 6f74 206f 7468 6572 5f2e 6973 5f64 696d  ot other_.is_dim
+0000ded0: 5f6b 6e6f 776e 2829 290a 2020 2020 2020  _known()).      
+0000dee0: 2020 2020 2020 6f72 0a20 2020 2020 2020        or.       
+0000def0: 2020 2020 2023 204c 696b 6520 6973 5f64       # Like is_d
+0000df00: 696d 5f6b 6e6f 776e 2062 7574 2066 6f72  im_known but for
+0000df10: 2073 7461 7469 6320 6469 6d73 2c20 7765   static dims, we
+0000df20: 206d 6967 6874 206b 6e6f 7720 626f 7468   might know both
+0000df30: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0000df40: 6275 7420 7468 6520 6465 7269 7665 645f  but the derived_
+0000df50: 6672 6f6d 5f6f 7020 7374 696c 6c20 776f  from_op still wo
+0000df60: 756c 6420 7072 6f76 6964 6520 6d6f 7265  uld provide more
+0000df70: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
+0000df80: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
+0000df90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dfa0: 5f73 616d 655f 6173 2e64 6572 6976 6564  _same_as.derived
+0000dfb0: 5f66 726f 6d5f 6f70 0a20 2020 2020 2020  _from_op.       
+0000dfc0: 2020 2020 2020 2020 2061 6e64 206e 6f74           and not
+0000dfd0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000dfe0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e000: 2061 6e64 206f 7468 6572 206e 6f74 2069   and other not i
+0000e010: 6e20 7365 6c66 2e67 6574 5f64 6572 6976  n self.get_deriv
+0000e020: 6564 5f62 6173 6573 5f73 6574 2829 0a20  ed_bases_set(). 
+0000e030: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000e040: 2020 2020 2020 2020 206f 7220 286e 6f74           or (not
+0000e050: 2073 656c 662e 756e 6465 6669 6e65 6420   self.undefined 
+0000e060: 616e 6420 6f74 6865 725f 2e75 6e64 6566  and other_.undef
+0000e070: 696e 6564 290a 2020 2020 2020 2020 293a  ined).        ):
+0000e080: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000e090: 6820 7574 696c 2e67 7561 7264 5f69 6e66  h util.guard_inf
+0000e0a0: 696e 6974 655f 7265 6375 7273 696f 6e28  inite_recursion(
+0000e0b0: 5f64 2e44 696d 2e64 6563 6c61 7265 5f73  _d.Dim.declare_s
+0000e0c0: 616d 655f 6173 2c20 6f74 6865 722c 2073  ame_as, other, s
+0000e0d0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+0000e0e0: 2020 2020 2020 7265 7475 726e 206f 7468        return oth
+0000e0f0: 6572 2e64 6563 6c61 7265 5f73 616d 655f  er.declare_same_
+0000e100: 6173 2873 656c 6629 0a20 2020 2020 2020  as(self).       
+0000e110: 206f 7468 6572 5f64 6572 6976 6564 5f62   other_derived_b
+0000e120: 6173 6573 203d 206f 7468 6572 2e67 6574  ases = other.get
+0000e130: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
+0000e140: 6574 2829 0a20 2020 2020 2020 2073 656c  et().        sel
+0000e150: 665f 6465 7269 7665 645f 6261 7365 7320  f_derived_bases 
+0000e160: 3d20 7365 6c66 2e67 6574 5f64 6572 6976  = self.get_deriv
+0000e170: 6564 5f62 6173 6573 5f73 6574 2829 0a20  ed_bases_set(). 
+0000e180: 2020 2020 2020 2069 6620 6f74 6865 725f         if other_
+0000e190: 6465 7269 7665 645f 6261 7365 7320 213d  derived_bases !=
+0000e1a0: 2073 656c 665f 6465 7269 7665 645f 6261   self_derived_ba
+0000e1b0: 7365 7320 616e 6420 7365 6c66 5f64 6572  ses and self_der
+0000e1c0: 6976 6564 5f62 6173 6573 2e69 7373 7562  ived_bases.issub
+0000e1d0: 7365 7428 6f74 6865 725f 6465 7269 7665  set(other_derive
+0000e1e0: 645f 6261 7365 7329 3a0a 2020 2020 2020  d_bases):.      
+0000e1f0: 2020 2020 2020 2320 4176 6f69 6420 6379        # Avoid cy
+0000e200: 636c 6573 206f 6e20 6465 7269 7665 645f  cles on derived_
+0000e210: 6672 6f6d 5f74 6167 2e20 6874 7470 733a  from_tag. https:
+0000e220: 2f2f 6769 7468 7562 2e63 6f6d 2f72 7774  //github.com/rwt
+0000e230: 682d 6936 2f72 6574 7572 6e6e 2f69 7373  h-i6/returnn/iss
+0000e240: 7565 732f 3130 3534 0a20 2020 2020 2020  ues/1054.       
+0000e250: 2020 2020 2077 6974 6820 7574 696c 2e67       with util.g
+0000e260: 7561 7264 5f69 6e66 696e 6974 655f 7265  uard_infinite_re
+0000e270: 6375 7273 696f 6e28 5f64 2e44 696d 2e64  cursion(_d.Dim.d
+0000e280: 6563 6c61 7265 5f73 616d 655f 6173 2c20  eclare_same_as, 
+0000e290: 6f74 6865 722c 2073 656c 6629 3a0a 2020  other, self):.  
+0000e2a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000e2b0: 7475 726e 206f 7468 6572 2e64 6563 6c61  turn other.decla
+0000e2c0: 7265 5f73 616d 655f 6173 2873 656c 6629  re_same_as(self)
+0000e2d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e2e0: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+0000e2f0: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
+0000e300: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000e310: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000e320: 2020 2020 7365 6c66 2e5f 6578 7472 612e      self._extra.
+0000e330: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+0000e340: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000e350: 6966 2073 656c 665f 7361 6d65 5f61 7320  if self_same_as 
+0000e360: 6973 206e 6f74 2073 656c 663a 0a20 2020  is not self:.   
+0000e370: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000e380: 6e6f 7420 7365 6c66 5f73 616d 655f 6173  not self_same_as
+0000e390: 2e73 616d 655f 6173 0a20 2020 2020 2020  .same_as.       
+0000e3a0: 2020 2020 2069 6620 7365 6c66 5f73 616d       if self_sam
+0000e3b0: 655f 6173 2069 7320 6f74 6865 725f 7361  e_as is other_sa
+0000e3c0: 6d65 5f62 6173 653a 0a20 2020 2020 2020  me_base:.       
+0000e3d0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000e3e0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000e3f0: 2075 7469 6c2e 6775 6172 645f 696e 6669   util.guard_infi
+0000e400: 6e69 7465 5f72 6563 7572 7369 6f6e 285f  nite_recursion(_
+0000e410: 642e 4469 6d2e 6465 636c 6172 655f 7361  d.Dim.declare_sa
+0000e420: 6d65 5f61 732c 2073 656c 665f 7361 6d65  me_as, self_same
+0000e430: 5f61 732c 206f 7468 6572 5f73 616d 655f  _as, other_same_
+0000e440: 6261 7365 293a 0a20 2020 2020 2020 2020  base):.         
+0000e450: 2020 2020 2020 2073 656c 665f 7361 6d65         self_same
+0000e460: 5f61 732e 6465 636c 6172 655f 7361 6d65  _as.declare_same
+0000e470: 5f61 7328 6f74 6865 725f 7361 6d65 5f62  _as(other_same_b
+0000e480: 6173 6529 0a20 2020 2020 2020 2020 2020  ase).           
+0000e490: 2069 6620 2873 656c 662e 6479 6e5f 7369   if (self.dyn_si
+0000e4a0: 7a65 5f65 7874 2069 7320 4e6f 6e65 206f  ze_ext is None o
+0000e4b0: 7220 6e6f 7420 7365 6c66 2e5f 7661 6c69  r not self._vali
+0000e4c0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
+0000e4d0: 6772 6170 6828 2929 2061 6e64 2073 656c  graph()) and sel
+0000e4e0: 665f 7361 6d65 5f61 732e 6479 6e5f 7369  f_same_as.dyn_si
+0000e4f0: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+0000e500: 2020 2020 2020 2020 7365 6c66 2e64 796e          self.dyn
+0000e510: 5f73 697a 655f 6578 7420 3d20 7365 6c66  _size_ext = self
+0000e520: 5f73 616d 655f 6173 2e67 6574 5f64 796e  _same_as.get_dyn
+0000e530: 5f73 697a 655f 6578 745f 666f 725f 6261  _size_ext_for_ba
+0000e540: 7463 685f 6374 7828 0a20 2020 2020 2020  tch_ctx(.       
+0000e550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e560: 662e 6261 7463 682c 2073 656c 662e 636f  f.batch, self.co
+0000e570: 6e74 726f 6c5f 666c 6f77 5f63 7478 2c20  ntrol_flow_ctx, 
+0000e580: 7465 6d70 6c61 7465 5f6f 6e6c 793d 5472  template_only=Tr
+0000e590: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+0000e5a0: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+0000e5b0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+0000e5c0: 6620 7365 6c66 2e5f 6578 7472 613a 0a20  f self._extra:. 
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e5e0: 6f72 2064 696d 5f20 696e 2073 656c 662e  or dim_ in self.
+0000e5f0: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000e600: 6261 7463 685f 6374 782e 7661 6c75 6573  batch_ctx.values
+0000e610: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000e620: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
+0000e630: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
+0000e640: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
+0000e650: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e660: 6469 6d5f 2e5f 6578 7472 613a 0a20 2020  dim_._extra:.   
+0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e680: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
+0000e690: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
+0000e6a0: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0000e6c0: 6d5f 2e5f 6578 7472 612e 6465 7269 7665  m_._extra.derive
+0000e6d0: 645f 6672 6f6d 5f6f 7020 3d20 4e6f 6e65  d_from_op = None
+0000e6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e6f0: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
+0000e700: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
+0000e710: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
 0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e730: 2020 2020 2020 2020 6469 6d5f 2e5f 6578          dim_._ex
-0000e740: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
-0000e750: 5f74 6167 203d 204e 6f6e 650a 2020 2020  _tag = None.    
-0000e760: 2020 2020 2320 4e6f 7720 6d65 7267 6520      # Now merge 
-0000e770: 6578 6973 7469 6e67 2076 6172 6961 6e74  existing variant
-0000e780: 732e 2042 7574 206f 6e6c 7920 6966 206e  s. But only if n
-0000e790: 6f74 2064 6572 6976 6564 2076 6961 206f  ot derived via o
-0000e7a0: 702c 2062 6563 6175 7365 2069 6e20 7468  p, because in th
-0000e7b0: 6174 2063 6173 652c 2077 6520 6361 6e20  at case, we can 
-0000e7c0: 2861 6e64 2073 686f 756c 6421 290a 2020  (and should!).  
-0000e7d0: 2020 2020 2020 2320 6175 746f 6d61 7469        # automati
-0000e7e0: 6361 6c6c 7920 696e 6665 7220 6974 2e20  cally infer it. 
-0000e7f0: 4e6f 7465 2074 6861 7420 7765 206f 6e6c  Note that we onl
-0000e800: 7920 676f 7420 6865 7265 2077 6865 6e20  y got here when 
-0000e810: 7468 6520 6f74 6865 7220 6973 206e 6f74  the other is not
-0000e820: 2074 6865 2073 616d 6520 6469 6d2c 2073   the same dim, s
-0000e830: 6f20 6974 206d 6561 6e73 2074 6861 740a  o it means that.
-0000e840: 2020 2020 2020 2020 2320 7468 6520 6f74          # the ot
-0000e850: 6865 7220 6973 2072 6561 6c6c 7920 6469  her is really di
-0000e860: 6666 6572 656e 742c 2074 6865 2073 697a  fferent, the siz
-0000e870: 6573 2061 7265 2070 6f74 656e 7469 616c  es are potential
-0000e880: 6c79 2064 6966 6665 7265 6e74 2c20 6275  ly different, bu
-0000e890: 7420 7765 2077 616e 7420 746f 206f 7665  t we want to ove
-0000e8a0: 7274 616b 6520 7468 6520 6f74 6865 722e  rtake the other.
-0000e8b0: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-0000e8c0: 725f 7361 6d65 5f62 6173 652e 6465 7269  r_same_base.deri
-0000e8d0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
-0000e8e0: 2020 2020 2020 2020 2023 2043 6c65 616e           # Clean
-0000e8f0: 7570 2065 7665 7279 7468 696e 672c 2065  up everything, e
-0000e900: 7370 2070 6f74 656e 7469 616c 2061 6c72  sp potential alr
-0000e910: 6561 6479 2063 6f6d 7075 7465 6420 7369  eady computed si
-0000e920: 7a65 732c 2061 7320 7468 6573 6520 6d69  zes, as these mi
-0000e930: 6768 7420 6265 2069 6e76 616c 6964 2e0a  ght be invalid..
-0000e940: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e950: 6469 6d5f 2069 6e20 5b73 656c 665f 7361  dim_ in [self_sa
-0000e960: 6d65 5f61 732c 2073 656c 665d 202b 2028  me_as, self] + (
-0000e970: 6c69 7374 2873 656c 662e 5f65 7874 7261  list(self._extra
-0000e980: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-0000e990: 6374 782e 7661 6c75 6573 2829 2920 6966  ctx.values()) if
-0000e9a0: 2073 656c 662e 5f65 7874 7261 2065 6c73   self._extra els
-0000e9b0: 6520 5b5d 293a 0a20 2020 2020 2020 2020  e []):.         
-0000e9c0: 2020 2020 2020 2069 6620 6469 6d5f 2e64         if dim_.d
-0000e9d0: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2064 696d 5f2e 6479 6e5f 7369 7a65 5f65   dim_.dyn_size_e
-0000ea00: 7874 2e70 6c61 6365 686f 6c64 6572 203d  xt.placeholder =
-0000ea10: 204e 6f6e 650a 2020 2020 2020 2020 6f74   None.        ot
-0000ea20: 6865 725f 7361 6d65 5f62 6173 652e 5f6d  her_same_base._m
-0000ea30: 6572 6765 5f73 616d 655f 666f 725f 6261  erge_same_for_ba
-0000ea40: 7463 685f 6374 785f 6469 6374 2873 656c  tch_ctx_dict(sel
-0000ea50: 6629 0a20 2020 2020 2020 206f 7468 6572  f).        other
-0000ea60: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
-0000ea70: 0a20 2020 2020 2020 2073 656c 662e 7361  .        self.sa
-0000ea80: 6d65 5f61 7320 3d20 6f74 6865 725f 7361  me_as = other_sa
-0000ea90: 6d65 5f62 6173 650a 2020 2020 2020 2020  me_base.        
-0000eaa0: 7365 6c66 2e5f 6d61 7962 655f 7570 6461  self._maybe_upda
-0000eab0: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
-0000eac0: 7365 6c66 2e64 796e 5f73 697a 6520 6973  self.dyn_size is
-0000ead0: 206e 6f74 204e 6f6e 6520 616e 6420 6f74   not None and ot
-0000eae0: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
-0000eaf0: 6e5f 7369 7a65 2069 7320 6e6f 7420 4e6f  n_size is not No
-0000eb00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000eb10: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-0000eb20: 2069 7320 6e6f 7420 6f74 6865 725f 7361   is not other_sa
-0000eb30: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
-0000eb40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eb50: 2020 6966 2073 656c 662e 6261 7463 6820    if self.batch 
-0000eb60: 3d3d 206f 7468 6572 5f73 616d 655f 6261  == other_same_ba
-0000eb70: 7365 2e62 6174 6368 2061 6e64 2073 656c  se.batch and sel
-0000eb80: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-0000eb90: 7478 203d 3d20 6f74 6865 725f 7361 6d65  tx == other_same
-0000eba0: 5f62 6173 652e 636f 6e74 726f 6c5f 666c  _base.control_fl
-0000ebb0: 6f77 5f63 7478 3a0a 2020 2020 2020 2020  ow_ctx:.        
-0000ebc0: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
-0000ebd0: 7465 3a20 496e 7374 6561 6420 6f66 206d  te: Instead of m
-0000ebe0: 616b 696e 6720 7468 6973 2061 2077 6172  aking this a war
-0000ebf0: 6e69 6e67 2c20 7765 2063 6f75 6c64 2061  ning, we could a
-0000ec00: 6c73 6f20 656e 666f 7263 6520 7468 6973  lso enforce this
-0000ec10: 2061 7420 736f 6d65 2070 6f69 6e74 2e0a   at some point..
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec30: 2020 2020 2320 2020 5468 6520 7573 6572      #   The user
-0000ec40: 2073 686f 756c 6420 6265 2061 626c 6520   should be able 
-0000ec50: 746f 2066 6978 2060 6578 7465 726e 5f64  to fix `extern_d
-0000ec60: 6174 6160 2069 6e20 7468 6520 636f 6e66  ata` in the conf
-0000ec70: 6967 0a20 2020 2020 2020 2020 2020 2020  ig.             
-0000ec80: 2020 2020 2020 2023 2020 2073 7563 6820         #   such 
-0000ec90: 7468 6174 2074 6869 7320 6973 2063 6f72  that this is cor
-0000eca0: 7265 6374 2069 6e20 7468 6520 6669 7273  rect in the firs
-0000ecb0: 7420 706c 6163 652e 0a20 2020 2020 2020  t place..       
-0000ecc0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-0000ecd0: 2041 6c73 6f2c 2069 6e20 6164 6469 7469   Also, in additi
-0000ece0: 6f6e 2074 6f20 7468 6973 2077 6172 6e69  on to this warni
-0000ecf0: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-0000ed00: 2020 2020 2020 2020 2320 2020 7765 206d          #   we m
-0000ed10: 6967 6874 2077 616e 7420 746f 2061 6464  ight want to add
-0000ed20: 2073 6f6d 6520 7275 6e74 696d 6520 6368   some runtime ch
-0000ed30: 6563 6b20 6f6e 2074 6865 2065 7120 6f66  eck on the eq of
-0000ed40: 2074 6865 2064 796e 2073 697a 6573 2e0a   the dyn sizes..
-0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed60: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
-0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed80: 2020 2022 5761 726e 696e 673a 2061 7373     "Warning: ass
-0000ed90: 756d 696e 6720 6469 6d20 7461 6773 2061  uming dim tags a
-0000eda0: 7265 2073 616d 6520 7769 7468 2064 6966  re same with dif
-0000edb0: 6665 7265 6e74 2073 697a 6520 706c 6163  ferent size plac
-0000edc0: 6568 6f6c 6465 7273 3a20 2572 2076 7320  eholders: %r vs 
-0000edd0: 2572 220a 2020 2020 2020 2020 2020 2020  %r".            
-0000ede0: 2020 2020 2020 2020 2020 2020 2520 2873              % (s
-0000edf0: 656c 662e 6479 6e5f 7369 7a65 2c20 6f74  elf.dyn_size, ot
-0000ee00: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
-0000ee10: 6e5f 7369 7a65 290a 2020 2020 2020 2020  n_size).        
-0000ee20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000ee30: 2020 2020 2020 2320 4966 2077 6520 6861        # If we ha
-0000ee40: 7665 2061 2064 6566 696e 6564 2073 6f75  ve a defined sou
-0000ee50: 7263 652c 2061 6e64 2074 6869 7320 6973  rce, and this is
-0000ee60: 2061 2064 796e 616d 6963 2073 7061 7469   a dynamic spati
-0000ee70: 616c 2061 7869 732c 2061 6e64 2069 7420  al axis, and it 
-0000ee80: 7761 7320 756e 6465 6669 6e65 6420 6265  was undefined be
-0000ee90: 666f 7265 2c0a 2020 2020 2020 2020 2320  fore,.        # 
-0000eea0: 6d61 7962 6520 7765 2063 616e 206f 7665  maybe we can ove
-0000eeb0: 7274 616b 6520 7468 6520 7369 7a65 5f70  rtake the size_p
-0000eec0: 6c61 6365 686f 6c64 6572 206e 6f77 2e0a  laceholder now..
-0000eed0: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-0000eee0: 5f73 616d 655f 6261 7365 2e64 796e 5f73  _same_base.dyn_s
-0000eef0: 697a 6520 6973 206e 6f74 204e 6f6e 6520  ize is not None 
-0000ef00: 616e 6420 7365 6c66 2e5f 6578 7472 6120  and self._extra 
-0000ef10: 616e 6420 7365 6c66 2e5f 6578 7472 612e  and self._extra.
-0000ef20: 7372 635f 6461 7461 3a0a 2020 2020 2020  src_data:.      
-0000ef30: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-0000ef40: 6e73 7461 6e63 6528 7365 6c66 2e5f 6578  nstance(self._ex
-0000ef50: 7472 612e 7372 635f 6178 6973 2c20 696e  tra.src_axis, in
-0000ef60: 7429 0a20 2020 2020 2020 2020 2020 2023  t).            #
-0000ef70: 204d 6179 6265 2069 7420 6368 616e 6765   Maybe it change
-0000ef80: 6420 696e 2074 6865 206d 6561 6e77 6869  d in the meanwhi
-0000ef90: 6c65 2c20 736f 2063 6865 636b 2e0a 2020  le, so check..  
-0000efa0: 2020 2020 2020 2020 2020 7461 6720 3d20            tag = 
-0000efb0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
-0000efc0: 6461 7461 2e67 6574 5f64 696d 5f74 6167  data.get_dim_tag
-0000efd0: 2873 656c 662e 5f65 7874 7261 2e73 7263  (self._extra.src
-0000efe0: 5f61 7869 7329 0a20 2020 2020 2020 2020  _axis).         
-0000eff0: 2020 2069 6620 7461 672e 6465 7363 7269     if tag.descri
-0000f000: 7074 696f 6e20 3d3d 2073 656c 662e 6465  ption == self.de
-0000f010: 7363 7269 7074 696f 6e20 616e 6420 286e  scription and (n
-0000f020: 6f74 2074 6167 2e64 796e 5f73 697a 655f  ot tag.dyn_size_
-0000f030: 6578 7420 6f72 206e 6f74 2074 6167 2e5f  ext or not tag._
-0000f040: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000f050: 656e 745f 6772 6170 6828 2929 3a0a 2020  ent_graph()):.  
-0000f060: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000f070: 672e 6479 6e5f 7369 7a65 5f65 7874 203d  g.dyn_size_ext =
-0000f080: 2073 656c 662e 6765 745f 6479 6e5f 7369   self.get_dyn_si
-0000f090: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000f0a0: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000f0b0: 2020 2020 2020 2020 2020 7461 672e 6261            tag.ba
-0000f0c0: 7463 682c 2074 6167 2e63 6f6e 7472 6f6c  tch, tag.control
-0000f0d0: 5f66 6c6f 775f 6374 782c 2074 656d 706c  _flow_ctx, templ
-0000f0e0: 6174 655f 6f6e 6c79 3d54 7275 650a 2020  ate_only=True.  
-0000f0f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 7461 672e 5f6d 6179 6265 5f75 7064 6174  tag._maybe_updat
-0000f120: 6528 290a 2020 2020 2020 2020 2320 4966  e().        # If
-0000f130: 206f 7468 6572 7320 6479 6e5f 7369 7a65   others dyn_size
-0000f140: 2069 7320 4e6f 6e65 2062 7574 2077 6520   is None but we 
-0000f150: 6861 7665 2061 2064 796e 5f73 697a 652c  have a dyn_size,
-0000f160: 206d 6179 6265 2075 7064 6174 6520 6f74   maybe update ot
-0000f170: 6865 7273 2064 796e 5f73 697a 652e 0a20  hers dyn_size.. 
-0000f180: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0000f190: 796e 5f73 697a 6520 6973 206e 6f74 204e  yn_size is not N
-0000f1a0: 6f6e 6520 616e 6420 6f74 6865 725f 7361  one and other_sa
-0000f1b0: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
-0000f1c0: 2069 7320 6e6f 7420 7365 6c66 2e64 796e   is not self.dyn
-0000f1d0: 5f73 697a 653a 0a20 2020 2020 2020 2020  _size:.         
-0000f1e0: 2020 2023 2043 6f75 6c64 2062 6520 756e     # Could be un
-0000f1f0: 7365 7420 6966 2069 7420 636f 6d65 7320  set if it comes 
-0000f200: 6672 6f6d 2074 6865 2063 6f6e 6669 672c  from the config,
-0000f210: 206f 7220 6672 6f6d 2070 7265 7620 6772   or from prev gr
-0000f220: 6170 6820 6372 6561 7469 6f6e 2e0a 2020  aph creation..  
-0000f230: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-0000f240: 2069 7320 696d 706f 7274 616e 7420 7375   is important su
-0000f250: 6368 2074 6861 7420 7365 6c66 2e63 616e  ch that self.can
-0000f260: 5f63 6f6d 7061 7265 2829 2069 7320 7361  _compare() is sa
-0000f270: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
-0000f280: 6966 206f 7468 6572 5f73 616d 655f 6261  if other_same_ba
-0000f290: 7365 2e64 796e 5f73 697a 6520 6973 204e  se.dyn_size is N
-0000f2a0: 6f6e 6520 6f72 206e 6f74 206f 7468 6572  one or not other
-0000f2b0: 5f73 616d 655f 6261 7365 2e5f 7661 6c69  _same_base._vali
-0000f2c0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000f2d0: 6772 6170 6828 293a 0a20 2020 2020 2020  graph():.       
-0000f2e0: 2020 2020 2020 2020 206f 7468 6572 5f73           other_s
-0000f2f0: 616d 655f 6261 7365 2e64 796e 5f73 697a  ame_base.dyn_siz
-0000f300: 655f 6578 7420 3d20 7365 6c66 2e67 6574  e_ext = self.get
-0000f310: 5f64 796e 5f73 697a 655f 6578 745f 666f  _dyn_size_ext_fo
-0000f320: 725f 6261 7463 685f 6374 7828 0a20 2020  r_batch_ctx(.   
-0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f340: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000f350: 2e62 6174 6368 2c20 6f74 6865 725f 7361  .batch, other_sa
-0000f360: 6d65 5f62 6173 652e 636f 6e74 726f 6c5f  me_base.control_
-0000f370: 666c 6f77 5f63 7478 2c20 7465 6d70 6c61  flow_ctx, templa
-0000f380: 7465 5f6f 6e6c 793d 5472 7565 0a20 2020  te_only=True.   
-0000f390: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000f3b0: 7468 6572 5f73 616d 655f 6261 7365 2e5f  ther_same_base._
-0000f3c0: 6d61 7962 655f 7570 6461 7465 2829 0a20  maybe_update(). 
-0000f3d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000f3e0: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
-0000f3f0: 6f72 206e 6f74 2073 656c 662e 5f76 616c  or not self._val
-0000f400: 6964 6174 655f 696e 5f63 7572 7265 6e74  idate_in_current
-0000f410: 5f67 7261 7068 2829 3a0a 2020 2020 2020  _graph():.      
-0000f420: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-0000f430: 697a 655f 6578 7420 3d20 6f74 6865 725f  ize_ext = other_
-0000f440: 7361 6d65 5f62 6173 652e 6765 745f 6479  same_base.get_dy
-0000f450: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
-0000f460: 6174 6368 5f63 7478 280a 2020 2020 2020  atch_ctx(.      
-0000f470: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0000f480: 6174 6368 2c20 7365 6c66 2e63 6f6e 7472  atch, self.contr
-0000f490: 6f6c 5f66 6c6f 775f 6374 782c 2074 656d  ol_flow_ctx, tem
-0000f4a0: 706c 6174 655f 6f6e 6c79 3d54 7275 650a  plate_only=True.
-0000f4b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000f4c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000f4d0: 6d61 7962 655f 7570 6461 7465 2829 0a20  maybe_update(). 
-0000f4e0: 2020 2020 2020 2065 6c69 6620 6f74 6865         elif othe
-0000f4f0: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
-0000f500: 7369 7a65 5f65 7874 2069 7320 4e6f 6e65  size_ext is None
-0000f510: 206f 7220 6e6f 7420 6f74 6865 725f 7361   or not other_sa
-0000f520: 6d65 5f62 6173 652e 5f76 616c 6964 6174  me_base._validat
-0000f530: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000f540: 7068 2829 3a0a 2020 2020 2020 2020 2020  ph():.          
-0000f550: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000f560: 652e 6479 6e5f 7369 7a65 5f65 7874 203d  e.dyn_size_ext =
-0000f570: 2073 656c 662e 6765 745f 6479 6e5f 7369   self.get_dyn_si
-0000f580: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000f590: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000f5a0: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000f5b0: 5f62 6173 652e 6261 7463 682c 206f 7468  _base.batch, oth
-0000f5c0: 6572 5f73 616d 655f 6261 7365 2e63 6f6e  er_same_base.con
-0000f5d0: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
-0000f5e0: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
-0000f5f0: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
-0000f600: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-0000f610: 725f 7361 6d65 5f62 6173 652e 5f6d 6179  r_same_base._may
-0000f620: 6265 5f75 7064 6174 6528 290a 2020 2020  be_update().    
-0000f630: 2020 2020 6966 2073 656c 662e 6973 5f64      if self.is_d
-0000f640: 696d 5f6b 6e6f 776e 2829 2061 6e64 206f  im_known() and o
-0000f650: 7468 6572 2e69 735f 6469 6d5f 6b6e 6f77  ther.is_dim_know
-0000f660: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-0000f670: 2061 7373 6572 7420 7365 6c66 2e64 696d   assert self.dim
-0000f680: 656e 7369 6f6e 203d 3d20 6f74 6865 722e  ension == other.
-0000f690: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
-0000f6a0: 2020 656c 6966 2073 656c 662e 6973 5f64    elif self.is_d
-0000f6b0: 696d 5f6b 6e6f 776e 2829 2061 6e64 206e  im_known() and n
-0000f6c0: 6f74 206f 7468 6572 2e69 735f 6469 6d5f  ot other.is_dim_
-0000f6d0: 6b6e 6f77 6e28 293a 0a20 2020 2020 2020  known():.       
-0000f6e0: 2020 2020 206f 7468 6572 2e63 6170 6163       other.capac
-0000f6f0: 6974 7920 3d20 7365 6c66 2e63 6170 6163  ity = self.capac
-0000f700: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
-0000f710: 6f74 6865 722e 7369 7a65 203d 2073 656c  other.size = sel
-0000f720: 662e 7369 7a65 0a20 2020 2020 2020 2065  f.size.        e
-0000f730: 6c69 6620 6e6f 7420 7365 6c66 2e69 735f  lif not self.is_
-0000f740: 6469 6d5f 6b6e 6f77 6e28 2920 616e 6420  dim_known() and 
-0000f750: 6f74 6865 722e 6973 5f64 696d 5f6b 6e6f  other.is_dim_kno
-0000f760: 776e 2829 3a0a 2020 2020 2020 2020 2020  wn():.          
-0000f770: 2020 7365 6c66 2e63 6170 6163 6974 7920    self.capacity 
-0000f780: 3d20 6f74 6865 722e 6361 7061 6369 7479  = other.capacity
-0000f790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f7a0: 662e 7369 7a65 203d 206f 7468 6572 2e73  f.size = other.s
-0000f7b0: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
-0000f7c0: 656c 662e 766f 6361 6220 616e 6420 6e6f  elf.vocab and no
-0000f7d0: 7420 6f74 6865 725f 7361 6d65 5f62 6173  t other_same_bas
-0000f7e0: 652e 766f 6361 623a 0a20 2020 2020 2020  e.vocab:.       
-0000f7f0: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
-0000f800: 6261 7365 2e76 6f63 6162 203d 2073 656c  base.vocab = sel
-0000f810: 662e 766f 6361 620a 2020 2020 2020 2020  f.vocab.        
-0000f820: 656c 6966 206f 7468 6572 5f73 616d 655f  elif other_same_
-0000f830: 6261 7365 2e76 6f63 6162 2061 6e64 206e  base.vocab and n
-0000f840: 6f74 2073 656c 662e 766f 6361 623a 0a20  ot self.vocab:. 
-0000f850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f860: 766f 6361 6220 3d20 6f74 6865 725f 7361  vocab = other_sa
-0000f870: 6d65 5f62 6173 652e 766f 6361 620a 2020  me_base.vocab.  
-0000f880: 2020 2020 2020 7365 6c66 2e5f 6d61 6b65        self._make
-0000f890: 5f65 7874 7261 2829 0a20 2020 2020 2020  _extra().       
-0000f8a0: 2073 656c 665f 7361 6d65 5f61 732e 5f6d   self_same_as._m
-0000f8b0: 616b 655f 6578 7472 6128 290a 2020 2020  ake_extra().    
-0000f8c0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-0000f8d0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-0000f8e0: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
-0000f8f0: 662e 5f65 7874 7261 2e61 7574 6f5f 6765  f._extra.auto_ge
-0000f900: 6e65 7261 7465 6420 3d20 7365 6c66 5f73  nerated = self_s
-0000f910: 616d 655f 6173 2e5f 6578 7472 612e 6175  ame_as._extra.au
-0000f920: 746f 5f67 656e 6572 6174 6564 203d 206f  to_generated = o
-0000f930: 7468 6572 5f73 616d 655f 6261 7365 2e61  ther_same_base.a
-0000f940: 7574 6f5f 6765 6e65 7261 7465 640a 2020  uto_generated.  
-0000f950: 2020 2020 2020 2320 5461 6b65 206f 7665        # Take ove
-0000f960: 7220 6465 7269 7665 645f 6672 6f6d 5f6f  r derived_from_o
-0000f970: 702e 2048 6f77 6576 6572 2c20 6f6e 6c79  p. However, only
-0000f980: 2069 6620 7468 6973 2077 6f75 6c64 206e   if this would n
-0000f990: 6f74 2069 6e74 726f 6475 6365 2063 7963  ot introduce cyc
-0000f9a0: 6c65 7321 0a20 2020 2020 2020 2069 6620  les!.        if 
-0000f9b0: 6e6f 7420 7365 6c66 5f64 6572 6976 6564  not self_derived
-0000f9c0: 5f62 6173 6573 2e69 7373 7570 6572 7365  _bases.issuperse
-0000f9d0: 7428 6f74 6865 725f 6465 7269 7665 645f  t(other_derived_
-0000f9e0: 6261 7365 7329 3a0a 2020 2020 2020 2020  bases):.        
-0000f9f0: 2020 2020 6966 2073 656c 662e 6465 7269      if self.deri
-0000fa00: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-0000fa10: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000fa20: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-0000fa30: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
-0000fa40: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
-0000fa50: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
-0000fa60: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
-0000fa70: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000fa80: 5f62 6173 652e 5f6d 616b 655f 6578 7472  _base._make_extr
-0000fa90: 6128 292e 6465 7269 7665 645f 6672 6f6d  a().derived_from
-0000faa0: 5f6f 7020 3d20 7365 6c66 2e64 6572 6976  _op = self.deriv
-0000fab0: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000fac0: 2020 2020 2020 2065 6c69 6620 6f74 6865         elif othe
-0000fad0: 725f 7361 6d65 5f62 6173 652e 6465 7269  r_same_base.deri
-0000fae0: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-0000faf0: 6e6f 7420 7365 6c66 2e64 6572 6976 6564  not self.derived
-0000fb00: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-0000fb10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000fb20: 6d61 6b65 5f65 7874 7261 2829 2e64 6572  make_extra().der
-0000fb30: 6976 6564 5f66 726f 6d5f 6f70 203d 206f  ived_from_op = o
-0000fb40: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
-0000fb50: 6572 6976 6564 5f66 726f 6d5f 6f70 0a20  erived_from_op. 
-0000fb60: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000fb70: 6578 7472 6120 616e 6420 6e6f 7420 6f74  extra and not ot
-0000fb80: 6865 725f 7361 6d65 5f62 6173 652e 6973  her_same_base.is
-0000fb90: 5f64 796e 616d 6963 2829 3a0a 2020 2020  _dynamic():.    
-0000fba0: 2020 2020 2020 2020 2320 5468 6f73 6520          # Those 
-0000fbb0: 6d69 6768 7420 6265 2073 6574 2076 6961  might be set via
-0000fbc0: 2067 6574 5f62 6174 6368 5f66 6f72 5f63   get_batch_for_c
-0000fbd0: 7478 2066 6f72 2061 6e20 756e 6465 6669  tx for an undefi
-0000fbe0: 6e65 6420 6469 6d2c 0a20 2020 2020 2020  ned dim,.       
-0000fbf0: 2020 2020 2023 2077 6869 6368 206e 6f77       # which now
-0000fc00: 2062 6563 6f6d 6573 2073 7461 7469 6320   becomes static 
-0000fc10: 6475 6520 746f 2060 6f74 6865 7260 2e0a  due to `other`..
-0000fc20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fc30: 2e5f 6578 7472 612e 6261 7463 6820 3d20  ._extra.batch = 
-0000fc40: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000fc50: 2073 656c 662e 5f65 7874 7261 2e63 6f6e   self._extra.con
-0000fc60: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d20  trol_flow_ctx = 
-0000fc70: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000fc80: 2066 6f72 206b 6579 2c20 6469 6d5f 2069   for key, dim_ i
-0000fc90: 6e20 7365 6c66 2e5f 6578 7472 612e 7361  n self._extra.sa
-0000fca0: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
-0000fcb0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-0000fcc0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-0000fcd0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-0000fce0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-0000fcf0: 2020 2020 2020 2020 2020 2064 696d 5f65             dim_e
-0000fd00: 7874 7261 203d 2064 696d 5f2e 5f65 7874  xtra = dim_._ext
-0000fd10: 7261 0a20 2020 2020 2020 2020 2020 2020  ra.             
-0000fd20: 2020 2069 6620 6469 6d5f 6578 7472 613a     if dim_extra:
-0000fd30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd40: 2020 2020 2064 696d 5f65 7874 7261 2e62       dim_extra.b
-0000fd50: 6174 6368 203d 204e 6f6e 650a 2020 2020  atch = None.    
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd70: 6469 6d5f 6578 7472 612e 636f 6e74 726f  dim_extra.contro
-0000fd80: 6c5f 666c 6f77 5f63 7478 203d 204e 6f6e  l_flow_ctx = Non
-0000fd90: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000fda0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
-0000fdb0: 2020 2020 2073 656c 665f 203d 2073 656c       self_ = sel
-0000fdc0: 662e 6765 745f 666f 725f 6261 7463 685f  f.get_for_batch_
-0000fdd0: 6374 7828 6261 7463 683d 7365 6c66 2e62  ctx(batch=self.b
-0000fde0: 6174 6368 2c20 6374 783d 7365 6c66 2e63  atch, ctx=self.c
-0000fdf0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7829  ontrol_flow_ctx)
-0000fe00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000fe10: 7365 6c66 5f20 6973 206e 6f74 2073 656c  self_ is not sel
-0000fe20: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-0000fe30: 2020 2073 656c 662e 636f 6e74 726f 6c5f     self.control_
-0000fe40: 666c 6f77 5f63 7478 203d 2073 656c 665f  flow_ctx = self_
-0000fe50: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000fe60: 7820 2023 206d 6967 6874 2062 6520 6469  x  # might be di
-0000fe70: 6666 6572 656e 740a 2020 2020 2020 2020  fferent.        
-0000fe80: 2020 2020 2020 2020 7365 6c66 2e64 796e          self.dyn
-0000fe90: 5f73 697a 655f 6578 7420 3d20 7365 6c66  _size_ext = self
-0000fea0: 5f2e 6479 6e5f 7369 7a65 5f65 7874 2020  _.dyn_size_ext  
-0000feb0: 2320 6d69 6768 7420 6265 2075 6e73 6574  # might be unset
-0000fec0: 0a0a 2020 2020 6465 6620 5f6d 6572 6765  ..    def _merge
-0000fed0: 5f73 616d 655f 666f 725f 6261 7463 685f  _same_for_batch_
-0000fee0: 6374 785f 6469 6374 2873 656c 663a 205f  ctx_dict(self: _
-0000fef0: 642e 4469 6d2c 206f 7468 6572 3a20 5f64  d.Dim, other: _d
-0000ff00: 2e44 696d 293a 0a20 2020 2020 2020 2022  .Dim):.        "
-0000ff10: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0000ff20: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-0000ff30: 2022 2222 0a20 2020 2020 2020 2023 206e   """.        # n
-0000ff40: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
-0000ff50: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
-0000ff60: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000ff70: 662e 5f65 7874 7261 2061 6e64 206e 6f74  f._extra and not
-0000ff80: 206f 7468 6572 2e5f 6578 7472 613a 0a20   other._extra:. 
-0000ff90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ffa0: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
-0000ffb0: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000ffc0: 656e 745f 6772 6170 6828 290a 2020 2020  ent_graph().    
-0000ffd0: 2020 2020 6966 2073 656c 662e 5f65 7874      if self._ext
-0000ffe0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
-0000fff0: 666f 7220 5f2c 2064 696d 2069 6e20 6c69  for _, dim in li
-00010000: 7374 2873 656c 662e 5f65 7874 7261 2e73  st(self._extra.s
-00010010: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
-00010020: 782e 6974 656d 7328 2929 3a0a 2020 2020  x.items()):.    
-00010030: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00010040: 7274 2069 7369 6e73 7461 6e63 6528 6469  rt isinstance(di
-00010050: 6d2c 205f 642e 4469 6d29 0a20 2020 2020  m, _d.Dim).     
-00010060: 2020 2020 2020 2020 2020 2064 696d 2e5f             dim._
-00010070: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-00010080: 656e 745f 6772 6170 6828 290a 2020 2020  ent_graph().    
-00010090: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-000100a0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-000100b0: 6d62 6572 0a20 2020 2020 2020 2069 6620  mber.        if 
-000100c0: 6f74 6865 722e 5f65 7874 7261 3a0a 2020  other._extra:.  
-000100d0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-000100e0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-000100f0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-00010100: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
-00010110: 6469 6d20 696e 206f 7468 6572 2e5f 6578  dim in other._ex
-00010120: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
-00010130: 6368 5f63 7478 2e69 7465 6d73 2829 3a0a  ch_ctx.items():.
-00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010150: 6966 206e 6f74 2064 696d 2e5f 7661 6c69  if not dim._vali
-00010160: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-00010170: 6772 6170 6828 293a 0a20 2020 2020 2020  graph():.       
-00010180: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00010190: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-000101a0: 2020 2020 2020 7365 6c66 5f64 696d 203d        self_dim =
-000101b0: 2073 656c 662e 5f6d 616b 655f 6578 7472   self._make_extr
-000101c0: 6128 292e 7361 6d65 5f66 6f72 5f62 6174  a().same_for_bat
-000101d0: 6368 5f63 7478 2e67 6574 286b 6579 2c20  ch_ctx.get(key, 
-000101e0: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
-000101f0: 2020 2020 2020 6966 2073 656c 665f 6469        if self_di
-00010200: 6d20 616e 6420 2873 656c 665f 6469 6d2e  m and (self_dim.
-00010210: 6479 6e5f 7369 7a65 5f65 7874 206f 7220  dyn_size_ext or 
-00010220: 6e6f 7420 6469 6d2e 6479 6e5f 7369 7a65  not dim.dyn_size
-00010230: 5f65 7874 293a 0a20 2020 2020 2020 2020  _ext):.         
-00010240: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00010250: 6e75 6520 2023 206b 6565 7020 6f75 7273  nue  # keep ours
-00010260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010270: 2069 6620 6e6f 7420 6469 6d2e 6479 6e5f   if not dim.dyn_
-00010280: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-00010290: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000102a0: 6e74 696e 7565 2020 2320 756e 6465 6669  ntinue  # undefi
-000102b0: 6e65 642c 2064 6f20 6e6f 7420 6f76 6572  ned, do not over
-000102c0: 7461 6b65 0a20 2020 2020 2020 2020 2020  take.           
-000102d0: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
-000102e0: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-000102f0: 6374 785b 6b65 795d 203d 2064 696d 0a20  ctx[key] = dim. 
-00010300: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
-00010310: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-00010320: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-00010330: 2020 2020 2020 2020 6f74 6865 722e 5f65          other._e
-00010340: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
-00010350: 7463 685f 6374 782e 636c 6561 7228 2920  tch_ctx.clear() 
-00010360: 2023 2077 6520 6f6e 6c79 2077 616e 7420   # we only want 
-00010370: 746f 2068 6176 6520 6974 206f 6e63 650a  to have it once.
-00010380: 0a20 2020 2023 206e 6f69 6e73 7065 6374  .    # noinspect
-00010390: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
-000103a0: 656d 6265 720a 2020 2020 6465 6620 6465  ember.    def de
-000103b0: 7269 7665 5f66 726f 6d28 7365 6c66 3a20  rive_from(self: 
-000103c0: 5f64 2e44 696d 2c20 6261 7365 3a20 5f64  _d.Dim, base: _d
-000103d0: 2e44 696d 2c20 7365 745f 6465 7269 7665  .Dim, set_derive
-000103e0: 645f 6672 6f6d 5f66 6c61 673a 2062 6f6f  d_from_flag: boo
-000103f0: 6c20 3d20 5472 7565 293a 0a20 2020 2020  l = True):.     
-00010400: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00010410: 7061 7261 6d20 6261 7365 3a20 6469 6d0a  param base: dim.
-00010420: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00010430: 6574 5f64 6572 6976 6564 5f66 726f 6d5f  et_derived_from_
-00010440: 666c 6167 3a0a 2020 2020 2020 2020 2222  flag:.        ""
-00010450: 220a 2020 2020 2020 2020 7365 6c66 5f62  ".        self_b
-00010460: 6173 6520 3d20 7365 6c66 2e67 6574 5f73  ase = self.get_s
-00010470: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
-00010480: 2020 2073 656c 665f 6261 7365 5f65 7874     self_base_ext
-00010490: 7261 203d 2073 656c 665f 6261 7365 2e5f  ra = self_base._
-000104a0: 6d61 6b65 5f65 7874 7261 2829 0a20 2020  make_extra().   
-000104b0: 2020 2020 2069 6620 7365 745f 6465 7269       if set_deri
-000104c0: 7665 645f 6672 6f6d 5f66 6c61 673a 0a20  ved_from_flag:. 
-000104d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000104e0: 6c66 5f62 6173 655f 6578 7472 612e 6465  lf_base_extra.de
-000104f0: 7269 7665 645f 6672 6f6d 5f74 6167 3a0a  rived_from_tag:.
-00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 6173 7365 7274 2073 656c 665f 6261 7365  assert self_base
-00010520: 5f65 7874 7261 2e64 6572 6976 6564 5f66  _extra.derived_f
-00010530: 726f 6d5f 7461 6720 3d3d 2062 6173 650a  rom_tag == base.
-00010540: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00010550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010560: 2020 7365 6c66 5f62 6173 655f 6578 7472    self_base_extr
-00010570: 612e 6465 7269 7665 645f 6672 6f6d 5f74  a.derived_from_t
-00010580: 6167 203d 2062 6173 650a 2020 2020 2020  ag = base.      
-00010590: 2020 6966 2073 656c 662e 6973 5f64 796e    if self.is_dyn
-000105a0: 616d 6963 2829 206f 7220 6e6f 7420 7365  amic() or not se
-000105b0: 6c66 2e69 735f 6469 6d5f 6b6e 6f77 6e28  lf.is_dim_known(
-000105c0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-000105d0: 6620 6e6f 7420 7365 6c66 2e62 6174 6368  f not self.batch
-000105e0: 2061 6e64 2062 6173 652e 6261 7463 683a   and base.batch:
-000105f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010600: 2073 656c 662e 6261 7463 6820 3d20 6261   self.batch = ba
-00010610: 7365 2e62 6174 6368 0a20 2020 2020 2020  se.batch.       
-00010620: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00010630: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
-00010640: 2062 6173 652e 636f 6e74 726f 6c5f 666c   base.control_fl
-00010650: 6f77 5f63 7478 0a20 2020 2020 2020 2020  ow_ctx.         
-00010660: 2020 2020 2020 206b 6579 203d 2062 6173         key = bas
-00010670: 652e 6261 7463 682c 2062 6173 652e 636f  e.batch, base.co
-00010680: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a20  ntrol_flow_ctx. 
-00010690: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000106a0: 7373 6572 7420 6b65 7920 6e6f 7420 696e  ssert key not in
-000106b0: 2073 656c 665f 6261 7365 5f65 7874 7261   self_base_extra
-000106c0: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-000106d0: 6374 780a 2020 2020 2020 2020 2020 2020  ctx.            
-000106e0: 2020 2020 7365 6c66 5f62 6173 655f 6578      self_base_ex
-000106f0: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
-00010700: 6368 5f63 7478 5b6b 6579 5d20 3d20 7365  ch_ctx[key] = se
-00010710: 6c66 0a20 2020 2020 2020 2020 2020 2069  lf.            i
-00010720: 6620 6e6f 7420 7365 6c66 2e64 796e 5f73  f not self.dyn_s
-00010730: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-00010740: 2020 2020 2020 2020 2069 6620 6261 7365           if base
-00010750: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 2069 6620 6261 7365 2e62 6174 6368     if base.batch
-00010780: 2061 6e64 2062 6173 652e 6261 7463 6820   and base.batch 
-00010790: 3d3d 2073 656c 662e 6261 7463 6820 616e  == self.batch an
-000107a0: 6420 6261 7365 2e63 6f6e 7472 6f6c 5f66  d base.control_f
-000107b0: 6c6f 775f 6374 7820 3d3d 2073 656c 662e  low_ctx == self.
-000107c0: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-000107d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000107e0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000107f0: 796e 5f73 697a 655f 6578 7420 3d20 6261  yn_size_ext = ba
-00010800: 7365 2e64 796e 5f73 697a 655f 6578 742e  se.dyn_size_ext.
-00010810: 636f 7079 5f74 656d 706c 6174 6528 6e61  copy_template(na
-00010820: 6d65 3d22 2573 3a73 697a 6522 2025 2073  me="%s:size" % s
-00010830: 656c 665f 6261 7365 2e64 6573 6372 6970  elf_base.descrip
-00010840: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-00010850: 2020 2020 2020 656c 6966 2062 6173 652e        elif base.
-00010860: 6973 5f62 6174 6368 5f64 696d 2829 3a0a  is_batch_dim():.
-00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010880: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
-00010890: 655f 6578 7420 3d20 5f74 2e54 656e 736f  e_ext = _t.Tenso
-000108a0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-000108b0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-000108c0: 2225 733a 6261 7463 6822 2025 2073 656c  "%s:batch" % sel
-000108d0: 665f 6261 7365 2e64 6573 6372 6970 7469  f_base.descripti
-000108e0: 6f6e 2c20 7368 6170 653d 2829 2c20 6474  on, shape=(), dt
-000108f0: 7970 653d 2269 6e74 3332 222c 2062 6174  ype="int32", bat
-00010900: 6368 5f64 696d 5f61 7869 733d 4e6f 6e65  ch_dim_axis=None
-00010910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010920: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00010930: 636f 7079 5f66 726f 6d28 7365 6c66 3a20  copy_from(self: 
-00010940: 4469 6d2c 206f 7468 6572 3a20 4469 6d29  Dim, other: Dim)
-00010950: 3a0a 2020 2020 2020 2020 2222 2264 6566  :.        """def
-00010960: 696e 6522 2222 0a20 2020 2020 2020 2073  ine""".        s
-00010970: 656c 662e 7369 7a65 203d 206f 7468 6572  elf.size = other
-00010980: 2e73 697a 650a 2020 2020 2020 2020 7365  .size.        se
-00010990: 6c66 2e63 6170 6163 6974 7920 3d20 6f74  lf.capacity = ot
-000109a0: 6865 722e 6361 7061 6369 7479 0a20 2020  her.capacity.   
-000109b0: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
-000109c0: 7a65 5f65 7874 203d 206f 7468 6572 2e64  ze_ext = other.d
-000109d0: 796e 5f73 697a 655f 6578 740a 2020 2020  yn_size_ext.    
-000109e0: 2020 2020 7365 6c66 2e64 6572 6976 655f      self.derive_
-000109f0: 6672 6f6d 286f 7468 6572 290a 0a20 2020  from(other)..   
-00010a00: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00010a10: 2020 6465 6620 6765 745f 6578 6973 7469    def get_existi
-00010a20: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
-00010a30: 6563 7469 6f6e 2863 6c73 2c20 6f74 6865  ection(cls, othe
-00010a40: 722c 2074 6167 732c 2069 735f 6571 7561  r, tags, is_equa
-00010a50: 6c5f 6f70 7473 3d4e 6f6e 6529 3a0a 2020  l_opts=None):.  
-00010a60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010a70: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
-00010a80: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
-00010a90: 616d 206c 6973 745b 4469 6d5d 7c74 7570  am list[Dim]|tup
-00010aa0: 6c65 5b44 696d 5d7c 7365 745b 4469 6d5d  le[Dim]|set[Dim]
-00010ab0: 2074 6167 733a 0a20 2020 2020 2020 203a   tags:.        :
-00010ac0: 7061 7261 6d20 6469 6374 5b73 7472 5d7c  param dict[str]|
-00010ad0: 4e6f 6e65 2069 735f 6571 7561 6c5f 6f70  None is_equal_op
-00010ae0: 7473 3a20 7061 7373 6564 2074 6f20 4469  ts: passed to Di
-00010af0: 6d2e 6973 5f65 7175 616c 0a20 2020 2020  m.is_equal.     
-00010b00: 2020 203a 7274 7970 653a 2044 696d 7c4e     :rtype: Dim|N
-00010b10: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-00010b20: 2020 2020 2020 2020 6966 2069 735f 6571          if is_eq
-00010b30: 7561 6c5f 6f70 7473 2069 7320 4e6f 6e65  ual_opts is None
-00010b40: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
-00010b50: 5f65 7175 616c 5f6f 7074 7320 3d20 7b7d  _equal_opts = {}
-00010b60: 0a20 2020 2020 2020 2023 2057 6520 646f  .        # We do
-00010b70: 2070 6f74 656e 7469 616c 206d 756c 7469   potential multi
-00010b80: 706c 6520 726f 756e 6473 2c20 7375 6368  ple rounds, such
-00010b90: 2074 6861 7420 7765 2070 7265 6665 7220   that we prefer 
-00010ba0: 226d 6f72 6520 6571 7561 6c22 2028 7573  "more equal" (us
-00010bb0: 696e 6720 6c65 7373 2069 735f 6571 7561  ing less is_equa
-00010bc0: 6c5f 6f70 7473 292e 0a20 2020 2020 2020  l_opts)..       
-00010bd0: 2072 6f75 6e64 7320 3d20 5b7b 7d5d 0a20   rounds = [{}]. 
-00010be0: 2020 2020 2020 2069 6620 6973 5f65 7175         if is_equ
-00010bf0: 616c 5f6f 7074 733a 0a20 2020 2020 2020  al_opts:.       
-00010c00: 2020 2020 2069 6620 2262 726f 6164 6361       if "broadca
-00010c10: 7374 5f6d 6174 6368 6573 2220 696e 2069  st_matches" in i
-00010c20: 735f 6571 7561 6c5f 6f70 7473 3a0a 2020  s_equal_opts:.  
-00010c30: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00010c40: 756e 6473 2e61 7070 656e 6428 7b6b 3a20  unds.append({k: 
-00010c50: 7620 666f 7220 286b 2c20 7629 2069 6e20  v for (k, v) in 
-00010c60: 6973 5f65 7175 616c 5f6f 7074 732e 6974  is_equal_opts.it
-00010c70: 656d 7328 2920 6966 206b 2021 3d20 2262  ems() if k != "b
-00010c80: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-00010c90: 227d 290a 2020 2020 2020 2020 2020 2020  "}).            
-00010ca0: 726f 756e 6473 2e61 7070 656e 6428 6973  rounds.append(is
-00010cb0: 5f65 7175 616c 5f6f 7074 7329 0a20 2020  _equal_opts).   
-00010cc0: 2020 2020 2066 6f72 205f 6973 5f65 7175       for _is_equ
-00010cd0: 616c 5f6f 7074 7320 696e 2072 6f75 6e64  al_opts in round
-00010ce0: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00010cf0: 6f72 205f 7461 6720 696e 2074 6167 733a  or _tag in tags:
-00010d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d10: 2069 6620 5f74 6167 2e69 735f 6571 7561   if _tag.is_equa
-00010d20: 6c28 6f74 6865 722c 202a 2a5f 6973 5f65  l(other, **_is_e
-00010d30: 7175 616c 5f6f 7074 7329 3a0a 2020 2020  qual_opts):.    
-00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 7265 7475 726e 205f 7461 670a 2020 2020  return _tag.    
-00010d60: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00010d70: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00010d80: 640a 2020 2020 6465 6620 6765 745f 616c  d.    def get_al
-00010d90: 6c5f 6469 6d65 6e73 696f 6e5f 7461 6773  l_dimension_tags
-00010da0: 2863 6c73 2c20 6461 7461 5f6c 6973 742c  (cls, data_list,
-00010db0: 2069 735f 6571 7561 6c5f 6f70 7473 3d4e   is_equal_opts=N
-00010dc0: 6f6e 652c 2075 6e69 7175 655f 7365 7061  one, unique_sepa
-00010dd0: 7261 7465 5f61 7865 733d 5472 7565 293a  rate_axes=True):
-00010de0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010df0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
-00010e00: 5b5f 742e 5465 6e73 6f72 5d20 6461 7461  [_t.Tensor] data
-00010e10: 5f6c 6973 743a 0a20 2020 2020 2020 203a  _list:.        :
-00010e20: 7061 7261 6d20 6469 6374 5b73 7472 5d7c  param dict[str]|
-00010e30: 4e6f 6e65 2069 735f 6571 7561 6c5f 6f70  None is_equal_op
-00010e40: 7473 3a20 7061 7373 6564 2074 6f20 4469  ts: passed to Di
-00010e50: 6d2e 6973 5f65 7175 616c 0a20 2020 2020  m.is_equal.     
-00010e60: 2020 203a 7061 7261 6d20 626f 6f6c 2075     :param bool u
-00010e70: 6e69 7175 655f 7365 7061 7261 7465 5f61  nique_separate_a
-00010e80: 7865 733a 2065 2e67 2e20 6461 7461 5f6c  xes: e.g. data_l
-00010e90: 6973 743d 5b44 6174 6120 7769 7468 2073  ist=[Data with s
-00010ea0: 6861 7065 2028 422c 352c 352c 3130 295d  hape (B,5,5,10)]
-00010eb0: 2072 6573 756c 7473 2069 6e20 3420 6469   results in 4 di
-00010ec0: 6d20 7461 6773 2c20 6e6f 7420 332e 0a20  m tags, not 3.. 
-00010ed0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00010ee0: 6c69 7374 206f 6620 6469 6d65 6e73 696f  list of dimensio
-00010ef0: 6e20 7461 6773 2c20 6469 6374 2066 6f72  n tags, dict for
-00010f00: 2064 6174 6120 2d3e 206c 6973 7420 6f66   data -> list of
-00010f10: 2064 696d 656e 7369 6f6e 2074 6167 7320   dimension tags 
-00010f20: 2866 6f72 2065 6163 6820 6178 6973 290a  (for each axis).
-00010f30: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00010f40: 286c 6973 745b 4469 6d5d 2c20 7574 696c  (list[Dim], util
-00010f50: 2e44 6963 7452 6566 4b65 7973 5b5f 742e  .DictRefKeys[_t.
-00010f60: 5465 6e73 6f72 2c20 6c69 7374 5b44 696d  Tensor, list[Dim
-00010f70: 5d5d 290a 2020 2020 2020 2020 2222 220a  ]]).        """.
-00010f80: 2020 2020 2020 2020 7461 6773 203d 205b          tags = [
-00010f90: 5d0a 2020 2020 2020 2020 6461 7461 5f61  ].        data_a
-00010fa0: 7865 735f 6469 6374 203d 2075 7469 6c2e  xes_dict = util.
-00010fb0: 4469 6374 5265 664b 6579 7328 2920 2023  DictRefKeys()  #
-00010fc0: 2074 7970 653a 2075 7469 6c2e 4469 6374   type: util.Dict
-00010fd0: 5265 664b 6579 735b 5f74 2e54 656e 736f  RefKeys[_t.Tenso
-00010fe0: 722c 204c 6973 745b 4469 6d5d 5d0a 2020  r, List[Dim]].  
-00010ff0: 2020 2020 2020 666f 7220 6461 7461 2069        for data i
-00011000: 6e20 6461 7461 5f6c 6973 743a 0a20 2020  n data_list:.   
-00011010: 2020 2020 2020 2020 2064 6174 615f 6178           data_ax
-00011020: 6573 5f64 6963 745b 6461 7461 5d20 3d20  es_dict[data] = 
-00011030: 5b5d 0a20 2020 2020 2020 2020 2020 2065  [].            e
-00011040: 7869 7374 696e 675f 7461 675f 636f 6c6c  xisting_tag_coll
-00011050: 6563 7469 6f6e 5f66 6f72 5f64 6174 6120  ection_for_data 
-00011060: 3d20 6c69 7374 2874 6167 7329 2069 6620  = list(tags) if 
-00011070: 756e 6971 7565 5f73 6570 6172 6174 655f  unique_separate_
-00011080: 6178 6573 2065 6c73 6520 7461 6773 0a20  axes else tags. 
-00011090: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
-000110a0: 7869 7320 696e 2072 616e 6765 2864 6174  xis in range(dat
-000110b0: 612e 6261 7463 685f 6e64 696d 293a 0a20  a.batch_ndim):. 
-000110c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000110d0: 6167 203d 2064 6174 612e 6765 745f 6469  ag = data.get_di
-000110e0: 6d5f 7461 6728 6178 6973 290a 2020 2020  m_tag(axis).    
-000110f0: 2020 2020 2020 2020 2020 2020 6578 6973              exis
-00011100: 7469 6e67 5f74 6167 203d 2063 6c73 2e67  ting_tag = cls.g
-00011110: 6574 5f65 7869 7374 696e 675f 7461 675f  et_existing_tag_
-00011120: 6672 6f6d 5f63 6f6c 6c65 6374 696f 6e28  from_collection(
-00011130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011140: 2020 2020 2074 6167 2c20 7461 6773 3d65       tag, tags=e
-00011150: 7869 7374 696e 675f 7461 675f 636f 6c6c  xisting_tag_coll
-00011160: 6563 7469 6f6e 5f66 6f72 5f64 6174 612c  ection_for_data,
-00011170: 2069 735f 6571 7561 6c5f 6f70 7473 3d69   is_equal_opts=i
-00011180: 735f 6571 7561 6c5f 6f70 7473 0a20 2020  s_equal_opts.   
-00011190: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000111b0: 6620 6578 6973 7469 6e67 5f74 6167 3a0a  f existing_tag:.
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 2020 6966 2075 6e69 7175 655f 7365      if unique_se
-000111e0: 7061 7261 7465 5f61 7865 733a 0a20 2020  parate_axes:.   
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 2020 2020 2065 7869 7374 696e 675f 7461       existing_ta
-00011210: 675f 636f 6c6c 6563 7469 6f6e 5f66 6f72  g_collection_for
-00011220: 5f64 6174 612e 7265 6d6f 7665 2865 7869  _data.remove(exi
-00011230: 7374 696e 675f 7461 6729 2020 2320 646f  sting_tag)  # do
-00011240: 6e27 7420 7461 6b65 2069 7420 6167 6169  n't take it agai
-00011250: 6e20 666f 7220 7468 6973 2064 6174 610a  n for this data.
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 2020 2020 7265 706c 6163 655f 6578 6973      replace_exis
-00011280: 7469 6e67 203d 2028 0a20 2020 2020 2020  ting = (.       
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2065 7869 7374 696e 675f 7461 672e 756e   existing_tag.un
-000112b0: 6465 6669 6e65 6420 616e 6420 6e6f 7420  defined and not 
-000112c0: 7461 672e 756e 6465 6669 6e65 6420 616e  tag.undefined an
-000112d0: 6420 7461 672e 6469 6d65 6e73 696f 6e20  d tag.dimension 
-000112e0: 3d3d 2065 7869 7374 696e 675f 7461 672e  == existing_tag.
-000112f0: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
-00011300: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 6966 2072 6570 6c61 6365 5f65      if replace_e
-00011330: 7869 7374 696e 673a 2020 2320 5265 706c  xisting:  # Repl
-00011340: 6163 6520 7468 6520 6578 6973 7469 6e67  ace the existing
-00011350: 2062 7920 7468 6520 6e65 7720 7461 672e   by the new tag.
-00011360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011370: 2020 2020 2020 2020 2074 6167 735b 7461           tags[ta
-00011380: 6773 2e69 6e64 6578 2865 7869 7374 696e  gs.index(existin
-00011390: 675f 7461 6729 5d20 3d20 7461 670a 2020  g_tag)] = tag.  
+0000e730: 2020 6469 6d5f 2e5f 6578 7472 612e 6465    dim_._extra.de
+0000e740: 7269 7665 645f 6672 6f6d 5f74 6167 203d  rived_from_tag =
+0000e750: 204e 6f6e 650a 2020 2020 2020 2020 2320   None.        # 
+0000e760: 4e6f 7720 6d65 7267 6520 6578 6973 7469  Now merge existi
+0000e770: 6e67 2076 6172 6961 6e74 732e 2042 7574  ng variants. But
+0000e780: 206f 6e6c 7920 6966 206e 6f74 2064 6572   only if not der
+0000e790: 6976 6564 2076 6961 206f 702c 2062 6563  ived via op, bec
+0000e7a0: 6175 7365 2069 6e20 7468 6174 2063 6173  ause in that cas
+0000e7b0: 652c 2077 6520 6361 6e20 2861 6e64 2073  e, we can (and s
+0000e7c0: 686f 756c 6421 290a 2020 2020 2020 2020  hould!).        
+0000e7d0: 2320 6175 746f 6d61 7469 6361 6c6c 7920  # automatically 
+0000e7e0: 696e 6665 7220 6974 2e20 4e6f 7465 2074  infer it. Note t
+0000e7f0: 6861 7420 7765 206f 6e6c 7920 676f 7420  hat we only got 
+0000e800: 6865 7265 2077 6865 6e20 7468 6520 6f74  here when the ot
+0000e810: 6865 7220 6973 206e 6f74 2074 6865 2073  her is not the s
+0000e820: 616d 6520 6469 6d2c 2073 6f20 6974 206d  ame dim, so it m
+0000e830: 6561 6e73 2074 6861 740a 2020 2020 2020  eans that.      
+0000e840: 2020 2320 7468 6520 6f74 6865 7220 6973    # the other is
+0000e850: 2072 6561 6c6c 7920 6469 6666 6572 656e   really differen
+0000e860: 742c 2074 6865 2073 697a 6573 2061 7265  t, the sizes are
+0000e870: 2070 6f74 656e 7469 616c 6c79 2064 6966   potentially dif
+0000e880: 6665 7265 6e74 2c20 6275 7420 7765 2077  ferent, but we w
+0000e890: 616e 7420 746f 206f 7665 7274 616b 6520  ant to overtake 
+0000e8a0: 7468 6520 6f74 6865 722e 0a20 2020 2020  the other..     
+0000e8b0: 2020 2069 6620 6f74 6865 725f 7361 6d65     if other_same
+0000e8c0: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
+0000e8d0: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
+0000e8e0: 2020 2023 2043 6c65 616e 7570 2065 7665     # Cleanup eve
+0000e8f0: 7279 7468 696e 672c 2065 7370 2070 6f74  rything, esp pot
+0000e900: 656e 7469 616c 2061 6c72 6561 6479 2063  ential already c
+0000e910: 6f6d 7075 7465 6420 7369 7a65 732c 2061  omputed sizes, a
+0000e920: 7320 7468 6573 6520 6d69 6768 7420 6265  s these might be
+0000e930: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
+0000e940: 2020 2020 2020 666f 7220 6469 6d5f 2069        for dim_ i
+0000e950: 6e20 5b73 656c 665f 7361 6d65 5f61 732c  n [self_same_as,
+0000e960: 2073 656c 665d 202b 2028 6c69 7374 2873   self] + (list(s
+0000e970: 656c 662e 5f65 7874 7261 2e73 616d 655f  elf._extra.same_
+0000e980: 666f 725f 6261 7463 685f 6374 782e 7661  for_batch_ctx.va
+0000e990: 6c75 6573 2829 2920 6966 2073 656c 662e  lues()) if self.
+0000e9a0: 5f65 7874 7261 2065 6c73 6520 5b5d 293a  _extra else []):
+0000e9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9c0: 2069 6620 6469 6d5f 2e64 796e 5f73 697a   if dim_.dyn_siz
+0000e9d0: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
+0000e9e0: 2020 2020 2020 2020 2020 2064 696d 5f2e             dim_.
+0000e9f0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+0000ea00: 6365 686f 6c64 6572 203d 204e 6f6e 650a  ceholder = None.
+0000ea10: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
+0000ea20: 6d65 5f62 6173 652e 5f6d 6572 6765 5f73  me_base._merge_s
+0000ea30: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
+0000ea40: 785f 6469 6374 2873 656c 6629 0a20 2020  x_dict(self).   
+0000ea50: 2020 2020 206f 7468 6572 2e5f 6d61 7962       other._mayb
+0000ea60: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
+0000ea70: 2020 2073 656c 662e 7361 6d65 5f61 7320     self.same_as 
+0000ea80: 3d20 6f74 6865 725f 7361 6d65 5f62 6173  = other_same_bas
+0000ea90: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000eaa0: 6d61 7962 655f 7570 6461 7465 2829 0a20  maybe_update(). 
+0000eab0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000eac0: 796e 5f73 697a 6520 6973 206e 6f74 204e  yn_size is not N
+0000ead0: 6f6e 6520 616e 6420 6f74 6865 725f 7361  one and other_sa
+0000eae0: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
+0000eaf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000eb00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000eb10: 662e 6479 6e5f 7369 7a65 2069 7320 6e6f  f.dyn_size is no
+0000eb20: 7420 6f74 6865 725f 7361 6d65 5f62 6173  t other_same_bas
+0000eb30: 652e 6479 6e5f 7369 7a65 3a0a 2020 2020  e.dyn_size:.    
+0000eb40: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000eb50: 656c 662e 6261 7463 6820 3d3d 206f 7468  elf.batch == oth
+0000eb60: 6572 5f73 616d 655f 6261 7365 2e62 6174  er_same_base.bat
+0000eb70: 6368 2061 6e64 2073 656c 662e 636f 6e74  ch and self.cont
+0000eb80: 726f 6c5f 666c 6f77 5f63 7478 203d 3d20  rol_flow_ctx == 
+0000eb90: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000eba0: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+0000ebb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ebc0: 2020 2020 2020 2320 4e6f 7465 3a20 496e        # Note: In
+0000ebd0: 7374 6561 6420 6f66 206d 616b 696e 6720  stead of making 
+0000ebe0: 7468 6973 2061 2077 6172 6e69 6e67 2c20  this a warning, 
+0000ebf0: 7765 2063 6f75 6c64 2061 6c73 6f20 656e  we could also en
+0000ec00: 666f 7263 6520 7468 6973 2061 7420 736f  force this at so
+0000ec10: 6d65 2070 6f69 6e74 2e0a 2020 2020 2020  me point..      
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000ec30: 2020 5468 6520 7573 6572 2073 686f 756c    The user shoul
+0000ec40: 6420 6265 2061 626c 6520 746f 2066 6978  d be able to fix
+0000ec50: 2060 6578 7465 726e 5f64 6174 6160 2069   `extern_data` i
+0000ec60: 6e20 7468 6520 636f 6e66 6967 0a20 2020  n the config.   
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec80: 2023 2020 2073 7563 6820 7468 6174 2074   #   such that t
+0000ec90: 6869 7320 6973 2063 6f72 7265 6374 2069  his is correct i
+0000eca0: 6e20 7468 6520 6669 7273 7420 706c 6163  n the first plac
+0000ecb0: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000ecc0: 2020 2020 2020 2023 2020 2041 6c73 6f2c         #   Also,
+0000ecd0: 2069 6e20 6164 6469 7469 6f6e 2074 6f20   in addition to 
+0000ece0: 7468 6973 2077 6172 6e69 6e67 2c0a 2020  this warning,.  
+0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed00: 2020 2320 2020 7765 206d 6967 6874 2077    #   we might w
+0000ed10: 616e 7420 746f 2061 6464 2073 6f6d 6520  ant to add some 
+0000ed20: 7275 6e74 696d 6520 6368 6563 6b20 6f6e  runtime check on
+0000ed30: 2074 6865 2065 7120 6f66 2074 6865 2064   the eq of the d
+0000ed40: 796e 2073 697a 6573 2e0a 2020 2020 2020  yn sizes..      
+0000ed50: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000ed60: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+0000ed70: 2020 2020 2020 2020 2020 2020 2022 5761               "Wa
+0000ed80: 726e 696e 673a 2061 7373 756d 696e 6720  rning: assuming 
+0000ed90: 6469 6d20 7461 6773 2061 7265 2073 616d  dim tags are sam
+0000eda0: 6520 7769 7468 2064 6966 6665 7265 6e74  e with different
+0000edb0: 2073 697a 6520 706c 6163 6568 6f6c 6465   size placeholde
+0000edc0: 7273 3a20 2572 2076 7320 2572 220a 2020  rs: %r vs %r".  
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ede0: 2020 2020 2020 2520 2873 656c 662e 6479        % (self.dy
+0000edf0: 6e5f 7369 7a65 2c20 6f74 6865 725f 7361  n_size, other_sa
+0000ee00: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
+0000ee10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ee20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000ee30: 2320 4966 2077 6520 6861 7665 2061 2064  # If we have a d
+0000ee40: 6566 696e 6564 2073 6f75 7263 652c 2061  efined source, a
+0000ee50: 6e64 2074 6869 7320 6973 2061 2064 796e  nd this is a dyn
+0000ee60: 616d 6963 2073 7061 7469 616c 2061 7869  amic spatial axi
+0000ee70: 732c 2061 6e64 2069 7420 7761 7320 756e  s, and it was un
+0000ee80: 6465 6669 6e65 6420 6265 666f 7265 2c0a  defined before,.
+0000ee90: 2020 2020 2020 2020 2320 6d61 7962 6520          # maybe 
+0000eea0: 7765 2063 616e 206f 7665 7274 616b 6520  we can overtake 
+0000eeb0: 7468 6520 7369 7a65 5f70 6c61 6365 686f  the size_placeho
+0000eec0: 6c64 6572 206e 6f77 2e0a 2020 2020 2020  lder now..      
+0000eed0: 2020 6966 206f 7468 6572 5f73 616d 655f    if other_same_
+0000eee0: 6261 7365 2e64 796e 5f73 697a 6520 6973  base.dyn_size is
+0000eef0: 206e 6f74 204e 6f6e 6520 616e 6420 7365   not None and se
+0000ef00: 6c66 2e5f 6578 7472 6120 616e 6420 7365  lf._extra and se
+0000ef10: 6c66 2e5f 6578 7472 612e 7372 635f 6461  lf._extra.src_da
+0000ef20: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+0000ef30: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+0000ef40: 6528 7365 6c66 2e5f 6578 7472 612e 7372  e(self._extra.sr
+0000ef50: 635f 6178 6973 2c20 696e 7429 0a20 2020  c_axis, int).   
+0000ef60: 2020 2020 2020 2020 2023 204d 6179 6265           # Maybe
+0000ef70: 2069 7420 6368 616e 6765 6420 696e 2074   it changed in t
+0000ef80: 6865 206d 6561 6e77 6869 6c65 2c20 736f  he meanwhile, so
+0000ef90: 2063 6865 636b 2e0a 2020 2020 2020 2020   check..        
+0000efa0: 2020 2020 7461 6720 3d20 7365 6c66 2e5f      tag = self._
+0000efb0: 6578 7472 612e 7372 635f 6461 7461 2e67  extra.src_data.g
+0000efc0: 6574 5f64 696d 5f74 6167 2873 656c 662e  et_dim_tag(self.
+0000efd0: 5f65 7874 7261 2e73 7263 5f61 7869 7329  _extra.src_axis)
+0000efe0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000eff0: 7461 672e 6465 7363 7269 7074 696f 6e20  tag.description 
+0000f000: 3d3d 2073 656c 662e 6465 7363 7269 7074  == self.descript
+0000f010: 696f 6e20 616e 6420 286e 6f74 2074 6167  ion and (not tag
+0000f020: 2e64 796e 5f73 697a 655f 6578 7420 6f72  .dyn_size_ext or
+0000f030: 206e 6f74 2074 6167 2e5f 7661 6c69 6461   not tag._valida
+0000f040: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
+0000f050: 6170 6828 2929 3a0a 2020 2020 2020 2020  aph()):.        
+0000f060: 2020 2020 2020 2020 7461 672e 6479 6e5f          tag.dyn_
+0000f070: 7369 7a65 5f65 7874 203d 2073 656c 662e  size_ext = self.
+0000f080: 6765 745f 6479 6e5f 7369 7a65 5f65 7874  get_dyn_size_ext
+0000f090: 5f66 6f72 5f62 6174 6368 5f63 7478 280a  _for_batch_ctx(.
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0b0: 2020 2020 7461 672e 6261 7463 682c 2074      tag.batch, t
+0000f0c0: 6167 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  ag.control_flow_
+0000f0d0: 6374 782c 2074 656d 706c 6174 655f 6f6e  ctx, template_on
+0000f0e0: 6c79 3d54 7275 650a 2020 2020 2020 2020  ly=True.        
+0000f0f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f100: 2020 2020 2020 2020 2020 7461 672e 5f6d            tag._m
+0000f110: 6179 6265 5f75 7064 6174 6528 290a 2020  aybe_update().  
+0000f120: 2020 2020 2020 2320 4966 206f 7468 6572        # If other
+0000f130: 7320 6479 6e5f 7369 7a65 2069 7320 4e6f  s dyn_size is No
+0000f140: 6e65 2062 7574 2077 6520 6861 7665 2061  ne but we have a
+0000f150: 2064 796e 5f73 697a 652c 206d 6179 6265   dyn_size, maybe
+0000f160: 2075 7064 6174 6520 6f74 6865 7273 2064   update others d
+0000f170: 796e 5f73 697a 652e 0a20 2020 2020 2020  yn_size..       
+0000f180: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+0000f190: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
+0000f1a0: 6420 6f74 6865 725f 7361 6d65 5f62 6173  d other_same_bas
+0000f1b0: 652e 6479 6e5f 7369 7a65 2069 7320 6e6f  e.dyn_size is no
+0000f1c0: 7420 7365 6c66 2e64 796e 5f73 697a 653a  t self.dyn_size:
+0000f1d0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000f1e0: 6f75 6c64 2062 6520 756e 7365 7420 6966  ould be unset if
+0000f1f0: 2069 7420 636f 6d65 7320 6672 6f6d 2074   it comes from t
+0000f200: 6865 2063 6f6e 6669 672c 206f 7220 6672  he config, or fr
+0000f210: 6f6d 2070 7265 7620 6772 6170 6820 6372  om prev graph cr
+0000f220: 6561 7469 6f6e 2e0a 2020 2020 2020 2020  eation..        
+0000f230: 2020 2020 2320 5468 6973 2069 7320 696d      # This is im
+0000f240: 706f 7274 616e 7420 7375 6368 2074 6861  portant such tha
+0000f250: 7420 7365 6c66 2e63 616e 5f63 6f6d 7061  t self.can_compa
+0000f260: 7265 2829 2069 7320 7361 6e65 2e0a 2020  re() is sane..  
+0000f270: 2020 2020 2020 2020 2020 6966 206f 7468            if oth
+0000f280: 6572 5f73 616d 655f 6261 7365 2e64 796e  er_same_base.dyn
+0000f290: 5f73 697a 6520 6973 204e 6f6e 6520 6f72  _size is None or
+0000f2a0: 206e 6f74 206f 7468 6572 5f73 616d 655f   not other_same_
+0000f2b0: 6261 7365 2e5f 7661 6c69 6461 7465 5f69  base._validate_i
+0000f2c0: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000f2d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000f2e0: 2020 206f 7468 6572 5f73 616d 655f 6261     other_same_ba
+0000f2f0: 7365 2e64 796e 5f73 697a 655f 6578 7420  se.dyn_size_ext 
+0000f300: 3d20 7365 6c66 2e67 6574 5f64 796e 5f73  = self.get_dyn_s
+0000f310: 697a 655f 6578 745f 666f 725f 6261 7463  ize_ext_for_batc
+0000f320: 685f 6374 7828 0a20 2020 2020 2020 2020  h_ctx(.         
+0000f330: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000f340: 5f73 616d 655f 6261 7365 2e62 6174 6368  _same_base.batch
+0000f350: 2c20 6f74 6865 725f 7361 6d65 5f62 6173  , other_same_bas
+0000f360: 652e 636f 6e74 726f 6c5f 666c 6f77 5f63  e.control_flow_c
+0000f370: 7478 2c20 7465 6d70 6c61 7465 5f6f 6e6c  tx, template_onl
+0000f380: 793d 5472 7565 0a20 2020 2020 2020 2020  y=True.         
+0000f390: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000f3a0: 2020 2020 2020 2020 206f 7468 6572 5f73           other_s
+0000f3b0: 616d 655f 6261 7365 2e5f 6d61 7962 655f  ame_base._maybe_
+0000f3c0: 7570 6461 7465 2829 0a20 2020 2020 2020  update().       
+0000f3d0: 2069 6620 6e6f 7420 7365 6c66 2e64 796e   if not self.dyn
+0000f3e0: 5f73 697a 655f 6578 7420 6f72 206e 6f74  _size_ext or not
+0000f3f0: 2073 656c 662e 5f76 616c 6964 6174 655f   self._validate_
+0000f400: 696e 5f63 7572 7265 6e74 5f67 7261 7068  in_current_graph
+0000f410: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000f420: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+0000f430: 7420 3d20 6f74 6865 725f 7361 6d65 5f62  t = other_same_b
+0000f440: 6173 652e 6765 745f 6479 6e5f 7369 7a65  ase.get_dyn_size
+0000f450: 5f65 7874 5f66 6f72 5f62 6174 6368 5f63  _ext_for_batch_c
+0000f460: 7478 280a 2020 2020 2020 2020 2020 2020  tx(.            
+0000f470: 2020 2020 7365 6c66 2e62 6174 6368 2c20      self.batch, 
+0000f480: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
+0000f490: 775f 6374 782c 2074 656d 706c 6174 655f  w_ctx, template_
+0000f4a0: 6f6e 6c79 3d54 7275 650a 2020 2020 2020  only=True.      
+0000f4b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000f4c0: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
+0000f4d0: 7570 6461 7465 2829 0a20 2020 2020 2020  update().       
+0000f4e0: 2065 6c69 6620 6f74 6865 725f 7361 6d65   elif other_same
+0000f4f0: 5f62 6173 652e 6479 6e5f 7369 7a65 5f65  _base.dyn_size_e
+0000f500: 7874 2069 7320 4e6f 6e65 206f 7220 6e6f  xt is None or no
+0000f510: 7420 6f74 6865 725f 7361 6d65 5f62 6173  t other_same_bas
+0000f520: 652e 5f76 616c 6964 6174 655f 696e 5f63  e._validate_in_c
+0000f530: 7572 7265 6e74 5f67 7261 7068 2829 3a0a  urrent_graph():.
+0000f540: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000f550: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
+0000f560: 7369 7a65 5f65 7874 203d 2073 656c 662e  size_ext = self.
+0000f570: 6765 745f 6479 6e5f 7369 7a65 5f65 7874  get_dyn_size_ext
+0000f580: 5f66 6f72 5f62 6174 6368 5f63 7478 280a  _for_batch_ctx(.
+0000f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5a0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000f5b0: 6261 7463 682c 206f 7468 6572 5f73 616d  batch, other_sam
+0000f5c0: 655f 6261 7365 2e63 6f6e 7472 6f6c 5f66  e_base.control_f
+0000f5d0: 6c6f 775f 6374 782c 2074 656d 706c 6174  low_ctx, templat
+0000f5e0: 655f 6f6e 6c79 3d54 7275 650a 2020 2020  e_only=True.    
+0000f5f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f600: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
+0000f610: 5f62 6173 652e 5f6d 6179 6265 5f75 7064  _base._maybe_upd
+0000f620: 6174 6528 290a 2020 2020 2020 2020 6966  ate().        if
+0000f630: 2073 656c 662e 6973 5f64 696d 5f6b 6e6f   self.is_dim_kno
+0000f640: 776e 2829 2061 6e64 206f 7468 6572 2e69  wn() and other.i
+0000f650: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
+0000f660: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000f670: 7420 7365 6c66 2e64 696d 656e 7369 6f6e  t self.dimension
+0000f680: 203d 3d20 6f74 6865 722e 6469 6d65 6e73   == other.dimens
+0000f690: 696f 6e0a 2020 2020 2020 2020 656c 6966  ion.        elif
+0000f6a0: 2073 656c 662e 6973 5f64 696d 5f6b 6e6f   self.is_dim_kno
+0000f6b0: 776e 2829 2061 6e64 206e 6f74 206f 7468  wn() and not oth
+0000f6c0: 6572 2e69 735f 6469 6d5f 6b6e 6f77 6e28  er.is_dim_known(
+0000f6d0: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
+0000f6e0: 7468 6572 2e63 6170 6163 6974 7920 3d20  ther.capacity = 
+0000f6f0: 7365 6c66 2e63 6170 6163 6974 790a 2020  self.capacity.  
+0000f700: 2020 2020 2020 2020 2020 6f74 6865 722e            other.
+0000f710: 7369 7a65 203d 2073 656c 662e 7369 7a65  size = self.size
+0000f720: 0a20 2020 2020 2020 2065 6c69 6620 6e6f  .        elif no
+0000f730: 7420 7365 6c66 2e69 735f 6469 6d5f 6b6e  t self.is_dim_kn
+0000f740: 6f77 6e28 2920 616e 6420 6f74 6865 722e  own() and other.
+0000f750: 6973 5f64 696d 5f6b 6e6f 776e 2829 3a0a  is_dim_known():.
+0000f760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f770: 2e63 6170 6163 6974 7920 3d20 6f74 6865  .capacity = othe
+0000f780: 722e 6361 7061 6369 7479 0a20 2020 2020  r.capacity.     
+0000f790: 2020 2020 2020 2073 656c 662e 7369 7a65         self.size
+0000f7a0: 203d 206f 7468 6572 2e73 697a 650a 2020   = other.size.  
+0000f7b0: 2020 2020 2020 6966 2073 656c 662e 766f        if self.vo
+0000f7c0: 6361 6220 616e 6420 6e6f 7420 6f74 6865  cab and not othe
+0000f7d0: 725f 7361 6d65 5f62 6173 652e 766f 6361  r_same_base.voca
+0000f7e0: 623a 0a20 2020 2020 2020 2020 2020 206f  b:.            o
+0000f7f0: 7468 6572 5f73 616d 655f 6261 7365 2e76  ther_same_base.v
+0000f800: 6f63 6162 203d 2073 656c 662e 766f 6361  ocab = self.voca
+0000f810: 620a 2020 2020 2020 2020 656c 6966 206f  b.        elif o
+0000f820: 7468 6572 5f73 616d 655f 6261 7365 2e76  ther_same_base.v
+0000f830: 6f63 6162 2061 6e64 206e 6f74 2073 656c  ocab and not sel
+0000f840: 662e 766f 6361 623a 0a20 2020 2020 2020  f.vocab:.       
+0000f850: 2020 2020 2073 656c 662e 766f 6361 6220       self.vocab 
+0000f860: 3d20 6f74 6865 725f 7361 6d65 5f62 6173  = other_same_bas
+0000f870: 652e 766f 6361 620a 2020 2020 2020 2020  e.vocab.        
+0000f880: 7365 6c66 2e5f 6d61 6b65 5f65 7874 7261  self._make_extra
+0000f890: 2829 0a20 2020 2020 2020 2073 656c 665f  ().        self_
+0000f8a0: 7361 6d65 5f61 732e 5f6d 616b 655f 6578  same_as._make_ex
+0000f8b0: 7472 6128 290a 2020 2020 2020 2020 2320  tra().        # 
+0000f8c0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+0000f8d0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+0000f8e0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
+0000f8f0: 7261 2e61 7574 6f5f 6765 6e65 7261 7465  ra.auto_generate
+0000f900: 6420 3d20 7365 6c66 5f73 616d 655f 6173  d = self_same_as
+0000f910: 2e5f 6578 7472 612e 6175 746f 5f67 656e  ._extra.auto_gen
+0000f920: 6572 6174 6564 203d 206f 7468 6572 5f73  erated = other_s
+0000f930: 616d 655f 6261 7365 2e61 7574 6f5f 6765  ame_base.auto_ge
+0000f940: 6e65 7261 7465 640a 2020 2020 2020 2020  nerated.        
+0000f950: 2320 5461 6b65 206f 7665 7220 6465 7269  # Take over deri
+0000f960: 7665 645f 6672 6f6d 5f6f 702e 2048 6f77  ved_from_op. How
+0000f970: 6576 6572 2c20 6f6e 6c79 2069 6620 7468  ever, only if th
+0000f980: 6973 2077 6f75 6c64 206e 6f74 2069 6e74  is would not int
+0000f990: 726f 6475 6365 2063 7963 6c65 7321 0a20  roduce cycles!. 
+0000f9a0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000f9b0: 6c66 5f64 6572 6976 6564 5f62 6173 6573  lf_derived_bases
+0000f9c0: 2e69 7373 7570 6572 7365 7428 6f74 6865  .issuperset(othe
+0000f9d0: 725f 6465 7269 7665 645f 6261 7365 7329  r_derived_bases)
+0000f9e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000f9f0: 2073 656c 662e 6465 7269 7665 645f 6672   self.derived_fr
+0000fa00: 6f6d 5f6f 7020 616e 6420 6e6f 7420 6f74  om_op and not ot
+0000fa10: 6865 725f 7361 6d65 5f62 6173 652e 6465  her_same_base.de
+0000fa20: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000fa40: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+0000fa50: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa70: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000fa80: 5f6d 616b 655f 6578 7472 6128 292e 6465  _make_extra().de
+0000fa90: 7269 7665 645f 6672 6f6d 5f6f 7020 3d20  rived_from_op = 
+0000faa0: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
+0000fab0: 6d5f 6f70 0a20 2020 2020 2020 2020 2020  m_op.           
+0000fac0: 2065 6c69 6620 6f74 6865 725f 7361 6d65   elif other_same
+0000fad0: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
+0000fae0: 6f6d 5f6f 7020 616e 6420 6e6f 7420 7365  om_op and not se
+0000faf0: 6c66 2e64 6572 6976 6564 5f66 726f 6d5f  lf.derived_from_
+0000fb00: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+0000fb10: 2020 2020 7365 6c66 2e5f 6d61 6b65 5f65      self._make_e
+0000fb20: 7874 7261 2829 2e64 6572 6976 6564 5f66  xtra().derived_f
+0000fb30: 726f 6d5f 6f70 203d 206f 7468 6572 5f73  rom_op = other_s
+0000fb40: 616d 655f 6261 7365 2e64 6572 6976 6564  ame_base.derived
+0000fb50: 5f66 726f 6d5f 6f70 0a20 2020 2020 2020  _from_op.       
+0000fb60: 2069 6620 7365 6c66 2e5f 6578 7472 6120   if self._extra 
+0000fb70: 616e 6420 6e6f 7420 6f74 6865 725f 7361  and not other_sa
+0000fb80: 6d65 5f62 6173 652e 6973 5f64 796e 616d  me_base.is_dynam
+0000fb90: 6963 2829 3a0a 2020 2020 2020 2020 2020  ic():.          
+0000fba0: 2020 2320 5468 6f73 6520 6d69 6768 7420    # Those might 
+0000fbb0: 6265 2073 6574 2076 6961 2067 6574 5f62  be set via get_b
+0000fbc0: 6174 6368 5f66 6f72 5f63 7478 2066 6f72  atch_for_ctx for
+0000fbd0: 2061 6e20 756e 6465 6669 6e65 6420 6469   an undefined di
+0000fbe0: 6d2c 0a20 2020 2020 2020 2020 2020 2023  m,.            #
+0000fbf0: 2077 6869 6368 206e 6f77 2062 6563 6f6d   which now becom
+0000fc00: 6573 2073 7461 7469 6320 6475 6520 746f  es static due to
+0000fc10: 2060 6f74 6865 7260 2e0a 2020 2020 2020   `other`..      
+0000fc20: 2020 2020 2020 7365 6c66 2e5f 6578 7472        self._extr
+0000fc30: 612e 6261 7463 6820 3d20 4e6f 6e65 0a20  a.batch = None. 
+0000fc40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fc50: 5f65 7874 7261 2e63 6f6e 7472 6f6c 5f66  _extra.control_f
+0000fc60: 6c6f 775f 6374 7820 3d20 4e6f 6e65 0a20  low_ctx = None. 
+0000fc70: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+0000fc80: 6579 2c20 6469 6d5f 2069 6e20 7365 6c66  ey, dim_ in self
+0000fc90: 2e5f 6578 7472 612e 7361 6d65 5f66 6f72  ._extra.same_for
+0000fca0: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
+0000fcb0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000fcc0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+0000fcd0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+0000fce0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+0000fcf0: 2020 2020 2064 696d 5f65 7874 7261 203d       dim_extra =
+0000fd00: 2064 696d 5f2e 5f65 7874 7261 0a20 2020   dim_._extra.   
+0000fd10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000fd20: 6469 6d5f 6578 7472 613a 0a20 2020 2020  dim_extra:.     
+0000fd30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000fd40: 696d 5f65 7874 7261 2e62 6174 6368 203d  im_extra.batch =
+0000fd50: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000fd60: 2020 2020 2020 2020 2020 6469 6d5f 6578            dim_ex
+0000fd70: 7472 612e 636f 6e74 726f 6c5f 666c 6f77  tra.control_flow
+0000fd80: 5f63 7478 203d 204e 6f6e 650a 2020 2020  _ctx = None.    
+0000fd90: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
+0000fda0: 683a 0a20 2020 2020 2020 2020 2020 2073  h:.            s
+0000fdb0: 656c 665f 203d 2073 656c 662e 6765 745f  elf_ = self.get_
+0000fdc0: 666f 725f 6261 7463 685f 6374 7828 6261  for_batch_ctx(ba
+0000fdd0: 7463 683d 7365 6c66 2e62 6174 6368 2c20  tch=self.batch, 
+0000fde0: 6374 783d 7365 6c66 2e63 6f6e 7472 6f6c  ctx=self.control
+0000fdf0: 5f66 6c6f 775f 6374 7829 0a20 2020 2020  _flow_ctx).     
+0000fe00: 2020 2020 2020 2069 6620 7365 6c66 5f20         if self_ 
+0000fe10: 6973 206e 6f74 2073 656c 663a 0a20 2020  is not self:.   
+0000fe20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fe30: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+0000fe40: 7478 203d 2073 656c 665f 2e63 6f6e 7472  tx = self_.contr
+0000fe50: 6f6c 5f66 6c6f 775f 6374 7820 2023 206d  ol_flow_ctx  # m
+0000fe60: 6967 6874 2062 6520 6469 6666 6572 656e  ight be differen
+0000fe70: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000fe80: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+0000fe90: 6578 7420 3d20 7365 6c66 5f2e 6479 6e5f  ext = self_.dyn_
+0000fea0: 7369 7a65 5f65 7874 2020 2320 6d69 6768  size_ext  # migh
+0000feb0: 7420 6265 2075 6e73 6574 0a0a 2020 2020  t be unset..    
+0000fec0: 6465 6620 5f6d 6572 6765 5f73 616d 655f  def _merge_same_
+0000fed0: 666f 725f 6261 7463 685f 6374 785f 6469  for_batch_ctx_di
+0000fee0: 6374 2873 656c 663a 205f 642e 4469 6d2c  ct(self: _d.Dim,
+0000fef0: 206f 7468 6572 3a20 5f64 2e44 696d 293a   other: _d.Dim):
+0000ff00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ff10: 2020 2020 203a 7061 7261 6d20 6f74 6865       :param othe
+0000ff20: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+0000ff30: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
+0000ff40: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+0000ff50: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
+0000ff60: 6966 206e 6f74 2073 656c 662e 5f65 7874  if not self._ext
+0000ff70: 7261 2061 6e64 206e 6f74 206f 7468 6572  ra and not other
+0000ff80: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+0000ff90: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000ffa0: 2020 2020 7365 6c66 2e5f 7661 6c69 6461      self._valida
+0000ffb0: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
+0000ffc0: 6170 6828 290a 2020 2020 2020 2020 6966  aph().        if
+0000ffd0: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
+0000ffe0: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
+0000fff0: 2064 696d 2069 6e20 6c69 7374 2873 656c   dim in list(sel
+00010000: 662e 5f65 7874 7261 2e73 616d 655f 666f  f._extra.same_fo
+00010010: 725f 6261 7463 685f 6374 782e 6974 656d  r_batch_ctx.item
+00010020: 7328 2929 3a0a 2020 2020 2020 2020 2020  s()):.          
+00010030: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+00010040: 6e73 7461 6e63 6528 6469 6d2c 205f 642e  nstance(dim, _d.
+00010050: 4469 6d29 0a20 2020 2020 2020 2020 2020  Dim).           
+00010060: 2020 2020 2064 696d 2e5f 7661 6c69 6461       dim._valida
+00010070: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
+00010080: 6170 6828 290a 2020 2020 2020 2020 2320  aph().        # 
+00010090: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+000100a0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+000100b0: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+000100c0: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
+000100d0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+000100e0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+000100f0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+00010100: 2066 6f72 206b 6579 2c20 6469 6d20 696e   for key, dim in
+00010110: 206f 7468 6572 2e5f 6578 7472 612e 7361   other._extra.sa
+00010120: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
+00010130: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00010140: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00010150: 2064 696d 2e5f 7661 6c69 6461 7465 5f69   dim._validate_i
+00010160: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+00010170: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010180: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 7365 6c66 5f64 696d 203d 2073 656c 662e  self_dim = self.
+000101b0: 5f6d 616b 655f 6578 7472 6128 292e 7361  _make_extra().sa
+000101c0: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
+000101d0: 2e67 6574 286b 6579 2c20 4e6f 6e65 290a  .get(key, None).
+000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101f0: 6966 2073 656c 665f 6469 6d20 616e 6420  if self_dim and 
+00010200: 2873 656c 665f 6469 6d2e 6479 6e5f 7369  (self_dim.dyn_si
+00010210: 7a65 5f65 7874 206f 7220 6e6f 7420 6469  ze_ext or not di
+00010220: 6d2e 6479 6e5f 7369 7a65 5f65 7874 293a  m.dyn_size_ext):
+00010230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010240: 2020 2020 2063 6f6e 7469 6e75 6520 2023       continue  #
+00010250: 206b 6565 7020 6f75 7273 0a20 2020 2020   keep ours.     
+00010260: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00010270: 7420 6469 6d2e 6479 6e5f 7369 7a65 5f65  t dim.dyn_size_e
+00010280: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+00010290: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+000102a0: 2020 2320 756e 6465 6669 6e65 642c 2064    # undefined, d
+000102b0: 6f20 6e6f 7420 6f76 6572 7461 6b65 0a20  o not overtake. 
+000102c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000102d0: 656c 662e 5f65 7874 7261 2e73 616d 655f  elf._extra.same_
+000102e0: 666f 725f 6261 7463 685f 6374 785b 6b65  for_batch_ctx[ke
+000102f0: 795d 203d 2064 696d 0a20 2020 2020 2020  y] = dim.       
+00010300: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
+00010310: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
+00010320: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
+00010330: 2020 6f74 6865 722e 5f65 7874 7261 2e73    other._extra.s
+00010340: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
+00010350: 782e 636c 6561 7228 2920 2023 2077 6520  x.clear()  # we 
+00010360: 6f6e 6c79 2077 616e 7420 746f 2068 6176  only want to hav
+00010370: 6520 6974 206f 6e63 650a 0a20 2020 2023  e it once..    #
+00010380: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+00010390: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+000103a0: 2020 2020 6465 6620 6465 7269 7665 5f66      def derive_f
+000103b0: 726f 6d28 7365 6c66 3a20 5f64 2e44 696d  rom(self: _d.Dim
+000103c0: 2c20 6261 7365 3a20 5f64 2e44 696d 2c20  , base: _d.Dim, 
+000103d0: 7365 745f 6465 7269 7665 645f 6672 6f6d  set_derived_from
+000103e0: 5f66 6c61 673a 2062 6f6f 6c20 3d20 5472  _flag: bool = Tr
+000103f0: 7565 293a 0a20 2020 2020 2020 2022 2222  ue):.        """
+00010400: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010410: 6261 7365 3a20 6469 6d0a 2020 2020 2020  base: dim.      
+00010420: 2020 3a70 6172 616d 2073 6574 5f64 6572    :param set_der
+00010430: 6976 6564 5f66 726f 6d5f 666c 6167 3a0a  ived_from_flag:.
+00010440: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010450: 2020 2020 7365 6c66 5f62 6173 6520 3d20      self_base = 
+00010460: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
+00010470: 7365 2829 0a20 2020 2020 2020 2073 656c  se().        sel
+00010480: 665f 6261 7365 5f65 7874 7261 203d 2073  f_base_extra = s
+00010490: 656c 665f 6261 7365 2e5f 6d61 6b65 5f65  elf_base._make_e
+000104a0: 7874 7261 2829 0a20 2020 2020 2020 2069  xtra().        i
+000104b0: 6620 7365 745f 6465 7269 7665 645f 6672  f set_derived_fr
+000104c0: 6f6d 5f66 6c61 673a 0a20 2020 2020 2020  om_flag:.       
+000104d0: 2020 2020 2069 6620 7365 6c66 5f62 6173       if self_bas
+000104e0: 655f 6578 7472 612e 6465 7269 7665 645f  e_extra.derived_
+000104f0: 6672 6f6d 5f74 6167 3a0a 2020 2020 2020  from_tag:.      
+00010500: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00010510: 2073 656c 665f 6261 7365 5f65 7874 7261   self_base_extra
+00010520: 2e64 6572 6976 6564 5f66 726f 6d5f 7461  .derived_from_ta
+00010530: 6720 3d3d 2062 6173 650a 2020 2020 2020  g == base.      
+00010540: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010560: 5f62 6173 655f 6578 7472 612e 6465 7269  _base_extra.deri
+00010570: 7665 645f 6672 6f6d 5f74 6167 203d 2062  ved_from_tag = b
+00010580: 6173 650a 2020 2020 2020 2020 6966 2073  ase.        if s
+00010590: 656c 662e 6973 5f64 796e 616d 6963 2829  elf.is_dynamic()
+000105a0: 206f 7220 6e6f 7420 7365 6c66 2e69 735f   or not self.is_
+000105b0: 6469 6d5f 6b6e 6f77 6e28 293a 0a20 2020  dim_known():.   
+000105c0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000105d0: 7365 6c66 2e62 6174 6368 2061 6e64 2062  self.batch and b
+000105e0: 6173 652e 6261 7463 683a 0a20 2020 2020  ase.batch:.     
+000105f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010600: 6261 7463 6820 3d20 6261 7365 2e62 6174  batch = base.bat
+00010610: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
+00010620: 2020 2073 656c 662e 636f 6e74 726f 6c5f     self.control_
+00010630: 666c 6f77 5f63 7478 203d 2062 6173 652e  flow_ctx = base.
+00010640: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00010650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010660: 206b 6579 203d 2062 6173 652e 6261 7463   key = base.batc
+00010670: 682c 2062 6173 652e 636f 6e74 726f 6c5f  h, base.control_
+00010680: 666c 6f77 5f63 7478 0a20 2020 2020 2020  flow_ctx.       
+00010690: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000106a0: 6b65 7920 6e6f 7420 696e 2073 656c 665f  key not in self_
+000106b0: 6261 7365 5f65 7874 7261 2e73 616d 655f  base_extra.same_
+000106c0: 666f 725f 6261 7463 685f 6374 780a 2020  for_batch_ctx.  
+000106d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000106e0: 6c66 5f62 6173 655f 6578 7472 612e 7361  lf_base_extra.sa
+000106f0: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
+00010700: 5b6b 6579 5d20 3d20 7365 6c66 0a20 2020  [key] = self.   
+00010710: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00010720: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00010730: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00010740: 2020 2069 6620 6261 7365 2e64 796e 5f73     if base.dyn_s
+00010750: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
+00010760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010770: 6261 7365 2e62 6174 6368 2061 6e64 2062  base.batch and b
+00010780: 6173 652e 6261 7463 6820 3d3d 2073 656c  ase.batch == sel
+00010790: 662e 6261 7463 6820 616e 6420 6261 7365  f.batch and base
+000107a0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+000107b0: 7820 3d3d 2073 656c 662e 636f 6e74 726f  x == self.contro
+000107c0: 6c5f 666c 6f77 5f63 7478 3a0a 2020 2020  l_flow_ctx:.    
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107e0: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
+000107f0: 655f 6578 7420 3d20 6261 7365 2e64 796e  e_ext = base.dyn
+00010800: 5f73 697a 655f 6578 742e 636f 7079 5f74  _size_ext.copy_t
+00010810: 656d 706c 6174 6528 6e61 6d65 3d22 2573  emplate(name="%s
+00010820: 3a73 697a 6522 2025 2073 656c 665f 6261  :size" % self_ba
+00010830: 7365 2e64 6573 6372 6970 7469 6f6e 290a  se.description).
+00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010850: 656c 6966 2062 6173 652e 6973 5f62 6174  elif base.is_bat
+00010860: 6368 5f64 696d 2829 3a0a 2020 2020 2020  ch_dim():.      
+00010870: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010880: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
+00010890: 3d20 5f74 2e54 656e 736f 7228 0a20 2020  = _t.Tensor(.   
+000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108b0: 2020 2020 206e 616d 653d 2225 733a 6261       name="%s:ba
+000108c0: 7463 6822 2025 2073 656c 665f 6261 7365  tch" % self_base
+000108d0: 2e64 6573 6372 6970 7469 6f6e 2c20 7368  .description, sh
+000108e0: 6170 653d 2829 2c20 6474 7970 653d 2269  ape=(), dtype="i
+000108f0: 6e74 3332 222c 2062 6174 6368 5f64 696d  nt32", batch_dim
+00010900: 5f61 7869 733d 4e6f 6e65 0a20 2020 2020  _axis=None.     
+00010910: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010920: 0a0a 2020 2020 6465 6620 636f 7079 5f66  ..    def copy_f
+00010930: 726f 6d28 7365 6c66 3a20 4469 6d2c 206f  rom(self: Dim, o
+00010940: 7468 6572 3a20 4469 6d29 3a0a 2020 2020  ther: Dim):.    
+00010950: 2020 2020 2222 2264 6566 696e 6522 2222      """define"""
+00010960: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
+00010970: 7a65 203d 206f 7468 6572 2e73 697a 650a  ze = other.size.
+00010980: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
+00010990: 6163 6974 7920 3d20 6f74 6865 722e 6361  acity = other.ca
+000109a0: 7061 6369 7479 0a20 2020 2020 2020 2073  pacity.        s
+000109b0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+000109c0: 203d 206f 7468 6572 2e64 796e 5f73 697a   = other.dyn_siz
+000109d0: 655f 6578 740a 2020 2020 2020 2020 7365  e_ext.        se
+000109e0: 6c66 2e64 6572 6976 655f 6672 6f6d 286f  lf.derive_from(o
+000109f0: 7468 6572 290a 0a20 2020 2040 636c 6173  ther)..    @clas
+00010a00: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00010a10: 6765 745f 6578 6973 7469 6e67 5f74 6167  get_existing_tag
+00010a20: 5f66 726f 6d5f 636f 6c6c 6563 7469 6f6e  _from_collection
+00010a30: 2863 6c73 2c20 6f74 6865 722c 2074 6167  (cls, other, tag
+00010a40: 732c 2069 735f 6571 7561 6c5f 6f70 7473  s, is_equal_opts
+00010a50: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00010a60: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00010a70: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
+00010a80: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
+00010a90: 745b 4469 6d5d 7c74 7570 6c65 5b44 696d  t[Dim]|tuple[Dim
+00010aa0: 5d7c 7365 745b 4469 6d5d 2074 6167 733a  ]|set[Dim] tags:
+00010ab0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010ac0: 6469 6374 5b73 7472 5d7c 4e6f 6e65 2069  dict[str]|None i
+00010ad0: 735f 6571 7561 6c5f 6f70 7473 3a20 7061  s_equal_opts: pa
+00010ae0: 7373 6564 2074 6f20 4469 6d2e 6973 5f65  ssed to Dim.is_e
+00010af0: 7175 616c 0a20 2020 2020 2020 203a 7274  qual.        :rt
+00010b00: 7970 653a 2044 696d 7c4e 6f6e 650a 2020  ype: Dim|None.  
+00010b10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010b20: 2020 6966 2069 735f 6571 7561 6c5f 6f70    if is_equal_op
+00010b30: 7473 2069 7320 4e6f 6e65 3a0a 2020 2020  ts is None:.    
+00010b40: 2020 2020 2020 2020 6973 5f65 7175 616c          is_equal
+00010b50: 5f6f 7074 7320 3d20 7b7d 0a20 2020 2020  _opts = {}.     
+00010b60: 2020 2023 2057 6520 646f 2070 6f74 656e     # We do poten
+00010b70: 7469 616c 206d 756c 7469 706c 6520 726f  tial multiple ro
+00010b80: 756e 6473 2c20 7375 6368 2074 6861 7420  unds, such that 
+00010b90: 7765 2070 7265 6665 7220 226d 6f72 6520  we prefer "more 
+00010ba0: 6571 7561 6c22 2028 7573 696e 6720 6c65  equal" (using le
+00010bb0: 7373 2069 735f 6571 7561 6c5f 6f70 7473  ss is_equal_opts
+00010bc0: 292e 0a20 2020 2020 2020 2072 6f75 6e64  )..        round
+00010bd0: 7320 3d20 5b7b 7d5d 0a20 2020 2020 2020  s = [{}].       
+00010be0: 2069 6620 6973 5f65 7175 616c 5f6f 7074   if is_equal_opt
+00010bf0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00010c00: 6620 2262 726f 6164 6361 7374 5f6d 6174  f "broadcast_mat
+00010c10: 6368 6573 2220 696e 2069 735f 6571 7561  ches" in is_equa
+00010c20: 6c5f 6f70 7473 3a0a 2020 2020 2020 2020  l_opts:.        
+00010c30: 2020 2020 2020 2020 726f 756e 6473 2e61          rounds.a
+00010c40: 7070 656e 6428 7b6b 3a20 7620 666f 7220  ppend({k: v for 
+00010c50: 286b 2c20 7629 2069 6e20 6973 5f65 7175  (k, v) in is_equ
+00010c60: 616c 5f6f 7074 732e 6974 656d 7328 2920  al_opts.items() 
+00010c70: 6966 206b 2021 3d20 2262 726f 6164 6361  if k != "broadca
+00010c80: 7374 5f6d 6174 6368 6573 227d 290a 2020  st_matches"}).  
+00010c90: 2020 2020 2020 2020 2020 726f 756e 6473            rounds
+00010ca0: 2e61 7070 656e 6428 6973 5f65 7175 616c  .append(is_equal
+00010cb0: 5f6f 7074 7329 0a20 2020 2020 2020 2066  _opts).        f
+00010cc0: 6f72 205f 6973 5f65 7175 616c 5f6f 7074  or _is_equal_opt
+00010cd0: 7320 696e 2072 6f75 6e64 733a 0a20 2020  s in rounds:.   
+00010ce0: 2020 2020 2020 2020 2066 6f72 205f 7461           for _ta
+00010cf0: 6720 696e 2074 6167 733a 0a20 2020 2020  g in tags:.     
+00010d00: 2020 2020 2020 2020 2020 2069 6620 5f74             if _t
+00010d10: 6167 2e69 735f 6571 7561 6c28 6f74 6865  ag.is_equal(othe
+00010d20: 722c 202a 2a5f 6973 5f65 7175 616c 5f6f  r, **_is_equal_o
+00010d30: 7074 7329 3a0a 2020 2020 2020 2020 2020  pts):.          
+00010d40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010d50: 205f 7461 670a 2020 2020 2020 2020 7265   _tag.        re
+00010d60: 7475 726e 204e 6f6e 650a 0a20 2020 2040  turn None..    @
+00010d70: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00010d80: 6465 6620 6765 745f 616c 6c5f 6469 6d65  def get_all_dime
+00010d90: 6e73 696f 6e5f 7461 6773 2863 6c73 2c20  nsion_tags(cls, 
+00010da0: 6461 7461 5f6c 6973 742c 2069 735f 6571  data_list, is_eq
+00010db0: 7561 6c5f 6f70 7473 3d4e 6f6e 652c 2075  ual_opts=None, u
+00010dc0: 6e69 7175 655f 7365 7061 7261 7465 5f61  nique_separate_a
+00010dd0: 7865 733d 5472 7565 293a 0a20 2020 2020  xes=True):.     
+00010de0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00010df0: 7061 7261 6d20 6c69 7374 5b5f 742e 5465  param list[_t.Te
+00010e00: 6e73 6f72 5d20 6461 7461 5f6c 6973 743a  nsor] data_list:
+00010e10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010e20: 6469 6374 5b73 7472 5d7c 4e6f 6e65 2069  dict[str]|None i
+00010e30: 735f 6571 7561 6c5f 6f70 7473 3a20 7061  s_equal_opts: pa
+00010e40: 7373 6564 2074 6f20 4469 6d2e 6973 5f65  ssed to Dim.is_e
+00010e50: 7175 616c 0a20 2020 2020 2020 203a 7061  qual.        :pa
+00010e60: 7261 6d20 626f 6f6c 2075 6e69 7175 655f  ram bool unique_
+00010e70: 7365 7061 7261 7465 5f61 7865 733a 2065  separate_axes: e
+00010e80: 2e67 2e20 6461 7461 5f6c 6973 743d 5b44  .g. data_list=[D
+00010e90: 6174 6120 7769 7468 2073 6861 7065 2028  ata with shape (
+00010ea0: 422c 352c 352c 3130 295d 2072 6573 756c  B,5,5,10)] resul
+00010eb0: 7473 2069 6e20 3420 6469 6d20 7461 6773  ts in 4 dim tags
+00010ec0: 2c20 6e6f 7420 332e 0a20 2020 2020 2020  , not 3..       
+00010ed0: 203a 7265 7475 726e 3a20 6c69 7374 206f   :return: list o
+00010ee0: 6620 6469 6d65 6e73 696f 6e20 7461 6773  f dimension tags
+00010ef0: 2c20 6469 6374 2066 6f72 2064 6174 6120  , dict for data 
+00010f00: 2d3e 206c 6973 7420 6f66 2064 696d 656e  -> list of dimen
+00010f10: 7369 6f6e 2074 6167 7320 2866 6f72 2065  sion tags (for e
+00010f20: 6163 6820 6178 6973 290a 2020 2020 2020  ach axis).      
+00010f30: 2020 3a72 7479 7065 3a20 286c 6973 745b    :rtype: (list[
+00010f40: 4469 6d5d 2c20 7574 696c 2e44 6963 7452  Dim], util.DictR
+00010f50: 6566 4b65 7973 5b5f 742e 5465 6e73 6f72  efKeys[_t.Tensor
+00010f60: 2c20 6c69 7374 5b44 696d 5d5d 290a 2020  , list[Dim]]).  
+00010f70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010f80: 2020 7461 6773 203d 205b 5d0a 2020 2020    tags = [].    
+00010f90: 2020 2020 6461 7461 5f61 7865 735f 6469      data_axes_di
+00010fa0: 6374 203d 2075 7469 6c2e 4469 6374 5265  ct = util.DictRe
+00010fb0: 664b 6579 7328 2920 2023 2074 7970 653a  fKeys()  # type:
+00010fc0: 2075 7469 6c2e 4469 6374 5265 664b 6579   util.DictRefKey
+00010fd0: 735b 5f74 2e54 656e 736f 722c 204c 6973  s[_t.Tensor, Lis
+00010fe0: 745b 4469 6d5d 5d0a 2020 2020 2020 2020  t[Dim]].        
+00010ff0: 666f 7220 6461 7461 2069 6e20 6461 7461  for data in data
+00011000: 5f6c 6973 743a 0a20 2020 2020 2020 2020  _list:.         
+00011010: 2020 2064 6174 615f 6178 6573 5f64 6963     data_axes_dic
+00011020: 745b 6461 7461 5d20 3d20 5b5d 0a20 2020  t[data] = [].   
+00011030: 2020 2020 2020 2020 2065 7869 7374 696e           existin
+00011040: 675f 7461 675f 636f 6c6c 6563 7469 6f6e  g_tag_collection
+00011050: 5f66 6f72 5f64 6174 6120 3d20 6c69 7374  _for_data = list
+00011060: 2874 6167 7329 2069 6620 756e 6971 7565  (tags) if unique
+00011070: 5f73 6570 6172 6174 655f 6178 6573 2065  _separate_axes e
+00011080: 6c73 6520 7461 6773 0a20 2020 2020 2020  lse tags.       
+00011090: 2020 2020 2066 6f72 2061 7869 7320 696e       for axis in
+000110a0: 2072 616e 6765 2864 6174 612e 6261 7463   range(data.batc
+000110b0: 685f 6e64 696d 293a 0a20 2020 2020 2020  h_ndim):.       
+000110c0: 2020 2020 2020 2020 2074 6167 203d 2064           tag = d
+000110d0: 6174 612e 6765 745f 6469 6d5f 7461 6728  ata.get_dim_tag(
+000110e0: 6178 6973 290a 2020 2020 2020 2020 2020  axis).          
+000110f0: 2020 2020 2020 6578 6973 7469 6e67 5f74        existing_t
+00011100: 6167 203d 2063 6c73 2e67 6574 5f65 7869  ag = cls.get_exi
+00011110: 7374 696e 675f 7461 675f 6672 6f6d 5f63  sting_tag_from_c
+00011120: 6f6c 6c65 6374 696f 6e28 0a20 2020 2020  ollection(.     
+00011130: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011140: 6167 2c20 7461 6773 3d65 7869 7374 696e  ag, tags=existin
+00011150: 675f 7461 675f 636f 6c6c 6563 7469 6f6e  g_tag_collection
+00011160: 5f66 6f72 5f64 6174 612c 2069 735f 6571  _for_data, is_eq
+00011170: 7561 6c5f 6f70 7473 3d69 735f 6571 7561  ual_opts=is_equa
+00011180: 6c5f 6f70 7473 0a20 2020 2020 2020 2020  l_opts.         
+00011190: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000111a0: 2020 2020 2020 2020 2069 6620 6578 6973           if exis
+000111b0: 7469 6e67 5f74 6167 3a0a 2020 2020 2020  ting_tag:.      
+000111c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000111d0: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
+000111e0: 5f61 7865 733a 0a20 2020 2020 2020 2020  _axes:.         
+000111f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011200: 7869 7374 696e 675f 7461 675f 636f 6c6c  xisting_tag_coll
+00011210: 6563 7469 6f6e 5f66 6f72 5f64 6174 612e  ection_for_data.
+00011220: 7265 6d6f 7665 2865 7869 7374 696e 675f  remove(existing_
+00011230: 7461 6729 2020 2320 646f 6e27 7420 7461  tag)  # don't ta
+00011240: 6b65 2069 7420 6167 6169 6e20 666f 7220  ke it again for 
+00011250: 7468 6973 2064 6174 610a 2020 2020 2020  this data.      
+00011260: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00011270: 706c 6163 655f 6578 6973 7469 6e67 203d  place_existing =
+00011280: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00011290: 2020 2020 2020 2020 2020 2065 7869 7374             exist
+000112a0: 696e 675f 7461 672e 756e 6465 6669 6e65  ing_tag.undefine
+000112b0: 6420 616e 6420 6e6f 7420 7461 672e 756e  d and not tag.un
+000112c0: 6465 6669 6e65 6420 616e 6420 7461 672e  defined and tag.
+000112d0: 6469 6d65 6e73 696f 6e20 3d3d 2065 7869  dimension == exi
+000112e0: 7374 696e 675f 7461 672e 6469 6d65 6e73  sting_tag.dimens
+000112f0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00011300: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00011310: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011320: 2072 6570 6c61 6365 5f65 7869 7374 696e   replace_existin
+00011330: 673a 2020 2320 5265 706c 6163 6520 7468  g:  # Replace th
+00011340: 6520 6578 6973 7469 6e67 2062 7920 7468  e existing by th
+00011350: 6520 6e65 7720 7461 672e 0a20 2020 2020  e new tag..     
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 2020 2074 6167 735b 7461 6773 2e69 6e64     tags[tags.ind
+00011380: 6578 2865 7869 7374 696e 675f 7461 6729  ex(existing_tag)
+00011390: 5d20 3d20 7461 670a 2020 2020 2020 2020  ] = tag.        
 000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 666f 7220 5f2c 2064 696d        for _, dim
-000113c0: 735f 2069 6e20 6461 7461 5f61 7865 735f  s_ in data_axes_
-000113d0: 6469 6374 2e69 7465 6d73 2829 3a0a 2020  dict.items():.  
+000113b0: 666f 7220 5f2c 2064 696d 735f 2069 6e20  for _, dims_ in 
+000113c0: 6461 7461 5f61 7865 735f 6469 6374 2e69  data_axes_dict.i
+000113d0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
 000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113f0: 2020 2020 2020 2020 2020 6469 6d73 5f5b            dims_[
-00011400: 3a5d 203d 205b 7461 6720 6966 2064 203d  :] = [tag if d =
-00011410: 3d20 6578 6973 7469 6e67 5f74 6167 2065  = existing_tag e
-00011420: 6c73 6520 6420 666f 7220 6420 696e 2064  lse d for d in d
-00011430: 696d 735f 5d0a 2020 2020 2020 2020 2020  ims_].          
-00011440: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00011450: 6973 7469 6e67 5f74 6167 203d 2074 6167  isting_tag = tag
-00011460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011470: 2065 6c73 653a 2020 2320 6e6f 2065 7869   else:  # no exi
-00011480: 7374 696e 6720 7461 670a 2020 2020 2020  sting tag.      
-00011490: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-000114a0: 6773 2e61 7070 656e 6428 7461 6729 0a20  gs.append(tag). 
-000114b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000114c0: 6174 615f 6178 6573 5f64 6963 745b 6461  ata_axes_dict[da
-000114d0: 7461 5d2e 6170 7065 6e64 2865 7869 7374  ta].append(exist
-000114e0: 696e 675f 7461 6720 6f72 2074 6167 290a  ing_tag or tag).
-000114f0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00011500: 6167 732c 2064 6174 615f 6178 6573 5f64  ags, data_axes_d
-00011510: 6963 740a 0a20 2020 2040 636c 6173 736d  ict..    @classm
-00011520: 6574 686f 640a 2020 2020 6465 6620 6765  ethod.    def ge
-00011530: 745f 756e 6971 5f63 6f6c 6c65 6374 696f  t_uniq_collectio
-00011540: 6e28 636c 732c 2074 6167 732c 2069 735f  n(cls, tags, is_
-00011550: 6571 7561 6c5f 6f70 7473 3d4e 6f6e 6529  equal_opts=None)
-00011560: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00011570: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
-00011580: 745b 4469 6d5d 7c74 7570 6c65 5b44 696d  t[Dim]|tuple[Dim
-00011590: 5d7c 7365 745b 4469 6d5d 2074 6167 733a  ]|set[Dim] tags:
-000115a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000115b0: 6469 6374 5b73 7472 5d7c 4e6f 6e65 2069  dict[str]|None i
-000115c0: 735f 6571 7561 6c5f 6f70 7473 3a20 7061  s_equal_opts: pa
-000115d0: 7373 6564 2074 6f20 4469 6d2e 6973 5f65  ssed to Dim.is_e
-000115e0: 7175 616c 0a20 2020 2020 2020 203a 7274  qual.        :rt
-000115f0: 7970 653a 206c 6973 745b 4469 6d5d 0a20  ype: list[Dim]. 
-00011600: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011610: 2020 2072 6573 203d 205b 5d0a 2020 2020     res = [].    
-00011620: 2020 2020 666f 7220 7461 6720 696e 2074      for tag in t
-00011630: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
-00011640: 2065 7820 3d20 636c 732e 6765 745f 6578   ex = cls.get_ex
-00011650: 6973 7469 6e67 5f74 6167 5f66 726f 6d5f  isting_tag_from_
-00011660: 636f 6c6c 6563 7469 6f6e 2874 6167 2c20  collection(tag, 
-00011670: 7265 732c 2069 735f 6571 7561 6c5f 6f70  res, is_equal_op
-00011680: 7473 3d69 735f 6571 7561 6c5f 6f70 7473  ts=is_equal_opts
-00011690: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000116a0: 206e 6f74 2065 783a 0a20 2020 2020 2020   not ex:.       
-000116b0: 2020 2020 2020 2020 2072 6573 2e61 7070           res.app
-000116c0: 656e 6428 7461 6729 0a20 2020 2020 2020  end(tag).       
-000116d0: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
-000116e0: 2064 6566 2067 6574 5f73 697a 655f 7465   def get_size_te
-000116f0: 6e73 6f72 2873 656c 6629 202d 3e20 5f74  nsor(self) -> _t
-00011700: 2e54 656e 736f 723a 0a20 2020 2020 2020  .Tensor:.       
-00011710: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
-00011720: 7475 726e 3a20 7369 7a65 2074 656e 736f  turn: size tenso
-00011730: 722c 206f 7220 6479 6e5f 7369 7a65 5f65  r, or dyn_size_e
-00011740: 7874 2069 6620 6465 6669 6e65 640a 2020  xt if defined.  
-00011750: 2020 2020 2020 3a72 7479 7065 3a20 5f74        :rtype: _t
-00011760: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
-00011770: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00011780: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00011790: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000117a0: 7475 726e 2073 656c 662e 6479 6e5f 7369  turn self.dyn_si
-000117b0: 7a65 5f65 7874 0a0a 2020 2020 2020 2020  ze_ext..        
-000117c0: 696d 706f 7274 2072 6574 7572 6e6e 2e66  import returnn.f
-000117d0: 726f 6e74 656e 6420 6173 2072 660a 0a20  rontend as rf.. 
-000117e0: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-000117f0: 6c66 2e73 697a 6520 6973 206e 6f74 204e  lf.size is not N
-00011800: 6f6e 650a 2020 2020 2020 2020 7265 7475  one.        retu
-00011810: 726e 2072 662e 636f 6e76 6572 745f 746f  rn rf.convert_to
-00011820: 5f74 656e 736f 7228 7365 6c66 2e73 697a  _tensor(self.siz
-00011830: 652c 206e 616d 653d 2225 733a 7369 7a65  e, name="%s:size
-00011840: 2220 2520 7365 6c66 2e64 6573 6372 6970  " % self.descrip
-00011850: 7469 6f6e 290a 0a20 2020 2064 6566 2067  tion)..    def g
-00011860: 6574 5f64 696d 5f76 616c 7565 2873 656c  et_dim_value(sel
-00011870: 6629 202d 3e20 556e 696f 6e5b 696e 742c  f) -> Union[int,
-00011880: 205f 742e 5261 7754 656e 736f 7254 7970   _t.RawTensorTyp
-00011890: 655d 3a0a 2020 2020 2020 2020 2222 220a  e]:.        """.
-000118a0: 2020 2020 2020 2020 496e 6665 7273 2074          Infers t
-000118b0: 6865 2064 696d 2074 6869 7320 6178 6973  he dim this axis
-000118c0: 2073 686f 756c 6420 6861 7665 2069 6620   should have if 
-000118d0: 756e 6272 6f61 6463 6173 7465 642e 0a20  unbroadcasted.. 
-000118e0: 2020 2020 2020 2049 6620 6073 656c 662e         If `self.
-000118f0: 7372 635f 6461 7461 6020 6861 7320 6120  src_data` has a 
-00011900: 706c 6163 6568 6f6c 6465 722c 2077 696c  placeholder, wil
-00011910: 6c20 7573 6520 7468 6520 7368 6170 6520  l use the shape 
-00011920: 6672 6f6d 2074 6865 7265 2e0a 2020 2020  from there..    
-00011930: 2020 2020 4f74 6865 7277 6973 652c 2075      Otherwise, u
-00011940: 7365 7320 6073 656c 662e 6469 6d65 6e73  ses `self.dimens
-00011950: 696f 6e60 2028 6966 2073 7461 7469 6329  ion` (if static)
-00011960: 206f 7220 6073 656c 662e 6479 6e5f 7369   or `self.dyn_si
-00011970: 7a65 6020 2869 6620 6479 6e61 6d69 6329  ze` (if dynamic)
-00011980: 2e0a 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
-00011990: 726e 3a20 6d61 7828 7369 7a65 206f 7220  rn: max(size or 
-000119a0: 6479 6e5f 7369 7a65 290a 2020 2020 2020  dyn_size).      
-000119b0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-000119c0: 7320 3d20 7365 6c66 2e67 6574 5f64 696d  s = self.get_dim
-000119d0: 5f76 616c 7565 5f74 656e 736f 7228 290a  _value_tensor().
-000119e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000119f0: 7461 6e63 6528 7265 732c 205f 742e 5465  tance(res, _t.Te
-00011a00: 6e73 6f72 293a 0a20 2020 2020 2020 2020  nsor):.         
-00011a10: 2020 2061 7373 6572 7420 7265 732e 6469     assert res.di
-00011a20: 6d73 203d 3d20 2829 0a20 2020 2020 2020  ms == ().       
-00011a30: 2020 2020 2072 6574 7572 6e20 7265 732e       return res.
-00011a40: 7261 775f 7465 6e73 6f72 0a20 2020 2020  raw_tensor.     
-00011a50: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00011a60: 616e 6365 2872 6573 2c20 696e 7429 0a20  ance(res, int). 
-00011a70: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00011a80: 730a 0a20 2020 2064 6566 2067 6574 5f64  s..    def get_d
-00011a90: 696d 5f76 616c 7565 5f74 656e 736f 7228  im_value_tensor(
-00011aa0: 7365 6c66 2920 2d3e 2055 6e69 6f6e 5b69  self) -> Union[i
-00011ab0: 6e74 2c20 5f74 2e54 656e 736f 725d 3a0a  nt, _t.Tensor]:.
-00011ac0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011ad0: 2020 2020 496e 6665 7273 2074 6865 2064      Infers the d
-00011ae0: 696d 2074 6869 7320 6178 6973 2073 686f  im this axis sho
-00011af0: 756c 6420 6861 7665 2069 6620 756e 6272  uld have if unbr
-00011b00: 6f61 6463 6173 7465 642e 0a20 2020 2020  oadcasted..     
-00011b10: 2020 2049 6620 6073 656c 662e 7372 635f     If `self.src_
-00011b20: 6461 7461 6020 6861 7320 6120 706c 6163  data` has a plac
-00011b30: 6568 6f6c 6465 722c 2077 696c 6c20 7573  eholder, will us
-00011b40: 6520 7468 6520 7368 6170 6520 6672 6f6d  e the shape from
-00011b50: 2074 6865 7265 2e0a 2020 2020 2020 2020   there..        
-00011b60: 4f74 6865 7277 6973 652c 2075 7365 7320  Otherwise, uses 
-00011b70: 6073 656c 662e 6469 6d65 6e73 696f 6e60  `self.dimension`
-00011b80: 2028 6966 2073 7461 7469 6329 206f 7220   (if static) or 
-00011b90: 6073 656c 662e 6479 6e5f 7369 7a65 6020  `self.dyn_size` 
-00011ba0: 2869 6620 6479 6e61 6d69 6329 2e0a 0a20  (if dynamic)... 
-00011bb0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00011bc0: 6d61 7828 7369 7a65 206f 7220 6479 6e5f  max(size or dyn_
-00011bd0: 7369 7a65 290a 2020 2020 2020 2020 2222  size).        ""
-00011be0: 220a 2020 2020 2020 2020 696d 706f 7274  ".        import
-00011bf0: 2072 6574 7572 6e6e 2e66 726f 6e74 656e   returnn.fronten
-00011c00: 6420 6173 2072 660a 0a20 2020 2020 2020  d as rf..       
-00011c10: 2069 6620 7365 6c66 2e64 696d 656e 7369   if self.dimensi
-00011c20: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00011c30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011c40: 726e 2073 656c 662e 6469 6d65 6e73 696f  rn self.dimensio
-00011c50: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-00011c60: 662e 6479 6e5f 7369 7a65 5f65 7874 2061  f.dyn_size_ext a
-00011c70: 6e64 2073 656c 662e 6479 6e5f 7369 7a65  nd self.dyn_size
-00011c80: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
-00011c90: 2069 7320 6e6f 7420 4e6f 6e65 3a20 2023   is not None:  #
-00011ca0: 2066 6173 7420 7061 7468 0a20 2020 2020   fast path.     
-00011cb0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011cc0: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
-00011cd0: 685f 6e64 696d 203e 2030 3a0a 2020 2020  h_ndim > 0:.    
-00011ce0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011cf0: 726e 2072 662e 7265 6475 6365 5f6d 6178  rn rf.reduce_max
-00011d00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011d10: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-00011d20: 697a 655f 6578 742c 0a20 2020 2020 2020  ize_ext,.       
-00011d30: 2020 2020 2020 2020 2020 2020 2061 7869               axi
-00011d40: 733d 7365 6c66 2e64 796e 5f73 697a 655f  s=self.dyn_size_
-00011d50: 6578 742e 6469 6d5f 7461 6773 2c0a 2020  ext.dim_tags,.  
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 2320 4d61 736b 696e 6720 6973 206e    # Masking is n
-00011d80: 6f74 2061 6c77 6179 7320 706f 7373 6962  ot always possib
-00011d90: 6c65 2068 6572 652c 2065 2e67 2e0a 2020  le here, e.g..  
-00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011db0: 2020 2320 7365 6c66 203d 2044 696d 7b27    # self = Dim{'
-00011dc0: 7365 6c66 2d61 7474 2d6b 6579 7327 5b27  self-att-keys'['
-00011dd0: 7469 6d65 3a76 6172 3a65 7874 6572 6e5f  time:var:extern_
-00011de0: 6461 7461 3a63 6c61 7373 6573 275b 425d  data:classes'[B]
-00011df0: 5d7d 2e0a 2020 2020 2020 2020 2020 2020  ]}..            
-00011e00: 2020 2020 2020 2020 7573 655f 6d61 736b          use_mask
-00011e10: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00011e20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011e30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00011e40: 662e 6479 6e5f 7369 7a65 5f65 7874 0a20  f.dyn_size_ext. 
-00011e50: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00011e60: 735f 6261 7463 685f 6469 6d28 293a 0a20  s_batch_dim():. 
-00011e70: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00011e80: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00011e90: 2020 6966 2073 656c 662e 5f65 7874 7261    if self._extra
-00011ea0: 2061 6e64 2073 656c 662e 5f65 7874 7261   and self._extra
-00011eb0: 2e73 7263 5f64 6174 613a 0a20 2020 2020  .src_data:.     
-00011ec0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00011ed0: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
-00011ee0: 5f64 6174 612e 6765 745f 6261 7463 685f  _data.get_batch_
-00011ef0: 6469 6d28 290a 2020 2020 2020 2020 2020  dim().          
-00011f00: 2020 656c 6966 2073 656c 662e 6261 7463    elif self.batc
-00011f10: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00011f20: 2020 2072 6573 203d 2073 656c 662e 6261     res = self.ba
-00011f30: 7463 682e 6469 6d0a 2020 2020 2020 2020  tch.dim.        
-00011f40: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00011f50: 6528 7265 732c 2069 6e74 293a 0a20 2020  e(res, int):.   
-00011f60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00011f70: 7572 6e20 7265 730a 2020 2020 2020 2020  urn res.        
-00011f80: 2020 2020 6966 2072 6573 2069 7320 6e6f      if res is no
-00011f90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00011fa0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00011fb0: 742e 5465 6e73 6f72 2822 6261 7463 6822  t.Tensor("batch"
-00011fc0: 2c20 6469 6d73 3d28 292c 2064 7479 7065  , dims=(), dtype
-00011fd0: 3d72 662e 6765 745f 6465 6661 756c 745f  =rf.get_default_
-00011fe0: 6172 7261 795f 696e 6465 785f 6474 7970  array_index_dtyp
-00011ff0: 6528 292c 2072 6177 5f74 656e 736f 723d  e(), raw_tensor=
-00012000: 7265 7329 0a20 2020 2020 2020 2069 6620  res).        if 
-00012010: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00012020: 6c66 2e5f 6578 7472 610a 2020 2020 2020  lf._extra.      
-00012030: 2020 2020 2020 616e 6420 7365 6c66 2e5f        and self._
-00012040: 6578 7472 612e 7372 635f 6461 7461 2069  extra.src_data i
-00012050: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00012060: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
-00012070: 5f65 7874 7261 2e73 7263 5f61 7869 7320  _extra.src_axis 
-00012080: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00012090: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
-000120a0: 2e5f 6578 7472 612e 7372 635f 6461 7461  ._extra.src_data
-000120b0: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
-000120c0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-000120d0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-000120e0: 7265 7320 3d20 7365 6c66 2e5f 6578 7472  res = self._extr
-000120f0: 612e 7372 635f 6461 7461 2e67 6574 5f64  a.src_data.get_d
-00012100: 696d 2873 656c 662e 5f65 7874 7261 2e73  im(self._extra.s
-00012110: 7263 5f61 7869 7329 0a20 2020 2020 2020  rc_axis).       
-00012120: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00012130: 6365 2872 6573 2c20 696e 7429 3a0a 2020  ce(res, int):.  
-00012140: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00012150: 7475 726e 2072 6573 0a20 2020 2020 2020  turn res.       
-00012160: 2020 2020 2072 6574 7572 6e20 5f74 2e54       return _t.T
-00012170: 656e 736f 7228 2262 6174 6368 222c 2064  ensor("batch", d
-00012180: 696d 733d 2829 2c20 6474 7970 653d 7266  ims=(), dtype=rf
-00012190: 2e67 6574 5f64 6566 6175 6c74 5f61 7272  .get_default_arr
-000121a0: 6179 5f69 6e64 6578 5f64 7479 7065 2829  ay_index_dtype()
-000121b0: 2c20 7261 775f 7465 6e73 6f72 3d72 6573  , raw_tensor=res
-000121c0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-000121d0: 6f6d 706c 6574 655f 6479 6e5f 7369 7a65  omplete_dyn_size
-000121e0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000121f0: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
-00012200: 616e 6420 7365 6c66 2e64 796e 5f73 697a  and self.dyn_siz
-00012210: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-00012220: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-00012230: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00012240: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00012250: 6261 7463 685f 6e64 696d 203e 2030 3a0a  batch_ndim > 0:.
-00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 7265 7475 726e 2072 662e 7265 6475 6365  return rf.reduce
-00012280: 5f6d 6178 2873 656c 662e 6479 6e5f 7369  _max(self.dyn_si
-00012290: 7a65 5f65 7874 2c20 6178 6973 3d73 656c  ze_ext, axis=sel
-000122a0: 662e 6479 6e5f 7369 7a65 5f65 7874 2e64  f.dyn_size_ext.d
-000122b0: 696d 5f74 6167 7329 0a20 2020 2020 2020  im_tags).       
-000122c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000122d0: 2e64 796e 5f73 697a 655f 6578 740a 2020  .dyn_size_ext.  
-000122e0: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-000122f0: 7074 696f 6e28 2225 733a 206e 6565 6420  ption("%s: need 
-00012300: 706c 6163 6568 6f6c 6465 722c 2073 656c  placeholder, sel
-00012310: 662e 6469 6d65 6e73 696f 6e20 6f72 2073  f.dimension or s
-00012320: 656c 662e 6479 6e5f 7369 7a65 2066 6f72  elf.dyn_size for
-00012330: 2064 696d 2076 616c 7565 2220 2520 7365   dim value" % se
-00012340: 6c66 290a 0a20 2020 2064 6566 2061 7869  lf)..    def axi
-00012350: 735f 7370 6c69 745f 696e 666f 2873 656c  s_split_info(sel
-00012360: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00012370: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00012380: 2061 7869 7320 7370 6c69 7420 696e 666f   axis split info
-00012390: 2e20 7365 6520 3a66 756e 633a 6067 6574  . see :func:`get
-000123a0: 5f70 6172 616d 5f61 7865 735f 7370 6c69  _param_axes_spli
-000123b0: 745f 696e 666f 6020 616e 6420 7573 6167  t_info` and usag
-000123c0: 6520 2865 2e67 2e20 7072 6574 7261 696e  e (e.g. pretrain
-000123d0: 696e 6729 0a20 2020 2020 2020 203a 7274  ing).        :rt
-000123e0: 7970 653a 206c 6973 745b 696e 747c 4e6f  ype: list[int|No
-000123f0: 6e65 5d0a 2020 2020 2020 2020 2222 220a  ne].        """.
-00012400: 2020 2020 2020 2020 7361 6d65 5f62 6173          same_bas
-00012410: 6520 3d20 7365 6c66 2e67 6574 5f73 616d  e = self.get_sam
-00012420: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
-00012430: 206f 7020 3d20 7365 6c66 2e64 6572 6976   op = self.deriv
-00012440: 6564 5f66 726f 6d5f 6f70 206f 7220 7361  ed_from_op or sa
-00012450: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-00012460: 6672 6f6d 5f6f 700a 2020 2020 2020 2020  from_op.        
-00012470: 6966 206e 6f74 206f 703a 0a20 2020 2020  if not op:.     
-00012480: 2020 2020 2020 2072 6574 7572 6e20 5b73         return [s
-00012490: 656c 662e 6469 6d65 6e73 696f 6e5d 0a20  elf.dimension]. 
-000124a0: 2020 2020 2020 2069 6620 6f70 2e6b 696e         if op.kin
-000124b0: 6420 3d3d 2022 6164 6422 3a0a 2020 2020  d == "add":.    
-000124c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000124d0: 756d 285b 782e 6178 6973 5f73 706c 6974  um([x.axis_split
-000124e0: 5f69 6e66 6f28 2920 666f 7220 7820 696e  _info() for x in
-000124f0: 206f 702e 696e 7075 7473 5d2c 205b 5d29   op.inputs], [])
-00012500: 2020 2320 666c 6174 7465 6e0a 2020 2020    # flatten.    
-00012510: 2020 2020 6966 206f 702e 6b69 6e64 203d      if op.kind =
-00012520: 3d20 226d 756c 223a 0a20 2020 2020 2020  = "mul":.       
-00012530: 2020 2020 2072 6573 203d 205b 315d 0a20       res = [1]. 
-00012540: 2020 2020 2020 2020 2020 2066 6f72 2078             for x
-00012550: 2069 6e20 6f70 2e69 6e70 7574 733a 0a20   in op.inputs:. 
-00012560: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012570: 6573 203d 2073 756d 285b 6e20 2a20 782e  es = sum([n * x.
-00012580: 6178 6973 5f73 706c 6974 5f69 6e66 6f28  axis_split_info(
-00012590: 2920 6966 206e 2069 7320 6e6f 7420 4e6f  ) if n is not No
-000125a0: 6e65 2065 6c73 6520 4e6f 6e65 2066 6f72  ne else None for
-000125b0: 206e 2069 6e20 7265 735d 2c20 5b5d 2920   n in res], []) 
-000125c0: 2023 2066 6c61 7474 656e 0a20 2020 2020   # flatten.     
-000125d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000125e0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-000125f0: 205b 7365 6c66 2e64 696d 656e 7369 6f6e   [self.dimension
-00012600: 5d0a 0a20 2020 2064 6566 205f 6765 745f  ]..    def _get_
-00012610: 7361 6d65 5f62 6173 655f 6578 7472 6128  same_base_extra(
-00012620: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-00012630: 6c5b 5f44 696d 4578 7472 615d 3a0a 2020  l[_DimExtra]:.  
-00012640: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00012650: 662e 5f65 7874 7261 3a0a 2020 2020 2020  f._extra:.      
-00012660: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00012670: 650a 2020 2020 2020 2020 6261 7365 203d  e.        base =
-00012680: 2073 656c 662e 6765 745f 7361 6d65 5f62   self.get_same_b
-00012690: 6173 6528 290a 2020 2020 2020 2020 2320  ase().        # 
-000126a0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-000126b0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-000126c0: 2020 2020 2020 2072 6574 7572 6e20 6261         return ba
-000126d0: 7365 2e5f 6578 7472 610a 0a20 2020 2064  se._extra..    d
-000126e0: 6566 205f 6d61 6b65 5f65 7874 7261 2873  ef _make_extra(s
-000126f0: 656c 663a 205f 642e 4469 6d29 202d 3e20  elf: _d.Dim) -> 
-00012700: 5f44 696d 4578 7472 613a 0a20 2020 2020  _DimExtra:.     
-00012710: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-00012720: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
-00012730: 2020 2073 656c 662e 5f65 7874 7261 203d     self._extra =
-00012740: 205f 4469 6d45 7874 7261 2864 696d 3d73   _DimExtra(dim=s
-00012750: 656c 6629 0a20 2020 2020 2020 2072 6574  elf).        ret
-00012760: 7572 6e20 7365 6c66 2e5f 6578 7472 610a  urn self._extra.
-00012770: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00012780: 2020 2064 6566 2076 6f63 6162 2873 656c     def vocab(sel
-00012790: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000127a0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000127b0: 7265 7475 726e 6e2e 6461 7461 7365 7473  returnn.datasets
-000127c0: 2e75 7469 6c2e 766f 6361 6275 6c61 7279  .util.vocabulary
-000127d0: 2e56 6f63 6162 756c 6172 797c 4e6f 6e65  .Vocabulary|None
-000127e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000127f0: 2020 2020 2065 7874 7261 203d 2073 656c       extra = sel
-00012800: 662e 5f67 6574 5f73 616d 655f 6261 7365  f._get_same_base
-00012810: 5f65 7874 7261 2829 0a20 2020 2020 2020  _extra().       
-00012820: 2069 6620 6578 7472 613a 0a20 2020 2020   if extra:.     
-00012830: 2020 2020 2020 2072 6574 7572 6e20 6578         return ex
-00012840: 7472 612e 766f 6361 620a 2020 2020 2020  tra.vocab.      
-00012850: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-00012860: 2020 2040 766f 6361 622e 7365 7474 6572     @vocab.setter
-00012870: 0a20 2020 2064 6566 2076 6f63 6162 2873  .    def vocab(s
-00012880: 656c 662c 2076 6f63 6162 293a 0a20 2020  elf, vocab):.   
-00012890: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000128a0: 203a 7061 7261 6d20 7265 7475 726e 6e2e   :param returnn.
-000128b0: 6461 7461 7365 7473 2e75 7469 6c2e 766f  datasets.util.vo
-000128c0: 6361 6275 6c61 7279 2e56 6f63 6162 756c  cabulary.Vocabul
-000128d0: 6172 797c 4e6f 6e65 2076 6f63 6162 3a0a  ary|None vocab:.
-000128e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000128f0: 2020 2020 6966 2076 6f63 6162 2069 7320      if vocab is 
-00012900: 7365 6c66 2e76 6f63 6162 3a0a 2020 2020  self.vocab:.    
-00012910: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00012920: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00012930: 616d 655f 6173 3a0a 2020 2020 2020 2020  ame_as:.        
-00012940: 2020 2020 7365 6c66 2e67 6574 5f73 616d      self.get_sam
-00012950: 655f 6261 7365 2829 2e76 6f63 6162 203d  e_base().vocab =
-00012960: 2076 6f63 6162 0a20 2020 2020 2020 2020   vocab.         
-00012970: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00012980: 2020 6578 7472 6120 3d20 7365 6c66 2e5f    extra = self._
-00012990: 6765 745f 7361 6d65 5f62 6173 655f 6578  get_same_base_ex
-000129a0: 7472 6128 290a 2020 2020 2020 2020 6966  tra().        if
-000129b0: 2065 7874 7261 3a0a 2020 2020 2020 2020   extra:.        
-000129c0: 2020 2020 6578 7472 612e 766f 6361 6220      extra.vocab 
-000129d0: 3d20 766f 6361 620a 0a20 2020 2023 2054  = vocab..    # T
-000129e0: 6865 206b 696e 6420 6f66 206f 7065 7261  he kind of opera
-000129f0: 7469 6f6e 7320 7765 2068 6176 653a 0a20  tions we have:. 
-00012a00: 2020 2023 2061 202b 2062 3a20 7061 6464     # a + b: padd
-00012a10: 696e 672c 2063 6f6e 6361 740a 2020 2020  ing, concat.    
-00012a20: 2320 6120 2d20 623a 2077 696e 646f 7720  # a - b: window 
-00012a30: 7769 7468 2076 616c 6964 2066 7261 6d65  with valid frame
-00012a40: 7320 6f6e 6c79 0a20 2020 2023 2061 202a  s only.    # a *
-00012a50: 2062 3a20 6d65 7267 6520 6469 6d73 2c20   b: merge dims, 
-00012a60: 7570 7361 6d70 6c65 2c20 7472 616e 7370  upsample, transp
-00012a70: 6f73 6564 2063 6f6e 7620 7769 7468 2073  osed conv with s
-00012a80: 7472 6964 696e 670a 2020 2020 2320 6120  triding.    # a 
-00012a90: 2f20 6220 2877 6865 6e20 6120 2520 6220  / b (when a % b 
-00012aa0: 3d3d 2030 293a 2073 706c 6974 2064 696d  == 0): split dim
-00012ab0: 732c 2064 6f77 6e73 616d 706c 652c 2063  s, downsample, c
-00012ac0: 6f6e 7620 7769 7468 2073 7472 6964 696e  onv with stridin
-00012ad0: 670a 2020 2020 2320 6365 696c 6469 7628  g.    # ceildiv(
-00012ae0: 612c 2062 293a 2063 6f6e 7620 7769 7468  a, b): conv with
-00012af0: 2073 7472 6964 696e 670a 2020 2020 2320   striding.    # 
-00012b00: 6375 7374 6f6d 3a20 7265 7065 6174 2c20  custom: repeat, 
-00012b10: 7265 6d6f 7665 2c20 6d61 736b 2c20 6c6f  remove, mask, lo
-00012b20: 6f70 2077 6974 6820 6479 6e20 656e 640a  op with dyn end.
-00012b30: 2020 2020 2320 4e6f 7465 2074 6861 7420      # Note that 
-00012b40: 7765 2064 6966 6665 7265 6e74 6961 7465  we differentiate
-00012b50: 2062 6574 7765 656e 2074 6865 206f 7264   between the ord
-00012b60: 6572 2c20 692e 652e 2061 202b 2062 2021  er, i.e. a + b !
-00012b70: 3d20 6220 2b20 612e 0a20 2020 2023 204e  = b + a..    # N
-00012b80: 6f74 6520 7468 6174 2077 6520 616c 7761  ote that we alwa
-00012b90: 7973 2068 6176 6520 7468 6520 6173 7375  ys have the assu
-00012ba0: 6d70 7469 6f6e 2074 6861 7420 6120 6469  mption that a di
-00012bb0: 6d65 6e73 696f 6e20 6973 206e 6f6e 2d6e  mension is non-n
-00012bc0: 6567 6174 6976 652e 0a20 2020 2023 2054  egative..    # T
-00012bd0: 6869 7320 6173 7375 6d70 7469 6f6e 2069  his assumption i
-00012be0: 7320 6e65 6365 7373 6172 7920 666f 7220  s necessary for 
-00012bf0: 736f 6d65 2073 696d 706c 6966 6963 6174  some simplificat
-00012c00: 696f 6e73 2e0a 2020 2020 2320 6874 7470  ions..    # http
-00012c10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00012c20: 7774 682d 6936 2f72 6574 7572 6e6e 2f70  wth-i6/returnn/p
-00012c30: 756c 6c2f 3835 330a 0a20 2020 2064 6566  ull/853..    def
-00012c40: 205f 5f61 6464 5f5f 2873 656c 663a 2044   __add__(self: D
-00012c50: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
-00012c60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012c70: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
-00012c80: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
-00012c90: 6574 7572 6e3a 2073 656c 6620 2b20 6f74  eturn: self + ot
-00012ca0: 6865 722e 206e 6f74 6520 7468 6174 2074  her. note that t
-00012cb0: 6869 7320 6973 206e 6f74 2063 6f6d 6d75  his is not commu
-00012cc0: 7461 7469 7665 2c20 692e 652e 2064 6966  tative, i.e. dif
-00012cd0: 6665 7265 6e74 2066 726f 6d20 6f74 6865  ferent from othe
-00012ce0: 7220 2b20 7365 6c66 2e0a 2020 2020 2020  r + self..      
-00012cf0: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
-00012d00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012d10: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
-00012d20: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
-00012d30: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
-00012d40: 726d 2e65 7874 656e 645f 6164 645f 7375  rm.extend_add_su
-00012d50: 625f 286f 7468 6572 2c20 6b69 6e64 3d22  b_(other, kind="
-00012d60: 6164 6422 2c20 7269 6768 743d 5472 7565  add", right=True
-00012d70: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00012d80: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
-00012d90: 2020 2020 6465 6620 5f5f 7261 6464 5f5f      def __radd__
-00012da0: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
-00012db0: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
-00012dc0: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00012dd0: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
-00012de0: 2020 2020 2020 3a72 6574 7572 6e3a 206f        :return: o
-00012df0: 7468 6572 202b 2073 656c 660a 2020 2020  ther + self.    
-00012e00: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00012e10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012e20: 2020 2020 7465 726d 203d 205f 4f70 4c69      term = _OpLi
-00012e30: 6e65 6172 5465 726d 2e66 726f 6d5f 6469  nearTerm.from_di
-00012e40: 6d28 7365 6c66 290a 2020 2020 2020 2020  m(self).        
-00012e50: 7465 726d 2e65 7874 656e 645f 6164 645f  term.extend_add_
-00012e60: 7375 625f 286f 7468 6572 2c20 6b69 6e64  sub_(other, kind
-00012e70: 3d22 6164 6422 2c20 7269 6768 743d 4661  ="add", right=Fa
-00012e80: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
-00012e90: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
-00012ea0: 290a 0a20 2020 2064 6566 205f 5f73 7562  )..    def __sub
-00012eb0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-00012ec0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012ed0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00012ee0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00012ef0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00012f00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012f10: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
-00012f20: 7562 5f72 6967 6874 286f 7468 6572 290a  ub_right(other).
-00012f30: 0a20 2020 2064 6566 2073 7562 5f72 6967  .    def sub_rig
-00012f40: 6874 2873 656c 663a 2044 696d 2c20 6f74  ht(self: Dim, ot
-00012f50: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
-00012f60: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00012f70: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
-00012f80: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00012f90: 2073 656c 6620 2d20 6f74 6865 720a 2020   self - other.  
-00012fa0: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
-00012fb0: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
-00012fc0: 2020 2020 2020 7465 726d 203d 205f 4f70        term = _Op
-00012fd0: 4c69 6e65 6172 5465 726d 2e66 726f 6d5f  LinearTerm.from_
-00012fe0: 6469 6d28 7365 6c66 290a 2020 2020 2020  dim(self).      
-00012ff0: 2020 7465 726d 2e65 7874 656e 645f 6164    term.extend_ad
-00013000: 645f 7375 625f 286f 7468 6572 2c20 6b69  d_sub_(other, ki
-00013010: 6e64 3d22 7375 6222 2c20 7269 6768 743d  nd="sub", right=
-00013020: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
-00013030: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
-00013040: 2829 0a0a 2020 2020 6465 6620 7375 625f  ()..    def sub_
-00013050: 6c65 6674 2873 656c 663a 2044 696d 2c20  left(self: Dim, 
-00013060: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00013070: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00013080: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
-00013090: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-000130a0: 6e3a 2028 2d6f 7468 6572 2920 2b20 7365  n: (-other) + se
-000130b0: 6c66 0a20 2020 2020 2020 203a 7274 7970  lf.        :rtyp
-000130c0: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-000130d0: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
-000130e0: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
-000130f0: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
-00013100: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
-00013110: 6e64 5f61 6464 5f73 7562 5f28 6f74 6865  nd_add_sub_(othe
-00013120: 722c 206b 696e 643d 2273 7562 222c 2072  r, kind="sub", r
-00013130: 6967 6874 3d46 616c 7365 290a 2020 2020  ight=False).    
-00013140: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
-00013150: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
-00013160: 6620 5f5f 6d75 6c5f 5f28 7365 6c66 3a20  f __mul__(self: 
-00013170: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
-00013180: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013190: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-000131a0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000131b0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-000131c0: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-000131d0: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
-000131e0: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
-000131f0: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
-00013200: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
-00013210: 6f74 6865 722c 206b 696e 643d 226d 756c  other, kind="mul
-00013220: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
-00013230: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-00013240: 726d 2e61 735f 6469 6d28 290a 0a20 2020  rm.as_dim()..   
-00013250: 2064 6566 205f 5f72 6d75 6c5f 5f28 7365   def __rmul__(se
-00013260: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
-00013270: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013280: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00013290: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-000132a0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-000132b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000132c0: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-000132d0: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-000132e0: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-000132f0: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
-00013300: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
-00013310: 226d 756c 222c 2072 6967 6874 3d46 616c  "mul", right=Fal
-00013320: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
-00013330: 726e 2074 6572 6d2e 6173 5f64 696d 2829  rn term.as_dim()
-00013340: 0a0a 2020 2020 6465 6620 5f5f 666c 6f6f  ..    def __floo
-00013350: 7264 6976 5f5f 2873 656c 663a 2044 696d  rdiv__(self: Dim
-00013360: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00013370: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00013380: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
-00013390: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
-000133a0: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
-000133b0: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
-000133c0: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
-000133d0: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
-000133e0: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
-000133f0: 656e 645f 6d75 6c5f 6469 765f 286f 7468  end_mul_div_(oth
-00013400: 6572 2c20 6b69 6e64 3d22 666c 6f6f 7264  er, kind="floord
-00013410: 6976 222c 2072 6967 6874 3d54 7275 6529  iv", right=True)
-00013420: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013430: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-00013440: 2020 2064 6566 205f 5f74 7275 6564 6976     def __truediv
-00013450: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-00013460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013470: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00013480: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00013490: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-000134a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000134b0: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
-000134c0: 6976 5f72 6967 6874 286f 7468 6572 290a  iv_right(other).
-000134d0: 0a20 2020 2064 6566 2064 6976 5f6c 6566  .    def div_lef
-000134e0: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
-000134f0: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
-00013500: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00013510: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-00013520: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00013530: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00013540: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-00013550: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00013560: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00013570: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
-00013580: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
-00013590: 696e 643d 2274 7275 6564 6976 222c 2072  ind="truediv", r
-000135a0: 6967 6874 3d46 616c 7365 290a 2020 2020  ight=False).    
-000135b0: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
-000135c0: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
-000135d0: 6620 6469 765f 7269 6768 7428 7365 6c66  f div_right(self
-000135e0: 3a20 4469 6d2c 206f 7468 6572 293a 0a20  : Dim, other):. 
-000135f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013600: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
-00013610: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
-00013620: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
-00013630: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013640: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
-00013650: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
-00013660: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
-00013670: 6d2e 6578 7465 6e64 5f6d 756c 5f64 6976  m.extend_mul_div
-00013680: 5f28 6f74 6865 722c 206b 696e 643d 2274  _(other, kind="t
-00013690: 7275 6564 6976 222c 2072 6967 6874 3d54  ruediv", right=T
-000136a0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-000136b0: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
-000136c0: 290a 0a20 2020 2064 6566 2063 6569 6c64  )..    def ceild
-000136d0: 6976 5f6c 6566 7428 7365 6c66 3a20 4469  iv_left(self: Di
-000136e0: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
-000136f0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00013700: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
-00013710: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
-00013720: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
-00013730: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
-00013740: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
-00013750: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
-00013760: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
-00013770: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
-00013780: 6865 722c 206b 696e 643d 2263 6569 6c64  her, kind="ceild
-00013790: 6976 222c 2072 6967 6874 3d46 616c 7365  iv", right=False
-000137a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000137b0: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
-000137c0: 2020 2020 6465 6620 6365 696c 6469 765f      def ceildiv_
-000137d0: 7269 6768 7428 7365 6c66 3a20 4469 6d2c  right(self: Dim,
-000137e0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-000137f0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00013800: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00013810: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-00013820: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00013830: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
-00013840: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
-00013850: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
-00013860: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
-00013870: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
-00013880: 722c 206b 696e 643d 2263 6569 6c64 6976  r, kind="ceildiv
-00013890: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
-000138a0: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-000138b0: 726d 2e61 735f 6469 6d28 290a 0a20 2020  rm.as_dim()..   
-000138c0: 2064 6566 205f 5f6e 6567 5f5f 2873 656c   def __neg__(sel
-000138d0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000138e0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000138f0: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00013900: 2020 2020 2020 2020 7265 7475 726e 202d          return -
-00013910: 3120 2a20 7365 6c66 0a0a 2020 2020 6465  1 * self..    de
-00013920: 6620 6973 5f63 6f6e 7374 616e 745f 7374  f is_constant_st
-00013930: 6174 6963 5f64 696d 2873 656c 6629 202d  atic_dim(self) -
-00013940: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00013950: 2222 220a 2020 2020 2020 2020 3a72 6574  """.        :ret
-00013960: 7572 6e3a 2064 6572 6976 6564 206f 7020  urn: derived op 
-00013970: 6f66 2074 7970 6520 636f 6e73 7461 6e74  of type constant
-00013980: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013990: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000139a0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-000139b0: 2061 6e64 2073 656c 662e 6465 7269 7665   and self.derive
-000139c0: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
-000139d0: 3d20 2263 6f6e 7374 616e 7422 0a0a 0a64  = "constant"...d
-000139e0: 6566 205f 6d61 6b65 5f63 6f6e 7374 616e  ef _make_constan
-000139f0: 745f 7374 6174 6963 5f64 696d 2876 616c  t_static_dim(val
-00013a00: 7565 2c20 6b69 6e64 3d4e 6f6e 6529 3a0a  ue, kind=None):.
-00013a10: 2020 2020 2222 220a 2020 2020 3a70 6172      """.    :par
-00013a20: 616d 2069 6e74 2076 616c 7565 3a0a 2020  am int value:.  
-00013a30: 2020 3a70 6172 616d 2045 6e74 6974 797c    :param Entity|
-00013a40: 4e6f 6e65 206b 696e 643a 0a20 2020 203a  None kind:.    :
-00013a50: 7274 7970 653a 2044 696d 0a20 2020 2022  rtype: Dim.    "
-00013a60: 2222 0a20 2020 2072 6574 7572 6e20 5f64  "".    return _d
-00013a70: 2e44 696d 280a 2020 2020 2020 2020 6469  .Dim(.        di
-00013a80: 6d65 6e73 696f 6e3d 7661 6c75 652c 0a20  mension=value,. 
-00013a90: 2020 2020 2020 206b 696e 643d 6b69 6e64         kind=kind
-00013aa0: 206f 7220 4469 6d54 7970 6573 2e55 6e73   or DimTypes.Uns
-00013ab0: 7065 6369 6669 6564 2c0a 2020 2020 2020  pecified,.      
-00013ac0: 2020 6465 7363 7269 7074 696f 6e3d 2275    description="u
-00013ad0: 6e6e 616d 6564 5f25 7364 696d 5f25 6922  nnamed_%sdim_%i"
-00013ae0: 2025 2028 6b69 6e64 2e6e 616d 6520 2b20   % (kind.name + 
-00013af0: 225f 2220 6966 206b 696e 6420 656c 7365  "_" if kind else
-00013b00: 2022 222c 2076 616c 7565 292c 0a20 2020   "", value),.   
-00013b10: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
-00013b20: 6d5f 6f70 3d4f 7028 6b69 6e64 3d22 636f  m_op=Op(kind="co
-00013b30: 6e73 7461 6e74 222c 2069 6e70 7574 733d  nstant", inputs=
-00013b40: 5b5d 2c20 6174 7472 6962 733d 7b22 7661  [], attribs={"va
-00013b50: 6c75 6522 3a20 7661 6c75 657d 292c 0a20  lue": value}),. 
-00013b60: 2020 2020 2020 2061 7574 6f5f 6765 6e65         auto_gene
-00013b70: 7261 7465 643d 5472 7565 2c0a 2020 2020  rated=True,.    
-00013b80: 290a 0a0a 636c 6173 7320 4f70 3a0a 2020  )...class Op:.  
-00013b90: 2020 2222 220a 2020 2020 4f70 206f 6e20    """.    Op on 
-00013ba0: 3a63 6c61 7373 3a60 4469 6d60 2077 6869  :class:`Dim` whi
-00013bb0: 6368 2072 6573 756c 7473 2069 6e20 6120  ch results in a 
-00013bc0: 6465 7269 7665 6420 3a63 6c61 7373 3a60  derived :class:`
-00013bd0: 4469 6d60 2e0a 2020 2020 2222 220a 0a20  Dim`..    """.. 
-00013be0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00013bf0: 7365 6c66 2c20 6b69 6e64 2c20 696e 7075  self, kind, inpu
-00013c00: 7473 2c20 6174 7472 6962 733d 4e6f 6e65  ts, attribs=None
-00013c10: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00013c20: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-00013c30: 7220 6b69 6e64 3a20 2261 6464 222c 2022  r kind: "add", "
-00013c40: 7375 6222 2c20 226d 756c 222c 2022 6365  sub", "mul", "ce
-00013c50: 696c 6469 7622 0a20 2020 2020 2020 203a  ildiv".        :
-00013c60: 7061 7261 6d20 6c69 7374 5b44 696d 5d20  param list[Dim] 
-00013c70: 696e 7075 7473 3a0a 2020 2020 2020 2020  inputs:.        
-00013c80: 3a70 6172 616d 2064 6963 745b 7374 725d  :param dict[str]
-00013c90: 7c4e 6f6e 6520 6174 7472 6962 733a 0a20  |None attribs:. 
-00013ca0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013cb0: 2020 2073 656c 662e 6b69 6e64 203d 206b     self.kind = k
-00013cc0: 696e 640a 2020 2020 2020 2020 7365 6c66  ind.        self
-00013cd0: 2e69 6e70 7574 7320 3d20 696e 7075 7473  .inputs = inputs
-00013ce0: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
-00013cf0: 7470 7574 203d 204e 6f6e 6520 2023 2074  tput = None  # t
-00013d00: 7970 653a 204f 7074 696f 6e61 6c5b 5f64  ype: Optional[_d
-00013d10: 2e44 696d 5d0a 2020 2020 2020 2020 7365  .Dim].        se
-00013d20: 6c66 2e61 7474 7269 6273 203d 2061 7474  lf.attribs = att
-00013d30: 7269 6273 0a0a 2020 2020 6465 6620 5f5f  ribs..    def __
-00013d40: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
-00013d50: 2020 2020 2020 6174 7472 6962 7320 3d20        attribs = 
-00013d60: 2822 2025 7222 2025 2073 656c 662e 6174  (" %r" % self.at
-00013d70: 7472 6962 7329 2069 6620 7365 6c66 2e61  tribs) if self.a
-00013d80: 7474 7269 6273 2065 6c73 6520 2222 0a20  ttribs else "". 
-00013d90: 2020 2020 2020 2072 6574 7572 6e20 223c         return "<
-00013da0: 4469 6d2e 4f70 2025 7220 2573 2573 3e22  Dim.Op %r %s%s>"
-00013db0: 2025 2028 7365 6c66 2e6b 696e 642c 2073   % (self.kind, s
-00013dc0: 656c 662e 696e 7075 7473 2c20 6174 7472  elf.inputs, attr
-00013dd0: 6962 7329 0a0a 2020 2020 6465 6620 5f76  ibs)..    def _v
-00013de0: 616c 7565 2873 656c 6629 3a0a 2020 2020  alue(self):.    
-00013df0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00013e00: 6b69 6e64 2c20 7475 706c 6528 7365 6c66  kind, tuple(self
-00013e10: 2e69 6e70 7574 7329 2c20 6672 6f7a 656e  .inputs), frozen
-00013e20: 7365 7428 7365 6c66 2e61 7474 7269 6273  set(self.attribs
-00013e30: 2e69 7465 6d73 2829 2920 6966 2073 656c  .items()) if sel
-00013e40: 662e 6174 7472 6962 7320 656c 7365 204e  f.attribs else N
-00013e50: 6f6e 650a 0a20 2020 2064 6566 205f 5f68  one..    def __h
-00013e60: 6173 685f 5f28 7365 6c66 293a 0a20 2020  ash__(self):.   
-00013e70: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
-00013e80: 2873 656c 662e 5f76 616c 7565 2829 290a  (self._value()).
-00013e90: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
-00013ea0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-00013eb0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00013ec0: 6e63 6528 6f74 6865 722c 204f 7029 3a0a  nce(other, Op):.
-00013ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013ee0: 726e 2073 656c 662e 5f76 616c 7565 2829  rn self._value()
-00013ef0: 203d 3d20 6f74 6865 722e 5f76 616c 7565   == other._value
-00013f00: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00013f10: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00013f20: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
-00013f30: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-00013f40: 7475 726e 206e 6f74 2073 656c 662e 5f5f  turn not self.__
-00013f50: 6571 5f5f 286f 7468 6572 290a 0a0a 6465  eq__(other)...de
-00013f60: 6620 5f67 6574 5f64 6573 6372 6970 7469  f _get_descripti
-00013f70: 6f6e 2864 696d 2c20 6272 6163 6b65 7473  on(dim, brackets
-00013f80: 3d54 7275 6529 3a0a 2020 2020 2222 220a  =True):.    """.
-00013f90: 2020 2020 3a70 6172 616d 2044 696d 2064      :param Dim d
-00013fa0: 696d 3a0a 2020 2020 3a70 6172 616d 2062  im:.    :param b
-00013fb0: 6f6f 6c20 6272 6163 6b65 7473 3a20 6164  ool brackets: ad
-00013fc0: 6420 6272 6163 6b65 7473 2077 6865 6e20  d brackets when 
-00013fd0: 6e65 6365 7373 6172 790a 2020 2020 3a72  necessary.    :r
-00013fe0: 7479 7065 3a20 7374 720a 2020 2020 2222  type: str.    ""
-00013ff0: 220a 2020 2020 6966 2064 696d 2e64 6573  ".    if dim.des
-00014000: 6372 6970 7469 6f6e 2061 6e64 2064 696d  cription and dim
-00014010: 2e64 6573 6372 6970 7469 6f6e 2e73 7461  .description.sta
-00014020: 7274 7377 6974 6828 2275 6e6e 616d 6564  rtswith("unnamed
-00014030: 5f22 2920 616e 6420 6469 6d2e 6469 6d65  _") and dim.dime
-00014040: 6e73 696f 6e20 6973 206e 6f74 204e 6f6e  nsion is not Non
-00014050: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00014060: 6e20 7374 7228 6469 6d2e 6469 6d65 6e73  n str(dim.dimens
-00014070: 696f 6e29 0a20 2020 2069 6620 6469 6d2e  ion).    if dim.
-00014080: 6465 7363 7269 7074 696f 6e3a 0a20 2020  description:.   
-00014090: 2020 2020 2069 6620 6272 6163 6b65 7473       if brackets
-000140a0: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
-000140b0: 706f 7274 2072 650a 0a20 2020 2020 2020  port re..       
-000140c0: 2020 2020 2069 6620 7265 2e73 6561 7263       if re.searc
-000140d0: 6828 225b 2b5c 5c2d 2f20 5d22 2c20 6469  h("[+\\-/ ]", di
-000140e0: 6d2e 6465 7363 7269 7074 696f 6e29 3a0a  m.description):.
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014100: 7265 7475 726e 2022 2825 7329 2220 2520  return "(%s)" % 
-00014110: 6469 6d2e 6465 7363 7269 7074 696f 6e0a  dim.description.
-00014120: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00014130: 696d 2e64 6573 6372 6970 7469 6f6e 0a20  im.description. 
-00014140: 2020 2072 6574 7572 6e20 2275 6e6e 616d     return "unnam
-00014150: 6564 5f25 735f 6469 6d25 7322 2025 2028  ed_%s_dim%s" % (
-00014160: 6469 6d2e 6b69 6e64 2c20 6469 6d2e 6469  dim.kind, dim.di
-00014170: 6d65 6e73 696f 6e20 6966 2064 696d 2e64  mension if dim.d
-00014180: 696d 656e 7369 6f6e 2069 7320 6e6f 7420  imension is not 
-00014190: 4e6f 6e65 2065 6c73 6520 223f 2229 0a0a  None else "?")..
-000141a0: 0a63 6c61 7373 205f 4f70 4d75 6c74 5465  .class _OpMultTe
-000141b0: 726d 3a0a 2020 2020 2222 220a 2020 2020  rm:.    """.    
-000141c0: 7265 7072 6573 656e 7473 2073 7468 206c  represents sth l
-000141d0: 696b 6520 6120 2a20 6220 2a20 630a 2020  ike a * b * c.  
-000141e0: 2020 2222 220a 0a20 2020 2040 636c 6173    """..    @clas
-000141f0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00014200: 6672 6f6d 5f64 696d 2863 6c73 2c20 6469  from_dim(cls, di
-00014210: 6d3a 205f 642e 4469 6d29 202d 3e20 5f4f  m: _d.Dim) -> _O
-00014220: 704d 756c 7454 6572 6d3a 0a20 2020 2020  pMultTerm:.     
-00014230: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00014240: 7061 7261 6d20 6469 6d3a 0a20 2020 2020  param dim:.     
-00014250: 2020 203a 7265 7475 726e 3a20 6f70 206d     :return: op m
-00014260: 756c 7420 7465 726d 0a20 2020 2020 2020  ult term.       
-00014270: 2022 2222 0a20 2020 2020 2020 2064 696d   """.        dim
-00014280: 203d 2064 696d 2e67 6574 5f73 616d 655f   = dim.get_same_
-00014290: 6261 7365 2829 0a20 2020 2020 2020 2069  base().        i
-000142a0: 6620 6469 6d2e 6469 6d65 6e73 696f 6e20  f dim.dimension 
-000142b0: 3d3d 2031 2061 6e64 2064 696d 2e69 735f  == 1 and dim.is_
-000142c0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-000142d0: 6469 6d28 293a 0a20 2020 2020 2020 2020  dim():.         
-000142e0: 2020 2072 6574 7572 6e20 636c 732e 6f6e     return cls.on
-000142f0: 6528 290a 2020 2020 2020 2020 6966 2064  e().        if d
-00014300: 696d 2e64 6572 6976 6564 5f66 726f 6d5f  im.derived_from_
-00014310: 6f70 2061 6e64 2064 696d 2e64 6572 6976  op and dim.deriv
-00014320: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-00014330: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00014340: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
-00014350: 286c 6973 7428 6469 6d2e 6465 7269 7665  (list(dim.derive
-00014360: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
-00014370: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-00014380: 6e20 636c 7328 5b64 696d 5d29 0a0a 2020  n cls([dim])..  
-00014390: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-000143a0: 2020 2064 6566 2066 726f 6d5f 6469 6d5f     def from_dim_
-000143b0: 6661 6374 6f72 7328 636c 732c 2064 696d  factors(cls, dim
-000143c0: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
-000143d0: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-000143e0: 6973 745b 4469 6d5d 2064 696d 733a 0a20  ist[Dim] dims:. 
-000143f0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00014400: 696d 2e5f 4f70 4d75 6c74 5465 726d 0a20  im._OpMultTerm. 
-00014410: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014420: 2020 2072 6573 203d 2063 6c73 2e6f 6e65     res = cls.one
-00014430: 2829 0a20 2020 2020 2020 2066 6f72 2064  ().        for d
-00014440: 2069 6e20 6469 6d73 3a0a 2020 2020 2020   in dims:.      
-00014450: 2020 2020 2020 7265 732e 6578 7465 6e64        res.extend
-00014460: 5f6d 756c 5f64 6976 5f28 642c 206b 696e  _mul_div_(d, kin
-00014470: 643d 226d 756c 222c 2072 6967 6874 3d54  d="mul", right=T
-00014480: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-00014490: 7572 6e20 7265 730a 0a20 2020 2040 636c  urn res..    @cl
-000144a0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000144b0: 6620 6f6e 6528 636c 7329 3a0a 2020 2020  f one(cls):.    
-000144c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000144d0: 3a72 7479 7065 3a20 4469 6d2e 5f4f 704d  :rtype: Dim._OpM
-000144e0: 756c 7454 6572 6d0a 2020 2020 2020 2020  ultTerm.        
-000144f0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00014500: 726e 2063 6c73 285b 5d29 0a0a 2020 2020  rn cls([])..    
-00014510: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00014520: 662c 2074 6572 6d73 293a 0a20 2020 2020  f, terms):.     
-00014530: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00014540: 7061 7261 6d20 6c69 7374 5b44 696d 5d20  param list[Dim] 
-00014550: 7465 726d 733a 0a20 2020 2020 2020 2022  terms:.        "
-00014560: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00014570: 7465 726d 7320 3d20 7465 726d 730a 0a20  terms = terms.. 
-00014580: 2020 2064 6566 205f 5f68 6173 685f 5f28     def __hash__(
-00014590: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-000145a0: 6574 7572 6e20 6861 7368 2874 7570 6c65  eturn hash(tuple
-000145b0: 2873 656c 662e 7465 726d 7329 290a 0a20  (self.terms)).. 
-000145c0: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
-000145d0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-000145e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000145f0: 3a70 6172 616d 2044 696d 7c44 696d 2e5f  :param Dim|Dim._
-00014600: 4f70 4d75 6c74 5465 726d 206f 7468 6572  OpMultTerm other
-00014610: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00014620: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00014630: 6e63 6528 6f74 6865 722c 205f 4f70 4d75  nce(other, _OpMu
-00014640: 6c74 5465 726d 293a 0a20 2020 2020 2020  ltTerm):.       
-00014650: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00014660: 2e74 6572 6d73 203d 3d20 6f74 6865 722e  .terms == other.
-00014670: 7465 726d 730a 2020 2020 2020 2020 7265  terms.        re
-00014680: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-00014690: 6465 6620 5f5f 6e65 5f5f 2873 656c 662c  def __ne__(self,
-000146a0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-000146b0: 2072 6574 7572 6e20 6e6f 7420 7365 6c66   return not self
-000146c0: 2e5f 5f65 715f 5f28 6f74 6865 7229 0a0a  .__eq__(other)..
-000146d0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-000146e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000146f0: 7265 7475 726e 2022 4469 6d2e 5f4f 704d  return "Dim._OpM
-00014700: 756c 7454 6572 6d28 2572 2922 2025 2028  ultTerm(%r)" % (
-00014710: 7365 6c66 2e74 6572 6d73 2c29 0a0a 2020  self.terms,)..  
-00014720: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00014730: 6465 6620 6469 6d65 6e73 696f 6e28 7365  def dimension(se
-00014740: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00014750: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00014760: 2069 6e74 7c4e 6f6e 650a 2020 2020 2020   int|None.      
-00014770: 2020 2222 220a 2020 2020 2020 2020 6469    """.        di
-00014780: 6d20 3d20 310a 2020 2020 2020 2020 666f  m = 1.        fo
-00014790: 7220 7061 7274 2069 6e20 7365 6c66 2e74  r part in self.t
-000147a0: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
-000147b0: 2020 6966 2070 6172 742e 6469 6d65 6e73    if part.dimens
-000147c0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-000147d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000147e0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-000147f0: 2020 2020 2064 696d 202a 3d20 7061 7274       dim *= part
-00014800: 2e64 696d 656e 7369 6f6e 0a20 2020 2020  .dimension.     
-00014810: 2020 2072 6574 7572 6e20 6469 6d0a 0a20     return dim.. 
-00014820: 2020 2064 6566 2062 6173 655f 7465 726d     def base_term
-00014830: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00014840: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-00014850: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
-00014860: 2222 220a 2020 2020 2020 2020 6173 7365  """.        asse
-00014870: 7274 2073 656c 662e 7465 726d 730a 2020  rt self.terms.  
-00014880: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00014890: 662e 7465 726d 735b 2d31 5d0a 0a20 2020  f.terms[-1]..   
-000148a0: 2064 6566 2069 735f 6f6e 6528 7365 6c66   def is_one(self
-000148b0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000148c0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-000148d0: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-000148e0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-000148f0: 6f74 2073 656c 662e 7465 726d 730a 0a20  ot self.terms.. 
-00014900: 2020 2064 6566 2069 735f 636f 6e73 7461     def is_consta
-00014910: 6e74 5f73 7461 7469 635f 6469 6d28 7365  nt_static_dim(se
-00014920: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00014930: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00014940: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-00014950: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00014960: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
-00014970: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014980: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-00014990: 7572 6e20 616c 6c28 7465 726d 2e69 735f  urn all(term.is_
-000149a0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-000149b0: 6469 6d28 2920 666f 7220 7465 726d 2069  dim() for term i
-000149c0: 6e20 7365 6c66 2e74 6572 6d73 290a 0a20  n self.terms).. 
-000149d0: 2020 2064 6566 2063 6f70 7928 7365 6c66     def copy(self
-000149e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000149f0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00014a00: 696d 2e5f 4f70 4d75 6c74 5465 726d 0a20  im._OpMultTerm. 
-00014a10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014a20: 2020 2072 6574 7572 6e20 5f4f 704d 756c     return _OpMul
-00014a30: 7454 6572 6d28 6c69 7374 2873 656c 662e  tTerm(list(self.
-00014a40: 7465 726d 7329 290a 0a20 2020 2064 6566  terms))..    def
-00014a50: 206e 6567 6174 6976 6528 7365 6c66 293a   negative(self):
-00014a60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014a70: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00014a80: 2e5f 4f70 4d75 6c74 5465 726d 0a20 2020  ._OpMultTerm.   
-00014a90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014aa0: 2069 6620 7365 6c66 2e74 6572 6d73 2061   if self.terms a
-00014ab0: 6e64 2073 656c 662e 7465 726d 735b 305d  nd self.terms[0]
-00014ac0: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
-00014ad0: 7469 635f 6469 6d28 2920 616e 6420 7365  tic_dim() and se
-00014ae0: 6c66 2e74 6572 6d73 5b30 5d2e 6469 6d65  lf.terms[0].dime
-00014af0: 6e73 696f 6e20 3d3d 202d 313a 0a20 2020  nsion == -1:.   
-00014b00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014b10: 5f4f 704d 756c 7454 6572 6d28 7365 6c66  _OpMultTerm(self
-00014b20: 2e74 6572 6d73 5b31 3a5d 290a 2020 2020  .terms[1:]).    
-00014b30: 2020 2020 7265 7320 3d20 7365 6c66 2e63      res = self.c
-00014b40: 6f70 7928 290a 2020 2020 2020 2020 7265  opy().        re
-00014b50: 732e 6578 7465 6e64 5f6d 756c 5f64 6976  s.extend_mul_div
-00014b60: 5f28 5f6d 616b 655f 636f 6e73 7461 6e74  _(_make_constant
-00014b70: 5f73 7461 7469 635f 6469 6d28 2d31 292c  _static_dim(-1),
-00014b80: 206b 696e 643d 226d 756c 222c 2072 6967   kind="mul", rig
-00014b90: 6874 3d46 616c 7365 290a 2020 2020 2020  ht=False).      
-00014ba0: 2020 7265 7475 726e 2072 6573 0a0a 2020    return res..  
-00014bb0: 2020 6465 6620 6469 7669 7369 626c 6528    def divisible(
-00014bc0: 7365 6c66 2c20 6f74 6865 722c 2072 6967  self, other, rig
-00014bd0: 6874 293a 0a20 2020 2020 2020 2022 2222  ht):.        """
-00014be0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00014bf0: 4469 6d20 6f74 6865 723a 0a20 2020 2020  Dim other:.     
-00014c00: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-00014c10: 6967 6874 3a0a 2020 2020 2020 2020 3a72  ight:.        :r
-00014c20: 6574 7572 6e3a 2077 6865 7468 6572 2077  eturn: whether w
-00014c30: 6520 6361 6e20 6469 7669 6465 206f 7468  e can divide oth
-00014c40: 6572 2c20 7769 7468 6f75 7420 7265 6d61  er, without rema
-00014c50: 696e 6465 720a 2020 2020 2020 2020 3a72  inder.        :r
-00014c60: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
-00014c70: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00014c80: 6620 6e6f 7420 7365 6c66 2e74 6572 6d73  f not self.terms
-00014c90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00014ca0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00014cb0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-00014cc0: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-00014cd0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00014ce0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 226d  om_op.kind == "m
-00014cf0: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00014d00: 2074 6d70 203d 2073 656c 662e 636f 7079   tmp = self.copy
-00014d10: 2829 0a20 2020 2020 2020 2020 2020 2066  ().            f
-00014d20: 6f72 2074 6572 6d20 696e 206f 7468 6572  or term in other
-00014d30: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00014d40: 2e69 6e70 7574 7320 6966 2072 6967 6874  .inputs if right
-00014d50: 2065 6c73 6520 7265 7665 7273 6564 286f   else reversed(o
-00014d60: 7468 6572 2e64 6572 6976 6564 5f66 726f  ther.derived_fro
-00014d70: 6d5f 6f70 2e69 6e70 7574 7329 3a0a 2020  m_op.inputs):.  
-00014d80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014d90: 206e 6f74 2074 6d70 2e64 6976 6973 6962   not tmp.divisib
-00014da0: 6c65 2874 6572 6d2c 2072 6967 6874 3d72  le(term, right=r
-00014db0: 6967 6874 293a 0a20 2020 2020 2020 2020  ight):.         
-00014dc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014dd0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00014de0: 2020 2020 2020 2020 746d 702e 6578 7465          tmp.exte
-00014df0: 6e64 5f6d 756c 5f64 6976 5f28 7465 726d  nd_mul_div_(term
-00014e00: 2c20 6b69 6e64 3d22 7472 7565 6469 7622  , kind="truediv"
-00014e10: 2c20 7269 6768 743d 7269 6768 7429 0a20  , right=right). 
-00014e20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014e30: 6e20 5472 7565 0a20 2020 2020 2020 206d  n True.        m
-00014e40: 6f73 745f 7265 6365 6e74 5f74 6572 6d20  ost_recent_term 
-00014e50: 3d20 7365 6c66 2e74 6572 6d73 5b2d 3120  = self.terms[-1 
-00014e60: 6966 2072 6967 6874 2065 6c73 6520 305d  if right else 0]
-00014e70: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-00014e80: 7220 3d3d 206d 6f73 745f 7265 6365 6e74  r == most_recent
-00014e90: 5f74 6572 6d3a 0a20 2020 2020 2020 2020  _term:.         
-00014ea0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00014eb0: 2020 2020 2020 2069 6620 6d6f 7374 5f72         if most_r
-00014ec0: 6563 656e 745f 7465 726d 2e64 696d 656e  ecent_term.dimen
-00014ed0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-00014ee0: 2061 6e64 206f 7468 6572 2e64 696d 656e   and other.dimen
-00014ef0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-00014f00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014f10: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-00014f20: 6d2e 6469 6d65 6e73 696f 6e20 2520 6f74  m.dimension % ot
-00014f30: 6865 722e 6469 6d65 6e73 696f 6e20 3d3d  her.dimension ==
-00014f40: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00014f50: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00014f60: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00014f70: 616c 7365 0a0a 2020 2020 6465 6620 6361  alse..    def ca
-00014f80: 6e5f 7369 6d70 6c69 6679 2873 656c 662c  n_simplify(self,
-00014f90: 206f 7468 6572 2c20 6b69 6e64 2c20 7269   other, kind, ri
-00014fa0: 6768 7429 3a0a 2020 2020 2020 2020 2222  ght):.        ""
-00014fb0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00014fc0: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
-00014fd0: 2020 2020 3a70 6172 616d 2073 7472 206b      :param str k
-00014fe0: 696e 643a 0a20 2020 2020 2020 203a 7061  ind:.        :pa
-00014ff0: 7261 6d20 626f 6f6c 2072 6967 6874 3a0a  ram bool right:.
-00015000: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00015010: 2077 6865 7468 6572 2077 6520 6361 6e20   whether we can 
-00015020: 7369 6d70 6c69 6679 2077 6865 6e20 6170  simplify when ap
-00015030: 706c 7969 6e67 2074 6869 7320 6f70 6572  plying this oper
-00015040: 6174 696f 6e0a 2020 2020 2020 2020 3a72  ation.        :r
-00015050: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
-00015060: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00015070: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-00015080: 6672 6f6d 5f6f 7020 616e 6420 6f74 6865  from_op and othe
-00015090: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-000150a0: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
-000150b0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-000150c0: 203d 2073 656c 662e 636f 7079 2829 0a20   = self.copy(). 
-000150d0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-000150e0: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
-000150f0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00015100: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
-00015110: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
-00015120: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00015130: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
-00015140: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00015150: 2074 6d70 2e63 616e 5f73 696d 706c 6966   tmp.can_simplif
-00015160: 7928 7465 726d 2c20 6b69 6e64 3d6b 696e  y(term, kind=kin
-00015170: 642c 2072 6967 6874 3d72 6967 6874 293a  d, right=right):
-00015180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015190: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000151a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000151b0: 2020 746d 702e 6578 7465 6e64 5f6d 756c    tmp.extend_mul
-000151c0: 5f64 6976 5f28 7465 726d 2c20 6b69 6e64  _div_(term, kind
-000151d0: 3d6b 696e 642c 2072 6967 6874 3d72 6967  =kind, right=rig
-000151e0: 6874 290a 2020 2020 2020 2020 2020 2020  ht).            
-000151f0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00015200: 2020 2020 6964 7820 3d20 7365 6c66 2e5f      idx = self._
-00015210: 7369 6d70 6c69 6679 5f74 6572 6d5f 6964  simplify_term_id
-00015220: 7828 6f74 6865 722c 206b 696e 643d 6b69  x(other, kind=ki
-00015230: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
-00015240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015250: 6964 7820 6973 206e 6f74 204e 6f6e 650a  idx is not None.
-00015260: 0a20 2020 2064 6566 205f 7369 6d70 6c69  .    def _simpli
-00015270: 6679 5f74 6572 6d5f 6964 7828 7365 6c66  fy_term_idx(self
-00015280: 2c20 6f74 6865 722c 206b 696e 642c 2072  , other, kind, r
-00015290: 6967 6874 293a 0a20 2020 2020 2020 2022  ight):.        "
-000152a0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-000152b0: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
-000152c0: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
-000152d0: 6b69 6e64 3a0a 2020 2020 2020 2020 3a70  kind:.        :p
-000152e0: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
-000152f0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00015300: 3a20 696e 6465 7820 6f66 2074 6572 6d20  : index of term 
-00015310: 746f 2073 696d 706c 6966 790a 2020 2020  to simplify.    
-00015320: 2020 2020 3a72 7479 7065 3a20 696e 747c      :rtype: int|
-00015330: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00015340: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00015350: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
-00015360: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00015370: 6f6e 650a 2020 2020 2020 2020 6966 206b  one.        if k
-00015380: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
-00015390: 2020 2020 2020 2020 2020 2320 5765 2077            # We w
-000153a0: 616e 7420 2862 202a 2061 2920 2f2f 2062  ant (b * a) // b
-000153b0: 2021 3d20 612e 0a20 2020 2020 2020 2020   != a..         
-000153c0: 2020 2023 2048 6f77 6576 6572 2c20 7765     # However, we
-000153d0: 2077 616e 7420 6820 2a20 2832 202a 2061   want h * (2 * a
-000153e0: 202f 2f20 6829 203d 3d20 3220 2a20 612e   // h) == 2 * a.
-000153f0: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00015400: 6f2c 2066 6f72 2060 6d75 6c60 2c20 616e  o, for `mul`, an
-00015410: 6420 6f6e 6c79 2066 6f72 2060 6d75 6c60  d only for `mul`
-00015420: 2c20 6368 6563 6b20 616c 6c20 7465 726d  , check all term
-00015430: 732c 2077 6865 7468 6572 2077 6520 6361  s, whether we ca
-00015440: 6e20 7369 6d70 6c69 6679 2073 6f6d 6520  n simplify some 
-00015450: 6469 7669 7369 6f6e 2d74 6572 6d2e 0a20  division-term.. 
-00015460: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00015470: 2c20 7465 726d 2069 6e20 7265 7665 7273  , term in revers
-00015480: 6564 286c 6973 7428 656e 756d 6572 6174  ed(list(enumerat
-00015490: 6528 7365 6c66 2e74 6572 6d73 2929 2920  e(self.terms))) 
-000154a0: 6966 2072 6967 6874 2065 6c73 6520 656e  if right else en
-000154b0: 756d 6572 6174 6528 7365 6c66 2e74 6572  umerate(self.ter
-000154c0: 6d73 293a 0a20 2020 2020 2020 2020 2020  ms):.           
-000154d0: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-000154e0: 7374 616e 6365 2874 6572 6d2c 205f 642e  stance(term, _d.
-000154f0: 4469 6d29 0a20 2020 2020 2020 2020 2020  Dim).           
-00015500: 2020 2020 2069 6620 7465 726d 2e64 6572       if term.der
-00015510: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
-00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015530: 2020 6966 2074 6572 6d2e 6465 7269 7665    if term.derive
-00015540: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
-00015550: 3d20 2274 7275 6564 6976 5f22 202b 2028  = "truediv_" + (
-00015560: 2272 6967 6874 2220 6966 2072 6967 6874  "right" if right
-00015570: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
+000113f0: 2020 2020 6469 6d73 5f5b 3a5d 203d 205b      dims_[:] = [
+00011400: 7461 6720 6966 2064 203d 3d20 6578 6973  tag if d == exis
+00011410: 7469 6e67 5f74 6167 2065 6c73 6520 6420  ting_tag else d 
+00011420: 666f 7220 6420 696e 2064 696d 735f 5d0a  for d in dims_].
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
+00011450: 5f74 6167 203d 2074 6167 0a20 2020 2020  _tag = tag.     
+00011460: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011470: 2020 2320 6e6f 2065 7869 7374 696e 6720    # no existing 
+00011480: 7461 670a 2020 2020 2020 2020 2020 2020  tag.            
+00011490: 2020 2020 2020 2020 7461 6773 2e61 7070          tags.app
+000114a0: 656e 6428 7461 6729 0a20 2020 2020 2020  end(tag).       
+000114b0: 2020 2020 2020 2020 2064 6174 615f 6178           data_ax
+000114c0: 6573 5f64 6963 745b 6461 7461 5d2e 6170  es_dict[data].ap
+000114d0: 7065 6e64 2865 7869 7374 696e 675f 7461  pend(existing_ta
+000114e0: 6720 6f72 2074 6167 290a 2020 2020 2020  g or tag).      
+000114f0: 2020 7265 7475 726e 2074 6167 732c 2064    return tags, d
+00011500: 6174 615f 6178 6573 5f64 6963 740a 0a20  ata_axes_dict.. 
+00011510: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00011520: 2020 2020 6465 6620 6765 745f 756e 6971      def get_uniq
+00011530: 5f63 6f6c 6c65 6374 696f 6e28 636c 732c  _collection(cls,
+00011540: 2074 6167 732c 2069 735f 6571 7561 6c5f   tags, is_equal_
+00011550: 6f70 7473 3d4e 6f6e 6529 3a0a 2020 2020  opts=None):.    
+00011560: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011570: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
+00011580: 7c74 7570 6c65 5b44 696d 5d7c 7365 745b  |tuple[Dim]|set[
+00011590: 4469 6d5d 2074 6167 733a 0a20 2020 2020  Dim] tags:.     
+000115a0: 2020 203a 7061 7261 6d20 6469 6374 5b73     :param dict[s
+000115b0: 7472 5d7c 4e6f 6e65 2069 735f 6571 7561  tr]|None is_equa
+000115c0: 6c5f 6f70 7473 3a20 7061 7373 6564 2074  l_opts: passed t
+000115d0: 6f20 4469 6d2e 6973 5f65 7175 616c 0a20  o Dim.is_equal. 
+000115e0: 2020 2020 2020 203a 7274 7970 653a 206c         :rtype: l
+000115f0: 6973 745b 4469 6d5d 0a20 2020 2020 2020  ist[Dim].       
+00011600: 2022 2222 0a20 2020 2020 2020 2072 6573   """.        res
+00011610: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00011620: 7220 7461 6720 696e 2074 6167 733a 0a20  r tag in tags:. 
+00011630: 2020 2020 2020 2020 2020 2065 7820 3d20             ex = 
+00011640: 636c 732e 6765 745f 6578 6973 7469 6e67  cls.get_existing
+00011650: 5f74 6167 5f66 726f 6d5f 636f 6c6c 6563  _tag_from_collec
+00011660: 7469 6f6e 2874 6167 2c20 7265 732c 2069  tion(tag, res, i
+00011670: 735f 6571 7561 6c5f 6f70 7473 3d69 735f  s_equal_opts=is_
+00011680: 6571 7561 6c5f 6f70 7473 290a 2020 2020  equal_opts).    
+00011690: 2020 2020 2020 2020 6966 206e 6f74 2065          if not e
+000116a0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
+000116b0: 2020 2072 6573 2e61 7070 656e 6428 7461     res.append(ta
+000116c0: 6729 0a20 2020 2020 2020 2072 6574 7572  g).        retur
+000116d0: 6e20 7265 730a 0a20 2020 2064 6566 2067  n res..    def g
+000116e0: 6574 5f73 697a 655f 7465 6e73 6f72 2873  et_size_tensor(s
+000116f0: 656c 6629 202d 3e20 5f74 2e54 656e 736f  elf) -> _t.Tenso
+00011700: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+00011710: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00011720: 7369 7a65 2074 656e 736f 722c 206f 7220  size tensor, or 
+00011730: 6479 6e5f 7369 7a65 5f65 7874 2069 6620  dyn_size_ext if 
+00011740: 6465 6669 6e65 640a 2020 2020 2020 2020  defined.        
+00011750: 3a72 7479 7065 3a20 5f74 2e54 656e 736f  :rtype: _t.Tenso
+00011760: 720a 2020 2020 2020 2020 2222 220a 2020  r.        """.  
+00011770: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+00011780: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+00011790: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000117a0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+000117b0: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+000117c0: 2072 6574 7572 6e6e 2e66 726f 6e74 656e   returnn.fronten
+000117d0: 6420 6173 2072 660a 0a20 2020 2020 2020  d as rf..       
+000117e0: 2061 7373 6572 7420 7365 6c66 2e73 697a   assert self.siz
+000117f0: 6520 6973 206e 6f74 204e 6f6e 650a 2020  e is not None.  
+00011800: 2020 2020 2020 7265 7475 726e 2072 662e        return rf.
+00011810: 636f 6e76 6572 745f 746f 5f74 656e 736f  convert_to_tenso
+00011820: 7228 7365 6c66 2e73 697a 652c 206e 616d  r(self.size, nam
+00011830: 653d 2225 733a 7369 7a65 2220 2520 7365  e="%s:size" % se
+00011840: 6c66 2e64 6573 6372 6970 7469 6f6e 290a  lf.description).
+00011850: 0a20 2020 2064 6566 2067 6574 5f64 696d  .    def get_dim
+00011860: 5f76 616c 7565 2873 656c 6629 202d 3e20  _value(self) -> 
+00011870: 556e 696f 6e5b 696e 742c 205f 742e 5261  Union[int, _t.Ra
+00011880: 7754 656e 736f 7254 7970 655d 3a0a 2020  wTensorType]:.  
+00011890: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000118a0: 2020 496e 6665 7273 2074 6865 2064 696d    Infers the dim
+000118b0: 2074 6869 7320 6178 6973 2073 686f 756c   this axis shoul
+000118c0: 6420 6861 7665 2069 6620 756e 6272 6f61  d have if unbroa
+000118d0: 6463 6173 7465 642e 0a20 2020 2020 2020  dcasted..       
+000118e0: 2049 6620 6073 656c 662e 7372 635f 6461   If `self.src_da
+000118f0: 7461 6020 6861 7320 6120 706c 6163 6568  ta` has a placeh
+00011900: 6f6c 6465 722c 2077 696c 6c20 7573 6520  older, will use 
+00011910: 7468 6520 7368 6170 6520 6672 6f6d 2074  the shape from t
+00011920: 6865 7265 2e0a 2020 2020 2020 2020 4f74  here..        Ot
+00011930: 6865 7277 6973 652c 2075 7365 7320 6073  herwise, uses `s
+00011940: 656c 662e 6469 6d65 6e73 696f 6e60 2028  elf.dimension` (
+00011950: 6966 2073 7461 7469 6329 206f 7220 6073  if static) or `s
+00011960: 656c 662e 6479 6e5f 7369 7a65 6020 2869  elf.dyn_size` (i
+00011970: 6620 6479 6e61 6d69 6329 2e0a 0a20 2020  f dynamic)...   
+00011980: 2020 2020 203a 7265 7475 726e 3a20 6d61       :return: ma
+00011990: 7828 7369 7a65 206f 7220 6479 6e5f 7369  x(size or dyn_si
+000119a0: 7a65 290a 2020 2020 2020 2020 2222 220a  ze).        """.
+000119b0: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+000119c0: 6c66 2e67 6574 5f64 696d 5f76 616c 7565  lf.get_dim_value
+000119d0: 5f74 656e 736f 7228 290a 2020 2020 2020  _tensor().      
+000119e0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000119f0: 7265 732c 205f 742e 5465 6e73 6f72 293a  res, _t.Tensor):
+00011a00: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00011a10: 6572 7420 7265 732e 6469 6d73 203d 3d20  ert res.dims == 
+00011a20: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+00011a30: 6574 7572 6e20 7265 732e 7261 775f 7465  eturn res.raw_te
+00011a40: 6e73 6f72 0a20 2020 2020 2020 2061 7373  nsor.        ass
+00011a50: 6572 7420 6973 696e 7374 616e 6365 2872  ert isinstance(r
+00011a60: 6573 2c20 696e 7429 0a20 2020 2020 2020  es, int).       
+00011a70: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
+00011a80: 2064 6566 2067 6574 5f64 696d 5f76 616c   def get_dim_val
+00011a90: 7565 5f74 656e 736f 7228 7365 6c66 2920  ue_tensor(self) 
+00011aa0: 2d3e 2055 6e69 6f6e 5b69 6e74 2c20 5f74  -> Union[int, _t
+00011ab0: 2e54 656e 736f 725d 3a0a 2020 2020 2020  .Tensor]:.      
+00011ac0: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
+00011ad0: 6665 7273 2074 6865 2064 696d 2074 6869  fers the dim thi
+00011ae0: 7320 6178 6973 2073 686f 756c 6420 6861  s axis should ha
+00011af0: 7665 2069 6620 756e 6272 6f61 6463 6173  ve if unbroadcas
+00011b00: 7465 642e 0a20 2020 2020 2020 2049 6620  ted..        If 
+00011b10: 6073 656c 662e 7372 635f 6461 7461 6020  `self.src_data` 
+00011b20: 6861 7320 6120 706c 6163 6568 6f6c 6465  has a placeholde
+00011b30: 722c 2077 696c 6c20 7573 6520 7468 6520  r, will use the 
+00011b40: 7368 6170 6520 6672 6f6d 2074 6865 7265  shape from there
+00011b50: 2e0a 2020 2020 2020 2020 4f74 6865 7277  ..        Otherw
+00011b60: 6973 652c 2075 7365 7320 6073 656c 662e  ise, uses `self.
+00011b70: 6469 6d65 6e73 696f 6e60 2028 6966 2073  dimension` (if s
+00011b80: 7461 7469 6329 206f 7220 6073 656c 662e  tatic) or `self.
+00011b90: 6479 6e5f 7369 7a65 6020 2869 6620 6479  dyn_size` (if dy
+00011ba0: 6e61 6d69 6329 2e0a 0a20 2020 2020 2020  namic)...       
+00011bb0: 203a 7265 7475 726e 3a20 6d61 7828 7369   :return: max(si
+00011bc0: 7a65 206f 7220 6479 6e5f 7369 7a65 290a  ze or dyn_size).
+00011bd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011be0: 2020 2020 696d 706f 7274 2072 6574 7572      import retur
+00011bf0: 6e6e 2e66 726f 6e74 656e 6420 6173 2072  nn.frontend as r
+00011c00: 660a 0a20 2020 2020 2020 2069 6620 7365  f..        if se
+00011c10: 6c66 2e64 696d 656e 7369 6f6e 2069 7320  lf.dimension is 
+00011c20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011c30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00011c40: 662e 6469 6d65 6e73 696f 6e0a 2020 2020  f.dimension.    
+00011c50: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
+00011c60: 7369 7a65 5f65 7874 2061 6e64 2073 656c  size_ext and sel
+00011c70: 662e 6479 6e5f 7369 7a65 5f65 7874 2e70  f.dyn_size_ext.p
+00011c80: 6c61 6365 686f 6c64 6572 2069 7320 6e6f  laceholder is no
+00011c90: 7420 4e6f 6e65 3a20 2023 2066 6173 7420  t None:  # fast 
+00011ca0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00011cb0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+00011cc0: 655f 6578 742e 6261 7463 685f 6e64 696d  e_ext.batch_ndim
+00011cd0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00011ce0: 2020 2020 2020 7265 7475 726e 2072 662e        return rf.
+00011cf0: 7265 6475 6365 5f6d 6178 280a 2020 2020  reduce_max(.    
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d10: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00011d20: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00011d30: 2020 2020 2020 2061 7869 733d 7365 6c66         axis=self
+00011d40: 2e64 796e 5f73 697a 655f 6578 742e 6469  .dyn_size_ext.di
+00011d50: 6d5f 7461 6773 2c0a 2020 2020 2020 2020  m_tags,.        
+00011d60: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
+00011d70: 736b 696e 6720 6973 206e 6f74 2061 6c77  sking is not alw
+00011d80: 6179 7320 706f 7373 6962 6c65 2068 6572  ays possible her
+00011d90: 652c 2065 2e67 2e0a 2020 2020 2020 2020  e, e.g..        
+00011da0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00011db0: 6c66 203d 2044 696d 7b27 7365 6c66 2d61  lf = Dim{'self-a
+00011dc0: 7474 2d6b 6579 7327 5b27 7469 6d65 3a76  tt-keys'['time:v
+00011dd0: 6172 3a65 7874 6572 6e5f 6461 7461 3a63  ar:extern_data:c
+00011de0: 6c61 7373 6573 275b 425d 5d7d 2e0a 2020  lasses'[B]]}..  
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e00: 2020 7573 655f 6d61 736b 3d46 616c 7365    use_mask=False
+00011e10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011e20: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00011e30: 7265 7475 726e 2073 656c 662e 6479 6e5f  return self.dyn_
+00011e40: 7369 7a65 5f65 7874 0a20 2020 2020 2020  size_ext.       
+00011e50: 2069 6620 7365 6c66 2e69 735f 6261 7463   if self.is_batc
+00011e60: 685f 6469 6d28 293a 0a20 2020 2020 2020  h_dim():.       
+00011e70: 2020 2020 2072 6573 203d 204e 6f6e 650a       res = None.
+00011e80: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00011e90: 656c 662e 5f65 7874 7261 2061 6e64 2073  elf._extra and s
+00011ea0: 656c 662e 5f65 7874 7261 2e73 7263 5f64  elf._extra.src_d
+00011eb0: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00011ec0: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00011ed0: 5f65 7874 7261 2e73 7263 5f64 6174 612e  _extra.src_data.
+00011ee0: 6765 745f 6261 7463 685f 6469 6d28 290a  get_batch_dim().
+00011ef0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00011f00: 2073 656c 662e 6261 7463 683a 0a20 2020   self.batch:.   
+00011f10: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00011f20: 203d 2073 656c 662e 6261 7463 682e 6469   = self.batch.di
+00011f30: 6d0a 2020 2020 2020 2020 2020 2020 6966  m.            if
+00011f40: 2069 7369 6e73 7461 6e63 6528 7265 732c   isinstance(res,
+00011f50: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+00011f60: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00011f70: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
+00011f80: 2072 6573 2069 7320 6e6f 7420 4e6f 6e65   res is not None
+00011f90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011fa0: 2020 7265 7475 726e 205f 742e 5465 6e73    return _t.Tens
+00011fb0: 6f72 2822 6261 7463 6822 2c20 6469 6d73  or("batch", dims
+00011fc0: 3d28 292c 2064 7479 7065 3d72 662e 6765  =(), dtype=rf.ge
+00011fd0: 745f 6465 6661 756c 745f 6172 7261 795f  t_default_array_
+00011fe0: 696e 6465 785f 6474 7970 6528 292c 2072  index_dtype(), r
+00011ff0: 6177 5f74 656e 736f 723d 7265 7329 0a20  aw_tensor=res). 
+00012000: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00012010: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+00012020: 7472 610a 2020 2020 2020 2020 2020 2020  tra.            
+00012030: 616e 6420 7365 6c66 2e5f 6578 7472 612e  and self._extra.
+00012040: 7372 635f 6461 7461 2069 7320 6e6f 7420  src_data is not 
+00012050: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00012060: 2061 6e64 2073 656c 662e 5f65 7874 7261   and self._extra
+00012070: 2e73 7263 5f61 7869 7320 6973 206e 6f74  .src_axis is not
+00012080: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00012090: 2020 616e 6420 7365 6c66 2e5f 6578 7472    and self._extr
+000120a0: 612e 7372 635f 6461 7461 2e70 6c61 6365  a.src_data.place
+000120b0: 686f 6c64 6572 2069 7320 6e6f 7420 4e6f  holder is not No
+000120c0: 6e65 0a20 2020 2020 2020 2029 3a0a 2020  ne.        ):.  
+000120d0: 2020 2020 2020 2020 2020 7265 7320 3d20            res = 
+000120e0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
+000120f0: 6461 7461 2e67 6574 5f64 696d 2873 656c  data.get_dim(sel
+00012100: 662e 5f65 7874 7261 2e73 7263 5f61 7869  f._extra.src_axi
+00012110: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
+00012120: 6620 6973 696e 7374 616e 6365 2872 6573  f isinstance(res
+00012130: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
+00012140: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00012150: 6573 0a20 2020 2020 2020 2020 2020 2072  es.            r
+00012160: 6574 7572 6e20 5f74 2e54 656e 736f 7228  eturn _t.Tensor(
+00012170: 2262 6174 6368 222c 2064 696d 733d 2829  "batch", dims=()
+00012180: 2c20 6474 7970 653d 7266 2e67 6574 5f64  , dtype=rf.get_d
+00012190: 6566 6175 6c74 5f61 7272 6179 5f69 6e64  efault_array_ind
+000121a0: 6578 5f64 7479 7065 2829 2c20 7261 775f  ex_dtype(), raw_
+000121b0: 7465 6e73 6f72 3d72 6573 290a 2020 2020  tensor=res).    
+000121c0: 2020 2020 7365 6c66 2e63 6f6d 706c 6574      self.complet
+000121d0: 655f 6479 6e5f 7369 7a65 2829 0a20 2020  e_dyn_size().   
+000121e0: 2020 2020 2069 6620 7365 6c66 2e64 796e       if self.dyn
+000121f0: 5f73 697a 655f 6578 7420 616e 6420 7365  _size_ext and se
+00012200: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
+00012210: 706c 6163 6568 6f6c 6465 7220 6973 206e  placeholder is n
+00012220: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00012230: 2020 2020 2069 6620 7365 6c66 2e64 796e       if self.dyn
+00012240: 5f73 697a 655f 6578 742e 6261 7463 685f  _size_ext.batch_
+00012250: 6e64 696d 203e 2030 3a0a 2020 2020 2020  ndim > 0:.      
+00012260: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012270: 2072 662e 7265 6475 6365 5f6d 6178 2873   rf.reduce_max(s
+00012280: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00012290: 2c20 6178 6973 3d73 656c 662e 6479 6e5f  , axis=self.dyn_
+000122a0: 7369 7a65 5f65 7874 2e64 696d 5f74 6167  size_ext.dim_tag
+000122b0: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
+000122c0: 6574 7572 6e20 7365 6c66 2e64 796e 5f73  eturn self.dyn_s
+000122d0: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+000122e0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+000122f0: 2225 733a 206e 6565 6420 706c 6163 6568  "%s: need placeh
+00012300: 6f6c 6465 722c 2073 656c 662e 6469 6d65  older, self.dime
+00012310: 6e73 696f 6e20 6f72 2073 656c 662e 6479  nsion or self.dy
+00012320: 6e5f 7369 7a65 2066 6f72 2064 696d 2076  n_size for dim v
+00012330: 616c 7565 2220 2520 7365 6c66 290a 0a20  alue" % self).. 
+00012340: 2020 2064 6566 2061 7869 735f 7370 6c69     def axis_spli
+00012350: 745f 696e 666f 2873 656c 6629 3a0a 2020  t_info(self):.  
+00012360: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012370: 2020 3a72 6574 7572 6e3a 2061 7869 7320    :return: axis 
+00012380: 7370 6c69 7420 696e 666f 2e20 7365 6520  split info. see 
+00012390: 3a66 756e 633a 6067 6574 5f70 6172 616d  :func:`get_param
+000123a0: 5f61 7865 735f 7370 6c69 745f 696e 666f  _axes_split_info
+000123b0: 6020 616e 6420 7573 6167 6520 2865 2e67  ` and usage (e.g
+000123c0: 2e20 7072 6574 7261 696e 696e 6729 0a20  . pretraining). 
+000123d0: 2020 2020 2020 203a 7274 7970 653a 206c         :rtype: l
+000123e0: 6973 745b 696e 747c 4e6f 6e65 5d0a 2020  ist[int|None].  
+000123f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012400: 2020 7361 6d65 5f62 6173 6520 3d20 7365    same_base = se
+00012410: 6c66 2e67 6574 5f73 616d 655f 6261 7365  lf.get_same_base
+00012420: 2829 0a20 2020 2020 2020 206f 7020 3d20  ().        op = 
+00012430: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
+00012440: 6d5f 6f70 206f 7220 7361 6d65 5f62 6173  m_op or same_bas
+00012450: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
+00012460: 700a 2020 2020 2020 2020 6966 206e 6f74  p.        if not
+00012470: 206f 703a 0a20 2020 2020 2020 2020 2020   op:.           
+00012480: 2072 6574 7572 6e20 5b73 656c 662e 6469   return [self.di
+00012490: 6d65 6e73 696f 6e5d 0a20 2020 2020 2020  mension].       
+000124a0: 2069 6620 6f70 2e6b 696e 6420 3d3d 2022   if op.kind == "
+000124b0: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
+000124c0: 2020 7265 7475 726e 2073 756d 285b 782e    return sum([x.
+000124d0: 6178 6973 5f73 706c 6974 5f69 6e66 6f28  axis_split_info(
+000124e0: 2920 666f 7220 7820 696e 206f 702e 696e  ) for x in op.in
+000124f0: 7075 7473 5d2c 205b 5d29 2020 2320 666c  puts], [])  # fl
+00012500: 6174 7465 6e0a 2020 2020 2020 2020 6966  atten.        if
+00012510: 206f 702e 6b69 6e64 203d 3d20 226d 756c   op.kind == "mul
+00012520: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
+00012530: 6573 203d 205b 315d 0a20 2020 2020 2020  es = [1].       
+00012540: 2020 2020 2066 6f72 2078 2069 6e20 6f70       for x in op
+00012550: 2e69 6e70 7574 733a 0a20 2020 2020 2020  .inputs:.       
+00012560: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
+00012570: 756d 285b 6e20 2a20 782e 6178 6973 5f73  um([n * x.axis_s
+00012580: 706c 6974 5f69 6e66 6f28 2920 6966 206e  plit_info() if n
+00012590: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+000125a0: 6520 4e6f 6e65 2066 6f72 206e 2069 6e20  e None for n in 
+000125b0: 7265 735d 2c20 5b5d 2920 2023 2066 6c61  res], [])  # fla
+000125c0: 7474 656e 0a20 2020 2020 2020 2020 2020  tten.           
+000125d0: 2072 6574 7572 6e20 7265 730a 2020 2020   return res.    
+000125e0: 2020 2020 7265 7475 726e 205b 7365 6c66      return [self
+000125f0: 2e64 696d 656e 7369 6f6e 5d0a 0a20 2020  .dimension]..   
+00012600: 2064 6566 205f 6765 745f 7361 6d65 5f62   def _get_same_b
+00012610: 6173 655f 6578 7472 6128 7365 6c66 2920  ase_extra(self) 
+00012620: 2d3e 204f 7074 696f 6e61 6c5b 5f44 696d  -> Optional[_Dim
+00012630: 4578 7472 615d 3a0a 2020 2020 2020 2020  Extra]:.        
+00012640: 6966 206e 6f74 2073 656c 662e 5f65 7874  if not self._ext
+00012650: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+00012660: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+00012670: 2020 2020 6261 7365 203d 2073 656c 662e      base = self.
+00012680: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
+00012690: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
+000126a0: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
+000126b0: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
+000126c0: 2072 6574 7572 6e20 6261 7365 2e5f 6578   return base._ex
+000126d0: 7472 610a 0a20 2020 2064 6566 205f 6d61  tra..    def _ma
+000126e0: 6b65 5f65 7874 7261 2873 656c 663a 205f  ke_extra(self: _
+000126f0: 642e 4469 6d29 202d 3e20 5f44 696d 4578  d.Dim) -> _DimEx
+00012700: 7472 613a 0a20 2020 2020 2020 2069 6620  tra:.        if 
+00012710: 6e6f 7420 7365 6c66 2e5f 6578 7472 613a  not self._extra:
+00012720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012730: 662e 5f65 7874 7261 203d 205f 4469 6d45  f._extra = _DimE
+00012740: 7874 7261 2864 696d 3d73 656c 6629 0a20  xtra(dim=self). 
+00012750: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00012760: 6c66 2e5f 6578 7472 610a 0a20 2020 2040  lf._extra..    @
+00012770: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00012780: 2076 6f63 6162 2873 656c 6629 3a0a 2020   vocab(self):.  
+00012790: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000127a0: 2020 3a72 7479 7065 3a20 7265 7475 726e    :rtype: return
+000127b0: 6e2e 6461 7461 7365 7473 2e75 7469 6c2e  n.datasets.util.
+000127c0: 766f 6361 6275 6c61 7279 2e56 6f63 6162  vocabulary.Vocab
+000127d0: 756c 6172 797c 4e6f 6e65 0a20 2020 2020  ulary|None.     
+000127e0: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+000127f0: 7874 7261 203d 2073 656c 662e 5f67 6574  xtra = self._get
+00012800: 5f73 616d 655f 6261 7365 5f65 7874 7261  _same_base_extra
+00012810: 2829 0a20 2020 2020 2020 2069 6620 6578  ().        if ex
+00012820: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+00012830: 2072 6574 7572 6e20 6578 7472 612e 766f   return extra.vo
+00012840: 6361 620a 2020 2020 2020 2020 7265 7475  cab.        retu
+00012850: 726e 204e 6f6e 650a 0a20 2020 2040 766f  rn None..    @vo
+00012860: 6361 622e 7365 7474 6572 0a20 2020 2064  cab.setter.    d
+00012870: 6566 2076 6f63 6162 2873 656c 662c 2076  ef vocab(self, v
+00012880: 6f63 6162 293a 0a20 2020 2020 2020 2022  ocab):.        "
+00012890: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+000128a0: 6d20 7265 7475 726e 6e2e 6461 7461 7365  m returnn.datase
+000128b0: 7473 2e75 7469 6c2e 766f 6361 6275 6c61  ts.util.vocabula
+000128c0: 7279 2e56 6f63 6162 756c 6172 797c 4e6f  ry.Vocabulary|No
+000128d0: 6e65 2076 6f63 6162 3a0a 2020 2020 2020  ne vocab:.      
+000128e0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+000128f0: 2076 6f63 6162 2069 7320 7365 6c66 2e76   vocab is self.v
+00012900: 6f63 6162 3a0a 2020 2020 2020 2020 2020  ocab:.          
+00012910: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00012920: 2069 6620 7365 6c66 2e73 616d 655f 6173   if self.same_as
+00012930: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012940: 6c66 2e67 6574 5f73 616d 655f 6261 7365  lf.get_same_base
+00012950: 2829 2e76 6f63 6162 203d 2076 6f63 6162  ().vocab = vocab
+00012960: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00012970: 7572 6e0a 2020 2020 2020 2020 6578 7472  urn.        extr
+00012980: 6120 3d20 7365 6c66 2e5f 6765 745f 7361  a = self._get_sa
+00012990: 6d65 5f62 6173 655f 6578 7472 6128 290a  me_base_extra().
+000129a0: 2020 2020 2020 2020 6966 2065 7874 7261          if extra
+000129b0: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
+000129c0: 7472 612e 766f 6361 6220 3d20 766f 6361  tra.vocab = voca
+000129d0: 620a 0a20 2020 2023 2054 6865 206b 696e  b..    # The kin
+000129e0: 6420 6f66 206f 7065 7261 7469 6f6e 7320  d of operations 
+000129f0: 7765 2068 6176 653a 0a20 2020 2023 2061  we have:.    # a
+00012a00: 202b 2062 3a20 7061 6464 696e 672c 2063   + b: padding, c
+00012a10: 6f6e 6361 740a 2020 2020 2320 6120 2d20  oncat.    # a - 
+00012a20: 623a 2077 696e 646f 7720 7769 7468 2076  b: window with v
+00012a30: 616c 6964 2066 7261 6d65 7320 6f6e 6c79  alid frames only
+00012a40: 0a20 2020 2023 2061 202a 2062 3a20 6d65  .    # a * b: me
+00012a50: 7267 6520 6469 6d73 2c20 7570 7361 6d70  rge dims, upsamp
+00012a60: 6c65 2c20 7472 616e 7370 6f73 6564 2063  le, transposed c
+00012a70: 6f6e 7620 7769 7468 2073 7472 6964 696e  onv with stridin
+00012a80: 670a 2020 2020 2320 6120 2f20 6220 2877  g.    # a / b (w
+00012a90: 6865 6e20 6120 2520 6220 3d3d 2030 293a  hen a % b == 0):
+00012aa0: 2073 706c 6974 2064 696d 732c 2064 6f77   split dims, dow
+00012ab0: 6e73 616d 706c 652c 2063 6f6e 7620 7769  nsample, conv wi
+00012ac0: 7468 2073 7472 6964 696e 670a 2020 2020  th striding.    
+00012ad0: 2320 6365 696c 6469 7628 612c 2062 293a  # ceildiv(a, b):
+00012ae0: 2063 6f6e 7620 7769 7468 2073 7472 6964   conv with strid
+00012af0: 696e 670a 2020 2020 2320 6375 7374 6f6d  ing.    # custom
+00012b00: 3a20 7265 7065 6174 2c20 7265 6d6f 7665  : repeat, remove
+00012b10: 2c20 6d61 736b 2c20 6c6f 6f70 2077 6974  , mask, loop wit
+00012b20: 6820 6479 6e20 656e 640a 2020 2020 2320  h dyn end.    # 
+00012b30: 4e6f 7465 2074 6861 7420 7765 2064 6966  Note that we dif
+00012b40: 6665 7265 6e74 6961 7465 2062 6574 7765  ferentiate betwe
+00012b50: 656e 2074 6865 206f 7264 6572 2c20 692e  en the order, i.
+00012b60: 652e 2061 202b 2062 2021 3d20 6220 2b20  e. a + b != b + 
+00012b70: 612e 0a20 2020 2023 204e 6f74 6520 7468  a..    # Note th
+00012b80: 6174 2077 6520 616c 7761 7973 2068 6176  at we always hav
+00012b90: 6520 7468 6520 6173 7375 6d70 7469 6f6e  e the assumption
+00012ba0: 2074 6861 7420 6120 6469 6d65 6e73 696f   that a dimensio
+00012bb0: 6e20 6973 206e 6f6e 2d6e 6567 6174 6976  n is non-negativ
+00012bc0: 652e 0a20 2020 2023 2054 6869 7320 6173  e..    # This as
+00012bd0: 7375 6d70 7469 6f6e 2069 7320 6e65 6365  sumption is nece
+00012be0: 7373 6172 7920 666f 7220 736f 6d65 2073  ssary for some s
+00012bf0: 696d 706c 6966 6963 6174 696f 6e73 2e0a  implifications..
+00012c00: 2020 2020 2320 6874 7470 733a 2f2f 6769      # https://gi
+00012c10: 7468 7562 2e63 6f6d 2f72 7774 682d 6936  thub.com/rwth-i6
+00012c20: 2f72 6574 7572 6e6e 2f70 756c 6c2f 3835  /returnn/pull/85
+00012c30: 330a 0a20 2020 2064 6566 205f 5f61 6464  3..    def __add
+00012c40: 5f5f 2873 656c 663a 2044 696d 2c20 6f74  __(self: Dim, ot
+00012c50: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
+00012c60: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00012c70: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
+00012c80: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00012c90: 2073 656c 6620 2b20 6f74 6865 722e 206e   self + other. n
+00012ca0: 6f74 6520 7468 6174 2074 6869 7320 6973  ote that this is
+00012cb0: 206e 6f74 2063 6f6d 6d75 7461 7469 7665   not commutative
+00012cc0: 2c20 692e 652e 2064 6966 6665 7265 6e74  , i.e. different
+00012cd0: 2066 726f 6d20 6f74 6865 7220 2b20 7365   from other + se
+00012ce0: 6c66 2e0a 2020 2020 2020 2020 3a72 7479  lf..        :rty
+00012cf0: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
+00012d00: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
+00012d10: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
+00012d20: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
+00012d30: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+00012d40: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
+00012d50: 6572 2c20 6b69 6e64 3d22 6164 6422 2c20  er, kind="add", 
+00012d60: 7269 6768 743d 5472 7565 290a 2020 2020  right=True).    
+00012d70: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
+00012d80: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
+00012d90: 6620 5f5f 7261 6464 5f5f 2873 656c 663a  f __radd__(self:
+00012da0: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
+00012db0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012dc0: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
+00012dd0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00012de0: 3a72 6574 7572 6e3a 206f 7468 6572 202b  :return: other +
+00012df0: 2073 656c 660a 2020 2020 2020 2020 3a72   self.        :r
+00012e00: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00012e10: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
+00012e20: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
+00012e30: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
+00012e40: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
+00012e50: 7874 656e 645f 6164 645f 7375 625f 286f  xtend_add_sub_(o
+00012e60: 7468 6572 2c20 6b69 6e64 3d22 6164 6422  ther, kind="add"
+00012e70: 2c20 7269 6768 743d 4661 6c73 6529 0a20  , right=False). 
+00012e80: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00012e90: 726d 2e61 735f 6469 6d28 290a 0a20 2020  rm.as_dim()..   
+00012ea0: 2064 6566 205f 5f73 7562 5f5f 2873 656c   def __sub__(sel
+00012eb0: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+00012ec0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00012ed0: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00012ee0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+00012ef0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00012f00: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00012f10: 7572 6e20 7365 6c66 2e73 7562 5f72 6967  urn self.sub_rig
+00012f20: 6874 286f 7468 6572 290a 0a20 2020 2064  ht(other)..    d
+00012f30: 6566 2073 7562 5f72 6967 6874 2873 656c  ef sub_right(sel
+00012f40: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
+00012f50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012f60: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
+00012f70: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
+00012f80: 2020 3a72 6574 7572 6e3a 2073 656c 6620    :return: self 
+00012f90: 2d20 6f74 6865 720a 2020 2020 2020 2020  - other.        
+00012fa0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
+00012fb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012fc0: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
+00012fd0: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
+00012fe0: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
+00012ff0: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
+00013000: 286f 7468 6572 2c20 6b69 6e64 3d22 7375  (other, kind="su
+00013010: 6222 2c20 7269 6768 743d 5472 7565 290a  b", right=True).
+00013020: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00013030: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
+00013040: 2020 6465 6620 7375 625f 6c65 6674 2873    def sub_left(s
+00013050: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
+00013060: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013070: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00013080: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+00013090: 2020 2020 3a72 6574 7572 6e3a 2028 2d6f      :return: (-o
+000130a0: 7468 6572 2920 2b20 7365 6c66 0a20 2020  ther) + self.   
+000130b0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+000130c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000130d0: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
+000130e0: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
+000130f0: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
+00013100: 2074 6572 6d2e 6578 7465 6e64 5f61 6464   term.extend_add
+00013110: 5f73 7562 5f28 6f74 6865 722c 206b 696e  _sub_(other, kin
+00013120: 643d 2273 7562 222c 2072 6967 6874 3d46  d="sub", right=F
+00013130: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
+00013140: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
+00013150: 2829 0a0a 2020 2020 6465 6620 5f5f 6d75  ()..    def __mu
+00013160: 6c5f 5f28 7365 6c66 3a20 4469 6d2c 206f  l__(self: Dim, o
+00013170: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00013180: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00013190: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+000131a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000131b0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+000131c0: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
+000131d0: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
+000131e0: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
+000131f0: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
+00013200: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
+00013210: 206b 696e 643d 226d 756c 222c 2072 6967   kind="mul", rig
+00013220: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
+00013230: 2072 6574 7572 6e20 7465 726d 2e61 735f   return term.as_
+00013240: 6469 6d28 290a 0a20 2020 2064 6566 205f  dim()..    def _
+00013250: 5f72 6d75 6c5f 5f28 7365 6c66 3a20 4469  _rmul__(self: Di
+00013260: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
+00013270: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00013280: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00013290: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+000132a0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+000132b0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+000132c0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+000132d0: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+000132e0: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+000132f0: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
+00013300: 6865 722c 206b 696e 643d 226d 756c 222c  her, kind="mul",
+00013310: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
+00013320: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
+00013330: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
+00013340: 6465 6620 5f5f 666c 6f6f 7264 6976 5f5f  def __floordiv__
+00013350: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
+00013360: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
+00013370: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+00013380: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
+00013390: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+000133a0: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
+000133b0: 2020 2020 2020 7465 726d 203d 205f 4f70        term = _Op
+000133c0: 4c69 6e65 6172 5465 726d 2e66 726f 6d5f  LinearTerm.from_
+000133d0: 6469 6d28 7365 6c66 290a 2020 2020 2020  dim(self).      
+000133e0: 2020 7465 726d 2e65 7874 656e 645f 6d75    term.extend_mu
+000133f0: 6c5f 6469 765f 286f 7468 6572 2c20 6b69  l_div_(other, ki
+00013400: 6e64 3d22 666c 6f6f 7264 6976 222c 2072  nd="floordiv", r
+00013410: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00013420: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00013430: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00013440: 205f 5f74 7275 6564 6976 5f5f 2873 656c   __truediv__(sel
+00013450: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+00013460: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00013470: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00013480: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+00013490: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+000134a0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+000134b0: 7572 6e20 7365 6c66 2e64 6976 5f72 6967  urn self.div_rig
+000134c0: 6874 286f 7468 6572 290a 0a20 2020 2064  ht(other)..    d
+000134d0: 6566 2064 6976 5f6c 6566 7428 7365 6c66  ef div_left(self
+000134e0: 3a20 4469 6d2c 206f 7468 6572 293a 0a20  : Dim, other):. 
+000134f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013500: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00013510: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00013520: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00013530: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013540: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
+00013550: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
+00013560: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
+00013570: 6d2e 6578 7465 6e64 5f6d 756c 5f64 6976  m.extend_mul_div
+00013580: 5f28 6f74 6865 722c 206b 696e 643d 2274  _(other, kind="t
+00013590: 7275 6564 6976 222c 2072 6967 6874 3d46  ruediv", right=F
+000135a0: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
+000135b0: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
+000135c0: 2829 0a0a 2020 2020 6465 6620 6469 765f  ()..    def div_
+000135d0: 7269 6768 7428 7365 6c66 3a20 4469 6d2c  right(self: Dim,
+000135e0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+000135f0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+00013600: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
+00013610: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
+00013620: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
+00013630: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
+00013640: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
+00013650: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
+00013660: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
+00013670: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
+00013680: 722c 206b 696e 643d 2274 7275 6564 6976  r, kind="truediv
+00013690: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
+000136a0: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+000136b0: 726d 2e61 735f 6469 6d28 290a 0a20 2020  rm.as_dim()..   
+000136c0: 2064 6566 2063 6569 6c64 6976 5f6c 6566   def ceildiv_lef
+000136d0: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
+000136e0: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
+000136f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00013700: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
+00013710: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00013720: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+00013730: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
+00013740: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
+00013750: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
+00013760: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
+00013770: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
+00013780: 696e 643d 2263 6569 6c64 6976 222c 2072  ind="ceildiv", r
+00013790: 6967 6874 3d46 616c 7365 290a 2020 2020  ight=False).    
+000137a0: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
+000137b0: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
+000137c0: 6620 6365 696c 6469 765f 7269 6768 7428  f ceildiv_right(
+000137d0: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+000137e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000137f0: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00013800: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00013810: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00013820: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013830: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
+00013840: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
+00013850: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
+00013860: 2074 6572 6d2e 6578 7465 6e64 5f6d 756c   term.extend_mul
+00013870: 5f64 6976 5f28 6f74 6865 722c 206b 696e  _div_(other, kin
+00013880: 643d 2263 6569 6c64 6976 222c 2072 6967  d="ceildiv", rig
+00013890: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
+000138a0: 2072 6574 7572 6e20 7465 726d 2e61 735f   return term.as_
+000138b0: 6469 6d28 290a 0a20 2020 2064 6566 205f  dim()..    def _
+000138c0: 5f6e 6567 5f5f 2873 656c 6629 3a0a 2020  _neg__(self):.  
+000138d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000138e0: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+000138f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013900: 2020 7265 7475 726e 202d 3120 2a20 7365    return -1 * se
+00013910: 6c66 0a0a 2020 2020 6465 6620 6973 5f63  lf..    def is_c
+00013920: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+00013930: 696d 2873 656c 6629 202d 3e20 626f 6f6c  im(self) -> bool
+00013940: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013950: 2020 2020 2020 3a72 6574 7572 6e3a 2064        :return: d
+00013960: 6572 6976 6564 206f 7020 6f66 2074 7970  erived op of typ
+00013970: 6520 636f 6e73 7461 6e74 0a20 2020 2020  e constant.     
+00013980: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00013990: 6574 7572 6e20 7365 6c66 2e64 6572 6976  eturn self.deriv
+000139a0: 6564 5f66 726f 6d5f 6f70 2061 6e64 2073  ed_from_op and s
+000139b0: 656c 662e 6465 7269 7665 645f 6672 6f6d  elf.derived_from
+000139c0: 5f6f 702e 6b69 6e64 203d 3d20 2263 6f6e  _op.kind == "con
+000139d0: 7374 616e 7422 0a0a 0a64 6566 205f 6d61  stant"...def _ma
+000139e0: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
+000139f0: 6963 5f64 696d 2876 616c 7565 2c20 6b69  ic_dim(value, ki
+00013a00: 6e64 3d4e 6f6e 6529 3a0a 2020 2020 2222  nd=None):.    ""
+00013a10: 220a 2020 2020 3a70 6172 616d 2069 6e74  ".    :param int
+00013a20: 2076 616c 7565 3a0a 2020 2020 3a70 6172   value:.    :par
+00013a30: 616d 2045 6e74 6974 797c 4e6f 6e65 206b  am Entity|None k
+00013a40: 696e 643a 0a20 2020 203a 7274 7970 653a  ind:.    :rtype:
+00013a50: 2044 696d 0a20 2020 2022 2222 0a20 2020   Dim.    """.   
+00013a60: 2072 6574 7572 6e20 5f64 2e44 696d 280a   return _d.Dim(.
+00013a70: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
+00013a80: 6e3d 7661 6c75 652c 0a20 2020 2020 2020  n=value,.       
+00013a90: 206b 696e 643d 6b69 6e64 206f 7220 4469   kind=kind or Di
+00013aa0: 6d54 7970 6573 2e55 6e73 7065 6369 6669  mTypes.Unspecifi
+00013ab0: 6564 2c0a 2020 2020 2020 2020 6465 7363  ed,.        desc
+00013ac0: 7269 7074 696f 6e3d 2275 6e6e 616d 6564  ription="unnamed
+00013ad0: 5f25 7364 696d 5f25 6922 2025 2028 6b69  _%sdim_%i" % (ki
+00013ae0: 6e64 2e6e 616d 6520 2b20 225f 2220 6966  nd.name + "_" if
+00013af0: 206b 696e 6420 656c 7365 2022 222c 2076   kind else "", v
+00013b00: 616c 7565 292c 0a20 2020 2020 2020 2064  alue),.        d
+00013b10: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
+00013b20: 7028 6b69 6e64 3d22 636f 6e73 7461 6e74  p(kind="constant
+00013b30: 222c 2069 6e70 7574 733d 5b5d 2c20 6174  ", inputs=[], at
+00013b40: 7472 6962 733d 7b22 7661 6c75 6522 3a20  tribs={"value": 
+00013b50: 7661 6c75 657d 292c 0a20 2020 2020 2020  value}),.       
+00013b60: 2061 7574 6f5f 6765 6e65 7261 7465 643d   auto_generated=
+00013b70: 5472 7565 2c0a 2020 2020 290a 0a0a 636c  True,.    )...cl
+00013b80: 6173 7320 4f70 3a0a 2020 2020 2222 220a  ass Op:.    """.
+00013b90: 2020 2020 4f70 206f 6e20 3a63 6c61 7373      Op on :class
+00013ba0: 3a60 4469 6d60 2077 6869 6368 2072 6573  :`Dim` which res
+00013bb0: 756c 7473 2069 6e20 6120 6465 7269 7665  ults in a derive
+00013bc0: 6420 3a63 6c61 7373 3a60 4469 6d60 2e0a  d :class:`Dim`..
+00013bd0: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+00013be0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00013bf0: 6b69 6e64 2c20 696e 7075 7473 2c20 6174  kind, inputs, at
+00013c00: 7472 6962 733d 4e6f 6e65 293a 0a20 2020  tribs=None):.   
+00013c10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013c20: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
+00013c30: 3a20 2261 6464 222c 2022 7375 6222 2c20  : "add", "sub", 
+00013c40: 226d 756c 222c 2022 6365 696c 6469 7622  "mul", "ceildiv"
+00013c50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00013c60: 6c69 7374 5b44 696d 5d20 696e 7075 7473  list[Dim] inputs
+00013c70: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00013c80: 2064 6963 745b 7374 725d 7c4e 6f6e 6520   dict[str]|None 
+00013c90: 6174 7472 6962 733a 0a20 2020 2020 2020  attribs:.       
+00013ca0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00013cb0: 662e 6b69 6e64 203d 206b 696e 640a 2020  f.kind = kind.  
+00013cc0: 2020 2020 2020 7365 6c66 2e69 6e70 7574        self.input
+00013cd0: 7320 3d20 696e 7075 7473 0a20 2020 2020  s = inputs.     
+00013ce0: 2020 2073 656c 662e 6f75 7470 7574 203d     self.output =
+00013cf0: 204e 6f6e 6520 2023 2074 7970 653a 204f   None  # type: O
+00013d00: 7074 696f 6e61 6c5b 5f64 2e44 696d 5d0a  ptional[_d.Dim].
+00013d10: 2020 2020 2020 2020 7365 6c66 2e61 7474          self.att
+00013d20: 7269 6273 203d 2061 7474 7269 6273 0a0a  ribs = attribs..
+00013d30: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00013d40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00013d50: 6174 7472 6962 7320 3d20 2822 2025 7222  attribs = (" %r"
+00013d60: 2025 2073 656c 662e 6174 7472 6962 7329   % self.attribs)
+00013d70: 2069 6620 7365 6c66 2e61 7474 7269 6273   if self.attribs
+00013d80: 2065 6c73 6520 2222 0a20 2020 2020 2020   else "".       
+00013d90: 2072 6574 7572 6e20 223c 4469 6d2e 4f70   return "<Dim.Op
+00013da0: 2025 7220 2573 2573 3e22 2025 2028 7365   %r %s%s>" % (se
+00013db0: 6c66 2e6b 696e 642c 2073 656c 662e 696e  lf.kind, self.in
+00013dc0: 7075 7473 2c20 6174 7472 6962 7329 0a0a  puts, attribs)..
+00013dd0: 2020 2020 6465 6620 5f76 616c 7565 2873      def _value(s
+00013de0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00013df0: 7475 726e 2073 656c 662e 6b69 6e64 2c20  turn self.kind, 
+00013e00: 7475 706c 6528 7365 6c66 2e69 6e70 7574  tuple(self.input
+00013e10: 7329 2c20 6672 6f7a 656e 7365 7428 7365  s), frozenset(se
+00013e20: 6c66 2e61 7474 7269 6273 2e69 7465 6d73  lf.attribs.items
+00013e30: 2829 2920 6966 2073 656c 662e 6174 7472  ()) if self.attr
+00013e40: 6962 7320 656c 7365 204e 6f6e 650a 0a20  ibs else None.. 
+00013e50: 2020 2064 6566 205f 5f68 6173 685f 5f28     def __hash__(
+00013e60: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00013e70: 6574 7572 6e20 6861 7368 2873 656c 662e  eturn hash(self.
+00013e80: 5f76 616c 7565 2829 290a 0a20 2020 2064  _value())..    d
+00013e90: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
+00013ea0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00013eb0: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00013ec0: 6865 722c 204f 7029 3a0a 2020 2020 2020  her, Op):.      
+00013ed0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00013ee0: 662e 5f76 616c 7565 2829 203d 3d20 6f74  f._value() == ot
+00013ef0: 6865 722e 5f76 616c 7565 2829 0a20 2020  her._value().   
+00013f00: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00013f10: 650a 0a20 2020 2064 6566 205f 5f6e 655f  e..    def __ne_
+00013f20: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+00013f30: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00013f40: 6f74 2073 656c 662e 5f5f 6571 5f5f 286f  ot self.__eq__(o
+00013f50: 7468 6572 290a 0a0a 6465 6620 5f67 6574  ther)...def _get
+00013f60: 5f64 6573 6372 6970 7469 6f6e 2864 696d  _description(dim
+00013f70: 2c20 6272 6163 6b65 7473 3d54 7275 6529  , brackets=True)
+00013f80: 3a0a 2020 2020 2222 220a 2020 2020 3a70  :.    """.    :p
+00013f90: 6172 616d 2044 696d 2064 696d 3a0a 2020  aram Dim dim:.  
+00013fa0: 2020 3a70 6172 616d 2062 6f6f 6c20 6272    :param bool br
+00013fb0: 6163 6b65 7473 3a20 6164 6420 6272 6163  ackets: add brac
+00013fc0: 6b65 7473 2077 6865 6e20 6e65 6365 7373  kets when necess
+00013fd0: 6172 790a 2020 2020 3a72 7479 7065 3a20  ary.    :rtype: 
+00013fe0: 7374 720a 2020 2020 2222 220a 2020 2020  str.    """.    
+00013ff0: 6966 2064 696d 2e64 6573 6372 6970 7469  if dim.descripti
+00014000: 6f6e 2061 6e64 2064 696d 2e64 6573 6372  on and dim.descr
+00014010: 6970 7469 6f6e 2e73 7461 7274 7377 6974  iption.startswit
+00014020: 6828 2275 6e6e 616d 6564 5f22 2920 616e  h("unnamed_") an
+00014030: 6420 6469 6d2e 6469 6d65 6e73 696f 6e20  d dim.dimension 
+00014040: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00014050: 2020 2020 2072 6574 7572 6e20 7374 7228       return str(
+00014060: 6469 6d2e 6469 6d65 6e73 696f 6e29 0a20  dim.dimension). 
+00014070: 2020 2069 6620 6469 6d2e 6465 7363 7269     if dim.descri
+00014080: 7074 696f 6e3a 0a20 2020 2020 2020 2069  ption:.        i
+00014090: 6620 6272 6163 6b65 7473 3a0a 2020 2020  f brackets:.    
+000140a0: 2020 2020 2020 2020 696d 706f 7274 2072          import r
+000140b0: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
+000140c0: 6620 7265 2e73 6561 7263 6828 225b 2b5c  f re.search("[+\
+000140d0: 5c2d 2f20 5d22 2c20 6469 6d2e 6465 7363  \-/ ]", dim.desc
+000140e0: 7269 7074 696f 6e29 3a0a 2020 2020 2020  ription):.      
+000140f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014100: 2022 2825 7329 2220 2520 6469 6d2e 6465   "(%s)" % dim.de
+00014110: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
+00014120: 2020 7265 7475 726e 2064 696d 2e64 6573    return dim.des
+00014130: 6372 6970 7469 6f6e 0a20 2020 2072 6574  cription.    ret
+00014140: 7572 6e20 2275 6e6e 616d 6564 5f25 735f  urn "unnamed_%s_
+00014150: 6469 6d25 7322 2025 2028 6469 6d2e 6b69  dim%s" % (dim.ki
+00014160: 6e64 2c20 6469 6d2e 6469 6d65 6e73 696f  nd, dim.dimensio
+00014170: 6e20 6966 2064 696d 2e64 696d 656e 7369  n if dim.dimensi
+00014180: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2065  on is not None e
+00014190: 6c73 6520 223f 2229 0a0a 0a63 6c61 7373  lse "?")...class
+000141a0: 205f 4f70 4d75 6c74 5465 726d 3a0a 2020   _OpMultTerm:.  
+000141b0: 2020 2222 220a 2020 2020 7265 7072 6573    """.    repres
+000141c0: 656e 7473 2073 7468 206c 696b 6520 6120  ents sth like a 
+000141d0: 2a20 6220 2a20 630a 2020 2020 2222 220a  * b * c.    """.
+000141e0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+000141f0: 640a 2020 2020 6465 6620 6672 6f6d 5f64  d.    def from_d
+00014200: 696d 2863 6c73 2c20 6469 6d3a 205f 642e  im(cls, dim: _d.
+00014210: 4469 6d29 202d 3e20 5f4f 704d 756c 7454  Dim) -> _OpMultT
+00014220: 6572 6d3a 0a20 2020 2020 2020 2022 2222  erm:.        """
+00014230: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00014240: 6469 6d3a 0a20 2020 2020 2020 203a 7265  dim:.        :re
+00014250: 7475 726e 3a20 6f70 206d 756c 7420 7465  turn: op mult te
+00014260: 726d 0a20 2020 2020 2020 2022 2222 0a20  rm.        """. 
+00014270: 2020 2020 2020 2064 696d 203d 2064 696d         dim = dim
+00014280: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
+00014290: 0a20 2020 2020 2020 2069 6620 6469 6d2e  .        if dim.
+000142a0: 6469 6d65 6e73 696f 6e20 3d3d 2031 2061  dimension == 1 a
+000142b0: 6e64 2064 696d 2e69 735f 636f 6e73 7461  nd dim.is_consta
+000142c0: 6e74 5f73 7461 7469 635f 6469 6d28 293a  nt_static_dim():
+000142d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000142e0: 7572 6e20 636c 732e 6f6e 6528 290a 2020  urn cls.one().  
+000142f0: 2020 2020 2020 6966 2064 696d 2e64 6572        if dim.der
+00014300: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
+00014310: 2064 696d 2e64 6572 6976 6564 5f66 726f   dim.derived_fro
+00014320: 6d5f 6f70 2e6b 696e 6420 3d3d 2022 6d75  m_op.kind == "mu
+00014330: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+00014340: 7265 7475 726e 2063 6c73 286c 6973 7428  return cls(list(
+00014350: 6469 6d2e 6465 7269 7665 645f 6672 6f6d  dim.derived_from
+00014360: 5f6f 702e 696e 7075 7473 2929 0a20 2020  _op.inputs)).   
+00014370: 2020 2020 2072 6574 7572 6e20 636c 7328       return cls(
+00014380: 5b64 696d 5d29 0a0a 2020 2020 4063 6c61  [dim])..    @cla
+00014390: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+000143a0: 2066 726f 6d5f 6469 6d5f 6661 6374 6f72   from_dim_factor
+000143b0: 7328 636c 732c 2064 696d 7329 3a0a 2020  s(cls, dims):.  
+000143c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000143d0: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
+000143e0: 6d5d 2064 696d 733a 0a20 2020 2020 2020  m] dims:.       
+000143f0: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
+00014400: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
+00014410: 2022 2222 0a20 2020 2020 2020 2072 6573   """.        res
+00014420: 203d 2063 6c73 2e6f 6e65 2829 0a20 2020   = cls.one().   
+00014430: 2020 2020 2066 6f72 2064 2069 6e20 6469       for d in di
+00014440: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00014450: 7265 732e 6578 7465 6e64 5f6d 756c 5f64  res.extend_mul_d
+00014460: 6976 5f28 642c 206b 696e 643d 226d 756c  iv_(d, kind="mul
+00014470: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
+00014480: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00014490: 730a 0a20 2020 2040 636c 6173 736d 6574  s..    @classmet
+000144a0: 686f 640a 2020 2020 6465 6620 6f6e 6528  hod.    def one(
+000144b0: 636c 7329 3a0a 2020 2020 2020 2020 2222  cls):.        ""
+000144c0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+000144d0: 3a20 4469 6d2e 5f4f 704d 756c 7454 6572  : Dim._OpMultTer
+000144e0: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
+000144f0: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
+00014500: 285b 5d29 0a0a 2020 2020 6465 6620 5f5f  ([])..    def __
+00014510: 696e 6974 5f5f 2873 656c 662c 2074 6572  init__(self, ter
+00014520: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+00014530: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00014540: 6c69 7374 5b44 696d 5d20 7465 726d 733a  list[Dim] terms:
+00014550: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014560: 2020 2020 2073 656c 662e 7465 726d 7320       self.terms 
+00014570: 3d20 7465 726d 730a 0a20 2020 2064 6566  = terms..    def
+00014580: 205f 5f68 6173 685f 5f28 7365 6c66 293a   __hash__(self):
+00014590: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000145a0: 6861 7368 2874 7570 6c65 2873 656c 662e  hash(tuple(self.
+000145b0: 7465 726d 7329 290a 0a20 2020 2064 6566  terms))..    def
+000145c0: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
+000145d0: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
+000145e0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+000145f0: 2044 696d 7c44 696d 2e5f 4f70 4d75 6c74   Dim|Dim._OpMult
+00014600: 5465 726d 206f 7468 6572 3a0a 2020 2020  Term other:.    
+00014610: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014620: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00014630: 6865 722c 205f 4f70 4d75 6c74 5465 726d  her, _OpMultTerm
+00014640: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00014650: 6574 7572 6e20 7365 6c66 2e74 6572 6d73  eturn self.terms
+00014660: 203d 3d20 6f74 6865 722e 7465 726d 730a   == other.terms.
+00014670: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00014680: 616c 7365 0a0a 2020 2020 6465 6620 5f5f  alse..    def __
+00014690: 6e65 5f5f 2873 656c 662c 206f 7468 6572  ne__(self, other
+000146a0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000146b0: 6e20 6e6f 7420 7365 6c66 2e5f 5f65 715f  n not self.__eq_
+000146c0: 5f28 6f74 6865 7229 0a0a 2020 2020 6465  _(other)..    de
+000146d0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
+000146e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000146f0: 2022 4469 6d2e 5f4f 704d 756c 7454 6572   "Dim._OpMultTer
+00014700: 6d28 2572 2922 2025 2028 7365 6c66 2e74  m(%r)" % (self.t
+00014710: 6572 6d73 2c29 0a0a 2020 2020 4070 726f  erms,)..    @pro
+00014720: 7065 7274 790a 2020 2020 6465 6620 6469  perty.    def di
+00014730: 6d65 6e73 696f 6e28 7365 6c66 293a 0a20  mension(self):. 
+00014740: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014750: 2020 203a 7274 7970 653a 2069 6e74 7c4e     :rtype: int|N
+00014760: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+00014770: 2020 2020 2020 2020 6469 6d20 3d20 310a          dim = 1.
+00014780: 2020 2020 2020 2020 666f 7220 7061 7274          for part
+00014790: 2069 6e20 7365 6c66 2e74 6572 6d73 3a0a   in self.terms:.
+000147a0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000147b0: 6172 742e 6469 6d65 6e73 696f 6e20 6973  art.dimension is
+000147c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000147d0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000147e0: 6e65 0a20 2020 2020 2020 2020 2020 2064  ne.            d
+000147f0: 696d 202a 3d20 7061 7274 2e64 696d 656e  im *= part.dimen
+00014800: 7369 6f6e 0a20 2020 2020 2020 2072 6574  sion.        ret
+00014810: 7572 6e20 6469 6d0a 0a20 2020 2064 6566  urn dim..    def
+00014820: 2062 6173 655f 7465 726d 2873 656c 6629   base_term(self)
+00014830: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00014840: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+00014850: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
+00014860: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+00014870: 662e 7465 726d 730a 2020 2020 2020 2020  f.terms.        
+00014880: 7265 7475 726e 2073 656c 662e 7465 726d  return self.term
+00014890: 735b 2d31 5d0a 0a20 2020 2064 6566 2069  s[-1]..    def i
+000148a0: 735f 6f6e 6528 7365 6c66 293a 0a20 2020  s_one(self):.   
+000148b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000148c0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+000148d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000148e0: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
+000148f0: 662e 7465 726d 730a 0a20 2020 2064 6566  f.terms..    def
+00014900: 2069 735f 636f 6e73 7461 6e74 5f73 7461   is_constant_sta
+00014910: 7469 635f 6469 6d28 7365 6c66 293a 0a20  tic_dim(self):. 
+00014920: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014930: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+00014940: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014950: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00014960: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00014970: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00014980: 2020 2020 2020 2072 6574 7572 6e20 616c         return al
+00014990: 6c28 7465 726d 2e69 735f 636f 6e73 7461  l(term.is_consta
+000149a0: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+000149b0: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
+000149c0: 2e74 6572 6d73 290a 0a20 2020 2064 6566  .terms)..    def
+000149d0: 2063 6f70 7928 7365 6c66 293a 0a20 2020   copy(self):.   
+000149e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000149f0: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
+00014a00: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
+00014a10: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00014a20: 7572 6e20 5f4f 704d 756c 7454 6572 6d28  urn _OpMultTerm(
+00014a30: 6c69 7374 2873 656c 662e 7465 726d 7329  list(self.terms)
+00014a40: 290a 0a20 2020 2064 6566 206e 6567 6174  )..    def negat
+00014a50: 6976 6528 7365 6c66 293a 0a20 2020 2020  ive(self):.     
+00014a60: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00014a70: 7274 7970 653a 2044 696d 2e5f 4f70 4d75  rtype: Dim._OpMu
+00014a80: 6c74 5465 726d 0a20 2020 2020 2020 2022  ltTerm.        "
+00014a90: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00014aa0: 6c66 2e74 6572 6d73 2061 6e64 2073 656c  lf.terms and sel
+00014ab0: 662e 7465 726d 735b 305d 2e69 735f 636f  f.terms[0].is_co
+00014ac0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00014ad0: 6d28 2920 616e 6420 7365 6c66 2e74 6572  m() and self.ter
+00014ae0: 6d73 5b30 5d2e 6469 6d65 6e73 696f 6e20  ms[0].dimension 
+00014af0: 3d3d 202d 313a 0a20 2020 2020 2020 2020  == -1:.         
+00014b00: 2020 2072 6574 7572 6e20 5f4f 704d 756c     return _OpMul
+00014b10: 7454 6572 6d28 7365 6c66 2e74 6572 6d73  tTerm(self.terms
+00014b20: 5b31 3a5d 290a 2020 2020 2020 2020 7265  [1:]).        re
+00014b30: 7320 3d20 7365 6c66 2e63 6f70 7928 290a  s = self.copy().
+00014b40: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
+00014b50: 6e64 5f6d 756c 5f64 6976 5f28 5f6d 616b  nd_mul_div_(_mak
+00014b60: 655f 636f 6e73 7461 6e74 5f73 7461 7469  e_constant_stati
+00014b70: 635f 6469 6d28 2d31 292c 206b 696e 643d  c_dim(-1), kind=
+00014b80: 226d 756c 222c 2072 6967 6874 3d46 616c  "mul", right=Fal
+00014b90: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
+00014ba0: 726e 2072 6573 0a0a 2020 2020 6465 6620  rn res..    def 
+00014bb0: 6469 7669 7369 626c 6528 7365 6c66 2c20  divisible(self, 
+00014bc0: 6f74 6865 722c 2072 6967 6874 293a 0a20  other, right):. 
+00014bd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014be0: 2020 203a 7061 7261 6d20 4469 6d20 6f74     :param Dim ot
+00014bf0: 6865 723a 0a20 2020 2020 2020 203a 7061  her:.        :pa
+00014c00: 7261 6d20 626f 6f6c 2072 6967 6874 3a0a  ram bool right:.
+00014c10: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00014c20: 2077 6865 7468 6572 2077 6520 6361 6e20   whether we can 
+00014c30: 6469 7669 6465 206f 7468 6572 2c20 7769  divide other, wi
+00014c40: 7468 6f75 7420 7265 6d61 696e 6465 720a  thout remainder.
+00014c50: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00014c60: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
+00014c70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00014c80: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00014c90: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00014ca0: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
+00014cb0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00014cc0: 6f6d 5f6f 7020 616e 6420 6f74 6865 722e  om_op and other.
+00014cd0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00014ce0: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
+00014cf0: 2020 2020 2020 2020 2020 2074 6d70 203d             tmp =
+00014d00: 2073 656c 662e 636f 7079 2829 0a20 2020   self.copy().   
+00014d10: 2020 2020 2020 2020 2066 6f72 2074 6572           for ter
+00014d20: 6d20 696e 206f 7468 6572 2e64 6572 6976  m in other.deriv
+00014d30: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00014d40: 7320 6966 2072 6967 6874 2065 6c73 6520  s if right else 
+00014d50: 7265 7665 7273 6564 286f 7468 6572 2e64  reversed(other.d
+00014d60: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
+00014d70: 6e70 7574 7329 3a0a 2020 2020 2020 2020  nputs):.        
+00014d80: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
+00014d90: 6d70 2e64 6976 6973 6962 6c65 2874 6572  mp.divisible(ter
+00014da0: 6d2c 2072 6967 6874 3d72 6967 6874 293a  m, right=right):
+00014db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014dc0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00014dd0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00014de0: 2020 746d 702e 6578 7465 6e64 5f6d 756c    tmp.extend_mul
+00014df0: 5f64 6976 5f28 7465 726d 2c20 6b69 6e64  _div_(term, kind
+00014e00: 3d22 7472 7565 6469 7622 2c20 7269 6768  ="truediv", righ
+00014e10: 743d 7269 6768 7429 0a20 2020 2020 2020  t=right).       
+00014e20: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00014e30: 0a20 2020 2020 2020 206d 6f73 745f 7265  .        most_re
+00014e40: 6365 6e74 5f74 6572 6d20 3d20 7365 6c66  cent_term = self
+00014e50: 2e74 6572 6d73 5b2d 3120 6966 2072 6967  .terms[-1 if rig
+00014e60: 6874 2065 6c73 6520 305d 0a20 2020 2020  ht else 0].     
+00014e70: 2020 2069 6620 6f74 6865 7220 3d3d 206d     if other == m
+00014e80: 6f73 745f 7265 6365 6e74 5f74 6572 6d3a  ost_recent_term:
+00014e90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014ea0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00014eb0: 2069 6620 6d6f 7374 5f72 6563 656e 745f   if most_recent_
+00014ec0: 7465 726d 2e64 696d 656e 7369 6f6e 2069  term.dimension i
+00014ed0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206f  s not None and o
+00014ee0: 7468 6572 2e64 696d 656e 7369 6f6e 2069  ther.dimension i
+00014ef0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00014f00: 2020 2020 2020 2020 6966 206d 6f73 745f          if most_
+00014f10: 7265 6365 6e74 5f74 6572 6d2e 6469 6d65  recent_term.dime
+00014f20: 6e73 696f 6e20 2520 6f74 6865 722e 6469  nsion % other.di
+00014f30: 6d65 6e73 696f 6e20 3d3d 2030 3a0a 2020  mension == 0:.  
+00014f40: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00014f50: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00014f60: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00014f70: 2020 2020 6465 6620 6361 6e5f 7369 6d70      def can_simp
+00014f80: 6c69 6679 2873 656c 662c 206f 7468 6572  lify(self, other
+00014f90: 2c20 6b69 6e64 2c20 7269 6768 7429 3a0a  , kind, right):.
+00014fa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014fb0: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
+00014fc0: 7468 6572 3a0a 2020 2020 2020 2020 3a70  ther:.        :p
+00014fd0: 6172 616d 2073 7472 206b 696e 643a 0a20  aram str kind:. 
+00014fe0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+00014ff0: 6f6c 2072 6967 6874 3a0a 2020 2020 2020  ol right:.      
+00015000: 2020 3a72 6574 7572 6e3a 2077 6865 7468    :return: wheth
+00015010: 6572 2077 6520 6361 6e20 7369 6d70 6c69  er we can simpli
+00015020: 6679 2077 6865 6e20 6170 706c 7969 6e67  fy when applying
+00015030: 2074 6869 7320 6f70 6572 6174 696f 6e0a   this operation.
+00015040: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00015050: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
+00015060: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+00015070: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00015080: 7020 616e 6420 6f74 6865 722e 6465 7269  p and other.deri
+00015090: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+000150a0: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+000150b0: 2020 2020 2020 2074 6d70 203d 2073 656c         tmp = sel
+000150c0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+000150d0: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
+000150e0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+000150f0: 726f 6d5f 6f70 2e69 6e70 7574 7320 6966  rom_op.inputs if
+00015100: 2072 6967 6874 2065 6c73 6520 7265 7665   right else reve
+00015110: 7273 6564 286f 7468 6572 2e64 6572 6976  rsed(other.deriv
+00015120: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00015130: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00015140: 2020 2020 6966 206e 6f74 2074 6d70 2e63      if not tmp.c
+00015150: 616e 5f73 696d 706c 6966 7928 7465 726d  an_simplify(term
+00015160: 2c20 6b69 6e64 3d6b 696e 642c 2072 6967  , kind=kind, rig
+00015170: 6874 3d72 6967 6874 293a 0a20 2020 2020  ht=right):.     
+00015180: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015190: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+000151a0: 2020 2020 2020 2020 2020 2020 746d 702e              tmp.
+000151b0: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+000151c0: 7465 726d 2c20 6b69 6e64 3d6b 696e 642c  term, kind=kind,
+000151d0: 2072 6967 6874 3d72 6967 6874 290a 2020   right=right).  
+000151e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000151f0: 2054 7275 650a 2020 2020 2020 2020 6964   True.        id
+00015200: 7820 3d20 7365 6c66 2e5f 7369 6d70 6c69  x = self._simpli
+00015210: 6679 5f74 6572 6d5f 6964 7828 6f74 6865  fy_term_idx(othe
+00015220: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
+00015230: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
+00015240: 2020 2072 6574 7572 6e20 6964 7820 6973     return idx is
+00015250: 206e 6f74 204e 6f6e 650a 0a20 2020 2064   not None..    d
+00015260: 6566 205f 7369 6d70 6c69 6679 5f74 6572  ef _simplify_ter
+00015270: 6d5f 6964 7828 7365 6c66 2c20 6f74 6865  m_idx(self, othe
+00015280: 722c 206b 696e 642c 2072 6967 6874 293a  r, kind, right):
+00015290: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000152a0: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
+000152b0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+000152c0: 7061 7261 6d20 7374 7220 6b69 6e64 3a0a  param str kind:.
+000152d0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+000152e0: 6f6f 6c20 7269 6768 743a 0a20 2020 2020  ool right:.     
+000152f0: 2020 203a 7265 7475 726e 3a20 696e 6465     :return: inde
+00015300: 7820 6f66 2074 6572 6d20 746f 2073 696d  x of term to sim
+00015310: 706c 6966 790a 2020 2020 2020 2020 3a72  plify.        :r
+00015320: 7479 7065 3a20 696e 747c 4e6f 6e65 0a20  type: int|None. 
+00015330: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00015340: 2020 2069 6620 6e6f 7420 7365 6c66 2e74     if not self.t
+00015350: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+00015360: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00015370: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00015380: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
+00015390: 2020 2020 2320 5765 2077 616e 7420 2862      # We want (b
+000153a0: 202a 2061 2920 2f2f 2062 2021 3d20 612e   * a) // b != a.
+000153b0: 0a20 2020 2020 2020 2020 2020 2023 2048  .            # H
+000153c0: 6f77 6576 6572 2c20 7765 2077 616e 7420  owever, we want 
+000153d0: 6820 2a20 2832 202a 2061 202f 2f20 6829  h * (2 * a // h)
+000153e0: 203d 3d20 3220 2a20 612e 0a20 2020 2020   == 2 * a..     
+000153f0: 2020 2020 2020 2023 2053 6f2c 2066 6f72         # So, for
+00015400: 2060 6d75 6c60 2c20 616e 6420 6f6e 6c79   `mul`, and only
+00015410: 2066 6f72 2060 6d75 6c60 2c20 6368 6563   for `mul`, chec
+00015420: 6b20 616c 6c20 7465 726d 732c 2077 6865  k all terms, whe
+00015430: 7468 6572 2077 6520 6361 6e20 7369 6d70  ther we can simp
+00015440: 6c69 6679 2073 6f6d 6520 6469 7669 7369  lify some divisi
+00015450: 6f6e 2d74 6572 6d2e 0a20 2020 2020 2020  on-term..       
+00015460: 2020 2020 2066 6f72 2069 2c20 7465 726d       for i, term
+00015470: 2069 6e20 7265 7665 7273 6564 286c 6973   in reversed(lis
+00015480: 7428 656e 756d 6572 6174 6528 7365 6c66  t(enumerate(self
+00015490: 2e74 6572 6d73 2929 2920 6966 2072 6967  .terms))) if rig
+000154a0: 6874 2065 6c73 6520 656e 756d 6572 6174  ht else enumerat
+000154b0: 6528 7365 6c66 2e74 6572 6d73 293a 0a20  e(self.terms):. 
+000154c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000154d0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+000154e0: 2874 6572 6d2c 205f 642e 4469 6d29 0a20  (term, _d.Dim). 
+000154f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015500: 6620 7465 726d 2e64 6572 6976 6564 5f66  f term.derived_f
+00015510: 726f 6d5f 6f70 3a0a 2020 2020 2020 2020  rom_op:.        
+00015520: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00015530: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
+00015540: 5f6f 702e 6b69 6e64 203d 3d20 2274 7275  _op.kind == "tru
+00015550: 6564 6976 5f22 202b 2028 2272 6967 6874  ediv_" + ("right
+00015560: 2220 6966 2072 6967 6874 2065 6c73 6520  " if right else 
+00015570: 226c 6566 7422 293a 0a20 2020 2020 2020  "left"):.       
 00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015590: 2020 2020 2020 2069 6620 7465 726d 2e64         if term.d
-000155a0: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
-000155b0: 6e70 7574 735b 2d31 5d20 3d3d 206f 7468  nputs[-1] == oth
-000155c0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 7265 7475 726e 2069 0a20 2020 2020 2020  return i.       
-000155f0: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
-00015600: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00015610: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00015620: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
-00015630: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00015640: 6b69 6e64 203d 3d20 2274 7275 6564 6976  kind == "truediv
-00015650: 5f22 202b 2028 2272 6967 6874 2220 6966  _" + ("right" if
-00015660: 206e 6f74 2072 6967 6874 2065 6c73 6520   not right else 
-00015670: 226c 6566 7422 293a 0a20 2020 2020 2020  "left"):.       
-00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015690: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
-000156a0: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
-000156b0: 5b2d 315d 203d 3d20 7465 726d 3a0a 2020  [-1] == term:.  
+00015590: 2069 6620 7465 726d 2e64 6572 6976 6564   if term.derived
+000155a0: 5f66 726f 6d5f 6f70 2e69 6e70 7574 735b  _from_op.inputs[
+000155b0: 2d31 5d20 3d3d 206f 7468 6572 3a0a 2020  -1] == other:.  
+000155c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000155e0: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
+000155f0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
+00015600: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015620: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
+00015630: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
+00015640: 3d20 2274 7275 6564 6976 5f22 202b 2028  = "truediv_" + (
+00015650: 2272 6967 6874 2220 6966 206e 6f74 2072  "right" if not r
+00015660: 6967 6874 2065 6c73 6520 226c 6566 7422  ight else "left"
+00015670: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015680: 2020 2020 2020 2020 2020 2069 6620 6f74             if ot
+00015690: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+000156a0: 5f6f 702e 696e 7075 7473 5b2d 315d 203d  _op.inputs[-1] =
+000156b0: 3d20 7465 726d 3a0a 2020 2020 2020 2020  = term:.        
 000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000156e0: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
-000156f0: 2020 2069 6620 7465 726d 2e69 735f 636f     if term.is_co
-00015700: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
-00015710: 6d28 2920 616e 6420 6f74 6865 722e 6973  m() and other.is
-00015720: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00015730: 5f64 696d 2829 3a0a 2020 2020 2020 2020  _dim():.        
-00015740: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015750: 726e 2069 0a20 2020 2020 2020 2023 2046  rn i.        # F
-00015760: 6f72 2074 6865 206c 6173 742f 6669 7273  or the last/firs
-00015770: 7420 7465 726d 2c20 6578 7472 6120 6368  t term, extra ch
-00015780: 6563 6b73 2e0a 2020 2020 2020 2020 6920  ecks..        i 
-00015790: 3d20 6c65 6e28 7365 6c66 2e74 6572 6d73  = len(self.terms
-000157a0: 2920 2d20 3120 6966 2072 6967 6874 2065  ) - 1 if right e
-000157b0: 6c73 6520 300a 2020 2020 2020 2020 7465  lse 0.        te
-000157c0: 726d 203d 2073 656c 662e 7465 726d 735b  rm = self.terms[
-000157d0: 695d 0a20 2020 2020 2020 2069 6620 6b69  i].        if ki
-000157e0: 6e64 2e65 6e64 7377 6974 6828 2264 6976  nd.endswith("div
-000157f0: 2229 2061 6e64 206f 7468 6572 203d 3d20  ") and other == 
-00015800: 7465 726d 3a0a 2020 2020 2020 2020 2020  term:.          
-00015810: 2020 7265 7475 726e 2069 0a20 2020 2020    return i.     
-00015820: 2020 206f 705f 6b69 6e64 203d 206b 696e     op_kind = kin
-00015830: 6420 2b20 225f 2220 2b20 2822 7269 6768  d + "_" + ("righ
-00015840: 7422 2069 6620 7269 6768 7420 656c 7365  t" if right else
-00015850: 2022 6c65 6674 2229 0a20 2020 2020 2020   "left").       
-00015860: 2069 6620 7465 726d 2e64 6572 6976 6564   if term.derived
-00015870: 5f66 726f 6d5f 6f70 2061 6e64 2074 6572  _from_op and ter
-00015880: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
-00015890: 702e 6b69 6e64 203d 3d20 6f70 5f6b 696e  p.kind == op_kin
-000158a0: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-000158b0: 6574 7572 6e20 690a 2020 2020 2020 2020  eturn i.        
-000158c0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-000158d0: 2064 6566 2065 7874 656e 645f 6d75 6c5f   def extend_mul_
-000158e0: 6469 765f 2873 656c 662c 206f 7468 6572  div_(self, other
-000158f0: 2c20 6b69 6e64 2c20 7269 6768 7429 3a0a  , kind, right):.
-00015900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015910: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
-00015920: 7468 6572 3a0a 2020 2020 2020 2020 3a70  ther:.        :p
-00015930: 6172 616d 2073 7472 206b 696e 643a 0a20  aram str kind:. 
-00015940: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-00015950: 6f6c 2072 6967 6874 3a0a 2020 2020 2020  ol right:.      
-00015960: 2020 2222 220a 2020 2020 2020 2020 6173    """.        as
-00015970: 7365 7274 206b 696e 6420 696e 207b 226d  sert kind in {"m
-00015980: 756c 222c 2022 666c 6f6f 7264 6976 222c  ul", "floordiv",
-00015990: 2022 7472 7565 6469 7622 2c20 2263 6569   "truediv", "cei
-000159a0: 6c64 6976 227d 0a20 2020 2020 2020 2069  ldiv"}.        i
-000159b0: 6620 6f74 6865 722e 6973 5f63 6f6e 7374  f other.is_const
-000159c0: 616e 745f 7374 6174 6963 5f64 696d 2829  ant_static_dim()
-000159d0: 2061 6e64 206f 7468 6572 2e64 696d 656e   and other.dimen
-000159e0: 7369 6f6e 203d 3d20 313a 0a20 2020 2020  sion == 1:.     
-000159f0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00015a00: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00015a10: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
-00015a20: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
-00015a30: 226d 756c 223a 0a20 2020 2020 2020 2020  "mul":.         
-00015a40: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00015a50: 732e 6170 7065 6e64 286f 7468 6572 290a  s.append(other).
-00015a60: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00015a70: 206b 696e 642e 656e 6473 7769 7468 2822   kind.endswith("
-00015a80: 6469 7622 293a 0a20 2020 2020 2020 2020  div"):.         
-00015a90: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00015aa0: 7320 3d20 5b5f 4f70 4d75 6c74 5465 726d  s = [_OpMultTerm
-00015ab0: 2e6e 6577 5f64 6976 5f64 696d 2873 656c  .new_div_dim(sel
-00015ac0: 662e 6173 5f64 696d 2829 2c20 6f74 6865  f.as_dim(), othe
-00015ad0: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-00015ae0: 6768 743d 7269 6768 7429 5d0a 2020 2020  ght=right)].    
-00015af0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00015b00: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
-00015b10: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-00015b20: 616e 6420 6f74 6865 722e 6465 7269 7665  and other.derive
-00015b30: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
-00015b40: 3d20 226d 756c 223a 0a20 2020 2020 2020  = "mul":.       
-00015b50: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
-00015b60: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
-00015b70: 726f 6d5f 6f70 2e69 6e70 7574 7320 6966  rom_op.inputs if
-00015b80: 2072 6967 6874 2065 6c73 6520 7265 7665   right else reve
-00015b90: 7273 6564 286f 7468 6572 2e64 6572 6976  rsed(other.deriv
-00015ba0: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00015bb0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00015bc0: 2020 2020 7365 6c66 2e65 7874 656e 645f      self.extend_
-00015bd0: 6d75 6c5f 6469 765f 2874 6572 6d2c 206b  mul_div_(term, k
-00015be0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-00015bf0: 7269 6768 7429 0a20 2020 2020 2020 2020  right).         
-00015c00: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00015c10: 2020 6964 7820 3d20 7365 6c66 2e5f 7369    idx = self._si
-00015c20: 6d70 6c69 6679 5f74 6572 6d5f 6964 7828  mplify_term_idx(
-00015c30: 6f74 6865 722c 206b 696e 643d 6b69 6e64  other, kind=kind
-00015c40: 2c20 7269 6768 743d 7269 6768 7429 0a20  , right=right). 
-00015c50: 2020 2020 2020 2069 6620 6964 7820 6973         if idx is
-00015c60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00015c70: 2020 2020 2020 2074 6572 6d20 3d20 7365         term = se
-00015c80: 6c66 2e74 6572 6d73 5b69 6478 5d0a 2020  lf.terms[idx].  
-00015c90: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00015ca0: 2069 7369 6e73 7461 6e63 6528 7465 726d   isinstance(term
-00015cb0: 2c20 5f64 2e44 696d 290a 2020 2020 2020  , _d.Dim).      
-00015cc0: 2020 2020 2020 6966 206b 696e 642e 656e        if kind.en
-00015cd0: 6473 7769 7468 2822 6469 7622 2920 616e  dswith("div") an
-00015ce0: 6420 6f74 6865 7220 3d3d 2074 6572 6d3a  d other == term:
-00015cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015d00: 2073 656c 662e 7465 726d 732e 706f 7028   self.terms.pop(
-00015d10: 6964 7829 0a20 2020 2020 2020 2020 2020  idx).           
-00015d20: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00015d30: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
-00015d40: 3d3d 2022 6d75 6c22 2061 6e64 2074 6572  == "mul" and ter
-00015d50: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
-00015d60: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00015d70: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
-00015d80: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-00015d90: 3d3d 2022 7472 7565 6469 765f 2220 2b20  == "truediv_" + 
-00015da0: 2822 7269 6768 7422 2069 6620 7269 6768  ("right" if righ
-00015db0: 7420 656c 7365 2022 6c65 6674 2229 3a0a  t else "left"):.
-00015dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015dd0: 2020 2020 6966 2074 6572 6d2e 6465 7269      if term.deri
-00015de0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015df0: 7473 5b2d 315d 203d 3d20 6f74 6865 723a  ts[-1] == other:
-00015e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e10: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00015e20: 726d 735b 6964 785d 203d 2074 6572 6d2e  rms[idx] = term.
-00015e30: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00015e40: 696e 7075 7473 5b30 5d0a 2020 2020 2020  inputs[0].      
-00015e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e60: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00015e70: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
-00015e80: 226d 756c 2220 616e 6420 6f74 6865 722e  "mul" and other.
-00015e90: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
-00015ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015eb0: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
-00015ec0: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
-00015ed0: 3d20 2274 7275 6564 6976 5f22 202b 2028  = "truediv_" + (
-00015ee0: 2272 6967 6874 2220 6966 206e 6f74 2072  "right" if not r
-00015ef0: 6967 6874 2065 6c73 6520 226c 6566 7422  ight else "left"
-00015f00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00015f10: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
-00015f20: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00015f30: 696e 7075 7473 5b2d 315d 203d 3d20 7465  inputs[-1] == te
-00015f40: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
-00015f50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015f60: 2e74 6572 6d73 5b69 6478 5d20 3d20 6f74  .terms[idx] = ot
-00015f70: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
-00015f80: 5f6f 702e 696e 7075 7473 5b30 5d0a 2020  _op.inputs[0].  
+000156d0: 2020 2020 7265 7475 726e 2069 0a20 2020      return i.   
+000156e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000156f0: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
+00015700: 5f73 7461 7469 635f 6469 6d28 2920 616e  _static_dim() an
+00015710: 6420 6f74 6865 722e 6973 5f63 6f6e 7374  d other.is_const
+00015720: 616e 745f 7374 6174 6963 5f64 696d 2829  ant_static_dim()
+00015730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015740: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
+00015750: 2020 2020 2020 2023 2046 6f72 2074 6865         # For the
+00015760: 206c 6173 742f 6669 7273 7420 7465 726d   last/first term
+00015770: 2c20 6578 7472 6120 6368 6563 6b73 2e0a  , extra checks..
+00015780: 2020 2020 2020 2020 6920 3d20 6c65 6e28          i = len(
+00015790: 7365 6c66 2e74 6572 6d73 2920 2d20 3120  self.terms) - 1 
+000157a0: 6966 2072 6967 6874 2065 6c73 6520 300a  if right else 0.
+000157b0: 2020 2020 2020 2020 7465 726d 203d 2073          term = s
+000157c0: 656c 662e 7465 726d 735b 695d 0a20 2020  elf.terms[i].   
+000157d0: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
+000157e0: 7377 6974 6828 2264 6976 2229 2061 6e64  swith("div") and
+000157f0: 206f 7468 6572 203d 3d20 7465 726d 3a0a   other == term:.
+00015800: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015810: 726e 2069 0a20 2020 2020 2020 206f 705f  rn i.        op_
+00015820: 6b69 6e64 203d 206b 696e 6420 2b20 225f  kind = kind + "_
+00015830: 2220 2b20 2822 7269 6768 7422 2069 6620  " + ("right" if 
+00015840: 7269 6768 7420 656c 7365 2022 6c65 6674  right else "left
+00015850: 2229 0a20 2020 2020 2020 2069 6620 7465  ").        if te
+00015860: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
+00015870: 6f70 2061 6e64 2074 6572 6d2e 6465 7269  op and term.deri
+00015880: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00015890: 203d 3d20 6f70 5f6b 696e 643a 0a20 2020   == op_kind:.   
+000158a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000158b0: 690a 2020 2020 2020 2020 7265 7475 726e  i.        return
+000158c0: 204e 6f6e 650a 0a20 2020 2064 6566 2065   None..    def e
+000158d0: 7874 656e 645f 6d75 6c5f 6469 765f 2873  xtend_mul_div_(s
+000158e0: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
+000158f0: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
+00015900: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00015910: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
+00015920: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+00015930: 7472 206b 696e 643a 0a20 2020 2020 2020  tr kind:.       
+00015940: 203a 7061 7261 6d20 626f 6f6c 2072 6967   :param bool rig
+00015950: 6874 3a0a 2020 2020 2020 2020 2222 220a  ht:.        """.
+00015960: 2020 2020 2020 2020 6173 7365 7274 206b          assert k
+00015970: 696e 6420 696e 207b 226d 756c 222c 2022  ind in {"mul", "
+00015980: 666c 6f6f 7264 6976 222c 2022 7472 7565  floordiv", "true
+00015990: 6469 7622 2c20 2263 6569 6c64 6976 227d  div", "ceildiv"}
+000159a0: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+000159b0: 722e 6973 5f63 6f6e 7374 616e 745f 7374  r.is_constant_st
+000159c0: 6174 6963 5f64 696d 2829 2061 6e64 206f  atic_dim() and o
+000159d0: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
+000159e0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+000159f0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00015a00: 6966 206e 6f74 2073 656c 662e 7465 726d  if not self.term
+00015a10: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00015a20: 6620 6b69 6e64 203d 3d20 226d 756c 223a  f kind == "mul":
+00015a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015a40: 2073 656c 662e 7465 726d 732e 6170 7065   self.terms.appe
+00015a50: 6e64 286f 7468 6572 290a 2020 2020 2020  nd(other).      
+00015a60: 2020 2020 2020 656c 6966 206b 696e 642e        elif kind.
+00015a70: 656e 6473 7769 7468 2822 6469 7622 293a  endswith("div"):
+00015a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015a90: 2073 656c 662e 7465 726d 7320 3d20 5b5f   self.terms = [_
+00015aa0: 4f70 4d75 6c74 5465 726d 2e6e 6577 5f64  OpMultTerm.new_d
+00015ab0: 6976 5f64 696d 2873 656c 662e 6173 5f64  iv_dim(self.as_d
+00015ac0: 696d 2829 2c20 6f74 6865 722c 206b 696e  im(), other, kin
+00015ad0: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+00015ae0: 6768 7429 5d0a 2020 2020 2020 2020 2020  ght)].          
+00015af0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00015b00: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
+00015b10: 645f 6672 6f6d 5f6f 7020 616e 6420 6f74  d_from_op and ot
+00015b20: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+00015b30: 5f6f 702e 6b69 6e64 203d 3d20 226d 756c  _op.kind == "mul
+00015b40: 223a 0a20 2020 2020 2020 2020 2020 2066  ":.            f
+00015b50: 6f72 2074 6572 6d20 696e 206f 7468 6572  or term in other
+00015b60: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015b70: 2e69 6e70 7574 7320 6966 2072 6967 6874  .inputs if right
+00015b80: 2065 6c73 6520 7265 7665 7273 6564 286f   else reversed(o
+00015b90: 7468 6572 2e64 6572 6976 6564 5f66 726f  ther.derived_fro
+00015ba0: 6d5f 6f70 2e69 6e70 7574 7329 3a0a 2020  m_op.inputs):.  
+00015bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015bc0: 6c66 2e65 7874 656e 645f 6d75 6c5f 6469  lf.extend_mul_di
+00015bd0: 765f 2874 6572 6d2c 206b 696e 643d 6b69  v_(term, kind=ki
+00015be0: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
+00015bf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015c00: 7572 6e0a 2020 2020 2020 2020 6964 7820  urn.        idx 
+00015c10: 3d20 7365 6c66 2e5f 7369 6d70 6c69 6679  = self._simplify
+00015c20: 5f74 6572 6d5f 6964 7828 6f74 6865 722c  _term_idx(other,
+00015c30: 206b 696e 643d 6b69 6e64 2c20 7269 6768   kind=kind, righ
+00015c40: 743d 7269 6768 7429 0a20 2020 2020 2020  t=right).       
+00015c50: 2069 6620 6964 7820 6973 206e 6f74 204e   if idx is not N
+00015c60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00015c70: 2074 6572 6d20 3d20 7365 6c66 2e74 6572   term = self.ter
+00015c80: 6d73 5b69 6478 5d0a 2020 2020 2020 2020  ms[idx].        
+00015c90: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00015ca0: 7461 6e63 6528 7465 726d 2c20 5f64 2e44  tance(term, _d.D
+00015cb0: 696d 290a 2020 2020 2020 2020 2020 2020  im).            
+00015cc0: 6966 206b 696e 642e 656e 6473 7769 7468  if kind.endswith
+00015cd0: 2822 6469 7622 2920 616e 6420 6f74 6865  ("div") and othe
+00015ce0: 7220 3d3d 2074 6572 6d3a 0a20 2020 2020  r == term:.     
+00015cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015d00: 7465 726d 732e 706f 7028 6964 7829 0a20  terms.pop(idx). 
+00015d10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015d20: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
+00015d30: 2020 6966 206b 696e 6420 3d3d 2022 6d75    if kind == "mu
+00015d40: 6c22 2061 6e64 2074 6572 6d2e 6465 7269  l" and term.deri
+00015d50: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+00015d60: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00015d70: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
+00015d80: 6d5f 6f70 2e6b 696e 6420 3d3d 2022 7472  m_op.kind == "tr
+00015d90: 7565 6469 765f 2220 2b20 2822 7269 6768  uediv_" + ("righ
+00015da0: 7422 2069 6620 7269 6768 7420 656c 7365  t" if right else
+00015db0: 2022 6c65 6674 2229 3a0a 2020 2020 2020   "left"):.      
+00015dc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00015dd0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
+00015de0: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
+00015df0: 203d 3d20 6f74 6865 723a 0a20 2020 2020   == other:.     
+00015e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e10: 2020 2073 656c 662e 7465 726d 735b 6964     self.terms[id
+00015e20: 785d 203d 2074 6572 6d2e 6465 7269 7665  x] = term.derive
+00015e30: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+00015e40: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00015e50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015e60: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00015e70: 6620 6b69 6e64 203d 3d20 226d 756c 2220  f kind == "mul" 
+00015e80: 616e 6420 6f74 6865 722e 6465 7269 7665  and other.derive
+00015e90: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
+00015ea0: 2020 2020 2020 2020 2020 2069 6620 6f74             if ot
+00015eb0: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+00015ec0: 5f6f 702e 6b69 6e64 203d 3d20 2274 7275  _op.kind == "tru
+00015ed0: 6564 6976 5f22 202b 2028 2272 6967 6874  ediv_" + ("right
+00015ee0: 2220 6966 206e 6f74 2072 6967 6874 2065  " if not right e
+00015ef0: 6c73 6520 226c 6566 7422 293a 0a20 2020  lse "left"):.   
+00015f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f10: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
+00015f20: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+00015f30: 5b2d 315d 203d 3d20 7465 726d 3a0a 2020  [-1] == term:.  
+00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f50: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00015f60: 5b69 6478 5d20 3d20 6f74 6865 722e 6465  [idx] = other.de
+00015f70: 7269 7665 645f 6672 6f6d 5f6f 702e 696e  rived_from_op.in
+00015f80: 7075 7473 5b30 5d0a 2020 2020 2020 2020  puts[0].        
 00015f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fa0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00015fb0: 2020 2020 2020 2020 2069 6620 7465 726d           if term
-00015fc0: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
-00015fd0: 7469 635f 6469 6d28 2920 616e 6420 6f74  tic_dim() and ot
-00015fe0: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
-00015ff0: 7374 6174 6963 5f64 696d 2829 3a0a 2020  static_dim():.  
-00016000: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016010: 206b 696e 6420 3d3d 2022 6d75 6c22 3a0a   kind == "mul":.
-00016020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016030: 2020 2020 6966 2074 6572 6d2e 6469 6d65      if term.dime
-00016040: 6e73 696f 6e20 2a20 6f74 6865 722e 6469  nsion * other.di
-00016050: 6d65 6e73 696f 6e20 3d3d 2031 3a0a 2020  mension == 1:.  
+00015fa0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00015fb0: 2020 2069 6620 7465 726d 2e69 735f 636f     if term.is_co
+00015fc0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00015fd0: 6d28 2920 616e 6420 6f74 6865 722e 6973  m() and other.is
+00015fe0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+00015ff0: 5f64 696d 2829 3a0a 2020 2020 2020 2020  _dim():.        
+00016000: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
+00016010: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
+00016020: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016030: 2074 6572 6d2e 6469 6d65 6e73 696f 6e20   term.dimension 
+00016040: 2a20 6f74 6865 722e 6469 6d65 6e73 696f  * other.dimensio
+00016050: 6e20 3d3d 2031 3a0a 2020 2020 2020 2020  n == 1:.        
 00016060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016070: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00016080: 2e70 6f70 2869 6478 290a 2020 2020 2020  .pop(idx).      
-00016090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160a0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-000160b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000160c0: 662e 7465 726d 735b 6964 785d 203d 205f  f.terms[idx] = _
-000160d0: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-000160e0: 6174 6963 5f64 696d 2874 6572 6d2e 6469  atic_dim(term.di
-000160f0: 6d65 6e73 696f 6e20 2a20 6f74 6865 722e  mension * other.
-00016100: 6469 6d65 6e73 696f 6e2c 206b 696e 643d  dimension, kind=
-00016110: 7465 726d 2e6b 696e 6429 0a20 2020 2020  term.kind).     
-00016120: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00016130: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00016140: 2020 2020 2020 6966 206b 696e 642e 656e        if kind.en
-00016150: 6473 7769 7468 2822 6469 7622 2920 616e  dswith("div") an
-00016160: 6420 7465 726d 2e64 696d 656e 7369 6f6e  d term.dimension
-00016170: 2025 206f 7468 6572 2e64 696d 656e 7369   % other.dimensi
-00016180: 6f6e 203d 3d20 303a 0a20 2020 2020 2020  on == 0:.       
-00016190: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000161a0: 662e 7465 726d 735b 6964 785d 203d 205f  f.terms[idx] = _
-000161b0: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-000161c0: 6174 6963 5f64 696d 2874 6572 6d2e 6469  atic_dim(term.di
-000161d0: 6d65 6e73 696f 6e20 2f2f 206f 7468 6572  mension // other
-000161e0: 2e64 696d 656e 7369 6f6e 2c20 6b69 6e64  .dimension, kind
-000161f0: 3d74 6572 6d2e 6b69 6e64 290a 2020 2020  =term.kind).    
-00016200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016210: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00016220: 2020 2020 2020 2023 2046 616c 6c62 6163         # Fallbac
-00016230: 6b20 7769 7468 2067 656e 6572 6963 2068  k with generic h
-00016240: 616e 646c 696e 672e 0a20 2020 2020 2020  andling..       
-00016250: 2020 2020 206f 705f 6b69 6e64 203d 206b       op_kind = k
-00016260: 696e 6420 2b20 225f 2220 2b20 2822 7269  ind + "_" + ("ri
-00016270: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-00016280: 7365 2022 6c65 6674 2229 0a20 2020 2020  se "left").     
-00016290: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-000162a0: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
-000162b0: 6e64 2074 6572 6d2e 6465 7269 7665 645f  nd term.derived_
-000162c0: 6672 6f6d 5f6f 7020 616e 6420 7465 726d  from_op and term
-000162d0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-000162e0: 2e6b 696e 6420 3d3d 206f 705f 6b69 6e64  .kind == op_kind
-000162f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016300: 2020 6e75 6d65 7261 746f 7220 3d20 7465    numerator = te
-00016310: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
-00016320: 6f70 2e69 6e70 7574 735b 305d 0a20 2020  op.inputs[0].   
-00016330: 2020 2020 2020 2020 2020 2020 2064 656e               den
-00016340: 6f6d 696e 6174 6f72 203d 2074 6572 6d2e  ominator = term.
-00016350: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00016360: 696e 7075 7473 5b31 5d0a 2020 2020 2020  inputs[1].      
-00016370: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00016380: 6572 6d73 5b69 6478 5d20 3d20 5f4f 704d  erms[idx] = _OpM
-00016390: 756c 7454 6572 6d2e 6e65 775f 6469 765f  ultTerm.new_div_
-000163a0: 6469 6d28 6e75 6d65 7261 746f 722c 2064  dim(numerator, d
-000163b0: 656e 6f6d 696e 6174 6f72 202a 206f 7468  enominator * oth
-000163c0: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
-000163d0: 6967 6874 3d72 6967 6874 290a 2020 2020  ight=right).    
-000163e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000163f0: 726e 0a20 2020 2020 2020 2069 6620 6b69  rn.        if ki
-00016400: 6e64 2e65 6e64 7377 6974 6828 2264 6976  nd.endswith("div
-00016410: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00016420: 7365 6c66 2e74 6572 6d73 203d 205b 5f4f  self.terms = [_O
-00016430: 704d 756c 7454 6572 6d2e 6e65 775f 6469  pMultTerm.new_di
-00016440: 765f 6469 6d28 7365 6c66 2e61 735f 6469  v_dim(self.as_di
-00016450: 6d28 292c 206f 7468 6572 2c20 6b69 6e64  m(), other, kind
-00016460: 3d6b 696e 642c 2072 6967 6874 3d72 6967  =kind, right=rig
-00016470: 6874 295d 0a20 2020 2020 2020 2020 2020  ht)].           
-00016480: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00016490: 6966 206b 696e 6420 3d3d 2022 6d75 6c22  if kind == "mul"
-000164a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000164b0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-000164c0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-000164d0: 6d73 2e61 7070 656e 6428 6f74 6865 7229  ms.append(other)
-000164e0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000164f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00016500: 2020 2073 656c 662e 7465 726d 732e 696e     self.terms.in
-00016510: 7365 7274 2830 2c20 6f74 6865 7229 0a20  sert(0, other). 
-00016520: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00016530: 6e0a 2020 2020 2020 2020 6173 7365 7274  n.        assert
-00016540: 2046 616c 7365 0a0a 2020 2020 4063 6c61   False..    @cla
-00016550: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00016560: 206e 6577 5f64 6976 5f64 696d 2863 6c73   new_div_dim(cls
-00016570: 2c20 6e75 6d65 7261 746f 722c 2064 656e  , numerator, den
-00016580: 6f6d 696e 6174 6f72 2c20 6b69 6e64 2c20  ominator, kind, 
-00016590: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
-000165a0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-000165b0: 616d 2044 696d 206e 756d 6572 6174 6f72  am Dim numerator
-000165c0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-000165d0: 2044 696d 2064 656e 6f6d 696e 6174 6f72   Dim denominator
-000165e0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-000165f0: 2073 7472 206b 696e 643a 2022 666c 6f6f   str kind: "floo
-00016600: 7264 6976 2220 6f72 2022 6365 696c 6469  rdiv" or "ceildi
-00016610: 7622 206f 7220 2274 7275 6564 6976 220a  v" or "truediv".
-00016620: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-00016630: 6f6f 6c20 7269 6768 743a 0a20 2020 2020  ool right:.     
-00016640: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00016650: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016660: 2020 2064 696d 5f76 616c 7565 203d 204e     dim_value = N
-00016670: 6f6e 650a 2020 2020 2020 2020 6120 3d20  one.        a = 
-00016680: 6e75 6d65 7261 746f 722e 6469 6d65 6e73  numerator.dimens
-00016690: 696f 6e0a 2020 2020 2020 2020 6220 3d20  ion.        b = 
-000166a0: 6465 6e6f 6d69 6e61 746f 722e 6469 6d65  denominator.dime
-000166b0: 6e73 696f 6e0a 2020 2020 2020 2020 6966  nsion.        if
-000166c0: 2061 2069 7320 6e6f 7420 4e6f 6e65 2061   a is not None a
-000166d0: 6e64 2062 2069 7320 6e6f 7420 4e6f 6e65  nd b is not None
-000166e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000166f0: 206b 696e 6420 3d3d 2022 666c 6f6f 7264   kind == "floord
-00016700: 6976 223a 0a20 2020 2020 2020 2020 2020  iv":.           
-00016710: 2020 2020 2064 696d 5f76 616c 7565 203d       dim_value =
-00016720: 2061 202f 2f20 620a 2020 2020 2020 2020   a // b.        
-00016730: 2020 2020 656c 6966 206b 696e 6420 3d3d      elif kind ==
-00016740: 2022 6365 696c 6469 7622 3a0a 2020 2020   "ceildiv":.    
-00016750: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
-00016760: 7661 6c75 6520 3d20 2d28 2d61 202f 2f20  value = -(-a // 
-00016770: 6229 0a20 2020 2020 2020 2020 2020 2020  b).             
-00016780: 2020 2069 6620 6120 2520 6220 3d3d 2030     if a % b == 0
-00016790: 2061 6e64 2072 6967 6874 3a0a 2020 2020   and right:.    
-000167a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167b0: 6b69 6e64 203d 2022 666c 6f6f 7264 6976  kind = "floordiv
-000167c0: 2220 2023 2066 6f72 206e 6963 6572 2064  "  # for nicer d
-000167d0: 6573 6372 6970 7469 6f6e 2c20 616e 6420  escription, and 
-000167e0: 646f 6573 206e 6f74 206d 6174 7465 720a  does not matter.
-000167f0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00016800: 206b 696e 6420 3d3d 2022 7472 7565 6469   kind == "truedi
-00016810: 7622 3a0a 2020 2020 2020 2020 2020 2020  v":.            
-00016820: 2020 2020 6966 2061 2025 2062 2021 3d20      if a % b != 
-00016830: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00016840: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00016850: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016870: 2022 2573 2074 7275 6564 6976 2025 7320   "%s truediv %s 
-00016880: 6f6e 6c79 2061 6c6c 6f77 6564 2069 6620  only allowed if 
-00016890: 7468 6520 7265 7375 6c74 2069 7320 616e  the result is an
-000168a0: 2069 6e74 6567 6572 2220 2520 286e 756d   integer" % (num
-000168b0: 6572 6174 6f72 2c20 6465 6e6f 6d69 6e61  erator, denomina
-000168c0: 746f 7229 0a20 2020 2020 2020 2020 2020  tor).           
-000168d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000168e0: 2020 2020 2020 2020 2020 2064 696d 5f76             dim_v
-000168f0: 616c 7565 203d 2061 202f 2f20 620a 2020  alue = a // b.  
-00016900: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016910: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-00016920: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-00016930: 203d 2022 666c 6f6f 7264 6976 2220 2023   = "floordiv"  #
-00016940: 2066 6f72 206e 6963 6572 2064 6573 6372   for nicer descr
-00016950: 6970 7469 6f6e 2c20 616e 6420 646f 6573  iption, and does
-00016960: 206e 6f74 206d 6174 7465 720a 2020 2020   not matter.    
-00016970: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016980: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00016990: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-000169a0: 696e 7661 6c69 6420 6b69 6e64 2025 7222  invalid kind %r"
-000169b0: 2025 2028 6b69 6e64 2c29 290a 2020 2020   % (kind,)).    
-000169c0: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
-000169d0: 666c 6f6f 7264 6976 2220 616e 6420 7269  floordiv" and ri
-000169e0: 6768 743a 0a20 2020 2020 2020 2020 2020  ght:.           
-000169f0: 2064 6573 6372 6970 7469 6f6e 203d 2022   description = "
-00016a00: 2573 2f2f 2573 2220 2520 285f 6765 745f  %s//%s" % (_get_
-00016a10: 6465 7363 7269 7074 696f 6e28 6e75 6d65  description(nume
-00016a20: 7261 746f 7229 2c20 5f67 6574 5f64 6573  rator), _get_des
-00016a30: 6372 6970 7469 6f6e 2864 656e 6f6d 696e  cription(denomin
-00016a40: 6174 6f72 2929 0a20 2020 2020 2020 2065  ator)).        e
-00016a50: 6c69 6620 6b69 6e64 203d 3d20 2263 6569  lif kind == "cei
-00016a60: 6c64 6976 2220 616e 6420 7269 6768 743a  ldiv" and right:
-00016a70: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00016a80: 6372 6970 7469 6f6e 203d 2022 e28c 8825  cription = "...%
-00016a90: 732f 2573 e28c 8922 2025 2028 5f67 6574  s/%s..." % (_get
-00016aa0: 5f64 6573 6372 6970 7469 6f6e 286e 756d  _description(num
-00016ab0: 6572 6174 6f72 292c 205f 6765 745f 6465  erator), _get_de
-00016ac0: 7363 7269 7074 696f 6e28 6465 6e6f 6d69  scription(denomi
-00016ad0: 6e61 746f 7229 290a 2020 2020 2020 2020  nator)).        
-00016ae0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016af0: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
-00016b00: 2225 735f 2573 2825 732c 2025 7329 2220  "%s_%s(%s, %s)" 
-00016b10: 2520 280a 2020 2020 2020 2020 2020 2020  % (.            
-00016b20: 2020 2020 6b69 6e64 2c0a 2020 2020 2020      kind,.      
-00016b30: 2020 2020 2020 2020 2020 2272 6967 6874            "right
-00016b40: 2220 6966 2072 6967 6874 2065 6c73 6520  " if right else 
-00016b50: 226c 6566 7422 2c0a 2020 2020 2020 2020  "left",.        
-00016b60: 2020 2020 2020 2020 5f67 6574 5f64 6573          _get_des
-00016b70: 6372 6970 7469 6f6e 286e 756d 6572 6174  cription(numerat
-00016b80: 6f72 2c20 6272 6163 6b65 7473 3d46 616c  or, brackets=Fal
-00016b90: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
-00016ba0: 2020 2020 205f 6765 745f 6465 7363 7269       _get_descri
-00016bb0: 7074 696f 6e28 6465 6e6f 6d69 6e61 746f  ption(denominato
-00016bc0: 722c 2062 7261 636b 6574 733d 4661 6c73  r, brackets=Fals
-00016bd0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00016be0: 290a 2020 2020 2020 2020 6f70 5f6b 696e  ).        op_kin
-00016bf0: 6420 3d20 6b69 6e64 0a20 2020 2020 2020  d = kind.       
-00016c00: 2069 6620 6120 6973 206e 6f74 204e 6f6e   if a is not Non
-00016c10: 6520 616e 6420 6220 6973 206e 6f74 204e  e and b is not N
-00016c20: 6f6e 6520 616e 6420 6120 2520 6220 3d3d  one and a % b ==
-00016c30: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00016c40: 6f70 5f6b 696e 6420 3d20 2274 7275 6564  op_kind = "trued
-00016c50: 6976 2220 2023 206d 616b 6573 2073 6f6d  iv"  # makes som
-00016c60: 6520 6f74 6865 7220 6368 6563 6b73 2073  e other checks s
-00016c70: 696d 706c 6572 0a20 2020 2020 2020 206f  impler.        o
-00016c80: 705f 6b69 6e64 202b 3d20 225f 2220 2b20  p_kind += "_" + 
-00016c90: 2822 7269 6768 7422 2069 6620 7269 6768  ("right" if righ
-00016ca0: 7420 656c 7365 2022 6c65 6674 2229 0a20  t else "left"). 
-00016cb0: 2020 2020 2020 2072 6574 7572 6e20 5f64         return _d
-00016cc0: 2e44 696d 280a 2020 2020 2020 2020 2020  .Dim(.          
-00016cd0: 2020 6465 7363 7269 7074 696f 6e3d 6465    description=de
-00016ce0: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
-00016cf0: 2020 2020 2020 206b 696e 643d 6e75 6d65         kind=nume
-00016d00: 7261 746f 722e 6b69 6e64 2c0a 2020 2020  rator.kind,.    
-00016d10: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
-00016d20: 6e3d 6469 6d5f 7661 6c75 652c 0a20 2020  n=dim_value,.   
-00016d30: 2020 2020 2020 2020 2064 6572 6976 6564           derived
-00016d40: 5f66 726f 6d5f 6f70 3d4f 7028 6b69 6e64  _from_op=Op(kind
-00016d50: 3d6f 705f 6b69 6e64 2c20 696e 7075 7473  =op_kind, inputs
-00016d60: 3d5b 6e75 6d65 7261 746f 722c 2064 656e  =[numerator, den
-00016d70: 6f6d 696e 6174 6f72 5d29 2c0a 2020 2020  ominator]),.    
-00016d80: 2020 2020 2020 2020 6465 7269 7665 645f          derived_
-00016d90: 6672 6f6d 5f74 6167 3d6e 756d 6572 6174  from_tag=numerat
-00016da0: 6f72 2c0a 2020 2020 2020 2020 290a 0a20  or,.        ).. 
-00016db0: 2020 2064 6566 2061 735f 6469 6d28 7365     def as_dim(se
-00016dc0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00016dd0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00016de0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-00016df0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00016e00: 2e69 735f 6f6e 6528 293a 0a20 2020 2020  .is_one():.     
-00016e10: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00016e20: 616b 655f 636f 6e73 7461 6e74 5f73 7461  ake_constant_sta
-00016e30: 7469 635f 6469 6d28 3129 0a20 2020 2020  tic_dim(1).     
-00016e40: 2020 2069 6620 6c65 6e28 7365 6c66 2e74     if len(self.t
-00016e50: 6572 6d73 2920 3d3d 2031 3a0a 2020 2020  erms) == 1:.    
-00016e60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00016e70: 656c 662e 7465 726d 735b 305d 0a20 2020  elf.terms[0].   
-00016e80: 2020 2020 2064 696d 5f6b 696e 6420 3d20       dim_kind = 
-00016e90: 5f67 6574 5f6d 6572 6765 645f 6469 6d5f  _get_merged_dim_
-00016ea0: 6b69 6e64 2873 656c 662e 7465 726d 7329  kind(self.terms)
-00016eb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016ec0: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
-00016ed0: 2020 2020 6b69 6e64 3d64 696d 5f6b 696e      kind=dim_kin
-00016ee0: 642c 0a20 2020 2020 2020 2020 2020 2064  d,.            d
-00016ef0: 6573 6372 6970 7469 6f6e 3d22 2a22 2e6a  escription="*".j
-00016f00: 6f69 6e28 6d61 7028 5f67 6574 5f64 6573  oin(map(_get_des
-00016f10: 6372 6970 7469 6f6e 2c20 7365 6c66 2e74  cription, self.t
-00016f20: 6572 6d73 2929 2c0a 2020 2020 2020 2020  erms)),.        
-00016f30: 2020 2020 6469 6d65 6e73 696f 6e3d 7365      dimension=se
-00016f40: 6c66 2e64 696d 656e 7369 6f6e 2c0a 2020  lf.dimension,.  
-00016f50: 2020 2020 2020 2020 2020 6465 7269 7665            derive
-00016f60: 645f 6672 6f6d 5f6f 703d 4f70 286b 696e  d_from_op=Op(kin
-00016f70: 643d 226d 756c 222c 2069 6e70 7574 733d  d="mul", inputs=
-00016f80: 6c69 7374 2873 656c 662e 7465 726d 7329  list(self.terms)
-00016f90: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
-00016fa0: 6572 6976 6564 5f66 726f 6d5f 7461 673d  erived_from_tag=
-00016fb0: 7365 6c66 2e72 6570 7265 7365 6e74 6174  self.representat
-00016fc0: 6976 655f 7461 6728 292c 0a20 2020 2020  ive_tag(),.     
-00016fd0: 2020 2029 0a0a 2020 2020 6465 6620 7265     )..    def re
-00016fe0: 7072 6573 656e 7461 7469 7665 5f74 6167  presentative_tag
-00016ff0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00017000: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-00017010: 7065 3a20 4469 6d7c 4e6f 6e65 0a20 2020  pe: Dim|None.   
-00017020: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00017030: 2023 2041 6c73 6f20 7365 6520 4469 6d2e   # Also see Dim.
-00017040: 5f4f 704c 696e 6561 7254 6572 6d2e 7265  _OpLinearTerm.re
-00017050: 7072 6573 656e 7461 7469 7665 5f74 6167  presentative_tag
-00017060: 2829 2e0a 2020 2020 2020 2020 2320 4669  ()..        # Fi
-00017070: 7273 7420 6669 6e64 2061 6e79 2064 796e  rst find any dyn
-00017080: 616d 6963 2e0a 2020 2020 2020 2020 666f  amic..        fo
-00017090: 7220 7465 726d 5f20 696e 2073 656c 662e  r term_ in self.
-000170a0: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-000170b0: 2020 2069 6620 7465 726d 5f2e 6973 5f64     if term_.is_d
-000170c0: 796e 616d 6963 2829 3a0a 2020 2020 2020  ynamic():.      
-000170d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000170e0: 2074 6572 6d5f 0a20 2020 2020 2020 2023   term_.        #
-000170f0: 204e 6f77 2066 696e 6420 6e6f 6e2d 756e   Now find non-un
-00017100: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
-00017110: 2020 2066 6f72 2074 6572 6d5f 2069 6e20     for term_ in 
-00017120: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
-00017130: 2020 2020 2020 2020 6966 2074 6572 6d5f          if term_
-00017140: 2e6b 696e 6420 213d 2044 696d 5479 7065  .kind != DimType
-00017150: 732e 556e 7370 6563 6966 6965 643a 0a20  s.Unspecified:. 
-00017160: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017170: 6574 7572 6e20 7465 726d 5f0a 2020 2020  eturn term_.    
-00017180: 2020 2020 2320 4e6f 7720 6669 6e64 2061      # Now find a
-00017190: 6e79 2e0a 2020 2020 2020 2020 666f 7220  ny..        for 
-000171a0: 7465 726d 5f20 696e 2073 656c 662e 7465  term_ in self.te
-000171b0: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
-000171c0: 2072 6574 7572 6e20 7465 726d 5f0a 2020   return term_.  
-000171d0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000171e0: 650a 0a0a 636c 6173 7320 5f4f 704c 696e  e...class _OpLin
-000171f0: 6561 7254 6572 6d3a 0a20 2020 2022 2222  earTerm:.    """
-00017200: 0a20 2020 2072 6570 7265 7365 6e74 7320  .    represents 
-00017210: 7374 6820 6c69 6b65 2061 202a 2062 202b  sth like a * b +
-00017220: 2063 0a20 2020 2022 2222 0a0a 2020 2020   c.    """..    
-00017230: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00017240: 2064 6566 2066 726f 6d5f 6469 6d28 636c   def from_dim(cl
-00017250: 732c 2064 696d 293a 0a20 2020 2020 2020  s, dim):.       
-00017260: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00017270: 7261 6d20 4469 6d20 6469 6d3a 0a20 2020  ram Dim dim:.   
-00017280: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00017290: 2e5f 4f70 4c69 6e65 6172 5465 726d 0a20  ._OpLinearTerm. 
-000172a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000172b0: 2020 2072 6573 203d 2063 6c73 2e7a 6572     res = cls.zer
-000172c0: 6f28 290a 2020 2020 2020 2020 7265 732e  o().        res.
-000172d0: 6578 7465 6e64 5f61 6464 5f73 7562 5f28  extend_add_sub_(
-000172e0: 6469 6d2c 206b 696e 643d 2261 6464 222c  dim, kind="add",
-000172f0: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
-00017300: 2020 2020 2072 6574 7572 6e20 7265 730a       return res.
-00017310: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00017320: 640a 2020 2020 6465 6620 7a65 726f 2863  d.    def zero(c
-00017330: 6c73 293a 0a20 2020 2020 2020 2022 2222  ls):.        """
-00017340: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00017350: 2044 696d 2e5f 4f70 4c69 6e65 6172 5465   Dim._OpLinearTe
-00017360: 726d 0a20 2020 2020 2020 2022 2222 0a20  rm.        """. 
-00017370: 2020 2020 2020 2072 6574 7572 6e20 5f4f         return _O
-00017380: 704c 696e 6561 7254 6572 6d28 5b5d 290a  pLinearTerm([]).
-00017390: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000173a0: 5f28 7365 6c66 2c20 7465 726d 7329 3a0a  _(self, terms):.
-000173b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000173c0: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
-000173d0: 4469 6d2e 5f4f 704d 756c 7454 6572 6d5d  Dim._OpMultTerm]
-000173e0: 2074 6572 6d73 3a0a 2020 2020 2020 2020   terms:.        
-000173f0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00017400: 2e74 6572 6d73 203d 2074 6572 6d73 0a0a  .terms = terms..
-00017410: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
-00017420: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00017430: 7265 7475 726e 2068 6173 6828 7475 706c  return hash(tupl
-00017440: 6528 7365 6c66 2e74 6572 6d73 2929 0a0a  e(self.terms))..
-00017450: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-00017460: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00017470: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00017480: 6365 286f 7468 6572 2c20 5f4f 704c 696e  ce(other, _OpLin
-00017490: 6561 7254 6572 6d29 3a0a 2020 2020 2020  earTerm):.      
-000174a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000174b0: 662e 7465 726d 7320 3d3d 206f 7468 6572  f.terms == other
-000174c0: 2e74 6572 6d73 0a20 2020 2020 2020 2072  .terms.        r
-000174d0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-000174e0: 2064 6566 205f 5f6e 655f 5f28 7365 6c66   def __ne__(self
-000174f0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00017500: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
-00017510: 662e 5f5f 6571 5f5f 286f 7468 6572 290a  f.__eq__(other).
-00017520: 0a20 2020 2064 6566 2061 735f 6469 6d28  .    def as_dim(
-00017530: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00017540: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
-00017550: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00017560: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00017570: 6c66 2e69 735f 7a65 726f 2829 3a0a 2020  lf.is_zero():.  
-00017580: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017590: 205f 6d61 6b65 5f63 6f6e 7374 616e 745f   _make_constant_
-000175a0: 7374 6174 6963 5f64 696d 2830 290a 2020  static_dim(0).  
-000175b0: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
-000175c0: 662e 7465 726d 7329 203d 3d20 313a 0a20  f.terms) == 1:. 
-000175d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000175e0: 6e20 7365 6c66 2e74 6572 6d73 5b30 5d2e  n self.terms[0].
-000175f0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
-00017600: 2061 6464 5f70 6172 7473 203d 205b 5d0a   add_parts = [].
-00017610: 2020 2020 2020 2020 6465 7363 5f70 6172          desc_par
-00017620: 7473 203d 205b 5d0a 2020 2020 2020 2020  ts = [].        
-00017630: 6469 6d20 3d20 300a 2020 2020 2020 2020  dim = 0.        
-00017640: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
-00017650: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00017660: 2020 2020 7320 3d20 7465 726d 2e61 735f      s = term.as_
-00017670: 6469 6d28 290a 2020 2020 2020 2020 2020  dim().          
-00017680: 2020 6164 645f 7061 7274 732e 6170 7065    add_parts.appe
-00017690: 6e64 2873 290a 2020 2020 2020 2020 2020  nd(s).          
-000176a0: 2020 6465 7363 5f70 6172 7473 2e61 7070    desc_parts.app
-000176b0: 656e 6428 5f67 6574 5f64 6573 6372 6970  end(_get_descrip
-000176c0: 7469 6f6e 2873 2929 0a20 2020 2020 2020  tion(s)).       
-000176d0: 2020 2020 2069 6620 6469 6d20 6973 206e       if dim is n
-000176e0: 6f74 204e 6f6e 6520 616e 6420 732e 6469  ot None and s.di
-000176f0: 6d65 6e73 696f 6e20 6973 206e 6f74 204e  mension is not N
-00017700: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00017710: 2020 2020 2064 696d 202b 3d20 732e 6469       dim += s.di
-00017720: 6d65 6e73 696f 6e0a 2020 2020 2020 2020  mension.        
-00017730: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00017740: 2020 2020 2020 2020 2020 6469 6d20 3d20            dim = 
-00017750: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00017760: 6c65 6e28 6164 645f 7061 7274 7329 203d  len(add_parts) =
-00017770: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00017780: 2072 6574 7572 6e20 6164 645f 7061 7274   return add_part
-00017790: 735b 305d 0a20 2020 2020 2020 2072 6574  s[0].        ret
-000177a0: 7572 6e20 5f64 2e44 696d 280a 2020 2020  urn _d.Dim(.    
-000177b0: 2020 2020 2020 2020 6b69 6e64 3d5f 6765          kind=_ge
-000177c0: 745f 6d65 7267 6564 5f64 696d 5f6b 696e  t_merged_dim_kin
-000177d0: 6428 6164 645f 7061 7274 7329 2c0a 2020  d(add_parts),.  
-000177e0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-000177f0: 7074 696f 6e3d 222b 222e 6a6f 696e 2864  ption="+".join(d
-00017800: 6573 635f 7061 7274 7329 2c0a 2020 2020  esc_parts),.    
-00017810: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
-00017820: 6e3d 6469 6d2c 0a20 2020 2020 2020 2020  n=dim,.         
-00017830: 2020 2064 6572 6976 6564 5f66 726f 6d5f     derived_from_
-00017840: 6f70 3d4f 7028 6b69 6e64 3d22 6164 6422  op=Op(kind="add"
-00017850: 2c20 696e 7075 7473 3d61 6464 5f70 6172  , inputs=add_par
-00017860: 7473 292c 0a20 2020 2020 2020 2020 2020  ts),.           
-00017870: 2064 6572 6976 6564 5f66 726f 6d5f 7461   derived_from_ta
-00017880: 673d 7365 6c66 2e72 6570 7265 7365 6e74  g=self.represent
-00017890: 6174 6976 655f 7461 6728 292c 0a20 2020  ative_tag(),.   
-000178a0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-000178b0: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
-000178c0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-000178d0: 4469 6d2e 5f4f 704c 696e 6561 7254 6572  Dim._OpLinearTer
-000178e0: 6d28 2572 2922 2025 2028 7365 6c66 2e74  m(%r)" % (self.t
-000178f0: 6572 6d73 2c29 0a0a 2020 2020 6465 6620  erms,)..    def 
-00017900: 6973 5f7a 6572 6f28 7365 6c66 293a 0a20  is_zero(self):. 
-00017910: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00017920: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00017930: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017940: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
-00017950: 656c 662e 7465 726d 730a 0a20 2020 2064  elf.terms..    d
-00017960: 6566 2065 7874 656e 645f 6164 645f 7375  ef extend_add_su
-00017970: 625f 2873 656c 662c 206f 7468 6572 2c20  b_(self, other, 
-00017980: 6b69 6e64 2c20 7269 6768 7429 3a0a 2020  kind, right):.  
-00017990: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000179a0: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
-000179b0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-000179c0: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
-000179d0: 2022 6164 6422 206f 7220 2273 7562 220a   "add" or "sub".
-000179e0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-000179f0: 6f6f 6c20 7269 6768 743a 206f 7220 6c65  ool right: or le
-00017a00: 6674 2e20 7269 6768 7420 6d65 616e 7320  ft. right means 
-00017a10: 7365 6c66 202b 206f 7468 6572 2c20 6c65  self + other, le
-00017a20: 6674 206d 6561 6e73 206f 7468 6572 202b  ft means other +
-00017a30: 2073 656c 660a 2020 2020 2020 2020 2222   self.        ""
-00017a40: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00017a50: 206b 696e 6420 696e 207b 2261 6464 222c   kind in {"add",
-00017a60: 2022 7375 6222 7d0a 2020 2020 2020 2020   "sub"}.        
-00017a70: 6f74 6865 7220 3d20 7365 6c66 2e5f 6d61  other = self._ma
-00017a80: 6b65 5f64 696d 286f 7468 6572 2c20 6b69  ke_dim(other, ki
-00017a90: 6e64 3d6b 696e 6429 0a20 2020 2020 2020  nd=kind).       
-00017aa0: 2069 6620 6f74 6865 722e 6973 5f63 6f6e   if other.is_con
-00017ab0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-00017ac0: 2829 2061 6e64 206f 7468 6572 2e64 696d  () and other.dim
-00017ad0: 656e 7369 6f6e 203d 3d20 303a 0a20 2020  ension == 0:.   
-00017ae0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00017af0: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-00017b00: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00017b10: 2061 6e64 206f 7468 6572 2e64 6572 6976   and other.deriv
-00017b20: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
-00017b30: 3d3d 2022 6164 6422 3a0a 2020 2020 2020  == "add":.      
-00017b40: 2020 2020 2020 666f 7220 6f74 6865 725f        for other_
-00017b50: 2069 6e20 6f74 6865 722e 6465 7269 7665   in other.derive
-00017b60: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
-00017b70: 2069 6620 7269 6768 7420 656c 7365 2072   if right else r
-00017b80: 6576 6572 7365 6428 6f74 6865 722e 6465  eversed(other.de
-00017b90: 7269 7665 645f 6672 6f6d 5f6f 702e 696e  rived_from_op.in
-00017ba0: 7075 7473 293a 0a20 2020 2020 2020 2020  puts):.         
-00017bb0: 2020 2020 2020 2073 656c 662e 6578 7465         self.exte
-00017bc0: 6e64 5f61 6464 5f73 7562 5f28 6f74 6865  nd_add_sub_(othe
-00017bd0: 725f 2c20 6b69 6e64 3d6b 696e 642c 2072  r_, kind=kind, r
-00017be0: 6967 6874 3d72 6967 6874 290a 2020 2020  ight=right).    
-00017bf0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00017c00: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-00017c10: 704d 756c 7454 6572 6d2e 6672 6f6d 5f64  pMultTerm.from_d
-00017c20: 696d 286f 7468 6572 290a 2020 2020 2020  im(other).      
-00017c30: 2020 6e65 675f 7465 726d 203d 2074 6572    neg_term = ter
-00017c40: 6d2e 6e65 6761 7469 7665 2829 0a20 2020  m.negative().   
-00017c50: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
-00017c60: 2273 7562 223a 0a20 2020 2020 2020 2020  "sub":.         
-00017c70: 2020 2074 6572 6d2c 206e 6567 5f74 6572     term, neg_ter
-00017c80: 6d20 3d20 6e65 675f 7465 726d 2c20 7465  m = neg_term, te
-00017c90: 726d 0a20 2020 2020 2020 206d 6f73 745f  rm.        most_
-00017ca0: 7265 6365 6e74 5f74 6572 6d20 3d20 7365  recent_term = se
-00017cb0: 6c66 2e74 6572 6d73 5b2d 3120 6966 2072  lf.terms[-1 if r
-00017cc0: 6967 6874 2065 6c73 6520 305d 2069 6620  ight else 0] if 
-00017cd0: 7365 6c66 2e74 6572 6d73 2065 6c73 6520  self.terms else 
-00017ce0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00017cf0: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
-00017d00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00017d10: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-00017d20: 6d20 3d3d 206e 6567 5f74 6572 6d3a 0a20  m == neg_term:. 
-00017d30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017d40: 656c 662e 7465 726d 732e 706f 7028 2d31  elf.terms.pop(-1
-00017d50: 2069 6620 7269 6768 7420 656c 7365 2030   if right else 0
-00017d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017d70: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00017d80: 2020 2020 2069 6620 6d6f 7374 5f72 6563       if most_rec
-00017d90: 656e 745f 7465 726d 2e69 735f 636f 6e73  ent_term.is_cons
-00017da0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00017db0: 2920 616e 6420 7465 726d 2e69 735f 636f  ) and term.is_co
-00017dc0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
-00017dd0: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
-00017de0: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
-00017df0: 2d31 2069 6620 7269 6768 7420 656c 7365  -1 if right else
-00017e00: 2030 5d20 3d20 5f4f 704d 756c 7454 6572   0] = _OpMultTer
-00017e10: 6d2e 6672 6f6d 5f64 696d 280a 2020 2020  m.from_dim(.    
-00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e30: 5f6d 616b 655f 636f 6e73 7461 6e74 5f73  _make_constant_s
-00017e40: 7461 7469 635f 6469 6d28 6d6f 7374 5f72  tatic_dim(most_r
-00017e50: 6563 656e 745f 7465 726d 2e64 696d 656e  ecent_term.dimen
-00017e60: 7369 6f6e 202b 2074 6572 6d2e 6469 6d65  sion + term.dime
-00017e70: 6e73 696f 6e2c 206b 696e 643d 6f74 6865  nsion, kind=othe
-00017e80: 722e 6b69 6e64 290a 2020 2020 2020 2020  r.kind).        
-00017e90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017ea0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017eb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00017ec0: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
-00017ed0: 2e74 6572 6d73 2061 6e64 2074 6572 6d2e  .terms and term.
-00017ee0: 7465 726d 7320 616e 6420 6d6f 7374 5f72  terms and most_r
-00017ef0: 6563 656e 745f 7465 726d 2e74 6572 6d73  ecent_term.terms
-00017f00: 5b2d 315d 203d 3d20 7465 726d 2e74 6572  [-1] == term.ter
-00017f10: 6d73 5b2d 315d 3a0a 2020 2020 2020 2020  ms[-1]:.        
-00017f20: 2020 2020 2020 2020 2320 4d65 7267 6520          # Merge 
-00017f30: 7465 726d 730a 2020 2020 2020 2020 2020  terms.          
-00017f40: 2020 2020 2020 6120 3d20 5f4f 704d 756c        a = _OpMul
-00017f50: 7454 6572 6d2e 6672 6f6d 5f64 696d 5f66  tTerm.from_dim_f
-00017f60: 6163 746f 7273 286d 6f73 745f 7265 6365  actors(most_rece
-00017f70: 6e74 5f74 6572 6d2e 7465 726d 735b 3a2d  nt_term.terms[:-
-00017f80: 315d 292e 6173 5f64 696d 2829 0a20 2020  1]).as_dim().   
-00017f90: 2020 2020 2020 2020 2020 2020 2062 203d               b =
-00017fa0: 205f 4f70 4d75 6c74 5465 726d 2e66 726f   _OpMultTerm.fro
-00017fb0: 6d5f 6469 6d5f 6661 6374 6f72 7328 7465  m_dim_factors(te
-00017fc0: 726d 2e74 6572 6d73 5b3a 2d31 5d29 2e61  rm.terms[:-1]).a
-00017fd0: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
-00017fe0: 2020 2020 2020 2020 7265 7320 3d20 5f4f          res = _O
-00017ff0: 704d 756c 7454 6572 6d2e 6672 6f6d 5f64  pMultTerm.from_d
-00018000: 696d 2828 6120 2b20 6229 2069 6620 7269  im((a + b) if ri
-00018010: 6768 7420 656c 7365 2028 6220 2b20 6129  ght else (b + a)
-00018020: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00018030: 2020 7265 732e 6578 7465 6e64 5f6d 756c    res.extend_mul
-00018040: 5f64 6976 5f28 7465 726d 2e74 6572 6d73  _div_(term.terms
-00018050: 5b2d 315d 2c20 6b69 6e64 3d22 6d75 6c22  [-1], kind="mul"
-00018060: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
-00018070: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018080: 6c66 2e74 6572 6d73 5b2d 3120 6966 2072  lf.terms[-1 if r
-00018090: 6967 6874 2065 6c73 6520 305d 203d 2072  ight else 0] = r
-000180a0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-000180b0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000180c0: 2020 6966 2072 6967 6874 3a0a 2020 2020    if right:.    
-000180d0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-000180e0: 6d73 2e61 7070 656e 6428 7465 726d 290a  ms.append(term).
-000180f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00018100: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00018110: 6572 6d73 2e69 6e73 6572 7428 302c 2074  erms.insert(0, t
-00018120: 6572 6d29 0a0a 2020 2020 6465 6620 6578  erm)..    def ex
-00018130: 7465 6e64 5f6d 756c 5f64 6976 5f28 7365  tend_mul_div_(se
-00018140: 6c66 2c20 6f74 6865 722c 206b 696e 642c  lf, other, kind,
-00018150: 2072 6967 6874 293a 0a20 2020 2020 2020   right):.       
-00018160: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00018170: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00018180: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00018190: 6d20 7374 7220 6b69 6e64 3a20 226d 756c  m str kind: "mul
-000181a0: 2220 6f72 2022 6365 696c 6469 7622 0a20  " or "ceildiv". 
-000181b0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-000181c0: 6f6c 2072 6967 6874 3a20 6f72 206c 6566  ol right: or lef
-000181d0: 742e 2072 6967 6874 206d 6561 6e73 2073  t. right means s
-000181e0: 656c 6620 2a20 6f74 6865 722c 206c 6566  elf * other, lef
-000181f0: 7420 6d65 616e 7320 6f74 6865 7220 2a20  t means other * 
-00018200: 7365 6c66 0a20 2020 2020 2020 2022 2222  self.        """
-00018210: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00018220: 6b69 6e64 2069 6e20 7b22 6d75 6c22 2c20  kind in {"mul", 
-00018230: 2266 6c6f 6f72 6469 7622 2c20 2274 7275  "floordiv", "tru
-00018240: 6564 6976 222c 2022 6365 696c 6469 7622  ediv", "ceildiv"
-00018250: 7d0a 2020 2020 2020 2020 6f74 6865 7220  }.        other 
-00018260: 3d20 7365 6c66 2e5f 6d61 6b65 5f64 696d  = self._make_dim
-00018270: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
-00018280: 6429 0a20 2020 2020 2020 2069 6620 6b69  d).        if ki
-00018290: 6e64 203d 3d20 226d 756c 2220 616e 6420  nd == "mul" and 
-000182a0: 7269 6768 743a 0a20 2020 2020 2020 2020  right:.         
-000182b0: 2020 2069 6620 6e6f 7420 616c 6c28 7465     if not all(te
-000182c0: 726d 2e63 616e 5f73 696d 706c 6966 7928  rm.can_simplify(
-000182d0: 6f74 6865 722c 206b 696e 643d 6b69 6e64  other, kind=kind
-000182e0: 2c20 7269 6768 743d 7269 6768 7429 2066  , right=right) f
-000182f0: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
-00018300: 7465 726d 7329 3a0a 2020 2020 2020 2020  terms):.        
-00018310: 2020 2020 2020 2020 2320 446f 2069 7420          # Do it 
-00018320: 7468 6520 6f74 6865 7220 7761 7920 6172  the other way ar
-00018330: 6f75 6e64 0a20 2020 2020 2020 2020 2020  ound.           
-00018340: 2020 2020 2073 656c 662e 7465 726d 732c       self.terms,
-00018350: 206f 7468 6572 203d 205f 4f70 4c69 6e65   other = _OpLine
-00018360: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
-00018370: 6f74 6865 7229 2e74 6572 6d73 2c20 7365  other).terms, se
-00018380: 6c66 2e61 735f 6469 6d28 290a 2020 2020  lf.as_dim().    
-00018390: 2020 2020 2020 2020 2020 2020 7269 6768              righ
-000183a0: 7420 3d20 4661 6c73 650a 2020 2020 2020  t = False.      
-000183b0: 2020 6966 206f 7468 6572 2e69 735f 636f    if other.is_co
-000183c0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
-000183d0: 6d28 2920 616e 6420 6f74 6865 722e 6469  m() and other.di
-000183e0: 6d65 6e73 696f 6e20 3d3d 2031 3a0a 2020  mension == 1:.  
-000183f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00018400: 0a20 2020 2020 2020 2069 6620 6b69 6e64  .        if kind
-00018410: 2e65 6e64 7377 6974 6828 2264 6976 2229  .endswith("div")
-00018420: 2061 6e64 206c 656e 2873 656c 662e 7465   and len(self.te
-00018430: 726d 7329 203e 3d20 323a 0a20 2020 2020  rms) >= 2:.     
-00018440: 2020 2020 2020 2069 6620 616e 7928 6e6f         if any(no
-00018450: 7420 7465 726d 2e64 6976 6973 6962 6c65  t term.divisible
-00018460: 286f 7468 6572 2c20 7269 6768 743d 7269  (other, right=ri
-00018470: 6768 7429 2066 6f72 2074 6572 6d20 696e  ght) for term in
-00018480: 2073 656c 662e 7465 726d 7329 3a0a 2020   self.terms):.  
-00018490: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000184a0: 6c66 2e74 6572 6d73 203d 205b 0a20 2020  lf.terms = [.   
-000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184c0: 205f 4f70 4d75 6c74 5465 726d 2e66 726f   _OpMultTerm.fro
-000184d0: 6d5f 6469 6d28 5f4f 704d 756c 7454 6572  m_dim(_OpMultTer
-000184e0: 6d2e 6e65 775f 6469 765f 6469 6d28 7365  m.new_div_dim(se
-000184f0: 6c66 2e61 735f 6469 6d28 292c 206f 7468  lf.as_dim(), oth
-00018500: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
-00018510: 6967 6874 3d72 6967 6874 2929 0a20 2020  ight=right)).   
-00018520: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-00018530: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018540: 6574 7572 6e0a 2020 2020 2020 2020 666f  eturn.        fo
-00018550: 7220 7465 726d 2069 6e20 7365 6c66 2e74  r term in self.t
-00018560: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
-00018570: 2020 7465 726d 2e65 7874 656e 645f 6d75    term.extend_mu
-00018580: 6c5f 6469 765f 286f 7468 6572 2c20 6b69  l_div_(other, ki
-00018590: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
-000185a0: 6967 6874 290a 0a20 2020 2064 6566 205f  ight)..    def _
-000185b0: 6d61 6b65 5f64 696d 2873 656c 662c 206f  make_dim(self, o
-000185c0: 7468 6572 2c20 6b69 6e64 293a 0a20 2020  ther, kind):.   
-000185d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000185e0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-000185f0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00018600: 7061 7261 6d20 7374 7220 6b69 6e64 3a0a  param str kind:.
-00018610: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00018620: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00018630: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00018640: 7461 6e63 6528 6f74 6865 722c 2069 6e74  tance(other, int
-00018650: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
-00018660: 6173 655f 7461 6720 3d20 7365 6c66 2e72  ase_tag = self.r
-00018670: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
-00018680: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
-00018690: 7265 7475 726e 205f 6d61 6b65 5f63 6f6e  return _make_con
-000186a0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-000186b0: 286f 7468 6572 2c20 6b69 6e64 3d62 6173  (other, kind=bas
-000186c0: 655f 7461 672e 6b69 6e64 2069 6620 6261  e_tag.kind if ba
-000186d0: 7365 5f74 6167 2065 6c73 6520 4e6f 6e65  se_tag else None
-000186e0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
-000186f0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-00018700: 205f 642e 4469 6d29 3a0a 2020 2020 2020   _d.Dim):.      
-00018710: 2020 2020 2020 7265 7475 726e 206f 7468        return oth
-00018720: 6572 2e67 6574 5f73 616d 655f 6261 7365  er.get_same_base
-00018730: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-00018740: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00018750: 7365 2054 7970 6545 7272 6f72 2822 2573  se TypeError("%s
-00018760: 2025 7320 2573 2069 6e76 616c 6964 2066   %s %s invalid f
-00018770: 6f72 2074 7970 6520 2573 2220 2520 2873  or type %s" % (s
-00018780: 656c 662c 206b 696e 642c 206f 7468 6572  elf, kind, other
-00018790: 2c20 7479 7065 286f 7468 6572 2929 290a  , type(other))).
-000187a0: 0a20 2020 2064 6566 2072 6570 7265 7365  .    def represe
-000187b0: 6e74 6174 6976 655f 7461 6728 7365 6c66  ntative_tag(self
-000187c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000187d0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-000187e0: 696d 7c4e 6f6e 650a 2020 2020 2020 2020  im|None.        
-000187f0: 2222 220a 2020 2020 2020 2020 2320 4669  """.        # Fi
-00018800: 7273 7420 6669 6e64 2061 6e79 2064 796e  rst find any dyn
-00018810: 616d 6963 2e0a 2020 2020 2020 2020 666f  amic..        fo
-00018820: 7220 7465 726d 2069 6e20 7365 6c66 2e74  r term in self.t
-00018830: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
-00018840: 2020 666f 7220 7465 726d 5f20 696e 2074    for term_ in t
-00018850: 6572 6d2e 7465 726d 733a 0a20 2020 2020  erm.terms:.     
-00018860: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00018870: 726d 5f2e 6973 5f64 796e 616d 6963 2829  rm_.is_dynamic()
-00018880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00018890: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-000188a0: 6d5f 0a20 2020 2020 2020 2023 204e 6f77  m_.        # Now
-000188b0: 2066 696e 6420 6e6f 6e2d 756e 7370 6563   find non-unspec
-000188c0: 6966 6965 642e 0a20 2020 2020 2020 2066  ified..        f
-000188d0: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
-000188e0: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-000188f0: 2020 2066 6f72 2074 6572 6d5f 2069 6e20     for term_ in 
-00018900: 7465 726d 2e74 6572 6d73 3a0a 2020 2020  term.terms:.    
-00018910: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00018920: 6572 6d5f 2e6b 696e 6420 213d 2044 696d  erm_.kind != Dim
-00018930: 5479 7065 732e 556e 7370 6563 6966 6965  Types.Unspecifie
-00018940: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-00018950: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-00018960: 726d 5f0a 2020 2020 2020 2020 2320 4e6f  rm_.        # No
-00018970: 7720 6669 6e64 2061 6e79 2e0a 2020 2020  w find any..    
-00018980: 2020 2020 666f 7220 7465 726d 2069 6e20      for term in 
-00018990: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
-000189a0: 2020 2020 2020 2020 666f 7220 7465 726d          for term
-000189b0: 5f20 696e 2074 6572 6d2e 7465 726d 733a  _ in term.terms:
-000189c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189d0: 2072 6574 7572 6e20 7465 726d 5f0a 2020   return term_.  
-000189e0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000189f0: 650a 0a0a 6465 6620 5f67 6574 5f6d 6572  e...def _get_mer
-00018a00: 6765 645f 6469 6d5f 6b69 6e64 2864 696d  ged_dim_kind(dim
-00018a10: 5f74 6167 7329 3a0a 2020 2020 2222 220a  _tags):.    """.
-00018a20: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
-00018a30: 4469 6d5d 7c74 7570 6c65 5b44 696d 5d20  Dim]|tuple[Dim] 
-00018a40: 6469 6d5f 7461 6773 3a0a 2020 2020 3a72  dim_tags:.    :r
-00018a50: 6574 7572 6e3a 2064 696d 206b 696e 640a  eturn: dim kind.
-00018a60: 2020 2020 3a72 7479 7065 3a20 456e 7469      :rtype: Enti
-00018a70: 7479 0a20 2020 2022 2222 0a20 2020 2069  ty.    """.    i
-00018a80: 6620 616e 7928 7461 672e 6973 5f62 6174  f any(tag.is_bat
-00018a90: 6368 5f64 696d 2829 2066 6f72 2074 6167  ch_dim() for tag
-00018aa0: 2069 6e20 6469 6d5f 7461 6773 293a 0a20   in dim_tags):. 
-00018ab0: 2020 2020 2020 2072 6574 7572 6e20 4469         return Di
-00018ac0: 6d54 7970 6573 2e42 6174 6368 0a20 2020  mTypes.Batch.   
-00018ad0: 2065 6c69 6620 616e 7928 7461 672e 6973   elif any(tag.is
-00018ae0: 5f66 6561 7475 7265 5f64 696d 2829 2066  _feature_dim() f
-00018af0: 6f72 2074 6167 2069 6e20 6469 6d5f 7461  or tag in dim_ta
-00018b00: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
-00018b10: 7572 6e20 4469 6d54 7970 6573 2e46 6561  urn DimTypes.Fea
-00018b20: 7475 7265 0a20 2020 2065 6c73 653a 0a20  ture.    else:. 
-00018b30: 2020 2020 2020 2072 6574 7572 6e20 4469         return Di
-00018b40: 6d54 7970 6573 2e53 7061 7469 616c 0a0a  mTypes.Spatial..
-00018b50: 0a64 6566 2064 696d 5f63 6d70 5f76 616c  .def dim_cmp_val
-00018b60: 7565 286f 626a 293a 0a20 2020 2022 2222  ue(obj):.    """
-00018b70: 0a20 2020 203a 7061 7261 6d20 4469 6d7c  .    :param Dim|
-00018b80: 5f4d 6172 6b65 6444 696d 206f 626a 3a0a  _MarkedDim obj:.
-00018b90: 2020 2020 3a72 6574 7572 6e3a 2061 6e79      :return: any
-00018ba0: 7468 696e 6720 7768 6963 6820 6361 6e20  thing which can 
-00018bb0: 6265 2063 6f6d 7061 7265 640a 2020 2020  be compared.    
-00018bc0: 2222 220a 2020 2020 2320 4d61 6b65 2044  """.    # Make D
-00018bd0: 696d 2061 6e64 205f 4d61 726b 6564 4469  im and _MarkedDi
-00018be0: 6d20 636f 6d70 6172 6162 6c65 2074 6f20  m comparable to 
-00018bf0: 6561 6368 206f 7468 6572 2e0a 2020 2020  each other..    
-00018c00: 2320 4e6f 7465 2074 6861 7420 7468 6520  # Note that the 
-00018c10: 6f72 6465 7220 6973 2072 6561 6c6c 7920  order is really 
-00018c20: 6172 6269 7472 6172 7920 616e 6420 646f  arbitrary and do
-00018c30: 6573 206e 6f74 206d 6174 7465 722e 0a20  es not matter.. 
-00018c40: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00018c50: 286f 626a 2c20 5f64 2e44 696d 293a 0a20  (obj, _d.Dim):. 
-00018c60: 2020 2020 2020 206f 626a 203d 206f 626a         obj = obj
-00018c70: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
-00018c80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018c90: 280a 2020 2020 2020 2020 2020 2020 2222  (.            ""
-00018ca0: 2c0a 2020 2020 2020 2020 2020 2020 6f62  ,.            ob
-00018cb0: 6a2e 6465 7363 7269 7074 696f 6e2c 0a20  j.description,. 
-00018cc0: 2020 2020 2020 2020 2020 206f 626a 2e6b             obj.k
-00018cd0: 696e 642c 0a20 2020 2020 2020 2020 2020  ind,.           
-00018ce0: 206f 626a 2e64 696d 656e 7369 6f6e 2c0a   obj.dimension,.
-00018cf0: 2020 2020 2020 2020 2020 2020 6f62 6a2e              obj.
-00018d00: 6479 6e5f 7369 7a65 5f65 7874 2e64 696d  dyn_size_ext.dim
-00018d10: 7320 6966 206f 626a 2e64 796e 5f73 697a  s if obj.dyn_siz
-00018d20: 655f 6578 7420 6973 206e 6f74 204e 6f6e  e_ext is not Non
-00018d30: 6520 656c 7365 204e 6f6e 652c 0a20 2020  e else None,.   
-00018d40: 2020 2020 2029 0a20 2020 2069 6620 6973       ).    if is
-00018d50: 696e 7374 616e 6365 286f 626a 2c20 5f6d  instance(obj, _m
-00018d60: 2e4d 6172 6b65 6444 696d 293a 0a20 2020  .MarkedDim):.   
-00018d70: 2020 2020 2072 6574 7572 6e20 6f62 6a2e       return obj.
-00018d80: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-00018d90: 5f5f 2c20 6f62 6a2e 7461 670a 2020 2020  __, obj.tag.    
-00018da0: 7265 7475 726e 206f 626a 0a              return obj.
+00016070: 7365 6c66 2e74 6572 6d73 2e70 6f70 2869  self.terms.pop(i
+00016080: 6478 290a 2020 2020 2020 2020 2020 2020  dx).            
+00016090: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000160a0: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
+000160b0: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+000160c0: 735b 6964 785d 203d 205f 6d61 6b65 5f63  s[idx] = _make_c
+000160d0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000160e0: 696d 2874 6572 6d2e 6469 6d65 6e73 696f  im(term.dimensio
+000160f0: 6e20 2a20 6f74 6865 722e 6469 6d65 6e73  n * other.dimens
+00016100: 696f 6e2c 206b 696e 643d 7465 726d 2e6b  ion, kind=term.k
+00016110: 696e 6429 0a20 2020 2020 2020 2020 2020  ind).           
+00016120: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016140: 6966 206b 696e 642e 656e 6473 7769 7468  if kind.endswith
+00016150: 2822 6469 7622 2920 616e 6420 7465 726d  ("div") and term
+00016160: 2e64 696d 656e 7369 6f6e 2025 206f 7468  .dimension % oth
+00016170: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
+00016180: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00016190: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+000161a0: 735b 6964 785d 203d 205f 6d61 6b65 5f63  s[idx] = _make_c
+000161b0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000161c0: 696d 2874 6572 6d2e 6469 6d65 6e73 696f  im(term.dimensio
+000161d0: 6e20 2f2f 206f 7468 6572 2e64 696d 656e  n // other.dimen
+000161e0: 7369 6f6e 2c20 6b69 6e64 3d74 6572 6d2e  sion, kind=term.
+000161f0: 6b69 6e64 290a 2020 2020 2020 2020 2020  kind).          
+00016200: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00016210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016220: 2023 2046 616c 6c62 6163 6b20 7769 7468   # Fallback with
+00016230: 2067 656e 6572 6963 2068 616e 646c 696e   generic handlin
+00016240: 672e 0a20 2020 2020 2020 2020 2020 206f  g..            o
+00016250: 705f 6b69 6e64 203d 206b 696e 6420 2b20  p_kind = kind + 
+00016260: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
+00016270: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
+00016280: 6674 2229 0a20 2020 2020 2020 2020 2020  ft").           
+00016290: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
+000162a0: 6828 2264 6976 2229 2061 6e64 2074 6572  h("div") and ter
+000162b0: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
+000162c0: 7020 616e 6420 7465 726d 2e64 6572 6976  p and term.deriv
+000162d0: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
+000162e0: 3d3d 206f 705f 6b69 6e64 3a0a 2020 2020  == op_kind:.    
+000162f0: 2020 2020 2020 2020 2020 2020 6e75 6d65              nume
+00016300: 7261 746f 7220 3d20 7465 726d 2e64 6572  rator = term.der
+00016310: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00016320: 7574 735b 305d 0a20 2020 2020 2020 2020  uts[0].         
+00016330: 2020 2020 2020 2064 656e 6f6d 696e 6174         denominat
+00016340: 6f72 203d 2074 6572 6d2e 6465 7269 7665  or = term.derive
+00016350: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+00016360: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
+00016370: 2020 2020 7365 6c66 2e74 6572 6d73 5b69      self.terms[i
+00016380: 6478 5d20 3d20 5f4f 704d 756c 7454 6572  dx] = _OpMultTer
+00016390: 6d2e 6e65 775f 6469 765f 6469 6d28 6e75  m.new_div_dim(nu
+000163a0: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
+000163b0: 6174 6f72 202a 206f 7468 6572 2c20 6b69  ator * other, ki
+000163c0: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+000163d0: 6967 6874 290a 2020 2020 2020 2020 2020  ight).          
+000163e0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000163f0: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
+00016400: 7377 6974 6828 2264 6976 2229 3a0a 2020  swith("div"):.  
+00016410: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00016420: 6572 6d73 203d 205b 5f4f 704d 756c 7454  erms = [_OpMultT
+00016430: 6572 6d2e 6e65 775f 6469 765f 6469 6d28  erm.new_div_dim(
+00016440: 7365 6c66 2e61 735f 6469 6d28 292c 206f  self.as_dim(), o
+00016450: 7468 6572 2c20 6b69 6e64 3d6b 696e 642c  ther, kind=kind,
+00016460: 2072 6967 6874 3d72 6967 6874 295d 0a20   right=right)]. 
+00016470: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016480: 6e0a 2020 2020 2020 2020 6966 206b 696e  n.        if kin
+00016490: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
+000164a0: 2020 2020 2020 2020 6966 2072 6967 6874          if right
+000164b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000164c0: 2020 7365 6c66 2e74 6572 6d73 2e61 7070    self.terms.app
+000164d0: 656e 6428 6f74 6865 7229 0a20 2020 2020  end(other).     
+000164e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000164f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016500: 662e 7465 726d 732e 696e 7365 7274 2830  f.terms.insert(0
+00016510: 2c20 6f74 6865 7229 0a20 2020 2020 2020  , other).       
+00016520: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00016530: 2020 2020 6173 7365 7274 2046 616c 7365      assert False
+00016540: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00016550: 6f64 0a20 2020 2064 6566 206e 6577 5f64  od.    def new_d
+00016560: 6976 5f64 696d 2863 6c73 2c20 6e75 6d65  iv_dim(cls, nume
+00016570: 7261 746f 722c 2064 656e 6f6d 696e 6174  rator, denominat
+00016580: 6f72 2c20 6b69 6e64 2c20 7269 6768 7429  or, kind, right)
+00016590: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000165a0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+000165b0: 206e 756d 6572 6174 6f72 3a0a 2020 2020   numerator:.    
+000165c0: 2020 2020 3a70 6172 616d 2044 696d 2064      :param Dim d
+000165d0: 656e 6f6d 696e 6174 6f72 3a0a 2020 2020  enominator:.    
+000165e0: 2020 2020 3a70 6172 616d 2073 7472 206b      :param str k
+000165f0: 696e 643a 2022 666c 6f6f 7264 6976 2220  ind: "floordiv" 
+00016600: 6f72 2022 6365 696c 6469 7622 206f 7220  or "ceildiv" or 
+00016610: 2274 7275 6564 6976 220a 2020 2020 2020  "truediv".      
+00016620: 2020 3a70 6172 616d 2062 6f6f 6c20 7269    :param bool ri
+00016630: 6768 743a 0a20 2020 2020 2020 203a 7274  ght:.        :rt
+00016640: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00016650: 2022 2222 0a20 2020 2020 2020 2064 696d   """.        dim
+00016660: 5f76 616c 7565 203d 204e 6f6e 650a 2020  _value = None.  
+00016670: 2020 2020 2020 6120 3d20 6e75 6d65 7261        a = numera
+00016680: 746f 722e 6469 6d65 6e73 696f 6e0a 2020  tor.dimension.  
+00016690: 2020 2020 2020 6220 3d20 6465 6e6f 6d69        b = denomi
+000166a0: 6e61 746f 722e 6469 6d65 6e73 696f 6e0a  nator.dimension.
+000166b0: 2020 2020 2020 2020 6966 2061 2069 7320          if a is 
+000166c0: 6e6f 7420 4e6f 6e65 2061 6e64 2062 2069  not None and b i
+000166d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000166e0: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
+000166f0: 3d3d 2022 666c 6f6f 7264 6976 223a 0a20  == "floordiv":. 
+00016700: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00016710: 696d 5f76 616c 7565 203d 2061 202f 2f20  im_value = a // 
+00016720: 620a 2020 2020 2020 2020 2020 2020 656c  b.            el
+00016730: 6966 206b 696e 6420 3d3d 2022 6365 696c  if kind == "ceil
+00016740: 6469 7622 3a0a 2020 2020 2020 2020 2020  div":.          
+00016750: 2020 2020 2020 6469 6d5f 7661 6c75 6520        dim_value 
+00016760: 3d20 2d28 2d61 202f 2f20 6229 0a20 2020  = -(-a // b).   
+00016770: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016780: 6120 2520 6220 3d3d 2030 2061 6e64 2072  a % b == 0 and r
+00016790: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
+000167a0: 2020 2020 2020 2020 2020 6b69 6e64 203d            kind =
+000167b0: 2022 666c 6f6f 7264 6976 2220 2023 2066   "floordiv"  # f
+000167c0: 6f72 206e 6963 6572 2064 6573 6372 6970  or nicer descrip
+000167d0: 7469 6f6e 2c20 616e 6420 646f 6573 206e  tion, and does n
+000167e0: 6f74 206d 6174 7465 720a 2020 2020 2020  ot matter.      
+000167f0: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
+00016800: 3d3d 2022 7472 7565 6469 7622 3a0a 2020  == "truediv":.  
+00016810: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016820: 2061 2025 2062 2021 3d20 303a 0a20 2020   a % b != 0:.   
+00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016840: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00016850: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00016860: 2020 2020 2020 2020 2020 2022 2573 2074             "%s t
+00016870: 7275 6564 6976 2025 7320 6f6e 6c79 2061  ruediv %s only a
+00016880: 6c6c 6f77 6564 2069 6620 7468 6520 7265  llowed if the re
+00016890: 7375 6c74 2069 7320 616e 2069 6e74 6567  sult is an integ
+000168a0: 6572 2220 2520 286e 756d 6572 6174 6f72  er" % (numerator
+000168b0: 2c20 6465 6e6f 6d69 6e61 746f 7229 0a20  , denominator). 
+000168c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000168e0: 2020 2020 2064 696d 5f76 616c 7565 203d       dim_value =
+000168f0: 2061 202f 2f20 620a 2020 2020 2020 2020   a // b.        
+00016900: 2020 2020 2020 2020 6966 2072 6967 6874          if right
+00016910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016920: 2020 2020 2020 6b69 6e64 203d 2022 666c        kind = "fl
+00016930: 6f6f 7264 6976 2220 2023 2066 6f72 206e  oordiv"  # for n
+00016940: 6963 6572 2064 6573 6372 6970 7469 6f6e  icer description
+00016950: 2c20 616e 6420 646f 6573 206e 6f74 206d  , and does not m
+00016960: 6174 7465 720a 2020 2020 2020 2020 2020  atter.          
+00016970: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00016980: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00016990: 6c75 6545 7272 6f72 2822 696e 7661 6c69  lueError("invali
+000169a0: 6420 6b69 6e64 2025 7222 2025 2028 6b69  d kind %r" % (ki
+000169b0: 6e64 2c29 290a 2020 2020 2020 2020 6966  nd,)).        if
+000169c0: 206b 696e 6420 3d3d 2022 666c 6f6f 7264   kind == "floord
+000169d0: 6976 2220 616e 6420 7269 6768 743a 0a20  iv" and right:. 
+000169e0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+000169f0: 6970 7469 6f6e 203d 2022 2573 2f2f 2573  iption = "%s//%s
+00016a00: 2220 2520 285f 6765 745f 6465 7363 7269  " % (_get_descri
+00016a10: 7074 696f 6e28 6e75 6d65 7261 746f 7229  ption(numerator)
+00016a20: 2c20 5f67 6574 5f64 6573 6372 6970 7469  , _get_descripti
+00016a30: 6f6e 2864 656e 6f6d 696e 6174 6f72 2929  on(denominator))
+00016a40: 0a20 2020 2020 2020 2065 6c69 6620 6b69  .        elif ki
+00016a50: 6e64 203d 3d20 2263 6569 6c64 6976 2220  nd == "ceildiv" 
+00016a60: 616e 6420 7269 6768 743a 0a20 2020 2020  and right:.     
+00016a70: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00016a80: 6f6e 203d 2022 e28c 8825 732f 2573 e28c  on = "...%s/%s..
+00016a90: 8922 2025 2028 5f67 6574 5f64 6573 6372  ." % (_get_descr
+00016aa0: 6970 7469 6f6e 286e 756d 6572 6174 6f72  iption(numerator
+00016ab0: 292c 205f 6765 745f 6465 7363 7269 7074  ), _get_descript
+00016ac0: 696f 6e28 6465 6e6f 6d69 6e61 746f 7229  ion(denominator)
+00016ad0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00016ae0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00016af0: 7269 7074 696f 6e20 3d20 2225 735f 2573  ription = "%s_%s
+00016b00: 2825 732c 2025 7329 2220 2520 280a 2020  (%s, %s)" % (.  
+00016b10: 2020 2020 2020 2020 2020 2020 2020 6b69                ki
+00016b20: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
+00016b30: 2020 2020 2272 6967 6874 2220 6966 2072      "right" if r
+00016b40: 6967 6874 2065 6c73 6520 226c 6566 7422  ight else "left"
+00016b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016b60: 2020 5f67 6574 5f64 6573 6372 6970 7469    _get_descripti
+00016b70: 6f6e 286e 756d 6572 6174 6f72 2c20 6272  on(numerator, br
+00016b80: 6163 6b65 7473 3d46 616c 7365 292c 0a20  ackets=False),. 
+00016b90: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00016ba0: 6765 745f 6465 7363 7269 7074 696f 6e28  get_description(
+00016bb0: 6465 6e6f 6d69 6e61 746f 722c 2062 7261  denominator, bra
+00016bc0: 636b 6574 733d 4661 6c73 6529 2c0a 2020  ckets=False),.  
+00016bd0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00016be0: 2020 2020 6f70 5f6b 696e 6420 3d20 6b69      op_kind = ki
+00016bf0: 6e64 0a20 2020 2020 2020 2069 6620 6120  nd.        if a 
+00016c00: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00016c10: 6220 6973 206e 6f74 204e 6f6e 6520 616e  b is not None an
+00016c20: 6420 6120 2520 6220 3d3d 2030 3a0a 2020  d a % b == 0:.  
+00016c30: 2020 2020 2020 2020 2020 6f70 5f6b 696e            op_kin
+00016c40: 6420 3d20 2274 7275 6564 6976 2220 2023  d = "truediv"  #
+00016c50: 206d 616b 6573 2073 6f6d 6520 6f74 6865   makes some othe
+00016c60: 7220 6368 6563 6b73 2073 696d 706c 6572  r checks simpler
+00016c70: 0a20 2020 2020 2020 206f 705f 6b69 6e64  .        op_kind
+00016c80: 202b 3d20 225f 2220 2b20 2822 7269 6768   += "_" + ("righ
+00016c90: 7422 2069 6620 7269 6768 7420 656c 7365  t" if right else
+00016ca0: 2022 6c65 6674 2229 0a20 2020 2020 2020   "left").       
+00016cb0: 2072 6574 7572 6e20 5f64 2e44 696d 280a   return _d.Dim(.
+00016cc0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00016cd0: 7269 7074 696f 6e3d 6465 7363 7269 7074  ription=descript
+00016ce0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00016cf0: 206b 696e 643d 6e75 6d65 7261 746f 722e   kind=numerator.
+00016d00: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
+00016d10: 2020 6469 6d65 6e73 696f 6e3d 6469 6d5f    dimension=dim_
+00016d20: 7661 6c75 652c 0a20 2020 2020 2020 2020  value,.         
+00016d30: 2020 2064 6572 6976 6564 5f66 726f 6d5f     derived_from_
+00016d40: 6f70 3d4f 7028 6b69 6e64 3d6f 705f 6b69  op=Op(kind=op_ki
+00016d50: 6e64 2c20 696e 7075 7473 3d5b 6e75 6d65  nd, inputs=[nume
+00016d60: 7261 746f 722c 2064 656e 6f6d 696e 6174  rator, denominat
+00016d70: 6f72 5d29 2c0a 2020 2020 2020 2020 2020  or]),.          
+00016d80: 2020 6465 7269 7665 645f 6672 6f6d 5f74    derived_from_t
+00016d90: 6167 3d6e 756d 6572 6174 6f72 2c0a 2020  ag=numerator,.  
+00016da0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00016db0: 2061 735f 6469 6d28 7365 6c66 293a 0a20   as_dim(self):. 
+00016dc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016dd0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
+00016de0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016df0: 2020 2069 6620 7365 6c66 2e69 735f 6f6e     if self.is_on
+00016e00: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
+00016e10: 2072 6574 7572 6e20 5f6d 616b 655f 636f   return _make_co
+00016e20: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00016e30: 6d28 3129 0a20 2020 2020 2020 2069 6620  m(1).        if 
+00016e40: 6c65 6e28 7365 6c66 2e74 6572 6d73 2920  len(self.terms) 
+00016e50: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00016e60: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
+00016e70: 726d 735b 305d 0a20 2020 2020 2020 2064  rms[0].        d
+00016e80: 696d 5f6b 696e 6420 3d20 5f67 6574 5f6d  im_kind = _get_m
+00016e90: 6572 6765 645f 6469 6d5f 6b69 6e64 2873  erged_dim_kind(s
+00016ea0: 656c 662e 7465 726d 7329 0a20 2020 2020  elf.terms).     
+00016eb0: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
+00016ec0: 280a 2020 2020 2020 2020 2020 2020 6b69  (.            ki
+00016ed0: 6e64 3d64 696d 5f6b 696e 642c 0a20 2020  nd=dim_kind,.   
+00016ee0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00016ef0: 7469 6f6e 3d22 2a22 2e6a 6f69 6e28 6d61  tion="*".join(ma
+00016f00: 7028 5f67 6574 5f64 6573 6372 6970 7469  p(_get_descripti
+00016f10: 6f6e 2c20 7365 6c66 2e74 6572 6d73 2929  on, self.terms))
+00016f20: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+00016f30: 6d65 6e73 696f 6e3d 7365 6c66 2e64 696d  mension=self.dim
+00016f40: 656e 7369 6f6e 2c0a 2020 2020 2020 2020  ension,.        
+00016f50: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
+00016f60: 5f6f 703d 4f70 286b 696e 643d 226d 756c  _op=Op(kind="mul
+00016f70: 222c 2069 6e70 7574 733d 6c69 7374 2873  ", inputs=list(s
+00016f80: 656c 662e 7465 726d 7329 292c 0a20 2020  elf.terms)),.   
+00016f90: 2020 2020 2020 2020 2064 6572 6976 6564           derived
+00016fa0: 5f66 726f 6d5f 7461 673d 7365 6c66 2e72  _from_tag=self.r
+00016fb0: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
+00016fc0: 6728 292c 0a20 2020 2020 2020 2029 0a0a  g(),.        )..
+00016fd0: 2020 2020 6465 6620 7265 7072 6573 656e      def represen
+00016fe0: 7461 7469 7665 5f74 6167 2873 656c 6629  tative_tag(self)
+00016ff0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00017000: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+00017010: 6d7c 4e6f 6e65 0a20 2020 2020 2020 2022  m|None.        "
+00017020: 2222 0a20 2020 2020 2020 2023 2041 6c73  "".        # Als
+00017030: 6f20 7365 6520 4469 6d2e 5f4f 704c 696e  o see Dim._OpLin
+00017040: 6561 7254 6572 6d2e 7265 7072 6573 656e  earTerm.represen
+00017050: 7461 7469 7665 5f74 6167 2829 2e0a 2020  tative_tag()..  
+00017060: 2020 2020 2020 2320 4669 7273 7420 6669        # First fi
+00017070: 6e64 2061 6e79 2064 796e 616d 6963 2e0a  nd any dynamic..
+00017080: 2020 2020 2020 2020 666f 7220 7465 726d          for term
+00017090: 5f20 696e 2073 656c 662e 7465 726d 733a  _ in self.terms:
+000170a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000170b0: 7465 726d 5f2e 6973 5f64 796e 616d 6963  term_.is_dynamic
+000170c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000170d0: 2020 2020 7265 7475 726e 2074 6572 6d5f      return term_
+000170e0: 0a20 2020 2020 2020 2023 204e 6f77 2066  .        # Now f
+000170f0: 696e 6420 6e6f 6e2d 756e 7370 6563 6966  ind non-unspecif
+00017100: 6965 642e 0a20 2020 2020 2020 2066 6f72  ied..        for
+00017110: 2074 6572 6d5f 2069 6e20 7365 6c66 2e74   term_ in self.t
+00017120: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+00017130: 2020 6966 2074 6572 6d5f 2e6b 696e 6420    if term_.kind 
+00017140: 213d 2044 696d 5479 7065 732e 556e 7370  != DimTypes.Unsp
+00017150: 6563 6966 6965 643a 0a20 2020 2020 2020  ecified:.       
+00017160: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00017170: 7465 726d 5f0a 2020 2020 2020 2020 2320  term_.        # 
+00017180: 4e6f 7720 6669 6e64 2061 6e79 2e0a 2020  Now find any..  
+00017190: 2020 2020 2020 666f 7220 7465 726d 5f20        for term_ 
+000171a0: 696e 2073 656c 662e 7465 726d 733a 0a20  in self.terms:. 
+000171b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000171c0: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
+000171d0: 7265 7475 726e 204e 6f6e 650a 0a0a 636c  return None...cl
+000171e0: 6173 7320 5f4f 704c 696e 6561 7254 6572  ass _OpLinearTer
+000171f0: 6d3a 0a20 2020 2022 2222 0a20 2020 2072  m:.    """.    r
+00017200: 6570 7265 7365 6e74 7320 7374 6820 6c69  epresents sth li
+00017210: 6b65 2061 202a 2062 202b 2063 0a20 2020  ke a * b + c.   
+00017220: 2022 2222 0a0a 2020 2020 4063 6c61 7373   """..    @class
+00017230: 6d65 7468 6f64 0a20 2020 2064 6566 2066  method.    def f
+00017240: 726f 6d5f 6469 6d28 636c 732c 2064 696d  rom_dim(cls, dim
+00017250: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00017260: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00017270: 6d20 6469 6d3a 0a20 2020 2020 2020 203a  m dim:.        :
+00017280: 7274 7970 653a 2044 696d 2e5f 4f70 4c69  rtype: Dim._OpLi
+00017290: 6e65 6172 5465 726d 0a20 2020 2020 2020  nearTerm.       
+000172a0: 2022 2222 0a20 2020 2020 2020 2072 6573   """.        res
+000172b0: 203d 2063 6c73 2e7a 6572 6f28 290a 2020   = cls.zero().  
+000172c0: 2020 2020 2020 7265 732e 6578 7465 6e64        res.extend
+000172d0: 5f61 6464 5f73 7562 5f28 6469 6d2c 206b  _add_sub_(dim, k
+000172e0: 696e 643d 2261 6464 222c 2072 6967 6874  ind="add", right
+000172f0: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00017300: 6574 7572 6e20 7265 730a 0a20 2020 2040  eturn res..    @
+00017310: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00017320: 6465 6620 7a65 726f 2863 6c73 293a 0a20  def zero(cls):. 
+00017330: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017340: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
+00017350: 4f70 4c69 6e65 6172 5465 726d 0a20 2020  OpLinearTerm.   
+00017360: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00017370: 2072 6574 7572 6e20 5f4f 704c 696e 6561   return _OpLinea
+00017380: 7254 6572 6d28 5b5d 290a 0a20 2020 2064  rTerm([])..    d
+00017390: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000173a0: 2c20 7465 726d 7329 3a0a 2020 2020 2020  , terms):.      
+000173b0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+000173c0: 6172 616d 206c 6973 745b 4469 6d2e 5f4f  aram list[Dim._O
+000173d0: 704d 756c 7454 6572 6d5d 2074 6572 6d73  pMultTerm] terms
+000173e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000173f0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00017400: 203d 2074 6572 6d73 0a0a 2020 2020 6465   = terms..    de
+00017410: 6620 5f5f 6861 7368 5f5f 2873 656c 6629  f __hash__(self)
+00017420: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00017430: 2068 6173 6828 7475 706c 6528 7365 6c66   hash(tuple(self
+00017440: 2e74 6572 6d73 2929 0a0a 2020 2020 6465  .terms))..    de
+00017450: 6620 5f5f 6571 5f5f 2873 656c 662c 206f  f __eq__(self, o
+00017460: 7468 6572 293a 0a20 2020 2020 2020 2069  ther):.        i
+00017470: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+00017480: 6572 2c20 5f4f 704c 696e 6561 7254 6572  er, _OpLinearTer
+00017490: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+000174a0: 7265 7475 726e 2073 656c 662e 7465 726d  return self.term
+000174b0: 7320 3d3d 206f 7468 6572 2e74 6572 6d73  s == other.terms
+000174c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000174d0: 4661 6c73 650a 0a20 2020 2064 6566 205f  False..    def _
+000174e0: 5f6e 655f 5f28 7365 6c66 2c20 6f74 6865  _ne__(self, othe
+000174f0: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
+00017500: 726e 206e 6f74 2073 656c 662e 5f5f 6571  rn not self.__eq
+00017510: 5f5f 286f 7468 6572 290a 0a20 2020 2064  __(other)..    d
+00017520: 6566 2061 735f 6469 6d28 7365 6c66 293a  ef as_dim(self):
+00017530: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017540: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00017550: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017560: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+00017570: 7a65 726f 2829 3a0a 2020 2020 2020 2020  zero():.        
+00017580: 2020 2020 7265 7475 726e 205f 6d61 6b65      return _make
+00017590: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+000175a0: 5f64 696d 2830 290a 2020 2020 2020 2020  _dim(0).        
+000175b0: 6966 206c 656e 2873 656c 662e 7465 726d  if len(self.term
+000175c0: 7329 203d 3d20 313a 0a20 2020 2020 2020  s) == 1:.       
+000175d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000175e0: 2e74 6572 6d73 5b30 5d2e 6173 5f64 696d  .terms[0].as_dim
+000175f0: 2829 0a20 2020 2020 2020 2061 6464 5f70  ().        add_p
+00017600: 6172 7473 203d 205b 5d0a 2020 2020 2020  arts = [].      
+00017610: 2020 6465 7363 5f70 6172 7473 203d 205b    desc_parts = [
+00017620: 5d0a 2020 2020 2020 2020 6469 6d20 3d20  ].        dim = 
+00017630: 300a 2020 2020 2020 2020 666f 7220 7465  0.        for te
+00017640: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
+00017650: 3a0a 2020 2020 2020 2020 2020 2020 7320  :.            s 
+00017660: 3d20 7465 726d 2e61 735f 6469 6d28 290a  = term.as_dim().
+00017670: 2020 2020 2020 2020 2020 2020 6164 645f              add_
+00017680: 7061 7274 732e 6170 7065 6e64 2873 290a  parts.append(s).
+00017690: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+000176a0: 5f70 6172 7473 2e61 7070 656e 6428 5f67  _parts.append(_g
+000176b0: 6574 5f64 6573 6372 6970 7469 6f6e 2873  et_description(s
+000176c0: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+000176d0: 6620 6469 6d20 6973 206e 6f74 204e 6f6e  f dim is not Non
+000176e0: 6520 616e 6420 732e 6469 6d65 6e73 696f  e and s.dimensio
+000176f0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00017700: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017710: 696d 202b 3d20 732e 6469 6d65 6e73 696f  im += s.dimensio
+00017720: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
+00017730: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00017740: 2020 2020 6469 6d20 3d20 4e6f 6e65 0a20      dim = None. 
+00017750: 2020 2020 2020 2069 6620 6c65 6e28 6164         if len(ad
+00017760: 645f 7061 7274 7329 203d 3d20 313a 0a20  d_parts) == 1:. 
+00017770: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017780: 6e20 6164 645f 7061 7274 735b 305d 0a20  n add_parts[0]. 
+00017790: 2020 2020 2020 2072 6574 7572 6e20 5f64         return _d
+000177a0: 2e44 696d 280a 2020 2020 2020 2020 2020  .Dim(.          
+000177b0: 2020 6b69 6e64 3d5f 6765 745f 6d65 7267    kind=_get_merg
+000177c0: 6564 5f64 696d 5f6b 696e 6428 6164 645f  ed_dim_kind(add_
+000177d0: 7061 7274 7329 2c0a 2020 2020 2020 2020  parts),.        
+000177e0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+000177f0: 222b 222e 6a6f 696e 2864 6573 635f 7061  "+".join(desc_pa
+00017800: 7274 7329 2c0a 2020 2020 2020 2020 2020  rts),.          
+00017810: 2020 6469 6d65 6e73 696f 6e3d 6469 6d2c    dimension=dim,
+00017820: 0a20 2020 2020 2020 2020 2020 2064 6572  .            der
+00017830: 6976 6564 5f66 726f 6d5f 6f70 3d4f 7028  ived_from_op=Op(
+00017840: 6b69 6e64 3d22 6164 6422 2c20 696e 7075  kind="add", inpu
+00017850: 7473 3d61 6464 5f70 6172 7473 292c 0a20  ts=add_parts),. 
+00017860: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
+00017870: 6564 5f66 726f 6d5f 7461 673d 7365 6c66  ed_from_tag=self
+00017880: 2e72 6570 7265 7365 6e74 6174 6976 655f  .representative_
+00017890: 7461 6728 292c 0a20 2020 2020 2020 2029  tag(),.        )
+000178a0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+000178b0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+000178c0: 2020 7265 7475 726e 2022 4469 6d2e 5f4f    return "Dim._O
+000178d0: 704c 696e 6561 7254 6572 6d28 2572 2922  pLinearTerm(%r)"
+000178e0: 2025 2028 7365 6c66 2e74 6572 6d73 2c29   % (self.terms,)
+000178f0: 0a0a 2020 2020 6465 6620 6973 5f7a 6572  ..    def is_zer
+00017900: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
+00017910: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00017920: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00017930: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00017940: 7475 726e 206e 6f74 2073 656c 662e 7465  turn not self.te
+00017950: 726d 730a 0a20 2020 2064 6566 2065 7874  rms..    def ext
+00017960: 656e 645f 6164 645f 7375 625f 2873 656c  end_add_sub_(sel
+00017970: 662c 206f 7468 6572 2c20 6b69 6e64 2c20  f, other, kind, 
+00017980: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
+00017990: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+000179a0: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
+000179b0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+000179c0: 2073 7472 206b 696e 643a 2022 6164 6422   str kind: "add"
+000179d0: 206f 7220 2273 7562 220a 2020 2020 2020   or "sub".      
+000179e0: 2020 3a70 6172 616d 2062 6f6f 6c20 7269    :param bool ri
+000179f0: 6768 743a 206f 7220 6c65 6674 2e20 7269  ght: or left. ri
+00017a00: 6768 7420 6d65 616e 7320 7365 6c66 202b  ght means self +
+00017a10: 206f 7468 6572 2c20 6c65 6674 206d 6561   other, left mea
+00017a20: 6e73 206f 7468 6572 202b 2073 656c 660a  ns other + self.
+00017a30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00017a40: 2020 2020 6173 7365 7274 206b 696e 6420      assert kind 
+00017a50: 696e 207b 2261 6464 222c 2022 7375 6222  in {"add", "sub"
+00017a60: 7d0a 2020 2020 2020 2020 6f74 6865 7220  }.        other 
+00017a70: 3d20 7365 6c66 2e5f 6d61 6b65 5f64 696d  = self._make_dim
+00017a80: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
+00017a90: 6429 0a20 2020 2020 2020 2069 6620 6f74  d).        if ot
+00017aa0: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
+00017ab0: 7374 6174 6963 5f64 696d 2829 2061 6e64  static_dim() and
+00017ac0: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
+00017ad0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00017ae0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00017af0: 2020 6966 206f 7468 6572 2e64 6572 6976    if other.deriv
+00017b00: 6564 5f66 726f 6d5f 6f70 2061 6e64 206f  ed_from_op and o
+00017b10: 7468 6572 2e64 6572 6976 6564 5f66 726f  ther.derived_fro
+00017b20: 6d5f 6f70 2e6b 696e 6420 3d3d 2022 6164  m_op.kind == "ad
+00017b30: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
+00017b40: 666f 7220 6f74 6865 725f 2069 6e20 6f74  for other_ in ot
+00017b50: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+00017b60: 5f6f 702e 696e 7075 7473 2069 6620 7269  _op.inputs if ri
+00017b70: 6768 7420 656c 7365 2072 6576 6572 7365  ght else reverse
+00017b80: 6428 6f74 6865 722e 6465 7269 7665 645f  d(other.derived_
+00017b90: 6672 6f6d 5f6f 702e 696e 7075 7473 293a  from_op.inputs):
+00017ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017bb0: 2073 656c 662e 6578 7465 6e64 5f61 6464   self.extend_add
+00017bc0: 5f73 7562 5f28 6f74 6865 725f 2c20 6b69  _sub_(other_, ki
+00017bd0: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+00017be0: 6967 6874 290a 2020 2020 2020 2020 2020  ight).          
+00017bf0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00017c00: 2074 6572 6d20 3d20 5f4f 704d 756c 7454   term = _OpMultT
+00017c10: 6572 6d2e 6672 6f6d 5f64 696d 286f 7468  erm.from_dim(oth
+00017c20: 6572 290a 2020 2020 2020 2020 6e65 675f  er).        neg_
+00017c30: 7465 726d 203d 2074 6572 6d2e 6e65 6761  term = term.nega
+00017c40: 7469 7665 2829 0a20 2020 2020 2020 2069  tive().        i
+00017c50: 6620 6b69 6e64 203d 3d20 2273 7562 223a  f kind == "sub":
+00017c60: 0a20 2020 2020 2020 2020 2020 2074 6572  .            ter
+00017c70: 6d2c 206e 6567 5f74 6572 6d20 3d20 6e65  m, neg_term = ne
+00017c80: 675f 7465 726d 2c20 7465 726d 0a20 2020  g_term, term.   
+00017c90: 2020 2020 206d 6f73 745f 7265 6365 6e74       most_recent
+00017ca0: 5f74 6572 6d20 3d20 7365 6c66 2e74 6572  _term = self.ter
+00017cb0: 6d73 5b2d 3120 6966 2072 6967 6874 2065  ms[-1 if right e
+00017cc0: 6c73 6520 305d 2069 6620 7365 6c66 2e74  lse 0] if self.t
+00017cd0: 6572 6d73 2065 6c73 6520 4e6f 6e65 0a20  erms else None. 
+00017ce0: 2020 2020 2020 2069 6620 6d6f 7374 5f72         if most_r
+00017cf0: 6563 656e 745f 7465 726d 3a0a 2020 2020  ecent_term:.    
+00017d00: 2020 2020 2020 2020 6966 206d 6f73 745f          if most_
+00017d10: 7265 6365 6e74 5f74 6572 6d20 3d3d 206e  recent_term == n
+00017d20: 6567 5f74 6572 6d3a 0a20 2020 2020 2020  eg_term:.       
+00017d30: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00017d40: 726d 732e 706f 7028 2d31 2069 6620 7269  rms.pop(-1 if ri
+00017d50: 6768 7420 656c 7365 2030 290a 2020 2020  ght else 0).    
+00017d60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017d70: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00017d80: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
+00017d90: 726d 2e69 735f 636f 6e73 7461 6e74 5f73  rm.is_constant_s
+00017da0: 7461 7469 635f 6469 6d28 2920 616e 6420  tatic_dim() and 
+00017db0: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
+00017dc0: 5f73 7461 7469 635f 6469 6d28 293a 0a20  _static_dim():. 
+00017dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017de0: 656c 662e 7465 726d 735b 2d31 2069 6620  elf.terms[-1 if 
+00017df0: 7269 6768 7420 656c 7365 2030 5d20 3d20  right else 0] = 
+00017e00: 5f4f 704d 756c 7454 6572 6d2e 6672 6f6d  _OpMultTerm.from
+00017e10: 5f64 696d 280a 2020 2020 2020 2020 2020  _dim(.          
+00017e20: 2020 2020 2020 2020 2020 5f6d 616b 655f            _make_
+00017e30: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+00017e40: 6469 6d28 6d6f 7374 5f72 6563 656e 745f  dim(most_recent_
+00017e50: 7465 726d 2e64 696d 656e 7369 6f6e 202b  term.dimension +
+00017e60: 2074 6572 6d2e 6469 6d65 6e73 696f 6e2c   term.dimension,
+00017e70: 206b 696e 643d 6f74 6865 722e 6b69 6e64   kind=other.kind
+00017e80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017e90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00017ea0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00017eb0: 2020 2020 2020 2069 6620 6d6f 7374 5f72         if most_r
+00017ec0: 6563 656e 745f 7465 726d 2e74 6572 6d73  ecent_term.terms
+00017ed0: 2061 6e64 2074 6572 6d2e 7465 726d 7320   and term.terms 
+00017ee0: 616e 6420 6d6f 7374 5f72 6563 656e 745f  and most_recent_
+00017ef0: 7465 726d 2e74 6572 6d73 5b2d 315d 203d  term.terms[-1] =
+00017f00: 3d20 7465 726d 2e74 6572 6d73 5b2d 315d  = term.terms[-1]
+00017f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017f20: 2020 2320 4d65 7267 6520 7465 726d 730a    # Merge terms.
+00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f40: 6120 3d20 5f4f 704d 756c 7454 6572 6d2e  a = _OpMultTerm.
+00017f50: 6672 6f6d 5f64 696d 5f66 6163 746f 7273  from_dim_factors
+00017f60: 286d 6f73 745f 7265 6365 6e74 5f74 6572  (most_recent_ter
+00017f70: 6d2e 7465 726d 735b 3a2d 315d 292e 6173  m.terms[:-1]).as
+00017f80: 5f64 696d 2829 0a20 2020 2020 2020 2020  _dim().         
+00017f90: 2020 2020 2020 2062 203d 205f 4f70 4d75         b = _OpMu
+00017fa0: 6c74 5465 726d 2e66 726f 6d5f 6469 6d5f  ltTerm.from_dim_
+00017fb0: 6661 6374 6f72 7328 7465 726d 2e74 6572  factors(term.ter
+00017fc0: 6d73 5b3a 2d31 5d29 2e61 735f 6469 6d28  ms[:-1]).as_dim(
+00017fd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017fe0: 2020 7265 7320 3d20 5f4f 704d 756c 7454    res = _OpMultT
+00017ff0: 6572 6d2e 6672 6f6d 5f64 696d 2828 6120  erm.from_dim((a 
+00018000: 2b20 6229 2069 6620 7269 6768 7420 656c  + b) if right el
+00018010: 7365 2028 6220 2b20 6129 290a 2020 2020  se (b + a)).    
+00018020: 2020 2020 2020 2020 2020 2020 7265 732e              res.
+00018030: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+00018040: 7465 726d 2e74 6572 6d73 5b2d 315d 2c20  term.terms[-1], 
+00018050: 6b69 6e64 3d22 6d75 6c22 2c20 7269 6768  kind="mul", righ
+00018060: 743d 5472 7565 290a 2020 2020 2020 2020  t=True).        
+00018070: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+00018080: 6d73 5b2d 3120 6966 2072 6967 6874 2065  ms[-1 if right e
+00018090: 6c73 6520 305d 203d 2072 6573 0a20 2020  lse 0] = res.   
+000180a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000180b0: 7572 6e0a 2020 2020 2020 2020 6966 2072  urn.        if r
+000180c0: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
+000180d0: 2020 7365 6c66 2e74 6572 6d73 2e61 7070    self.terms.app
+000180e0: 656e 6428 7465 726d 290a 2020 2020 2020  end(term).      
+000180f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00018100: 2020 2020 7365 6c66 2e74 6572 6d73 2e69      self.terms.i
+00018110: 6e73 6572 7428 302c 2074 6572 6d29 0a0a  nsert(0, term)..
+00018120: 2020 2020 6465 6620 6578 7465 6e64 5f6d      def extend_m
+00018130: 756c 5f64 6976 5f28 7365 6c66 2c20 6f74  ul_div_(self, ot
+00018140: 6865 722c 206b 696e 642c 2072 6967 6874  her, kind, right
+00018150: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00018160: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00018170: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00018180: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+00018190: 6b69 6e64 3a20 226d 756c 2220 6f72 2022  kind: "mul" or "
+000181a0: 6365 696c 6469 7622 0a20 2020 2020 2020  ceildiv".       
+000181b0: 203a 7061 7261 6d20 626f 6f6c 2072 6967   :param bool rig
+000181c0: 6874 3a20 6f72 206c 6566 742e 2072 6967  ht: or left. rig
+000181d0: 6874 206d 6561 6e73 2073 656c 6620 2a20  ht means self * 
+000181e0: 6f74 6865 722c 206c 6566 7420 6d65 616e  other, left mean
+000181f0: 7320 6f74 6865 7220 2a20 7365 6c66 0a20  s other * self. 
+00018200: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00018210: 2020 2061 7373 6572 7420 6b69 6e64 2069     assert kind i
+00018220: 6e20 7b22 6d75 6c22 2c20 2266 6c6f 6f72  n {"mul", "floor
+00018230: 6469 7622 2c20 2274 7275 6564 6976 222c  div", "truediv",
+00018240: 2022 6365 696c 6469 7622 7d0a 2020 2020   "ceildiv"}.    
+00018250: 2020 2020 6f74 6865 7220 3d20 7365 6c66      other = self
+00018260: 2e5f 6d61 6b65 5f64 696d 286f 7468 6572  ._make_dim(other
+00018270: 2c20 6b69 6e64 3d6b 696e 6429 0a20 2020  , kind=kind).   
+00018280: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
+00018290: 226d 756c 2220 616e 6420 7269 6768 743a  "mul" and right:
+000182a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000182b0: 6e6f 7420 616c 6c28 7465 726d 2e63 616e  not all(term.can
+000182c0: 5f73 696d 706c 6966 7928 6f74 6865 722c  _simplify(other,
+000182d0: 206b 696e 643d 6b69 6e64 2c20 7269 6768   kind=kind, righ
+000182e0: 743d 7269 6768 7429 2066 6f72 2074 6572  t=right) for ter
+000182f0: 6d20 696e 2073 656c 662e 7465 726d 7329  m in self.terms)
+00018300: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018310: 2020 2320 446f 2069 7420 7468 6520 6f74    # Do it the ot
+00018320: 6865 7220 7761 7920 6172 6f75 6e64 0a20  her way around. 
+00018330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018340: 656c 662e 7465 726d 732c 206f 7468 6572  elf.terms, other
+00018350: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
+00018360: 2e66 726f 6d5f 6469 6d28 6f74 6865 7229  .from_dim(other)
+00018370: 2e74 6572 6d73 2c20 7365 6c66 2e61 735f  .terms, self.as_
+00018380: 6469 6d28 290a 2020 2020 2020 2020 2020  dim().          
+00018390: 2020 2020 2020 7269 6768 7420 3d20 4661        right = Fa
+000183a0: 6c73 650a 2020 2020 2020 2020 6966 206f  lse.        if o
+000183b0: 7468 6572 2e69 735f 636f 6e73 7461 6e74  ther.is_constant
+000183c0: 5f73 7461 7469 635f 6469 6d28 2920 616e  _static_dim() an
+000183d0: 6420 6f74 6865 722e 6469 6d65 6e73 696f  d other.dimensio
+000183e0: 6e20 3d3d 2031 3a0a 2020 2020 2020 2020  n == 1:.        
+000183f0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00018400: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
+00018410: 6974 6828 2264 6976 2229 2061 6e64 206c  ith("div") and l
+00018420: 656e 2873 656c 662e 7465 726d 7329 203e  en(self.terms) >
+00018430: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
+00018440: 2069 6620 616e 7928 6e6f 7420 7465 726d   if any(not term
+00018450: 2e64 6976 6973 6962 6c65 286f 7468 6572  .divisible(other
+00018460: 2c20 7269 6768 743d 7269 6768 7429 2066  , right=right) f
+00018470: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
+00018480: 7465 726d 7329 3a0a 2020 2020 2020 2020  terms):.        
+00018490: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+000184a0: 6d73 203d 205b 0a20 2020 2020 2020 2020  ms = [.         
+000184b0: 2020 2020 2020 2020 2020 205f 4f70 4d75             _OpMu
+000184c0: 6c74 5465 726d 2e66 726f 6d5f 6469 6d28  ltTerm.from_dim(
+000184d0: 5f4f 704d 756c 7454 6572 6d2e 6e65 775f  _OpMultTerm.new_
+000184e0: 6469 765f 6469 6d28 7365 6c66 2e61 735f  div_dim(self.as_
+000184f0: 6469 6d28 292c 206f 7468 6572 2c20 6b69  dim(), other, ki
+00018500: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+00018510: 6967 6874 2929 0a20 2020 2020 2020 2020  ight)).         
+00018520: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00018530: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00018540: 2020 2020 2020 2020 666f 7220 7465 726d          for term
+00018550: 2069 6e20 7365 6c66 2e74 6572 6d73 3a0a   in self.terms:.
+00018560: 2020 2020 2020 2020 2020 2020 7465 726d              term
+00018570: 2e65 7874 656e 645f 6d75 6c5f 6469 765f  .extend_mul_div_
+00018580: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
+00018590: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
+000185a0: 0a20 2020 2064 6566 205f 6d61 6b65 5f64  .    def _make_d
+000185b0: 696d 2873 656c 662c 206f 7468 6572 2c20  im(self, other, 
+000185c0: 6b69 6e64 293a 0a20 2020 2020 2020 2022  kind):.        "
+000185d0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+000185e0: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+000185f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00018600: 7374 7220 6b69 6e64 3a0a 2020 2020 2020  str kind:.      
+00018610: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+00018620: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00018630: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00018640: 6f74 6865 722c 2069 6e74 293a 0a20 2020  other, int):.   
+00018650: 2020 2020 2020 2020 2062 6173 655f 7461           base_ta
+00018660: 6720 3d20 7365 6c66 2e72 6570 7265 7365  g = self.represe
+00018670: 6e74 6174 6976 655f 7461 6728 290a 2020  ntative_tag().  
+00018680: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00018690: 205f 6d61 6b65 5f63 6f6e 7374 616e 745f   _make_constant_
+000186a0: 7374 6174 6963 5f64 696d 286f 7468 6572  static_dim(other
+000186b0: 2c20 6b69 6e64 3d62 6173 655f 7461 672e  , kind=base_tag.
+000186c0: 6b69 6e64 2069 6620 6261 7365 5f74 6167  kind if base_tag
+000186d0: 2065 6c73 6520 4e6f 6e65 290a 2020 2020   else None).    
+000186e0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+000186f0: 6e63 6528 6f74 6865 722c 205f 642e 4469  nce(other, _d.Di
+00018700: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00018710: 7265 7475 726e 206f 7468 6572 2e67 6574  return other.get
+00018720: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
+00018730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00018740: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+00018750: 6545 7272 6f72 2822 2573 2025 7320 2573  eError("%s %s %s
+00018760: 2069 6e76 616c 6964 2066 6f72 2074 7970   invalid for typ
+00018770: 6520 2573 2220 2520 2873 656c 662c 206b  e %s" % (self, k
+00018780: 696e 642c 206f 7468 6572 2c20 7479 7065  ind, other, type
+00018790: 286f 7468 6572 2929 290a 0a20 2020 2064  (other)))..    d
+000187a0: 6566 2072 6570 7265 7365 6e74 6174 6976  ef representativ
+000187b0: 655f 7461 6728 7365 6c66 293a 0a20 2020  e_tag(self):.   
+000187c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000187d0: 203a 7274 7970 653a 2044 696d 7c4e 6f6e   :rtype: Dim|Non
+000187e0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+000187f0: 2020 2020 2020 2320 4669 7273 7420 6669        # First fi
+00018800: 6e64 2061 6e79 2064 796e 616d 6963 2e0a  nd any dynamic..
+00018810: 2020 2020 2020 2020 666f 7220 7465 726d          for term
+00018820: 2069 6e20 7365 6c66 2e74 6572 6d73 3a0a   in self.terms:.
+00018830: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00018840: 7465 726d 5f20 696e 2074 6572 6d2e 7465  term_ in term.te
+00018850: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
+00018860: 2020 2020 2069 6620 7465 726d 5f2e 6973       if term_.is
+00018870: 5f64 796e 616d 6963 2829 3a0a 2020 2020  _dynamic():.    
+00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018890: 7265 7475 726e 2074 6572 6d5f 0a20 2020  return term_.   
+000188a0: 2020 2020 2023 204e 6f77 2066 696e 6420       # Now find 
+000188b0: 6e6f 6e2d 756e 7370 6563 6966 6965 642e  non-unspecified.
+000188c0: 0a20 2020 2020 2020 2066 6f72 2074 6572  .        for ter
+000188d0: 6d20 696e 2073 656c 662e 7465 726d 733a  m in self.terms:
+000188e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000188f0: 2074 6572 6d5f 2069 6e20 7465 726d 2e74   term_ in term.t
+00018900: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+00018910: 2020 2020 2020 6966 2074 6572 6d5f 2e6b        if term_.k
+00018920: 696e 6420 213d 2044 696d 5479 7065 732e  ind != DimTypes.
+00018930: 556e 7370 6563 6966 6965 643a 0a20 2020  Unspecified:.   
+00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018950: 2072 6574 7572 6e20 7465 726d 5f0a 2020   return term_.  
+00018960: 2020 2020 2020 2320 4e6f 7720 6669 6e64        # Now find
+00018970: 2061 6e79 2e0a 2020 2020 2020 2020 666f   any..        fo
+00018980: 7220 7465 726d 2069 6e20 7365 6c66 2e74  r term in self.t
+00018990: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+000189a0: 2020 666f 7220 7465 726d 5f20 696e 2074    for term_ in t
+000189b0: 6572 6d2e 7465 726d 733a 0a20 2020 2020  erm.terms:.     
+000189c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000189d0: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
+000189e0: 7265 7475 726e 204e 6f6e 650a 0a0a 6465  return None...de
+000189f0: 6620 5f67 6574 5f6d 6572 6765 645f 6469  f _get_merged_di
+00018a00: 6d5f 6b69 6e64 2864 696d 5f74 6167 7329  m_kind(dim_tags)
+00018a10: 3a0a 2020 2020 2222 220a 2020 2020 3a70  :.    """.    :p
+00018a20: 6172 616d 206c 6973 745b 4469 6d5d 7c74  aram list[Dim]|t
+00018a30: 7570 6c65 5b44 696d 5d20 6469 6d5f 7461  uple[Dim] dim_ta
+00018a40: 6773 3a0a 2020 2020 3a72 6574 7572 6e3a  gs:.    :return:
+00018a50: 2064 696d 206b 696e 640a 2020 2020 3a72   dim kind.    :r
+00018a60: 7479 7065 3a20 456e 7469 7479 0a20 2020  type: Entity.   
+00018a70: 2022 2222 0a20 2020 2069 6620 616e 7928   """.    if any(
+00018a80: 7461 672e 6973 5f62 6174 6368 5f64 696d  tag.is_batch_dim
+00018a90: 2829 2066 6f72 2074 6167 2069 6e20 6469  () for tag in di
+00018aa0: 6d5f 7461 6773 293a 0a20 2020 2020 2020  m_tags):.       
+00018ab0: 2072 6574 7572 6e20 4469 6d54 7970 6573   return DimTypes
+00018ac0: 2e42 6174 6368 0a20 2020 2065 6c69 6620  .Batch.    elif 
+00018ad0: 616e 7928 7461 672e 6973 5f66 6561 7475  any(tag.is_featu
+00018ae0: 7265 5f64 696d 2829 2066 6f72 2074 6167  re_dim() for tag
+00018af0: 2069 6e20 6469 6d5f 7461 6773 293a 0a20   in dim_tags):. 
+00018b00: 2020 2020 2020 2072 6574 7572 6e20 4469         return Di
+00018b10: 6d54 7970 6573 2e46 6561 7475 7265 0a20  mTypes.Feature. 
+00018b20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00018b30: 2072 6574 7572 6e20 4469 6d54 7970 6573   return DimTypes
+00018b40: 2e53 7061 7469 616c 0a0a 0a64 6566 2064  .Spatial...def d
+00018b50: 696d 5f63 6d70 5f76 616c 7565 286f 626a  im_cmp_value(obj
+00018b60: 293a 0a20 2020 2022 2222 0a20 2020 203a  ):.    """.    :
+00018b70: 7061 7261 6d20 4469 6d7c 5f4d 6172 6b65  param Dim|_Marke
+00018b80: 6444 696d 206f 626a 3a0a 2020 2020 3a72  dDim obj:.    :r
+00018b90: 6574 7572 6e3a 2061 6e79 7468 696e 6720  eturn: anything 
+00018ba0: 7768 6963 6820 6361 6e20 6265 2063 6f6d  which can be com
+00018bb0: 7061 7265 640a 2020 2020 2222 220a 2020  pared.    """.  
+00018bc0: 2020 2320 4d61 6b65 2044 696d 2061 6e64    # Make Dim and
+00018bd0: 205f 4d61 726b 6564 4469 6d20 636f 6d70   _MarkedDim comp
+00018be0: 6172 6162 6c65 2074 6f20 6561 6368 206f  arable to each o
+00018bf0: 7468 6572 2e0a 2020 2020 2320 4e6f 7465  ther..    # Note
+00018c00: 2074 6861 7420 7468 6520 6f72 6465 7220   that the order 
+00018c10: 6973 2072 6561 6c6c 7920 6172 6269 7472  is really arbitr
+00018c20: 6172 7920 616e 6420 646f 6573 206e 6f74  ary and does not
+00018c30: 206d 6174 7465 722e 0a20 2020 2069 6620   matter..    if 
+00018c40: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
+00018c50: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
+00018c60: 206f 626a 203d 206f 626a 2e67 6574 5f73   obj = obj.get_s
+00018c70: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
+00018c80: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
+00018c90: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
+00018ca0: 2020 2020 2020 2020 6f62 6a2e 6465 7363          obj.desc
+00018cb0: 7269 7074 696f 6e2c 0a20 2020 2020 2020  ription,.       
+00018cc0: 2020 2020 206f 626a 2e6b 696e 642c 0a20       obj.kind,. 
+00018cd0: 2020 2020 2020 2020 2020 206f 626a 2e64             obj.d
+00018ce0: 696d 656e 7369 6f6e 2c0a 2020 2020 2020  imension,.      
+00018cf0: 2020 2020 2020 6f62 6a2e 6479 6e5f 7369        obj.dyn_si
+00018d00: 7a65 5f65 7874 2e64 696d 7320 6966 206f  ze_ext.dims if o
+00018d10: 626a 2e64 796e 5f73 697a 655f 6578 7420  bj.dyn_size_ext 
+00018d20: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00018d30: 204e 6f6e 652c 0a20 2020 2020 2020 2029   None,.        )
+00018d40: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00018d50: 6365 286f 626a 2c20 5f6d 2e4d 6172 6b65  ce(obj, _m.Marke
+00018d60: 6444 696d 293a 0a20 2020 2020 2020 2072  dDim):.        r
+00018d70: 6574 7572 6e20 6f62 6a2e 5f5f 636c 6173  eturn obj.__clas
+00018d80: 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20 6f62  s__.__name__, ob
+00018d90: 6a2e 7461 670a 2020 2020 7265 7475 726e  j.tag.    return
+00018da0: 206f 626a 0a                              obj.
```

### Comparing `returnn-1.20230719.100821/returnn/tensor/_tensor_extra.py` & `returnn-1.20230719.105013/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230719.105013/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230719.105013/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230719.105013/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/dim.py` & `returnn-1.20230719.105013/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/marked_dim.py` & `returnn-1.20230719.105013/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/tensor.py` & `returnn-1.20230719.105013/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/tensor_dict.py` & `returnn-1.20230719.105013/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tensor/utils.py` & `returnn-1.20230719.105013/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/compat.py` & `returnn-1.20230719.105013/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/data_pipeline.py` & `returnn-1.20230719.105013/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/distributed.py` & `returnn-1.20230719.105013/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/engine.py` & `returnn-1.20230719.105013/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230719.105013/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230719.105013/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/horovod.py` & `returnn-1.20230719.105013/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230719.105013/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/layers/base.py` & `returnn-1.20230719.105013/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/layers/basic.py` & `returnn-1.20230719.105013/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/layers/rec.py` & `returnn-1.20230719.105013/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/layers/segmental_model.py` & `returnn-1.20230719.105013/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/layers/signal_processing.py` & `returnn-1.20230719.105013/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/layers/variable.py` & `returnn-1.20230719.105013/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/native_op.py` & `returnn-1.20230719.105013/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/network.py` & `returnn-1.20230719.105013/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/sprint.py` & `returnn-1.20230719.105013/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/updater.py` & `returnn-1.20230719.105013/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/util/basic.py` & `returnn-1.20230719.105013/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/util/data.py` & `returnn-1.20230719.105013/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20230719.105013/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/util/ken_lm.py` & `returnn-1.20230719.105013/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/tf/util/open_fst.py` & `returnn-1.20230719.105013/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/data/pipeline.py` & `returnn-1.20230719.105013/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230719.105013/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/data/tensor_utils.py` & `returnn-1.20230719.105013/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/distributed.py` & `returnn-1.20230719.105013/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/engine.py` & `returnn-1.20230719.105013/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/frontend/_backend.py` & `returnn-1.20230719.105013/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/frontend/_rand.py` & `returnn-1.20230719.105013/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/frontend/bridge.py` & `returnn-1.20230719.105013/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/torch/updater.py` & `returnn-1.20230719.105013/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/basic.py` & `returnn-1.20230719.105013/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/better_exchook.py` & `returnn-1.20230719.105013/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/bpe.py` & `returnn-1.20230719.105013/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/debug.py` & `returnn-1.20230719.105013/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/debug_helpers.py` & `returnn-1.20230719.105013/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/fsa.py` & `returnn-1.20230719.105013/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230719.105013/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/pprint.py` & `returnn-1.20230719.105013/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/py-to-pickle.cpp` & `returnn-1.20230719.105013/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/sig_proc.py` & `returnn-1.20230719.105013/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn/util/task_system.py` & `returnn-1.20230719.105013/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/returnn.egg-info/PKG-INFO` & `returnn-1.20230719.105013/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230719.100821
+Version: 1.20230719.105013
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230719.100821/returnn.egg-info/SOURCES.txt` & `returnn-1.20230719.105013/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/setup.py` & `returnn-1.20230719.105013/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/DummySprintExec.py` & `returnn-1.20230719.105013/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230719.105013/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230719.105013/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230719.105013/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/_set_num_threads1.py` & `returnn-1.20230719.105013/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/_setup_test_env.py` & `returnn-1.20230719.105013/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/bpe-unicode-demo.codes` & `returnn-1.20230719.105013/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/bpe-unicode-demo.vocab` & `returnn-1.20230719.105013/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/lexicon_opt.isyms` & `returnn-1.20230719.105013/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/lexicon_opt.jpg` & `returnn-1.20230719.105013/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/lint_common.py` & `returnn-1.20230719.105013/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/pycharm-inspect.py` & `returnn-1.20230719.105013/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/pylint.py` & `returnn-1.20230719.105013/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/returnn-as-framework.py` & `returnn-1.20230719.105013/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/rf_utils.py` & `returnn-1.20230719.105013/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/spelling.dic` & `returnn-1.20230719.105013/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_Config.py` & `returnn-1.20230719.105013/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_Dataset.py` & `returnn-1.20230719.105013/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_Fsa.py` & `returnn-1.20230719.105013/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_GeneratingDataset.py` & `returnn-1.20230719.105013/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_HDFDataset.py` & `returnn-1.20230719.105013/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_LearningRateControl.py` & `returnn-1.20230719.105013/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_Log.py` & `returnn-1.20230719.105013/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_MultiProcDataset.py` & `returnn-1.20230719.105013/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_PTDataset.py` & `returnn-1.20230719.105013/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_Pretrain.py` & `returnn-1.20230719.105013/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_ResNet.py` & `returnn-1.20230719.105013/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_SprintDataset.py` & `returnn-1.20230719.105013/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_SprintInterface.py` & `returnn-1.20230719.105013/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFEngine.py` & `returnn-1.20230719.105013/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFNativeOp.py` & `returnn-1.20230719.105013/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFNetworkLayer.py` & `returnn-1.20230719.105013/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230719.105013/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230719.105013/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFUpdater.py` & `returnn-1.20230719.105013/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TFUtil.py` & `returnn-1.20230719.105013/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TF_determinism.py` & `returnn-1.20230719.105013/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TaskSystem.py` & `returnn-1.20230719.105013/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230719.105013/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_TranslationDataset.py` & `returnn-1.20230719.105013/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_Util.py` & `returnn-1.20230719.105013/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_demos.py` & `returnn-1.20230719.105013/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_fork_exec.py` & `returnn-1.20230719.105013/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_hdf_dump.py` & `returnn-1.20230719.105013/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_array.py` & `returnn-1.20230719.105013/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_attention.py` & `returnn-1.20230719.105013/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_base.py` & `returnn-1.20230719.105013/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_cond.py` & `returnn-1.20230719.105013/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_const.py` & `returnn-1.20230719.105013/tests/test_rf_const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_container.py` & `returnn-1.20230719.105013/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_conv.py` & `returnn-1.20230719.105013/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_encoder_conformer.py` & `returnn-1.20230719.105013/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_loop.py` & `returnn-1.20230719.105013/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_math.py` & `returnn-1.20230719.105013/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_normalization.py` & `returnn-1.20230719.105013/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_rec.py` & `returnn-1.20230719.105013/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_reduce.py` & `returnn-1.20230719.105013/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_rf_signal.py` & `returnn-1.20230719.105013/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_tensor.py` & `returnn-1.20230719.105013/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_tools.py` & `returnn-1.20230719.105013/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_torch_engine.py` & `returnn-1.20230719.105013/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_torch_frontend.py` & `returnn-1.20230719.105013/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tests/test_torch_internal_frontend.py` & `returnn-1.20230719.105013/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/analyze-dataset-batches.py` & `returnn-1.20230719.105013/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/bliss-collect-seq-lens.py` & `returnn-1.20230719.105013/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/bliss-dump-text.py` & `returnn-1.20230719.105013/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/bliss-get-segment-names.py` & `returnn-1.20230719.105013/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/bliss-to-ogg-zip.py` & `returnn-1.20230719.105013/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/bpe-create-lexicon.py` & `returnn-1.20230719.105013/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/calculate-word-error-rate.py` & `returnn-1.20230719.105013/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/cleanup-old-models.py` & `returnn-1.20230719.105013/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/collect-orth-symbols.py` & `returnn-1.20230719.105013/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/collect-words.py` & `returnn-1.20230719.105013/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/compile_native_op.py` & `returnn-1.20230719.105013/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/compile_tf_graph.py` & `returnn-1.20230719.105013/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/debug-dump-search-scores.py` & `returnn-1.20230719.105013/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/debug-plot-search-scores.py` & `returnn-1.20230719.105013/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/dump-dataset-raw-strings.py` & `returnn-1.20230719.105013/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/dump-dataset.py` & `returnn-1.20230719.105013/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/dump-forward-stats.py` & `returnn-1.20230719.105013/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/dump-forward.py` & `returnn-1.20230719.105013/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/dump-network-json.py` & `returnn-1.20230719.105013/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/dump-pickle.py` & `returnn-1.20230719.105013/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230719.105013/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/get-attention-weights.py` & `returnn-1.20230719.105013/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/get-best-model-epoch.py` & `returnn-1.20230719.105013/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/hdf_dump.py` & `returnn-1.20230719.105013/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230719.105013/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/import-blocks-mt-model.py` & `returnn-1.20230719.105013/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/import-t2t-mt-model.py` & `returnn-1.20230719.105013/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/Makefile` & `returnn-1.20230719.105013/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/README.md` & `returnn-1.20230719.105013/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/example/README.md` & `returnn-1.20230719.105013/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230719.105013/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230719.105013/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230719.105013/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/file.h` & `returnn-1.20230719.105013/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230719.105013/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230719.105013/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/main.cc` & `returnn-1.20230719.105013/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230719.105013/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230719.105013/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230719.105013/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/tf_avg_checkpoints.py` & `returnn-1.20230719.105013/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/tf_inspect_checkpoint.py` & `returnn-1.20230719.105013/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/tf_inspect_summary_log.py` & `returnn-1.20230719.105013/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230719.100821/tools/torch_export_to_onnx.py` & `returnn-1.20230719.105013/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

