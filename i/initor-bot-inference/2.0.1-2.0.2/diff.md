# Comparing `tmp/initor_bot_inference-2.0.1.tar.gz` & `tmp/initor_bot_inference-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "initor_bot_inference-2.0.1.tar", max compression
+gzip compressed data, was "initor_bot_inference-2.0.2.tar", max compression
```

## Comparing `initor_bot_inference-2.0.1.tar` & `initor_bot_inference-2.0.2.tar`

### file list

```diff
@@ -1,788 +1,788 @@
--rw-r--r--   0        0        0      797 2023-07-19 12:14:19.424217 initor_bot_inference-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-07-19 12:14:00.763945 initor_bot_inference-2.0.1/src/initor_bot_inference/__init__.py
--rw-r--r--   0        0        0     3746 2023-07-17 15:10:59.190603 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/FastReID-Logo.png
--rw-r--r--   0        0        0      955 2023-07-17 15:10:59.198603 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/bugs.md
--rw-r--r--   0        0        0      448 2023-07-17 15:10:59.206603 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      820 2023-07-17 15:10:59.214604 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/questions-help-support.md
--rw-r--r--   0        0        0     1087 2023-07-17 15:10:59.230604 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/unexpected-problems-bugs.md
--rw-r--r--   0        0        0   278762 2023-07-17 15:10:59.254604 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/wechat_group.png
--rw-r--r--   0        0        0      640 2023-07-17 15:10:59.262605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/workflows/issue_auto_close.yml
--rw-r--r--   0        0        0      563 2023-07-17 15:10:59.270605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/workflows/lint_python.yml
--rw-r--r--   0        0        0      333 2023-07-17 15:10:59.270605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.gitignore
--rw-r--r--   0        0        0      832 2023-07-17 15:10:59.278605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/CHANGELOG.md
--rw-r--r--   0        0        0     2219 2023-07-17 15:10:59.286605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/GETTING_STARTED.md
--rw-r--r--   0        0        0      798 2023-07-17 15:10:59.294605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/INSTALL.md
--rw-r--r--   0        0        0    11347 2023-07-17 15:10:59.302605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/LICENSE
--rw-r--r--   0        0        0    14758 2023-07-17 15:10:59.310605 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/MODEL_ZOO.md
--rw-r--r--   0        0        0     4264 2023-07-17 15:10:59.318606 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/README.md
--rw-r--r--   0        0        0     3674 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/__pycache__/fast_reid_interfece.cpython-38.pyc
--rw-r--r--   0        0        0      285 2023-07-17 15:10:59.334606 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Base-AGW.yml
--rw-r--r--   0        0        0      161 2023-07-17 15:10:59.338606 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Base-MGN.yml
--rw-r--r--   0        0        0      921 2023-07-17 15:10:59.346606 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Base-SBS.yml
--rw-r--r--   0        0        0     1112 2023-07-17 15:10:59.354606 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Base-bagtricks.yml
--rw-r--r--   0        0        0      176 2023-07-17 15:10:59.358606 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_R101-ibn.yml
--rw-r--r--   0        0        0      159 2023-07-17 15:10:59.366607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_R50-ibn.yml
--rw-r--r--   0        0        0      116 2023-07-17 15:10:59.374607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_R50.yml
--rw-r--r--   0        0        0      169 2023-07-17 15:10:59.382607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_S50.yml
--rw-r--r--   0        0        0      188 2023-07-17 15:10:59.390607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_R101-ibn.yml
--rw-r--r--   0        0        0      171 2023-07-17 15:10:59.402607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0      128 2023-07-17 15:10:59.410607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_R50.yml
--rw-r--r--   0        0        0      181 2023-07-17 15:10:59.414607 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_S50.yml
--rw-r--r--   0        0        0      159 2023-07-17 15:10:59.422608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/mgn_R50-ibn.yml
--rw-r--r--   0        0        0      176 2023-07-17 15:10:59.430608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_R101-ibn.yml
--rw-r--r--   0        0        0      159 2023-07-17 15:10:59.434608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_R50-ibn.yml
--rw-r--r--   0        0        0      116 2023-07-17 15:10:59.442608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_R50.yml
--rw-r--r--   0        0        0      169 2023-07-17 15:10:59.446608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_S50.yml
--rw-r--r--   0        0        0      167 2023-07-17 15:10:59.454608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_R101-ibn.yml
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.458608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_R50-ibn.yml
--rw-r--r--   0        0        0      107 2023-07-17 15:10:59.466608 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_R50.yml
--rw-r--r--   0        0        0      160 2023-07-17 15:10:59.474609 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_S50.yml
--rw-r--r--   0        0        0      179 2023-07-17 15:10:59.482609 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_R101-ibn.yml
--rw-r--r--   0        0        0      162 2023-07-17 15:10:59.490609 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0      119 2023-07-17 15:10:59.498609 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_R50.yml
--rw-r--r--   0        0        0      172 2023-07-17 15:10:59.510609 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_S50.yml
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.518609 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/mgn_R50-ibn.yml
--rw-r--r--   0        0        0      167 2023-07-17 15:10:59.526610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_R101-ibn.yml
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.534610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_R50-ibn.yml
--rw-r--r--   0        0        0      107 2023-07-17 15:10:59.542610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_R50.yml
--rw-r--r--   0        0        0      160 2023-07-17 15:10:59.550610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_S50.yml
--rw-r--r--   0        0        0      167 2023-07-17 15:10:59.558610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_R101-ibn.yml
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.566610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_R50-ibn.yml
--rw-r--r--   0        0        0      107 2023-07-17 15:10:59.570610 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_R50.yml
--rw-r--r--   0        0        0      160 2023-07-17 15:10:59.578611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_S50.yml
--rw-r--r--   0        0        0      179 2023-07-17 15:10:59.586611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_R101-ibn.yml
--rw-r--r--   0        0        0      162 2023-07-17 15:10:59.594611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0      119 2023-07-17 15:10:59.602611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_R50.yml
--rw-r--r--   0        0        0      172 2023-07-17 15:10:59.606611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_S50.yml
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.614611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/mgn_R50-ibn.yml
--rw-r--r--   0        0        0      167 2023-07-17 15:10:59.622611 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_R101-ibn.yml
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.630612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_R50-ibn.yml
--rw-r--r--   0        0        0      107 2023-07-17 15:10:59.638612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_R50.yml
--rw-r--r--   0        0        0      160 2023-07-17 15:10:59.646612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_S50.yml
--rw-r--r--   0        0        0      170 2023-07-17 15:10:59.654612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_R101-ibn.yml
--rw-r--r--   0        0        0      153 2023-07-17 15:10:59.662612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_R50-ibn.yml
--rw-r--r--   0        0        0      110 2023-07-17 15:10:59.666612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_R50.yml
--rw-r--r--   0        0        0      163 2023-07-17 15:10:59.674612 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_S50.yml
--rw-r--r--   0        0        0      183 2023-07-17 15:10:59.678613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_R101-ibn.yml
--rw-r--r--   0        0        0      166 2023-07-17 15:10:59.686613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0      122 2023-07-17 15:10:59.690613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_R50.yml
--rw-r--r--   0        0        0      176 2023-07-17 15:10:59.698613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_S50.yml
--rw-r--r--   0        0        0      153 2023-07-17 15:10:59.706613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/mgn_R50-ibn.yml
--rw-r--r--   0        0        0      170 2023-07-17 15:10:59.710613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_R101-ibn.yml
--rw-r--r--   0        0        0      153 2023-07-17 15:10:59.718613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_R50-ibn.yml
--rw-r--r--   0        0        0      110 2023-07-17 15:10:59.726613 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_R50.yml
--rw-r--r--   0        0        0      163 2023-07-17 15:10:59.730614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_S50.yml
--rw-r--r--   0        0        0      182 2023-07-17 15:10:59.738614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_R101-ibn.yml
--rw-r--r--   0        0        0      165 2023-07-17 15:10:59.746614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_R50-ibn.yml
--rw-r--r--   0        0        0      122 2023-07-17 15:10:59.754614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_R50.yml
--rw-r--r--   0        0        0      175 2023-07-17 15:10:59.762614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_S50.yml
--rw-r--r--   0        0        0      194 2023-07-17 15:10:59.766614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_R101-ibn.yml
--rw-r--r--   0        0        0      177 2023-07-17 15:10:59.774614 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0      134 2023-07-17 15:10:59.782615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_R50.yml
--rw-r--r--   0        0        0      187 2023-07-17 15:10:59.786615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_S50.yml
--rw-r--r--   0        0        0     1508 2023-07-17 15:10:59.790615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_vit.yml
--rw-r--r--   0        0        0      165 2023-07-17 15:10:59.798615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/mgn_R50-ibn.yml
--rw-r--r--   0        0        0      182 2023-07-17 15:10:59.802615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_R101-ibn.yml
--rw-r--r--   0        0        0      165 2023-07-17 15:10:59.810615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_R50-ibn.yml
--rw-r--r--   0        0        0      122 2023-07-17 15:10:59.814615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_R50.yml
--rw-r--r--   0        0        0      175 2023-07-17 15:10:59.818615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_S50.yml
--rw-r--r--   0        0        0      563 2023-07-17 15:10:59.826615 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/VERIWild/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0      483 2023-07-17 15:10:59.834616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/VeRi/sbs_R50-ibn.yml
--rw-r--r--   0        0        0      567 2023-07-17 15:10:59.842616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/VehicleID/bagtricks_R50-ibn.yml
--rw-r--r--   0        0        0     3744 2023-07-17 15:10:59.842616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/datasets/generate_mot_patches.py
--rw-r--r--   0        0        0      403 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/README.md
--rw-r--r--   0        0        0     3359 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/demo.py
--rw-r--r--   0        0        0      808 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/plot_roc_with_pickle.py
--rw-r--r--   0        0        0     5413 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/predictor.py
--rw-r--r--   0        0        0     5076 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/visualize_result.py
--rw-r--r--   0        0        0     1058 2023-07-17 15:10:59.854616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docker/Dockerfile
--rw-r--r--   0        0        0      663 2023-07-17 15:10:59.862616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docker/README.md
--rw-r--r--   0        0        0        6 2023-07-17 15:10:59.870616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/.gitignore
--rw-r--r--   0        0        0      630 2023-07-17 15:10:59.878616 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/Makefile
--rw-r--r--   0        0        0      542 2023-07-17 15:10:59.886617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/README.md
--rw-r--r--   0        0        0      428 2023-07-17 15:10:59.894617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/_static/css/custom.css
--rw-r--r--   0        0        0    11669 2023-07-17 15:10:59.894617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/conf.py
--rw-r--r--   0        0        0      377 2023-07-17 15:10:59.902617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/index.rst
--rw-r--r--   0        0        0      150 2023-07-17 15:10:59.906617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/checkpoint.rst
--rw-r--r--   0        0        0      372 2023-07-17 15:10:59.910617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/config.rst
--rw-r--r--   0        0        0     1929 2023-07-17 15:10:59.914617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/data.rst
--rw-r--r--   0        0        0      185 2023-07-17 15:10:59.922617 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/data_transforms.rst
--rw-r--r--   0        0        0      459 2023-07-17 15:10:59.938618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/engine.rst
--rw-r--r--   0        0        0      144 2023-07-17 15:10:59.942618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/evaluation.rst
--rw-r--r--   0        0        0      203 2023-07-17 15:10:59.946618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/index.rst
--rw-r--r--   0        0        0      132 2023-07-17 15:10:59.954618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/layers.rst
--rw-r--r--   0        0        0      758 2023-07-17 15:10:59.958618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/modeling.rst
--rw-r--r--   0        0        0      132 2023-07-17 15:10:59.966618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/solver.rst
--rw-r--r--   0        0        0     1521 2023-07-17 15:10:59.974618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/utils.rst
--rw-r--r--   0        0        0      180 2023-07-17 15:10:59.982618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/requirements.txt
--rw-r--r--   0        0        0     4756 2023-07-17 15:10:59.982618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fast_reid_interfece.py
--rw-r--r--   0        0        0      104 2023-07-17 15:10:59.982618 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/__init__.py
--rw-r--r--   0        0        0      255 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      266 2023-07-17 15:10:59.990619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/__init__.py
--rw-r--r--   0        0        0      428 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    10089 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/config.cpython-38.pyc
--rw-r--r--   0        0        0     3817 2023-07-18 15:12:32.712317 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/defaults.cpython-38.pyc
--rw-r--r--   0        0        0    11536 2023-07-17 15:11:00.006619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/config.py
--rw-r--r--   0        0        0    10644 2023-07-17 15:11:00.006619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/defaults.py
--rw-r--r--   0        0        0      390 2023-07-17 15:11:00.010619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__init__.py
--rw-r--r--   0        0        0      629 2023-07-17 18:04:56.408559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5228 2023-07-17 18:04:56.424559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     2063 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/common.cpython-38.pyc
--rw-r--r--   0        0        0     5715 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/data_utils.cpython-38.pyc
--rw-r--r--   0        0        0     6208 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/build.py
--rw-r--r--   0        0        0     1496 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/common.py
--rw-r--r--   0        0        0     7044 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/data_utils.py
--rw-r--r--   0        0        0     1505 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/AirportALERT.py
--rw-r--r--   0        0        0     1252 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/AirportALERT.cpython-38.pyc
--rw-r--r--   0        0        0     1753 2023-07-17 18:04:56.432559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6136 2023-07-17 18:04:56.432559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/bases.cpython-38.pyc
--rw-r--r--   0        0        0     1421 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/caviara.cpython-38.pyc
--rw-r--r--   0        0        0     7476 2023-07-17 18:04:56.436559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk03.cpython-38.pyc
--rw-r--r--   0        0        0     1914 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk_sysu.cpython-38.pyc
--rw-r--r--   0        0        0     2306 2023-07-17 18:04:56.436559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/dukemtmcreid.cpython-38.pyc
--rw-r--r--   0        0        0     1457 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/grid.cpython-38.pyc
--rw-r--r--   0        0        0     1499 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/iLIDS.cpython-38.pyc
--rw-r--r--   0        0        0     1562 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/lpw.cpython-38.pyc
--rw-r--r--   0        0        0     2934 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/market1501.cpython-38.pyc
--rw-r--r--   0        0        0     2709 2023-07-17 18:04:56.432559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot17.cpython-38.pyc
--rw-r--r--   0        0        0     2755 2023-07-17 18:04:56.436559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot20.cpython-38.pyc
--rw-r--r--   0        0        0     2800 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/msmt17.cpython-38.pyc
--rw-r--r--   0        0        0     1416 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pes3d.cpython-38.pyc
--rw-r--r--   0        0        0     1439 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pku.cpython-38.pyc
--rw-r--r--   0        0        0     1451 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prai.cpython-38.pyc
--rw-r--r--   0        0        0     1587 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prid.cpython-38.pyc
--rw-r--r--   0        0        0     1524 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/saivt.cpython-38.pyc
--rw-r--r--   0        0        0     1559 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sensereid.cpython-38.pyc
--rw-r--r--   0        0        0     1648 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/shinpuhkan.cpython-38.pyc
--rw-r--r--   0        0        0     1519 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sysu_mm.cpython-38.pyc
--rw-r--r--   0        0        0     1470 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/thermalworld.cpython-38.pyc
--rw-r--r--   0        0        0     3760 2023-07-17 18:04:56.456560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/vehicleid.cpython-38.pyc
--rw-r--r--   0        0        0     2173 2023-07-17 18:04:56.456560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veri.cpython-38.pyc
--rw-r--r--   0        0        0     4434 2023-07-17 18:04:56.456560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veriwild.cpython-38.pyc
--rw-r--r--   0        0        0     1450 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/viper.cpython-38.pyc
--rw-r--r--   0        0        0     2070 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/wildtracker.cpython-38.pyc
--rw-r--r--   0        0        0     5892 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/bases.py
--rw-r--r--   0        0        0     1122 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/caviara.py
--rw-r--r--   0        0        0    12054 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk03.py
--rw-r--r--   0        0        0     1635 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk_sysu.py
--rw-r--r--   0        0        0     2350 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/dukemtmcreid.py
--rw-r--r--   0        0        0     1186 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/grid.py
--rw-r--r--   0        0        0     1295 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/iLIDS.py
--rw-r--r--   0        0        0     1466 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/lpw.py
--rw-r--r--   0        0        0     3171 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/market1501.py
--rw-r--r--   0        0        0     3025 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot17.py
--rw-r--r--   0        0        0     3075 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20.py
--rw-r--r--   0        0        0     3247 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20_.py
--rw-r--r--   0        0        0     3871 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/msmt17.py
--rw-r--r--   0        0        0     1159 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pes3d.py
--rw-r--r--   0        0        0     1169 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pku.py
--rw-r--r--   0        0        0     1178 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prai.py
--rw-r--r--   0        0        0     1199 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prid.py
--rw-r--r--   0        0        0     1305 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/saivt.py
--rw-r--r--   0        0        0     1377 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sensereid.py
--rw-r--r--   0        0        0     1362 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/shinpuhkan.py
--rw-r--r--   0        0        0     1336 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sysu_mm.py
--rw-r--r--   0        0        0     1198 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/thermalworld.py
--rw-r--r--   0        0        0     3837 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/vehicleid.py
--rw-r--r--   0        0        0     2209 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veri.py
--rw-r--r--   0        0        0     4884 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veriwild.py
--rw-r--r--   0        0        0     1226 2023-07-17 15:11:00.226623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/viper.py
--rw-r--r--   0        0        0     1844 2023-07-17 15:11:00.226623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/wildtracker.py
--rw-r--r--   0        0        0      473 2023-07-17 15:11:00.226623 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__init__.py
--rw-r--r--   0        0        0      587 2023-07-17 18:04:56.424559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3580 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/data_sampler.cpython-38.pyc
--rw-r--r--   0        0        0     2408 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/imbalance_sampler.cpython-38.pyc
--rw-r--r--   0        0        0     7396 2023-07-17 18:04:56.424559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/triplet_sampler.cpython-38.pyc
--rw-r--r--   0        0        0     2917 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/data_sampler.py
--rw-r--r--   0        0        0     2241 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/imbalance_sampler.py
--rw-r--r--   0        0        0    10108 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/triplet_sampler.py
--rw-r--r--   0        0        0      246 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__init__.py
--rw-r--r--   0        0        0      547 2023-07-17 18:04:56.408559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22427 2023-07-17 18:04:56.416559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/autoaugment.cpython-38.pyc
--rw-r--r--   0        0        0     2310 2023-07-17 18:04:56.420559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     5060 2023-07-17 18:04:56.420559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/functional.cpython-38.pyc
--rw-r--r--   0        0        0     5517 2023-07-17 18:04:56.420559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/transforms.cpython-38.pyc
--rw-r--r--   0        0        0    29513 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/autoaugment.py
--rw-r--r--   0        0        0     3348 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/build.py
--rw-r--r--   0        0        0     5585 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/functional.py
--rw-r--r--   0        0        0     5713 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/transforms.py
--rw-r--r--   0        0        0      370 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__init__.py
--rw-r--r--   0        0        0      502 2023-07-17 18:04:55.372548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    16531 2023-07-17 18:04:56.408559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/defaults.cpython-38.pyc
--rw-r--r--   0        0        0    18614 2023-07-17 18:04:55.380548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/hooks.cpython-38.pyc
--rw-r--r--   0        0        0     2944 2023-07-17 18:04:56.460560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/launch.cpython-38.pyc
--rw-r--r--   0        0        0    11841 2023-07-17 18:04:55.376548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/train_loop.cpython-38.pyc
--rw-r--r--   0        0        0    20113 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/defaults.py
--rw-r--r--   0        0        0    19298 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/hooks.py
--rw-r--r--   0        0        0     3768 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/launch.py
--rw-r--r--   0        0        0    12215 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/train_loop.py
--rw-r--r--   0        0        0      286 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__init__.py
--rw-r--r--   0        0        0      637 2023-07-17 18:04:55.380548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2547 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/clas_evaluator.cpython-38.pyc
--rw-r--r--   0        0        0     5101 2023-07-17 18:04:55.380548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/evaluator.cpython-38.pyc
--rw-r--r--   0        0        0     1608 2023-07-17 18:04:56.236557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/query_expansion.cpython-38.pyc
--rw-r--r--   0        0        0     4074 2023-07-17 18:04:55.384548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/reid_evaluation.cpython-38.pyc
--rw-r--r--   0        0        0     2460 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/testing.cpython-38.pyc
--rw-r--r--   0        0        0     2295 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/clas_evaluator.py
--rw-r--r--   0        0        0     6660 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/evaluator.py
--rw-r--r--   0        0        0     1701 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/query_expansion.py
--rw-r--r--   0        0        0     7001 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank.py
--rw-r--r--   0        0        0      100 2023-07-17 15:11:00.358626 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/Makefile
--rw-r--r--   0        0        0      480 2023-07-17 15:11:00.358626 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/__init__.py
--rw-r--r--   0        0        0      731 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0  1033326 2023-07-17 15:11:00.406627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.c
--rw-r--r--   0        0        0     9675 2023-07-17 15:11:00.414627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.pyx
--rw-r--r--   0        0        0   908364 2023-07-17 15:11:00.446627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.c
--rw-r--r--   0        0        0     3064 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.pyx
--rw-r--r--   0        0        0      626 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/setup.py
--rw-r--r--   0        0        0     4083 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/test_cython.py
--rw-r--r--   0        0        0     4952 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/reid_evaluation.py
--rw-r--r--   0        0        0     3380 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rerank.py
--rw-r--r--   0        0        0     2784 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/roc.py
--rw-r--r--   0        0        0     2424 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/testing.py
--rw-r--r--   0        0        0      620 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__init__.py
--rw-r--r--   0        0        0      976 2023-07-17 18:04:55.304547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2487 2023-07-17 18:04:55.304547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/activation.cpython-38.pyc
--rw-r--r--   0        0        0     2743 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/any_softmax.cpython-38.pyc
--rw-r--r--   0        0        0     7495 2023-07-17 18:04:55.308547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/batch_norm.cpython-38.pyc
--rw-r--r--   0        0        0     3076 2023-07-17 18:04:55.308547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/context_block.cpython-38.pyc
--rw-r--r--   0        0        0     5722 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/drop.cpython-38.pyc
--rw-r--r--   0        0        0     6176 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/frn.cpython-38.pyc
--rw-r--r--   0        0        0     1261 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/gather_layer.cpython-38.pyc
--rw-r--r--   0        0        0      996 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1658 2023-07-17 18:04:55.316547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/non_local.cpython-38.pyc
--rw-r--r--   0        0        0     5639 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/pooling.cpython-38.pyc
--rw-r--r--   0        0        0     1088 2023-07-17 18:04:55.316547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/se_layer.cpython-38.pyc
--rw-r--r--   0        0        0     3666 2023-07-17 18:04:55.316547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/splat.cpython-38.pyc
--rw-r--r--   0        0        0     3564 2023-07-17 18:04:55.320547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/weight_init.cpython-38.pyc
--rw-r--r--   0        0        0     1334 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/activation.py
--rw-r--r--   0        0        0     2275 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/any_softmax.py
--rw-r--r--   0        0        0     8514 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/batch_norm.py
--rw-r--r--   0        0        0     4244 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/context_block.py
--rw-r--r--   0        0        0     6934 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/drop.py
--rw-r--r--   0        0        0     6499 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/frn.py
--rw-r--r--   0        0        0      816 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/gather_layer.py
--rw-r--r--   0        0        0      724 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/helpers.py
--rw-r--r--   0        0        0     1877 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/non_local.py
--rw-r--r--   0        0        0     3649 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/pooling.py
--rw-r--r--   0        0        0      681 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/se_layer.py
--rw-r--r--   0        0        0     3826 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/splat.py
--rw-r--r--   0        0        0     4216 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/weight_init.py
--rw-r--r--   0        0        0      416 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/__init__.py
--rw-r--r--   0        0        0      728 2023-07-17 18:04:55.288547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      619 2023-07-17 15:11:00.566630 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__init__.py
--rw-r--r--   0        0        0      918 2023-07-17 18:04:55.300547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      871 2023-07-17 18:04:55.300547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     5481 2023-07-17 18:04:55.348547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenet.cpython-38.pyc
--rw-r--r--   0        0        0     9231 2023-07-17 18:04:55.352548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenetv3.cpython-38.pyc
--rw-r--r--   0        0        0    12119 2023-07-17 18:04:55.328547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/osnet.cpython-38.pyc
--rw-r--r--   0        0        0     9497 2023-07-17 18:04:55.352548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/repvgg.cpython-38.pyc
--rw-r--r--   0        0        0     9235 2023-07-17 18:04:55.332547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnest.cpython-38.pyc
--rw-r--r--   0        0        0    10313 2023-07-17 18:04:55.304547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnet.cpython-38.pyc
--rw-r--r--   0        0        0    10098 2023-07-17 18:04:55.332547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnext.cpython-38.pyc
--rw-r--r--   0        0        0     5164 2023-07-17 18:04:55.348547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/shufflenet.cpython-38.pyc
--rw-r--r--   0        0        0    13440 2023-07-17 18:04:55.356547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/vision_transformer.cpython-38.pyc
--rw-r--r--   0        0        0      692 2023-07-17 15:11:00.638631 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/build.py
--rw-r--r--   0        0        0     6479 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenet.py
--rw-r--r--   0        0        0    11726 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenetv3.py
--rw-r--r--   0        0        0    15593 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/osnet.py
--rw-r--r--   0        0        0       86 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__init__.py
--rw-r--r--   0        0        0      292 2023-07-17 18:04:55.336547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4482 2023-07-17 18:04:55.340547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/config.cpython-38.pyc
--rw-r--r--   0        0        0     9617 2023-07-17 18:04:55.344547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/effnet.cpython-38.pyc
--rw-r--r--   0        0        0    21323 2023-07-17 18:04:55.340547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/regnet.cpython-38.pyc
--rw-r--r--   0        0        0    11067 2023-07-17 15:11:00.662631 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/config.py
--rw-r--r--   0        0        0      485 2023-07-17 15:11:00.670632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B0_dds_8gpu.yaml
--rw-r--r--   0        0        0      485 2023-07-17 15:11:00.674632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B1_dds_8gpu.yaml
--rw-r--r--   0        0        0      485 2023-07-17 15:11:00.682632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B2_dds_8gpu.yaml
--rw-r--r--   0        0        0      485 2023-07-17 15:11:00.690632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B3_dds_8gpu.yaml
--rw-r--r--   0        0        0      486 2023-07-17 15:11:00.694632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B4_dds_8gpu.yaml
--rw-r--r--   0        0        0      484 2023-07-17 15:11:00.698632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B5_dds_8gpu.yaml
--rw-r--r--   0        0        0     9933 2023-07-17 15:11:00.698632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet.py
--rw-r--r--   0        0        0    21652 2023-07-17 15:11:00.698632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnet.py
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.706632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-1.6GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      363 2023-07-17 15:11:00.714632 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-12GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.718633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-16GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      361 2023-07-17 15:11:00.726633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-200MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      361 2023-07-17 15:11:00.730633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-3.2GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.734633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-32GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      361 2023-07-17 15:11:00.742633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-4.0GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.746633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-400MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.750633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-6.4GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.762633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-600MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.766633 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-8.0GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      362 2023-07-17 15:11:00.774634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-800MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      376 2023-07-17 15:11:00.782634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-1.6GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      377 2023-07-17 15:11:00.790634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-12GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      378 2023-07-17 15:11:00.794634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-16GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      357 2023-07-17 15:11:00.802634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-200MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      375 2023-07-17 15:11:00.806634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-3.2GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      378 2023-07-17 15:11:00.814634 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-32GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      375 2023-07-17 15:11:00.822635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-4.0GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      375 2023-07-17 15:11:00.830635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-400MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      376 2023-07-17 15:11:00.838635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-6.4GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      376 2023-07-17 15:11:00.846635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-600MF_dds_8gpu.yaml
--rw-r--r--   0        0        0      376 2023-07-17 15:11:00.850635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-8.0GF_dds_8gpu.yaml
--rw-r--r--   0        0        0      375 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-800MF_dds_8gpu.yaml
--rw-r--r--   0        0        0    11722 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/repvgg.py
--rw-r--r--   0        0        0    15306 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnest.py
--rw-r--r--   0        0        0    12509 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnet.py
--rw-r--r--   0        0        0    11941 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnext.py
--rw-r--r--   0        0        0     7091 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/shufflenet.py
--rw-r--r--   0        0        0    16636 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/vision_transformer.py
--rw-r--r--   0        0        0      265 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__init__.py
--rw-r--r--   0        0        0      416 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      822 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     1162 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/clas_head.cpython-38.pyc
--rw-r--r--   0        0        0     3809 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/embedding_head.cpython-38.pyc
--rw-r--r--   0        0        0      630 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/build.py
--rw-r--r--   0        0        0     1050 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/clas_head.py
--rw-r--r--   0        0        0     4772 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/embedding_head.py
--rw-r--r--   0        0        0      313 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__init__.py
--rw-r--r--   0        0        0      608 2023-07-17 18:04:55.288547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1797 2023-07-17 18:04:55.292547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/circle_loss.cpython-38.pyc
--rw-r--r--   0        0        0     1639 2023-07-17 18:04:55.292547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/cross_entroy_loss.cpython-38.pyc
--rw-r--r--   0        0        0     2958 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/focal_loss.cpython-38.pyc
--rw-r--r--   0        0        0     3285 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/triplet_loss.cpython-38.pyc
--rw-r--r--   0        0        0     1859 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     2147 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/circle_loss.py
--rw-r--r--   0        0        0     1610 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/cross_entroy_loss.py
--rw-r--r--   0        0        0     3361 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/focal_loss.py
--rw-r--r--   0        0        0     3957 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/triplet_loss.py
--rw-r--r--   0        0        0     1302 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/utils.py
--rw-r--r--   0        0        0      299 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__init__.py
--rw-r--r--   0        0        0      473 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4325 2023-07-17 18:04:55.368548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/baseline.cpython-38.pyc
--rw-r--r--   0        0        0      919 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     3968 2023-07-17 18:04:55.372548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/distiller.cpython-38.pyc
--rw-r--r--   0        0        0     7310 2023-07-17 18:04:55.368548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/mgn.cpython-38.pyc
--rw-r--r--   0        0        0     3814 2023-07-17 18:04:55.372548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/moco.cpython-38.pyc
--rw-r--r--   0        0        0     6381 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/baseline.py
--rw-r--r--   0        0        0      747 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/build.py
--rw-r--r--   0        0        0     5007 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/distiller.py
--rw-r--r--   0        0        0    13405 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/mgn.py
--rw-r--r--   0        0        0     3978 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/moco.py
--rw-r--r--   0        0        0      138 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/__init__.py
--rw-r--r--   0        0        0      317 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    10015 2023-07-17 18:04:56.244557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     2440 2023-07-17 18:04:56.244557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/lr_scheduler.cpython-38.pyc
--rw-r--r--   0        0        0    12889 2023-07-17 15:11:00.982638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/build.py
--rw-r--r--   0        0        0     2067 2023-07-17 15:11:00.982638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/lr_scheduler.py
--rw-r--r--   0        0        0      179 2023-07-17 15:11:00.982638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__init__.py
--rw-r--r--   0        0        0      382 2023-07-17 18:04:56.244557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3840 2023-07-17 18:04:56.248557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/lamb.cpython-38.pyc
--rw-r--r--   0        0        0     3845 2023-07-17 18:04:56.404559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/radam.cpython-38.pyc
--rw-r--r--   0        0        0    10467 2023-07-17 18:04:56.400559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/swa.cpython-38.pyc
--rw-r--r--   0        0        0     5065 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/lamb.py
--rw-r--r--   0        0        0     5715 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/radam.py
--rw-r--r--   0        0        0    11090 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/swa.py
--rw-r--r--   0        0        0       81 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__init__.py
--rw-r--r--   0        0        0      235 2023-07-17 18:04:55.284547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    16201 2023-07-17 18:04:55.320547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/checkpoint.cpython-38.pyc
--rw-r--r--   0        0        0     3627 2023-07-17 18:04:56.460560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/collect_env.cpython-38.pyc
--rw-r--r--   0        0        0     7239 2023-07-17 18:04:55.324547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/comm.cpython-38.pyc
--rw-r--r--   0        0        0     4886 2023-07-17 18:04:56.156556 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/compute_dist.cpython-38.pyc
--rw-r--r--   0        0        0     3446 2023-07-17 18:04:56.460560 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/env.cpython-38.pyc
--rw-r--r--   0        0        0    15628 2023-07-17 18:04:55.292547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/events.cpython-38.pyc
--rw-r--r--   0        0        0     3057 2023-07-17 18:04:56.236557 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/faiss_utils.cpython-38.pyc
--rw-r--r--   0        0        0    16968 2023-07-17 18:04:55.288547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/file_io.cpython-38.pyc
--rw-r--r--   0        0        0     3051 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/history_buffer.cpython-38.pyc
--rw-r--r--   0        0        0     5883 2023-07-17 18:04:55.384548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/logger.cpython-38.pyc
--rw-r--r--   0        0        0     4055 2023-07-17 18:04:55.376548 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/params.cpython-38.pyc
--rw-r--r--   0        0        0     3603 2023-07-17 18:04:56.404559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/precision_bn.cpython-38.pyc
--rw-r--r--   0        0        0     2267 2023-07-17 18:04:55.300547 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/registry.cpython-38.pyc
--rw-r--r--   0        0        0     2258 2023-07-17 18:04:56.404559 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/timer.cpython-38.pyc
--rw-r--r--   0        0        0    18277 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/checkpoint.py
--rw-r--r--   0        0        0     4693 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/collect_env.py
--rw-r--r--   0        0        0     7676 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/comm.py
--rw-r--r--   0        0        0     6601 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/compute_dist.py
--rw-r--r--   0        0        0     3699 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/env.py
--rw-r--r--   0        0        0    16494 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/events.py
--rw-r--r--   0        0        0     3344 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/faiss_utils.py
--rw-r--r--   0        0        0    19186 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/file_io.py
--rw-r--r--   0        0        0     2273 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/history_buffer.py
--rw-r--r--   0        0        0     7224 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/logger.py
--rw-r--r--   0        0        0     4381 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/params.py
--rw-r--r--   0        0        0     3726 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/precision_bn.py
--rw-r--r--   0        0        0     2051 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/registry.py
--rw-r--r--   0        0        0     4454 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/summary.py
--rw-r--r--   0        0        0     1880 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/timer.py
--rw-r--r--   0        0        0    11831 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/visualizer.py
--rw-r--r--   0        0        0     3530 2023-07-17 15:11:01.098640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/CrossDomainReID/README.md
--rw-r--r--   0        0        0     3989 2023-07-17 15:11:01.106640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/DG-ReID/README.md
--rw-r--r--   0        0        0     1111 2023-07-17 15:11:01.110640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/README.md
--rw-r--r--   0        0        0     1054 2023-07-17 15:11:01.118640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/Base-attribute.yml
--rw-r--r--   0        0        0      189 2023-07-17 15:11:01.126640 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/dukemtmc.yml
--rw-r--r--   0        0        0      195 2023-07-17 15:11:01.134641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/market1501.yml
--rw-r--r--   0        0        0      138 2023-07-17 15:11:01.138641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/pa100.yml
--rw-r--r--   0        0        0      249 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/__init__.py
--rw-r--r--   0        0        0     1188 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_dataset.py
--rw-r--r--   0        0        0     3343 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_evaluation.py
--rw-r--r--   0        0        0      293 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/config.py
--rw-r--r--   0        0        0      215 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/__init__.py
--rw-r--r--   0        0        0     3412 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/bases.py
--rw-r--r--   0        0        0     2451 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/dukemtmcattr.py
--rw-r--r--   0        0        0     3137 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/market1501attr.py
--rw-r--r--   0        0        0     2088 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/pa100k.py
--rw-r--r--   0        0        0      205 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/__init__.py
--rw-r--r--   0        0        0     1285 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_baseline.py
--rw-r--r--   0        0        0     1171 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_head.py
--rw-r--r--   0        0        0      974 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/bce_loss.py
--rw-r--r--   0        0        0     3949 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/train_net.py
--rw-r--r--   0        0        0      574 2023-07-17 15:11:01.154641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/README.md
--rw-r--r--   0        0        0     1144 2023-07-17 15:11:01.158641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/configs/base-clas.yaml
--rw-r--r--   0        0        0      206 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/__init__.py
--rw-r--r--   0        0        0     1441 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/bee_ant.py
--rw-r--r--   0        0        0     1477 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/dataset.py
--rw-r--r--   0        0        0     2824 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/trainer.py
--rw-r--r--   0        0        0     1812 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/train_net.py
--rw-r--r--   0        0        0     1655 2023-07-17 15:11:01.174641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/README.md
--rw-r--r--   0        0        0      415 2023-07-17 15:11:01.178641 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/Base-kd.yml
--rw-r--r--   0        0        0      407 2023-07-17 15:11:01.190642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/kd-sbs_r101ibn-sbs_r34.yml
--rw-r--r--   0        0        0      188 2023-07-17 15:11:01.198642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/sbs_r101ibn.yml
--rw-r--r--   0        0        0      201 2023-07-17 15:11:01.202642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/sbs_r34.yml
--rw-r--r--   0        0        0      181 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/__init__.py
--rw-r--r--   0        0        0     4547 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/overhaul.py
--rw-r--r--   0        0        0    11483 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/resnet_distill.py
--rw-r--r--   0        0        0     1340 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/train_net.py
--rw-r--r--   0        0        0     1200 2023-07-17 15:11:01.214642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/README.md
--rw-r--r--   0        0        0     1169 2023-07-17 15:11:01.218642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/configs/face_base.yml
--rw-r--r--   0        0        0      239 2023-07-17 15:11:01.226642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/configs/r101_ir.yml
--rw-r--r--   0        0        0      198 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/configs/r50_ir.yml
--rw-r--r--   0        0        0      198 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/__init__.py
--rw-r--r--   0        0        0      331 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/config.py
--rw-r--r--   0        0        0      139 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/__init__.py
--rw-r--r--   0        0        0     1042 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/ms1mv2.py
--rw-r--r--   0        0        0     1479 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/test_dataset.py
--rw-r--r--   0        0        0     2382 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_data.py
--rw-r--r--   0        0        0     2247 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_evaluator.py
--rw-r--r--   0        0        0      234 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/__init__.py
--rw-r--r--   0        0        0     1481 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_baseline.py
--rw-r--r--   0        0        0     1097 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_head.py
--rw-r--r--   0        0        0     6407 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/iresnet.py
--rw-r--r--   0        0        0     6976 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/partial_fc.py
--rw-r--r--   0        0        0     3042 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/pfc_checkpointer.py
--rw-r--r--   0        0        0     8528 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/trainer.py
--rw-r--r--   0        0        0     3261 2023-07-17 15:11:01.242643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/utils_amp.py
--rw-r--r--   0        0        0     7666 2023-07-17 15:11:01.242643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/verification.py
--rw-r--r--   0        0        0     1339 2023-07-17 15:11:01.242643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/train_net.py
--rwxr-xr-x   0        0        0       34 2023-07-17 15:11:01.250643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/.gitignore
--rwxr-xr-x   0        0        0     2613 2023-07-17 15:11:01.254643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/CMakeLists.txt
--rwxr-xr-x   0        0        0     9609 2023-07-17 15:11:01.262643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/README.md
--rw-r--r--   0        0        0     1060 2023-07-17 15:11:01.262643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/demo/CMakeLists.txt
--rwxr-xr-x   0        0        0     5398 2023-07-17 15:11:01.266643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/demo/inference.cpp
--rw-r--r--   0        0        0      290 2023-07-17 15:11:01.274643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/docker/trt7cu100/Dockerfile
--rw-r--r--   0        0        0     1019 2023-07-17 15:11:01.278643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/docker/trt7cu102/Dockerfile
--rwxr-xr-x   0        0        0     1219 2023-07-17 15:11:01.286643 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/CMakeLists.txt
--rw-r--r--   0        0        0       85 2023-07-17 15:11:01.290644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/backbones/CMakeLists.txt
--rwxr-xr-x   0        0        0    19621 2023-07-17 15:11:01.298644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/backbones/sbs_resnet.cpp
--rwxr-xr-x   0        0        0     2782 2023-07-17 15:11:01.306644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/calibrator.cpp
--rw-r--r--   0        0        0     3694 2023-07-17 15:11:01.310644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/utils.cpp
--rw-r--r--   0        0        0       90 2023-07-17 15:11:01.318644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/engine/CMakeLists.txt
--rwxr-xr-x   0        0        0     3852 2023-07-17 15:11:01.322644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/engine/InferenceEngine.cpp
--rw-r--r--   0        0        0      135 2023-07-17 15:11:01.326644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/factory/CMakeLists.txt
--rwxr-xr-x   0        0        0     3559 2023-07-17 15:11:01.330644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/factory/factory.cpp
--rw-r--r--   0        0        0       89 2023-07-17 15:11:01.338644 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/heads/CMakeLists.txt
--rw-r--r--   0        0        0     1722 2023-07-17 15:11:01.346645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/heads/embedding_head.cpp
--rw-r--r--   0        0        0      177 2023-07-17 15:11:01.350645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/CMakeLists.txt
--rw-r--r--   0        0        0    22672 2023-07-17 15:11:01.354645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/layers.cpp
--rw-r--r--   0        0        0     1580 2023-07-17 15:11:01.362645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.cpp
--rw-r--r--   0        0        0     1207 2023-07-17 15:11:01.366645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.h
--rw-r--r--   0        0        0      123 2023-07-17 15:11:01.370645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/CMakeLists.txt
--rwxr-xr-x   0        0        0     1031 2023-07-17 15:11:01.374645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/baseline.cpp
--rwxr-xr-x   0        0        0     5605 2023-07-17 15:11:01.382645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/model.cpp
--rw-r--r--   0        0        0      405 2023-07-17 15:11:01.386645 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/IPoolingLayerRT.h
--rwxr-xr-x   0        0        0     2106 2023-07-17 15:11:01.394646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/InferenceEngine.h
--rw-r--r--   0        0        0      660 2023-07-17 15:11:01.398646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/baseline.h
--rwxr-xr-x   0        0        0     1173 2023-07-17 15:11:01.406646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/calibrator.h
--rwxr-xr-x   0        0        0      139 2023-07-17 15:11:01.414646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/config.h.in
--rwxr-xr-x   0        0        0      417 2023-07-17 15:11:01.418646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/cuda_utils.h
--rw-r--r--   0        0        0      675 2023-07-17 15:11:01.426646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/embedding_head.h
--rw-r--r--   0        0        0      584 2023-07-17 15:11:01.430646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/factory.h
--rwxr-xr-x   0        0        0     1060 2023-07-17 15:11:01.438646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/holder.h
--rw-r--r--   0        0        0     3175 2023-07-17 15:11:01.442646 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/layers.h
--rw-r--r--   0        0        0    16550 2023-07-17 15:11:01.446647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/logging.h
--rwxr-xr-x   0        0        0     2081 2023-07-17 15:11:01.454647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/model.h
--rw-r--r--   0        0        0      376 2023-07-17 15:11:01.458647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/module.h
--rwxr-xr-x   0        0        0     2086 2023-07-17 15:11:01.466647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/sbs_resnet.h
--rwxr-xr-x   0        0        0     1932 2023-07-17 15:11:01.470647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/struct.h
--rwxr-xr-x   0        0        0     2151 2023-07-17 15:11:01.470647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/utils.h
--rwxr-xr-x   0        0        0      960 2023-07-17 15:11:01.478647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/CMakeLists.txt
--rw-r--r--   0        0        0     1064 2023-07-17 15:11:01.482647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/docker/trt7cu100/Dockerfile
--rwxr-xr-x   0        0        0      325 2023-07-17 15:11:01.490647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/docker/trt7cu102_torch160/Dockerfile
--rwxr-xr-x   0        0        0     1765 2023-07-17 15:11:01.490647 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/market_benchmark.py
--rwxr-xr-x   0        0        0     4977 2023-07-17 15:11:01.494648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/reid.cpp
--rwxr-xr-x   0        0        0      550 2023-07-17 15:11:01.494648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/test.py
--rw-r--r--   0        0        0     1053 2023-07-17 15:11:01.502648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/CMakeLists.txt
--rw-r--r--   0        0        0     1073 2023-07-17 15:11:01.506648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/LICENSE
--rw-r--r--   0        0        0     2103 2023-07-17 15:11:01.510648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/README.md
--rw-r--r--   0        0        0    11468 2023-07-17 15:11:01.518648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.cpp
--rw-r--r--   0        0        0    10917 2023-07-17 15:11:01.522648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.h
--rw-r--r--   0        0        0     1961 2023-07-17 15:11:01.530648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/example1.cpp
--rw-r--r--   0        0        0      333 2023-07-17 15:11:01.538648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/mat2npz
--rw-r--r--   0        0        0      253 2023-07-17 15:11:01.542648 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/npy2mat
--rwxr-xr-x   0        0        0      271 2023-07-17 15:11:01.550649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/npz2mat
--rw-r--r--   0        0        0     2941 2023-07-17 15:11:01.554649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/tools/How_to_Generate.md
--rw-r--r--   0        0        0     3206 2023-07-17 15:11:01.554649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/tools/gen_wts.py
--rw-r--r--   0        0        0     2422 2023-07-17 15:11:01.566649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/README.md
--rw-r--r--   0        0        0     1202 2023-07-17 15:11:01.570649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/base-image_retri.yml
--rw-r--r--   0        0        0      451 2023-07-17 15:11:01.578649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/cars.yml
--rw-r--r--   0        0        0      457 2023-07-17 15:11:01.582649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/cub.yml
--rw-r--r--   0        0        0      324 2023-07-17 15:11:01.586649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/inshop.yml
--rw-r--r--   0        0        0      263 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/sop.yml
--rw-r--r--   0        0        0      189 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/__init__.py
--rw-r--r--   0        0        0      169 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/config.py
--rw-r--r--   0        0        0     2548 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/datasets.py
--rw-r--r--   0        0        0     4726 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/retri_evaluator.py
--rw-r--r--   0        0        0     1656 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/train_net.py
--rw-r--r--   0        0        0      572 2023-07-17 15:11:01.602650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/README.md
--rw-r--r--   0        0        0      123 2023-07-17 15:11:01.602650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/autotuner/__init__.py
--rw-r--r--   0        0        0     1850 2023-07-17 15:11:01.602650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/autotuner/tune_hooks.py
--rw-r--r--   0        0        0     1520 2023-07-17 15:11:01.606650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/configs/search_trial.yml
--rw-r--r--   0        0        0     8384 2023-07-17 15:11:01.610650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/tune_net.py
--rw-r--r--   0        0        0     1497 2023-07-17 15:11:01.614650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/HAA/Readme.md
--rw-r--r--   0        0        0     3135 2023-07-17 15:11:01.618650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/README.md
--rw-r--r--   0        0        0     1514 2023-07-17 15:11:01.626650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/Base-naic.yml
--rw-r--r--   0        0        0      179 2023-07-17 15:11:01.630650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/nest101-base.yml
--rw-r--r--   0        0        0      194 2023-07-17 15:11:01.638650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/r34-ibn.yml
--rw-r--r--   0        0        0      412 2023-07-17 15:11:01.642650 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/submit.yml
--rw-r--r--   0        0        0  1342300 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/label.txt
--rw-r--r--   0        0        0      189 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/__init__.py
--rw-r--r--   0        0        0      187 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/config.py
--rw-r--r--   0        0        0     7671 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_dataset.py
--rw-r--r--   0        0        0     3922 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_evaluator.py
--rw-r--r--   0        0        0  3757537 2023-07-17 15:11:01.794653 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic20r2_train_list_clean.txt
--rw-r--r--   0        0        0  1090705 2023-07-17 15:11:01.830654 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/train_list_clean.txt
--rw-r--r--   0        0        0     2192 2023-07-17 15:11:01.830654 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/train_net.py
--rw-r--r--   0        0        0   353057 2023-07-17 15:11:01.846654 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/val_gallery.txt
--rw-r--r--   0        0        0    48120 2023-07-17 15:11:01.854654 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/val_query.txt
--rw-r--r--   0        0        0     3019 2023-07-17 15:11:01.862655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/README.md
--rw-r--r--   0        0        0     1170 2023-07-17 15:11:01.866655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/configs/partial_market.yml
--rw-r--r--   0        0        0      274 2023-07-17 15:11:01.870655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/__init__.py
--rw-r--r--   0        0        0      224 2023-07-17 15:11:01.882655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/config.py
--rw-r--r--   0        0        0     1883 2023-07-17 15:11:01.890655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_distance.py
--rw-r--r--   0        0        0     4413 2023-07-17 15:11:01.898655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_evaluation.py
--rw-r--r--   0        0        0     5947 2023-07-17 15:11:01.906655 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_head.py
--rw-r--r--   0        0        0     2266 2023-07-17 15:11:01.918656 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partial_dataset.py
--rw-r--r--   0        0        0     1502 2023-07-17 15:11:01.926656 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partialbaseline.py
--rw-r--r--   0        0        0     2416 2023-07-17 15:11:01.930656 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/train_net.py
--rw-r--r--   0        0        0     1602 2023-07-17 15:11:01.946656 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/README.md
--rw-r--r--   0        0        0       80 2023-07-17 15:11:01.950656 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/__init__.py
--rw-r--r--   0        0        0     1414 2023-07-17 15:11:01.958656 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/dataset_test.py
--rw-r--r--   0        0        0     1226 2023-07-17 15:11:01.966657 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/feature_align.py
--rw-r--r--   0        0        0      676 2023-07-17 15:11:01.982657 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/interp_test.py
--rw-r--r--   0        0        0      646 2023-07-17 15:11:01.990657 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/lr_scheduler_test.py
--rw-r--r--   0        0        0     1217 2023-07-17 15:11:01.998657 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/model_test.py
--rw-r--r--   0        0        0      375 2023-07-17 15:11:02.006657 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/sampler_test.py
--rw-r--r--   0        0        0      804 2023-07-17 15:11:02.014658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/test_repvgg.py
--rw-r--r--   0        0        0     1369 2023-07-17 15:11:02.046658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/ReadMe.md
--rw-r--r--   0        0        0        0 2023-07-17 15:11:02.050658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/__init__.py
--rw-r--r--   0        0        0    93270 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe.proto
--rw-r--r--   0        0        0      984 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_lmdb.py
--rw-r--r--   0        0        0     4756 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_net.py
--rw-r--r--   0        0        0   502318 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_pb2.py
--rw-r--r--   0        0        0     5605 2023-07-17 15:11:02.062658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/layer_param.py
--rw-r--r--   0        0        0      100 2023-07-17 15:11:02.062658 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/net.py
--rw-r--r--   0        0        0     5305 2023-07-17 15:11:02.066659 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/README.md
--rw-r--r--   0        0        0     2282 2023-07-17 15:11:02.090659 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/caffe_export.py
--rw-r--r--   0        0        0     2823 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/caffe_inference.py
--rw-r--r--   0        0        0     4758 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/onnx_export.py
--rw-r--r--   0        0        0     2384 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/onnx_inference.py
--rw-r--r--   0        0        0    28802 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/pytorch_to_caffe.py
--rw-r--r--   0        0        0     2223 2023-07-17 15:11:02.150660 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0022_c6s1_002976_01.jpg
--rw-r--r--   0        0        0     2137 2023-07-17 15:11:02.162660 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0027_c2s2_091032_02.jpg
--rw-r--r--   0        0        0     2640 2023-07-17 15:11:02.170661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0032_c6s1_002851_01.jpg
--rw-r--r--   0        0        0     2149 2023-07-17 15:11:02.194661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0048_c1s1_005351_01.jpg
--rw-r--r--   0        0        0     1890 2023-07-17 15:11:02.198661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0065_c6s1_009501_02.jpg
--rw-r--r--   0        0        0     3554 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/trt_calibrator.py
--rw-r--r--   0        0        0     5602 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/trt_export.py
--rw-r--r--   0        0        0     6593 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/trt_inference.py
--rw-r--r--   0        0        0     7297 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/plain_train_net.py
--rw-r--r--   0        0        0     1321 2023-07-17 15:11:02.206661 initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/train_net.py
--rw-r--r--   0        0        0    11436 2023-07-18 15:18:02.865987 initor_bot_inference-2.0.1/src/initor_bot_inference/tools/__pycache__/demo.cpython-38.pyc
--rw-r--r--   0        0        0    15887 2023-07-18 15:19:40.319596 initor_bot_inference-2.0.1/src/initor_bot_inference/tools/demo.py
--rw-r--r--   0        0        0    18079 2023-07-17 15:12:35.360422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-02.txt
--rw-r--r--   0        0        0    31683 2023-07-17 15:12:35.364422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-04.txt
--rw-r--r--   0        0        0    25490 2023-07-17 15:12:35.372422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-05.txt
--rw-r--r--   0        0        0    15909 2023-07-17 15:12:35.380422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-09.txt
--rw-r--r--   0        0        0    19852 2023-07-17 15:12:35.384422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-10.txt
--rw-r--r--   0        0        0    27360 2023-07-17 15:12:35.388422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-11.txt
--rw-r--r--   0        0        0    23091 2023-07-17 15:12:35.396422 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-13.txt
--rw-r--r--   0        0        0    27319 2023-07-17 15:12:35.404423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-01.txt
--rw-r--r--   0        0        0    36372 2023-07-17 15:12:35.408423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-02.txt
--rw-r--r--   0        0        0    91385 2023-07-17 15:12:35.420423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-03.txt
--rw-r--r--   0        0        0    63832 2023-07-17 15:12:35.424423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-04.txt
--rw-r--r--   0        0        0    51181 2023-07-17 15:12:35.432423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-05.txt
--rw-r--r--   0        0        0    73362 2023-07-17 15:12:35.440423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-06.txt
--rw-r--r--   0        0        0    30617 2023-07-17 15:12:35.448423 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-07.txt
--rw-r--r--   0        0        0    37991 2023-07-17 15:12:35.452424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-08.txt
--rw-r--r--   0        0        0    31899 2023-07-17 15:12:35.460424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-09.txt
--rw-r--r--   0        0        0    39983 2023-07-17 15:12:35.468424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-10.txt
--rw-r--r--   0        0        0    55004 2023-07-17 15:12:35.472424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-11.txt
--rw-r--r--   0        0        0    55025 2023-07-17 15:12:35.480424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-12.txt
--rw-r--r--   0        0        0    46217 2023-07-17 15:12:35.488424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-13.txt
--rw-r--r--   0        0        0    46034 2023-07-17 15:12:35.496425 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-14.txt
--rw-r--r--   0        0        0    25981 2023-07-17 15:12:35.500424 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-01.txt
--rw-r--r--   0        0        0   170865 2023-07-17 15:12:35.520425 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-02.txt
--rw-r--r--   0        0        0   147829 2023-07-17 15:12:35.536425 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-03.txt
--rw-r--r--   0        0        0   127752 2023-07-17 15:12:35.544425 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-04.txt
--rw-r--r--   0        0        0   204914 2023-07-17 15:12:35.556426 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-05.txt
--rw-r--r--   0        0        0    61339 2023-07-17 15:12:35.564426 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-06.txt
--rw-r--r--   0        0        0    35519 2023-07-17 15:12:35.568426 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-07.txt
--rw-r--r--   0        0        0    49029 2023-07-17 15:12:35.576426 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-08.txt
--rw-r--r--   0        0        0     2159 2023-07-17 18:04:55.260546 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/basetrack.cpython-38.pyc
--rw-r--r--   0        0        0    12369 2023-07-17 18:04:54.908542 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/bot_sort.cpython-38.pyc
--rw-r--r--   0        0        0     6224 2023-07-17 18:04:55.260546 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/gmc.cpython-38.pyc
--rw-r--r--   0        0        0     8086 2023-07-17 18:04:55.256546 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/kalman_filter.cpython-38.pyc
--rw-r--r--   0        0        0     6739 2023-07-17 18:04:54.908542 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/matching.cpython-38.pyc
--rw-r--r--   0        0        0     1111 2023-07-17 15:12:35.624427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/basetrack.py
--rw-r--r--   0        0        0    16778 2023-07-17 15:12:35.624427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/bot_sort.py
--rw-r--r--   0        0        0    11753 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/gmc.py
--rw-r--r--   0        0        0     9671 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/kalman_filter.py
--rw-r--r--   0        0        0     6435 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/matching.py
--rw-r--r--   0        0        0    17072 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/mc_bot_sort.py
--rw-r--r--   0        0        0     1158 2023-07-17 15:12:35.632427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-37.pyc
--rw-r--r--   0        0        0     1139 2023-07-17 18:04:56.464560 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-38.pyc
--rw-r--r--   0        0        0     4050 2023-07-17 15:12:35.640427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/evaluation.py
--rw-r--r--   0        0        0     3627 2023-07-17 15:12:35.640427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/io.py
--rw-r--r--   0        0        0      958 2023-07-17 15:12:35.640427 initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/timer.py
--rwxr-xr-x   0        0        0  7620976 2023-07-17 15:12:35.860431 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/_C.cpython-38-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      126 2023-07-17 15:12:35.860431 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/__init__.py
--rw-r--r--   0        0        0      229 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      152 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/core/__init__.py
--rw-r--r--   0        0        0     7038 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/core/launch.py
--rw-r--r--   0        0        0    10932 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/core/trainer.py
--rw-r--r--   0        0        0      330 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__init__.py
--rw-r--r--   0        0        0      457 2023-07-17 15:12:35.908432 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      456 2023-07-17 18:04:54.404537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7352 2023-07-17 15:12:35.932433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-37.pyc
--rw-r--r--   0        0        0     7428 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-38.pyc
--rw-r--r--   0        0        0     2524 2023-07-17 15:12:35.944433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-37.pyc
--rw-r--r--   0        0        0     2553 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-38.pyc
--rw-r--r--   0        0        0     5419 2023-07-17 15:12:35.960433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-37.pyc
--rw-r--r--   0        0        0     5438 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-38.pyc
--rw-r--r--   0        0        0     3992 2023-07-17 15:12:35.972433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-37.pyc
--rw-r--r--   0        0        0     4035 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-38.pyc
--rw-r--r--   0        0        0     9378 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/data_augment.py
--rw-r--r--   0        0        0     2298 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/data_prefetcher.py
--rw-r--r--   0        0        0     6231 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/dataloading.py
--rw-r--r--   0        0        0      240 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__init__.py
--rw-r--r--   0        0        0      356 2023-07-17 15:12:36.008434 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      355 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4275 2023-07-17 15:12:36.024434 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-37.pyc
--rw-r--r--   0        0        0     4246 2023-07-17 18:04:54.412537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-38.pyc
--rw-r--r--   0        0        0     6232 2023-07-17 15:12:36.036435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-37.pyc
--rw-r--r--   0        0        0     6311 2023-07-17 18:04:54.412537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-38.pyc
--rw-r--r--   0        0        0     4818 2023-07-17 18:04:54.412537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/mot.cpython-38.pyc
--rw-r--r--   0        0        0     4250 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/datasets_wrapper.py
--rw-r--r--   0        0        0    10196 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/mosaicdetection.py
--rw-r--r--   0        0        0     4532 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/mot.py
--rw-r--r--   0        0        0     3356 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/samplers.py
--rw-r--r--   0        0        0      178 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/__init__.py
--rw-r--r--   0        0        0     7476 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/coco_evaluator.py
--rw-r--r--   0        0        0     6562 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/evaluation.py
--rw-r--r--   0        0        0    31896 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/mot_evaluator.py
--rw-r--r--   0        0        0      191 2023-07-17 15:12:36.056435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__init__.py
--rw-r--r--   0        0        0      269 2023-07-17 15:12:36.060435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      268 2023-07-17 18:04:54.896542 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2782 2023-07-17 15:12:36.076435 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-37.pyc
--rw-r--r--   0        0        0     2843 2023-07-17 18:04:54.896542 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-38.pyc
--rw-r--r--   0        0        0     1511 2023-07-17 15:12:36.088436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-37.pyc
--rw-r--r--   0        0        0     1532 2023-07-17 18:04:54.900542 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-38.pyc
--rw-r--r--   0        0        0     6032 2023-07-17 15:12:36.100436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-37.pyc
--rw-r--r--   0        0        0     6045 2023-07-17 18:04:54.904543 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-38.pyc
--rw-r--r--   0        0        0     2004 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/base_exp.py
--rw-r--r--   0        0        0     1493 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/build.py
--rw-r--r--   0        0        0     8227 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/yolox_base.py
--rw-r--r--   0        0        0     1320 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/nano.py
--rw-r--r--   0        0        0     3006 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolov3.py
--rw-r--r--   0        0        0      355 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolox_l.py
--rw-r--r--   0        0        0      357 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolox_m.py
--rw-r--r--   0        0        0      357 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolox_s.py
--rw-r--r--   0        0        0      496 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolox_tiny.py
--rw-r--r--   0        0        0      357 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolox_x.py
--rw-r--r--   0        0        0     3381 2023-07-17 15:12:36.128436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_ablation.cpython-37.pyc
--rw-r--r--   0        0        0     3383 2023-07-17 15:12:36.136436 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-37.pyc
--rw-r--r--   0        0        0     3420 2023-07-18 15:12:13.551974 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-38.pyc
--rw-r--r--   0        0        0     3384 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_mot20_ch.cpython-37.pyc
--rw-r--r--   0        0        0     4352 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_l_mix_det.py
--rw-r--r--   0        0        0     4354 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_m_mix_det.py
--rw-r--r--   0        0        0     5189 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_nano_mix_det.py
--rw-r--r--   0        0        0     4354 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_s_mix_det.py
--rw-r--r--   0        0        0     4387 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_tiny_mix_det.py
--rw-r--r--   0        0        0     4358 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ablation.py
--rw-r--r--   0        0        0     4354 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ch.py
--rw-r--r--   0        0        0     4605 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_det.py
--rw-r--r--   0        0        0     4498 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_mot20_ch.py
--rw-r--r--   0        0        0     4356 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mot17_half.py
--rw-r--r--   0        0        0      151 2023-07-17 15:12:36.152437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/__init__.py
--rw-r--r--   0        0        0    20824 2023-07-17 15:12:36.160437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.cpp
--rw-r--r--   0        0        0     3485 2023-07-17 15:12:36.164437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.h
--rw-r--r--   0        0        0      524 2023-07-17 15:12:36.172437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/csrc/vision.cpp
--rw-r--r--   0        0        0     5757 2023-07-17 15:12:36.172437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/fast_coco_eval_api.py
--rw-r--r--   0        0        0      297 2023-07-17 15:12:36.172437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__init__.py
--rw-r--r--   0        0        0      417 2023-07-17 15:12:36.184437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      414 2023-07-18 15:12:13.555975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4611 2023-07-17 15:12:36.196437 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-37.pyc
--rw-r--r--   0        0        0     4579 2023-07-18 15:12:13.555975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-38.pyc
--rw-r--r--   0        0        0     2903 2023-07-17 15:12:36.208438 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-37.pyc
--rw-r--r--   0        0        0     2930 2023-07-18 15:12:13.559975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-38.pyc
--rw-r--r--   0        0        0     6970 2023-07-17 15:12:36.220438 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-37.pyc
--rw-r--r--   0        0        0     6954 2023-07-18 15:12:13.559975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-38.pyc
--rw-r--r--   0        0        0     2557 2023-07-17 15:12:36.236438 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-37.pyc
--rw-r--r--   0        0        0     2584 2023-07-18 15:12:13.559975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-38.pyc
--rw-r--r--   0        0        0    11850 2023-07-17 15:12:36.248438 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-37.pyc
--rw-r--r--   0        0        0    12118 2023-07-18 15:12:13.563975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-38.pyc
--rw-r--r--   0        0        0     2495 2023-07-17 15:12:36.264439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-37.pyc
--rw-r--r--   0        0        0     2556 2023-07-18 15:12:13.567975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-38.pyc
--rw-r--r--   0        0        0     1300 2023-07-17 15:12:36.280439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-37.pyc
--rw-r--r--   0        0        0     1315 2023-07-18 15:12:13.567975 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-38.pyc
--rw-r--r--   0        0        0     6028 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/darknet.py
--rw-r--r--   0        0        0     2900 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/losses.py
--rw-r--r--   0        0        0     6102 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/network_blocks.py
--rw-r--r--   0        0        0     2486 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolo_fpn.py
--rw-r--r--   0        0        0    24140 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolo_head.py
--rw-r--r--   0        0        0     3540 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolo_pafpn.py
--rw-r--r--   0        0        0     1374 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolox.py
--rw-r--r--   0        0        0     3437 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/train.py
--rw-r--r--   0        0        0      450 2023-07-17 15:12:36.292439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__init__.py
--rw-r--r--   0        0        0      522 2023-07-17 15:12:36.296439 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      521 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3293 2023-07-17 15:12:36.308440 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-37.pyc
--rw-r--r--   0        0        0     3328 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-38.pyc
--rw-r--r--   0        0        0     3969 2023-07-17 15:12:36.324440 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-37.pyc
--rw-r--r--   0        0        0     4012 2023-07-17 18:04:54.016533 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-38.pyc
--rw-r--r--   0        0        0     1143 2023-07-17 15:12:36.332440 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-37.pyc
--rw-r--r--   0        0        0     1160 2023-07-17 18:04:54.340536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-38.pyc
--rw-r--r--   0        0        0     2601 2023-07-17 15:12:36.344440 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-37.pyc
--rw-r--r--   0        0        0     2607 2023-07-17 18:04:54.340536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-38.pyc
--rw-r--r--   0        0        0     6504 2023-07-17 15:12:36.360441 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-37.pyc
--rw-r--r--   0        0        0     6511 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-38.pyc
--rw-r--r--   0        0        0     2719 2023-07-17 15:12:36.372441 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-37.pyc
--rw-r--r--   0        0        0     2736 2023-07-17 18:04:54.344536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-38.pyc
--rw-r--r--   0        0        0     2888 2023-07-17 15:12:36.384441 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-37.pyc
--rw-r--r--   0        0        0     2913 2023-07-17 18:04:54.344536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-38.pyc
--rw-r--r--   0        0        0     3974 2023-07-17 15:12:36.396441 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-37.pyc
--rw-r--r--   0        0        0     3982 2023-07-17 18:04:54.344536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-38.pyc
--rw-r--r--   0        0        0     4477 2023-07-17 15:12:36.412441 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-37.pyc
--rw-r--r--   0        0        0     4546 2023-07-17 18:04:54.348536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0     2725 2023-07-17 15:12:36.424442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-37.pyc
--rw-r--r--   0        0        0     2750 2023-07-17 18:04:54.348536 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-38.pyc
--rw-r--r--   0        0        0     1336 2023-07-17 15:12:36.436442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-37.pyc
--rw-r--r--   0        0        0     1345 2023-07-17 18:04:54.396537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-38.pyc
--rw-r--r--   0        0        0     3636 2023-07-17 18:04:54.400537 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/visualize.cpython-38.pyc
--rw-r--r--   0        0        0     2845 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/allreduce_norm.py
--rw-r--r--   0        0        0     4269 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/boxes.py
--rw-r--r--   0        0        0     1331 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/checkpoint.py
--rw-r--r--   0        0        0     2806 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/demo_utils.py
--rw-r--r--   0        0        0     7066 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/dist.py
--rw-r--r--   0        0        0     2533 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/ema.py
--rw-r--r--   0        0        0     2751 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/logger.py
--rw-r--r--   0        0        0     6561 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/lr_scheduler.py
--rw-r--r--   0        0        0     3094 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/metric.py
--rw-r--r--   0        0        0     3269 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/model_utils.py
--rw-r--r--   0        0        0     1574 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/setup_env.py
--rw-r--r--   0        0        0     4958 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/visualize.py
--rw-r--r--   0        0        0     7857 2023-07-19 12:14:28.866214 initor_bot_inference-2.0.1/setup.py
--rw-r--r--   0        0        0     1373 2023-07-19 12:14:28.866730 initor_bot_inference-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      797 2023-07-19 12:17:15.086776 initor_bot_inference-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-07-19 12:14:00.763945 initor_bot_inference-2.0.2/src/initor_bot_inference/__init__.py
+-rw-r--r--   0        0        0     3746 2023-07-17 15:10:59.190603 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/FastReID-Logo.png
+-rw-r--r--   0        0        0      955 2023-07-17 15:10:59.198603 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/bugs.md
+-rw-r--r--   0        0        0      448 2023-07-17 15:10:59.206603 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      820 2023-07-17 15:10:59.214604 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/questions-help-support.md
+-rw-r--r--   0        0        0     1087 2023-07-17 15:10:59.230604 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/unexpected-problems-bugs.md
+-rw-r--r--   0        0        0   278762 2023-07-17 15:10:59.254604 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/wechat_group.png
+-rw-r--r--   0        0        0      640 2023-07-17 15:10:59.262605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/workflows/issue_auto_close.yml
+-rw-r--r--   0        0        0      563 2023-07-17 15:10:59.270605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/workflows/lint_python.yml
+-rw-r--r--   0        0        0      333 2023-07-17 15:10:59.270605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.gitignore
+-rw-r--r--   0        0        0      832 2023-07-17 15:10:59.278605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/CHANGELOG.md
+-rw-r--r--   0        0        0     2219 2023-07-17 15:10:59.286605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/GETTING_STARTED.md
+-rw-r--r--   0        0        0      798 2023-07-17 15:10:59.294605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/INSTALL.md
+-rw-r--r--   0        0        0    11347 2023-07-17 15:10:59.302605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/LICENSE
+-rw-r--r--   0        0        0    14758 2023-07-17 15:10:59.310605 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/MODEL_ZOO.md
+-rw-r--r--   0        0        0     4264 2023-07-17 15:10:59.318606 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/README.md
+-rw-r--r--   0        0        0     3674 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/__pycache__/fast_reid_interfece.cpython-38.pyc
+-rw-r--r--   0        0        0      285 2023-07-17 15:10:59.334606 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Base-AGW.yml
+-rw-r--r--   0        0        0      161 2023-07-17 15:10:59.338606 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Base-MGN.yml
+-rw-r--r--   0        0        0      921 2023-07-17 15:10:59.346606 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Base-SBS.yml
+-rw-r--r--   0        0        0     1112 2023-07-17 15:10:59.354606 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Base-bagtricks.yml
+-rw-r--r--   0        0        0      176 2023-07-17 15:10:59.358606 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_R101-ibn.yml
+-rw-r--r--   0        0        0      159 2023-07-17 15:10:59.366607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_R50-ibn.yml
+-rw-r--r--   0        0        0      116 2023-07-17 15:10:59.374607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_R50.yml
+-rw-r--r--   0        0        0      169 2023-07-17 15:10:59.382607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/AGW_S50.yml
+-rw-r--r--   0        0        0      188 2023-07-17 15:10:59.390607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_R101-ibn.yml
+-rw-r--r--   0        0        0      171 2023-07-17 15:10:59.402607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0      128 2023-07-17 15:10:59.410607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_R50.yml
+-rw-r--r--   0        0        0      181 2023-07-17 15:10:59.414607 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/bagtricks_S50.yml
+-rw-r--r--   0        0        0      159 2023-07-17 15:10:59.422608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/mgn_R50-ibn.yml
+-rw-r--r--   0        0        0      176 2023-07-17 15:10:59.430608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_R101-ibn.yml
+-rw-r--r--   0        0        0      159 2023-07-17 15:10:59.434608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_R50-ibn.yml
+-rw-r--r--   0        0        0      116 2023-07-17 15:10:59.442608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_R50.yml
+-rw-r--r--   0        0        0      169 2023-07-17 15:10:59.446608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/DukeMTMC/sbs_S50.yml
+-rw-r--r--   0        0        0      167 2023-07-17 15:10:59.454608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_R101-ibn.yml
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.458608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_R50-ibn.yml
+-rw-r--r--   0        0        0      107 2023-07-17 15:10:59.466608 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_R50.yml
+-rw-r--r--   0        0        0      160 2023-07-17 15:10:59.474609 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/AGW_S50.yml
+-rw-r--r--   0        0        0      179 2023-07-17 15:10:59.482609 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_R101-ibn.yml
+-rw-r--r--   0        0        0      162 2023-07-17 15:10:59.490609 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0      119 2023-07-17 15:10:59.498609 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_R50.yml
+-rw-r--r--   0        0        0      172 2023-07-17 15:10:59.510609 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/bagtricks_S50.yml
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.518609 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/mgn_R50-ibn.yml
+-rw-r--r--   0        0        0      167 2023-07-17 15:10:59.526610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_R101-ibn.yml
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.534610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_R50-ibn.yml
+-rw-r--r--   0        0        0      107 2023-07-17 15:10:59.542610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_R50.yml
+-rw-r--r--   0        0        0      160 2023-07-17 15:10:59.550610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT17/sbs_S50.yml
+-rw-r--r--   0        0        0      167 2023-07-17 15:10:59.558610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_R101-ibn.yml
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.566610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_R50-ibn.yml
+-rw-r--r--   0        0        0      107 2023-07-17 15:10:59.570610 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_R50.yml
+-rw-r--r--   0        0        0      160 2023-07-17 15:10:59.578611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/AGW_S50.yml
+-rw-r--r--   0        0        0      179 2023-07-17 15:10:59.586611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_R101-ibn.yml
+-rw-r--r--   0        0        0      162 2023-07-17 15:10:59.594611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0      119 2023-07-17 15:10:59.602611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_R50.yml
+-rw-r--r--   0        0        0      172 2023-07-17 15:10:59.606611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/bagtricks_S50.yml
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.614611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/mgn_R50-ibn.yml
+-rw-r--r--   0        0        0      167 2023-07-17 15:10:59.622611 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_R101-ibn.yml
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.630612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_R50-ibn.yml
+-rw-r--r--   0        0        0      107 2023-07-17 15:10:59.638612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_R50.yml
+-rw-r--r--   0        0        0      160 2023-07-17 15:10:59.646612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MOT20/sbs_S50.yml
+-rw-r--r--   0        0        0      170 2023-07-17 15:10:59.654612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_R101-ibn.yml
+-rw-r--r--   0        0        0      153 2023-07-17 15:10:59.662612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_R50-ibn.yml
+-rw-r--r--   0        0        0      110 2023-07-17 15:10:59.666612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_R50.yml
+-rw-r--r--   0        0        0      163 2023-07-17 15:10:59.674612 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/AGW_S50.yml
+-rw-r--r--   0        0        0      183 2023-07-17 15:10:59.678613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_R101-ibn.yml
+-rw-r--r--   0        0        0      166 2023-07-17 15:10:59.686613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0      122 2023-07-17 15:10:59.690613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_R50.yml
+-rw-r--r--   0        0        0      176 2023-07-17 15:10:59.698613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/bagtricks_S50.yml
+-rw-r--r--   0        0        0      153 2023-07-17 15:10:59.706613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/mgn_R50-ibn.yml
+-rw-r--r--   0        0        0      170 2023-07-17 15:10:59.710613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_R101-ibn.yml
+-rw-r--r--   0        0        0      153 2023-07-17 15:10:59.718613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_R50-ibn.yml
+-rw-r--r--   0        0        0      110 2023-07-17 15:10:59.726613 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_R50.yml
+-rw-r--r--   0        0        0      163 2023-07-17 15:10:59.730614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/MSMT17/sbs_S50.yml
+-rw-r--r--   0        0        0      182 2023-07-17 15:10:59.738614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_R101-ibn.yml
+-rw-r--r--   0        0        0      165 2023-07-17 15:10:59.746614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_R50-ibn.yml
+-rw-r--r--   0        0        0      122 2023-07-17 15:10:59.754614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_R50.yml
+-rw-r--r--   0        0        0      175 2023-07-17 15:10:59.762614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/AGW_S50.yml
+-rw-r--r--   0        0        0      194 2023-07-17 15:10:59.766614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_R101-ibn.yml
+-rw-r--r--   0        0        0      177 2023-07-17 15:10:59.774614 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0      134 2023-07-17 15:10:59.782615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_R50.yml
+-rw-r--r--   0        0        0      187 2023-07-17 15:10:59.786615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_S50.yml
+-rw-r--r--   0        0        0     1508 2023-07-17 15:10:59.790615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_vit.yml
+-rw-r--r--   0        0        0      165 2023-07-17 15:10:59.798615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/mgn_R50-ibn.yml
+-rw-r--r--   0        0        0      182 2023-07-17 15:10:59.802615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_R101-ibn.yml
+-rw-r--r--   0        0        0      165 2023-07-17 15:10:59.810615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_R50-ibn.yml
+-rw-r--r--   0        0        0      122 2023-07-17 15:10:59.814615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_R50.yml
+-rw-r--r--   0        0        0      175 2023-07-17 15:10:59.818615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/sbs_S50.yml
+-rw-r--r--   0        0        0      563 2023-07-17 15:10:59.826615 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/VERIWild/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0      483 2023-07-17 15:10:59.834616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/VeRi/sbs_R50-ibn.yml
+-rw-r--r--   0        0        0      567 2023-07-17 15:10:59.842616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/VehicleID/bagtricks_R50-ibn.yml
+-rw-r--r--   0        0        0     3744 2023-07-17 15:10:59.842616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/datasets/generate_mot_patches.py
+-rw-r--r--   0        0        0      403 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/README.md
+-rw-r--r--   0        0        0     3359 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/demo.py
+-rw-r--r--   0        0        0      808 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/plot_roc_with_pickle.py
+-rw-r--r--   0        0        0     5413 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/predictor.py
+-rw-r--r--   0        0        0     5076 2023-07-17 15:10:59.850616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/visualize_result.py
+-rw-r--r--   0        0        0     1058 2023-07-17 15:10:59.854616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docker/Dockerfile
+-rw-r--r--   0        0        0      663 2023-07-17 15:10:59.862616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docker/README.md
+-rw-r--r--   0        0        0        6 2023-07-17 15:10:59.870616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/.gitignore
+-rw-r--r--   0        0        0      630 2023-07-17 15:10:59.878616 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/Makefile
+-rw-r--r--   0        0        0      542 2023-07-17 15:10:59.886617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/README.md
+-rw-r--r--   0        0        0      428 2023-07-17 15:10:59.894617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    11669 2023-07-17 15:10:59.894617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/conf.py
+-rw-r--r--   0        0        0      377 2023-07-17 15:10:59.902617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/index.rst
+-rw-r--r--   0        0        0      150 2023-07-17 15:10:59.906617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/checkpoint.rst
+-rw-r--r--   0        0        0      372 2023-07-17 15:10:59.910617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/config.rst
+-rw-r--r--   0        0        0     1929 2023-07-17 15:10:59.914617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/data.rst
+-rw-r--r--   0        0        0      185 2023-07-17 15:10:59.922617 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/data_transforms.rst
+-rw-r--r--   0        0        0      459 2023-07-17 15:10:59.938618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/engine.rst
+-rw-r--r--   0        0        0      144 2023-07-17 15:10:59.942618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/evaluation.rst
+-rw-r--r--   0        0        0      203 2023-07-17 15:10:59.946618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/index.rst
+-rw-r--r--   0        0        0      132 2023-07-17 15:10:59.954618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/layers.rst
+-rw-r--r--   0        0        0      758 2023-07-17 15:10:59.958618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/modeling.rst
+-rw-r--r--   0        0        0      132 2023-07-17 15:10:59.966618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/solver.rst
+-rw-r--r--   0        0        0     1521 2023-07-17 15:10:59.974618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/utils.rst
+-rw-r--r--   0        0        0      180 2023-07-17 15:10:59.982618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/requirements.txt
+-rw-r--r--   0        0        0     4756 2023-07-17 15:10:59.982618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fast_reid_interfece.py
+-rw-r--r--   0        0        0      104 2023-07-17 15:10:59.982618 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      266 2023-07-17 15:10:59.990619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/__init__.py
+-rw-r--r--   0        0        0      428 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10089 2023-07-17 18:04:55.264546 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     3817 2023-07-18 15:12:32.712317 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/defaults.cpython-38.pyc
+-rw-r--r--   0        0        0    11536 2023-07-17 15:11:00.006619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/config.py
+-rw-r--r--   0        0        0    10644 2023-07-17 15:11:00.006619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/defaults.py
+-rw-r--r--   0        0        0      390 2023-07-17 15:11:00.010619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-17 18:04:56.408559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5228 2023-07-17 18:04:56.424559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     2063 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0     5715 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/data_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     6208 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/build.py
+-rw-r--r--   0        0        0     1496 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/common.py
+-rw-r--r--   0        0        0     7044 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/data_utils.py
+-rw-r--r--   0        0        0     1505 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/AirportALERT.py
+-rw-r--r--   0        0        0     1252 2023-07-17 15:11:00.038619 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/AirportALERT.cpython-38.pyc
+-rw-r--r--   0        0        0     1753 2023-07-17 18:04:56.432559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6136 2023-07-17 18:04:56.432559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/bases.cpython-38.pyc
+-rw-r--r--   0        0        0     1421 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/caviara.cpython-38.pyc
+-rw-r--r--   0        0        0     7476 2023-07-17 18:04:56.436559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk03.cpython-38.pyc
+-rw-r--r--   0        0        0     1914 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk_sysu.cpython-38.pyc
+-rw-r--r--   0        0        0     2306 2023-07-17 18:04:56.436559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/dukemtmcreid.cpython-38.pyc
+-rw-r--r--   0        0        0     1457 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/grid.cpython-38.pyc
+-rw-r--r--   0        0        0     1499 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/iLIDS.cpython-38.pyc
+-rw-r--r--   0        0        0     1562 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/lpw.cpython-38.pyc
+-rw-r--r--   0        0        0     2934 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/market1501.cpython-38.pyc
+-rw-r--r--   0        0        0     2709 2023-07-17 18:04:56.432559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot17.cpython-38.pyc
+-rw-r--r--   0        0        0     2755 2023-07-17 18:04:56.436559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot20.cpython-38.pyc
+-rw-r--r--   0        0        0     2800 2023-07-17 18:04:56.440559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/msmt17.cpython-38.pyc
+-rw-r--r--   0        0        0     1416 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pes3d.cpython-38.pyc
+-rw-r--r--   0        0        0     1439 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pku.cpython-38.pyc
+-rw-r--r--   0        0        0     1451 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prai.cpython-38.pyc
+-rw-r--r--   0        0        0     1587 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prid.cpython-38.pyc
+-rw-r--r--   0        0        0     1524 2023-07-17 18:04:56.444559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/saivt.cpython-38.pyc
+-rw-r--r--   0        0        0     1559 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sensereid.cpython-38.pyc
+-rw-r--r--   0        0        0     1648 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/shinpuhkan.cpython-38.pyc
+-rw-r--r--   0        0        0     1519 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sysu_mm.cpython-38.pyc
+-rw-r--r--   0        0        0     1470 2023-07-17 18:04:56.448560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/thermalworld.cpython-38.pyc
+-rw-r--r--   0        0        0     3760 2023-07-17 18:04:56.456560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/vehicleid.cpython-38.pyc
+-rw-r--r--   0        0        0     2173 2023-07-17 18:04:56.456560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veri.cpython-38.pyc
+-rw-r--r--   0        0        0     4434 2023-07-17 18:04:56.456560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veriwild.cpython-38.pyc
+-rw-r--r--   0        0        0     1450 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/viper.cpython-38.pyc
+-rw-r--r--   0        0        0     2070 2023-07-17 18:04:56.452560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/wildtracker.cpython-38.pyc
+-rw-r--r--   0        0        0     5892 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/bases.py
+-rw-r--r--   0        0        0     1122 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/caviara.py
+-rw-r--r--   0        0        0    12054 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk03.py
+-rw-r--r--   0        0        0     1635 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk_sysu.py
+-rw-r--r--   0        0        0     2350 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/dukemtmcreid.py
+-rw-r--r--   0        0        0     1186 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/grid.py
+-rw-r--r--   0        0        0     1295 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/iLIDS.py
+-rw-r--r--   0        0        0     1466 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/lpw.py
+-rw-r--r--   0        0        0     3171 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/market1501.py
+-rw-r--r--   0        0        0     3025 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot17.py
+-rw-r--r--   0        0        0     3075 2023-07-17 15:11:00.210623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20.py
+-rw-r--r--   0        0        0     3247 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20_.py
+-rw-r--r--   0        0        0     3871 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/msmt17.py
+-rw-r--r--   0        0        0     1159 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pes3d.py
+-rw-r--r--   0        0        0     1169 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pku.py
+-rw-r--r--   0        0        0     1178 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prai.py
+-rw-r--r--   0        0        0     1199 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prid.py
+-rw-r--r--   0        0        0     1305 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/saivt.py
+-rw-r--r--   0        0        0     1377 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sensereid.py
+-rw-r--r--   0        0        0     1362 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/shinpuhkan.py
+-rw-r--r--   0        0        0     1336 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sysu_mm.py
+-rw-r--r--   0        0        0     1198 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/thermalworld.py
+-rw-r--r--   0        0        0     3837 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/vehicleid.py
+-rw-r--r--   0        0        0     2209 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veri.py
+-rw-r--r--   0        0        0     4884 2023-07-17 15:11:00.214623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veriwild.py
+-rw-r--r--   0        0        0     1226 2023-07-17 15:11:00.226623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/viper.py
+-rw-r--r--   0        0        0     1844 2023-07-17 15:11:00.226623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/wildtracker.py
+-rw-r--r--   0        0        0      473 2023-07-17 15:11:00.226623 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__init__.py
+-rw-r--r--   0        0        0      587 2023-07-17 18:04:56.424559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3580 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/data_sampler.cpython-38.pyc
+-rw-r--r--   0        0        0     2408 2023-07-17 18:04:56.428559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/imbalance_sampler.cpython-38.pyc
+-rw-r--r--   0        0        0     7396 2023-07-17 18:04:56.424559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/triplet_sampler.cpython-38.pyc
+-rw-r--r--   0        0        0     2917 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/data_sampler.py
+-rw-r--r--   0        0        0     2241 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/imbalance_sampler.py
+-rw-r--r--   0        0        0    10108 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/triplet_sampler.py
+-rw-r--r--   0        0        0      246 2023-07-17 15:11:00.254624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__init__.py
+-rw-r--r--   0        0        0      547 2023-07-17 18:04:56.408559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22427 2023-07-17 18:04:56.416559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/autoaugment.cpython-38.pyc
+-rw-r--r--   0        0        0     2310 2023-07-17 18:04:56.420559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     5060 2023-07-17 18:04:56.420559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/functional.cpython-38.pyc
+-rw-r--r--   0        0        0     5517 2023-07-17 18:04:56.420559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/transforms.cpython-38.pyc
+-rw-r--r--   0        0        0    29513 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/autoaugment.py
+-rw-r--r--   0        0        0     3348 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/build.py
+-rw-r--r--   0        0        0     5585 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/functional.py
+-rw-r--r--   0        0        0     5713 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/transforms.py
+-rw-r--r--   0        0        0      370 2023-07-17 15:11:00.286624 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__init__.py
+-rw-r--r--   0        0        0      502 2023-07-17 18:04:55.372548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    16531 2023-07-17 18:04:56.408559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/defaults.cpython-38.pyc
+-rw-r--r--   0        0        0    18614 2023-07-17 18:04:55.380548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/hooks.cpython-38.pyc
+-rw-r--r--   0        0        0     2944 2023-07-17 18:04:56.460560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/launch.cpython-38.pyc
+-rw-r--r--   0        0        0    11841 2023-07-17 18:04:55.376548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/train_loop.cpython-38.pyc
+-rw-r--r--   0        0        0    20113 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/defaults.py
+-rw-r--r--   0        0        0    19298 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/hooks.py
+-rw-r--r--   0        0        0     3768 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/launch.py
+-rw-r--r--   0        0        0    12215 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/train_loop.py
+-rw-r--r--   0        0        0      286 2023-07-17 15:11:00.318625 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__init__.py
+-rw-r--r--   0        0        0      637 2023-07-17 18:04:55.380548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2547 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/clas_evaluator.cpython-38.pyc
+-rw-r--r--   0        0        0     5101 2023-07-17 18:04:55.380548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/evaluator.cpython-38.pyc
+-rw-r--r--   0        0        0     1608 2023-07-17 18:04:56.236557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/query_expansion.cpython-38.pyc
+-rw-r--r--   0        0        0     4074 2023-07-17 18:04:55.384548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/reid_evaluation.cpython-38.pyc
+-rw-r--r--   0        0        0     2460 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/testing.cpython-38.pyc
+-rw-r--r--   0        0        0     2295 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/clas_evaluator.py
+-rw-r--r--   0        0        0     6660 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1701 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/query_expansion.py
+-rw-r--r--   0        0        0     7001 2023-07-17 15:11:00.354626 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank.py
+-rw-r--r--   0        0        0      100 2023-07-17 15:11:00.358626 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/Makefile
+-rw-r--r--   0        0        0      480 2023-07-17 15:11:00.358626 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/__init__.py
+-rw-r--r--   0        0        0      731 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0  1033326 2023-07-17 15:11:00.406627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.c
+-rw-r--r--   0        0        0     9675 2023-07-17 15:11:00.414627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.pyx
+-rw-r--r--   0        0        0   908364 2023-07-17 15:11:00.446627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.c
+-rw-r--r--   0        0        0     3064 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.pyx
+-rw-r--r--   0        0        0      626 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/setup.py
+-rw-r--r--   0        0        0     4083 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/test_cython.py
+-rw-r--r--   0        0        0     4952 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/reid_evaluation.py
+-rw-r--r--   0        0        0     3380 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rerank.py
+-rw-r--r--   0        0        0     2784 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/roc.py
+-rw-r--r--   0        0        0     2424 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/testing.py
+-rw-r--r--   0        0        0      620 2023-07-17 15:11:00.454627 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-17 18:04:55.304547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2487 2023-07-17 18:04:55.304547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/activation.cpython-38.pyc
+-rw-r--r--   0        0        0     2743 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/any_softmax.cpython-38.pyc
+-rw-r--r--   0        0        0     7495 2023-07-17 18:04:55.308547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/batch_norm.cpython-38.pyc
+-rw-r--r--   0        0        0     3076 2023-07-17 18:04:55.308547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/context_block.cpython-38.pyc
+-rw-r--r--   0        0        0     5722 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/drop.cpython-38.pyc
+-rw-r--r--   0        0        0     6176 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/frn.cpython-38.pyc
+-rw-r--r--   0        0        0     1261 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/gather_layer.cpython-38.pyc
+-rw-r--r--   0        0        0      996 2023-07-17 18:04:55.312547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1658 2023-07-17 18:04:55.316547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/non_local.cpython-38.pyc
+-rw-r--r--   0        0        0     5639 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/pooling.cpython-38.pyc
+-rw-r--r--   0        0        0     1088 2023-07-17 18:04:55.316547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/se_layer.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-07-17 18:04:55.316547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/splat.cpython-38.pyc
+-rw-r--r--   0        0        0     3564 2023-07-17 18:04:55.320547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/weight_init.cpython-38.pyc
+-rw-r--r--   0        0        0     1334 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/activation.py
+-rw-r--r--   0        0        0     2275 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/any_softmax.py
+-rw-r--r--   0        0        0     8514 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/batch_norm.py
+-rw-r--r--   0        0        0     4244 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/context_block.py
+-rw-r--r--   0        0        0     6934 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/drop.py
+-rw-r--r--   0        0        0     6499 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/frn.py
+-rw-r--r--   0        0        0      816 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/gather_layer.py
+-rw-r--r--   0        0        0      724 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/helpers.py
+-rw-r--r--   0        0        0     1877 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/non_local.py
+-rw-r--r--   0        0        0     3649 2023-07-17 15:11:00.554629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/pooling.py
+-rw-r--r--   0        0        0      681 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/se_layer.py
+-rw-r--r--   0        0        0     3826 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/splat.py
+-rw-r--r--   0        0        0     4216 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/weight_init.py
+-rw-r--r--   0        0        0      416 2023-07-17 15:11:00.558629 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-17 18:04:55.288547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2023-07-17 15:11:00.566630 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__init__.py
+-rw-r--r--   0        0        0      918 2023-07-17 18:04:55.300547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      871 2023-07-17 18:04:55.300547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     5481 2023-07-17 18:04:55.348547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenet.cpython-38.pyc
+-rw-r--r--   0        0        0     9231 2023-07-17 18:04:55.352548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenetv3.cpython-38.pyc
+-rw-r--r--   0        0        0    12119 2023-07-17 18:04:55.328547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/osnet.cpython-38.pyc
+-rw-r--r--   0        0        0     9497 2023-07-17 18:04:55.352548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/repvgg.cpython-38.pyc
+-rw-r--r--   0        0        0     9235 2023-07-17 18:04:55.332547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnest.cpython-38.pyc
+-rw-r--r--   0        0        0    10313 2023-07-17 18:04:55.304547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0    10098 2023-07-17 18:04:55.332547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnext.cpython-38.pyc
+-rw-r--r--   0        0        0     5164 2023-07-17 18:04:55.348547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/shufflenet.cpython-38.pyc
+-rw-r--r--   0        0        0    13440 2023-07-17 18:04:55.356547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/vision_transformer.cpython-38.pyc
+-rw-r--r--   0        0        0      692 2023-07-17 15:11:00.638631 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/build.py
+-rw-r--r--   0        0        0     6479 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenet.py
+-rw-r--r--   0        0        0    11726 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenetv3.py
+-rw-r--r--   0        0        0    15593 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/osnet.py
+-rw-r--r--   0        0        0       86 2023-07-17 15:11:00.642631 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-17 18:04:55.336547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4482 2023-07-17 18:04:55.340547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     9617 2023-07-17 18:04:55.344547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/effnet.cpython-38.pyc
+-rw-r--r--   0        0        0    21323 2023-07-17 18:04:55.340547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/regnet.cpython-38.pyc
+-rw-r--r--   0        0        0    11067 2023-07-17 15:11:00.662631 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/config.py
+-rw-r--r--   0        0        0      485 2023-07-17 15:11:00.670632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B0_dds_8gpu.yaml
+-rw-r--r--   0        0        0      485 2023-07-17 15:11:00.674632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B1_dds_8gpu.yaml
+-rw-r--r--   0        0        0      485 2023-07-17 15:11:00.682632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B2_dds_8gpu.yaml
+-rw-r--r--   0        0        0      485 2023-07-17 15:11:00.690632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B3_dds_8gpu.yaml
+-rw-r--r--   0        0        0      486 2023-07-17 15:11:00.694632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B4_dds_8gpu.yaml
+-rw-r--r--   0        0        0      484 2023-07-17 15:11:00.698632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet/EN-B5_dds_8gpu.yaml
+-rw-r--r--   0        0        0     9933 2023-07-17 15:11:00.698632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet.py
+-rw-r--r--   0        0        0    21652 2023-07-17 15:11:00.698632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnet.py
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.706632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-1.6GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      363 2023-07-17 15:11:00.714632 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-12GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.718633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-16GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      361 2023-07-17 15:11:00.726633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-200MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      361 2023-07-17 15:11:00.730633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-3.2GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.734633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-32GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      361 2023-07-17 15:11:00.742633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-4.0GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.746633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-400MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.750633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-6.4GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.762633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-600MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.766633 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-8.0GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      362 2023-07-17 15:11:00.774634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnetx/RegNetX-800MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      376 2023-07-17 15:11:00.782634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-1.6GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      377 2023-07-17 15:11:00.790634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-12GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      378 2023-07-17 15:11:00.794634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-16GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      357 2023-07-17 15:11:00.802634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-200MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      375 2023-07-17 15:11:00.806634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-3.2GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      378 2023-07-17 15:11:00.814634 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-32GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      375 2023-07-17 15:11:00.822635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-4.0GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      375 2023-07-17 15:11:00.830635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-400MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      376 2023-07-17 15:11:00.838635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-6.4GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      376 2023-07-17 15:11:00.846635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-600MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      376 2023-07-17 15:11:00.850635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-8.0GF_dds_8gpu.yaml
+-rw-r--r--   0        0        0      375 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnety/RegNetY-800MF_dds_8gpu.yaml
+-rw-r--r--   0        0        0    11722 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/repvgg.py
+-rw-r--r--   0        0        0    15306 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnest.py
+-rw-r--r--   0        0        0    12509 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnet.py
+-rw-r--r--   0        0        0    11941 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnext.py
+-rw-r--r--   0        0        0     7091 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/shufflenet.py
+-rw-r--r--   0        0        0    16636 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/vision_transformer.py
+-rw-r--r--   0        0        0      265 2023-07-17 15:11:00.858635 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__init__.py
+-rw-r--r--   0        0        0      416 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      822 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     1162 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/clas_head.cpython-38.pyc
+-rw-r--r--   0        0        0     3809 2023-07-17 18:04:55.360547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/embedding_head.cpython-38.pyc
+-rw-r--r--   0        0        0      630 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/build.py
+-rw-r--r--   0        0        0     1050 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/clas_head.py
+-rw-r--r--   0        0        0     4772 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/embedding_head.py
+-rw-r--r--   0        0        0      313 2023-07-17 15:11:00.886636 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__init__.py
+-rw-r--r--   0        0        0      608 2023-07-17 18:04:55.288547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1797 2023-07-17 18:04:55.292547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/circle_loss.cpython-38.pyc
+-rw-r--r--   0        0        0     1639 2023-07-17 18:04:55.292547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/cross_entroy_loss.cpython-38.pyc
+-rw-r--r--   0        0        0     2958 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/focal_loss.cpython-38.pyc
+-rw-r--r--   0        0        0     3285 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/triplet_loss.cpython-38.pyc
+-rw-r--r--   0        0        0     1859 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2147 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/circle_loss.py
+-rw-r--r--   0        0        0     1610 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/cross_entroy_loss.py
+-rw-r--r--   0        0        0     3361 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/focal_loss.py
+-rw-r--r--   0        0        0     3957 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/triplet_loss.py
+-rw-r--r--   0        0        0     1302 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/utils.py
+-rw-r--r--   0        0        0      299 2023-07-17 15:11:00.926637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__init__.py
+-rw-r--r--   0        0        0      473 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4325 2023-07-17 18:04:55.368548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/baseline.cpython-38.pyc
+-rw-r--r--   0        0        0      919 2023-07-17 18:04:55.364548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     3968 2023-07-17 18:04:55.372548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/distiller.cpython-38.pyc
+-rw-r--r--   0        0        0     7310 2023-07-17 18:04:55.368548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/mgn.cpython-38.pyc
+-rw-r--r--   0        0        0     3814 2023-07-17 18:04:55.372548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/moco.cpython-38.pyc
+-rw-r--r--   0        0        0     6381 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/baseline.py
+-rw-r--r--   0        0        0      747 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/build.py
+-rw-r--r--   0        0        0     5007 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/distiller.py
+-rw-r--r--   0        0        0    13405 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/mgn.py
+-rw-r--r--   0        0        0     3978 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/moco.py
+-rw-r--r--   0        0        0      138 2023-07-17 15:11:00.962637 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/__init__.py
+-rw-r--r--   0        0        0      317 2023-07-17 18:04:56.240557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10015 2023-07-17 18:04:56.244557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     2440 2023-07-17 18:04:56.244557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/lr_scheduler.cpython-38.pyc
+-rw-r--r--   0        0        0    12889 2023-07-17 15:11:00.982638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/build.py
+-rw-r--r--   0        0        0     2067 2023-07-17 15:11:00.982638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/lr_scheduler.py
+-rw-r--r--   0        0        0      179 2023-07-17 15:11:00.982638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__init__.py
+-rw-r--r--   0        0        0      382 2023-07-17 18:04:56.244557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3840 2023-07-17 18:04:56.248557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/lamb.cpython-38.pyc
+-rw-r--r--   0        0        0     3845 2023-07-17 18:04:56.404559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/radam.cpython-38.pyc
+-rw-r--r--   0        0        0    10467 2023-07-17 18:04:56.400559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/swa.cpython-38.pyc
+-rw-r--r--   0        0        0     5065 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/lamb.py
+-rw-r--r--   0        0        0     5715 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/radam.py
+-rw-r--r--   0        0        0    11090 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/swa.py
+-rw-r--r--   0        0        0       81 2023-07-17 15:11:01.006638 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__init__.py
+-rw-r--r--   0        0        0      235 2023-07-17 18:04:55.284547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    16201 2023-07-17 18:04:55.320547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/checkpoint.cpython-38.pyc
+-rw-r--r--   0        0        0     3627 2023-07-17 18:04:56.460560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/collect_env.cpython-38.pyc
+-rw-r--r--   0        0        0     7239 2023-07-17 18:04:55.324547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/comm.cpython-38.pyc
+-rw-r--r--   0        0        0     4886 2023-07-17 18:04:56.156556 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/compute_dist.cpython-38.pyc
+-rw-r--r--   0        0        0     3446 2023-07-17 18:04:56.460560 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/env.cpython-38.pyc
+-rw-r--r--   0        0        0    15628 2023-07-17 18:04:55.292547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/events.cpython-38.pyc
+-rw-r--r--   0        0        0     3057 2023-07-17 18:04:56.236557 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/faiss_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    16968 2023-07-17 18:04:55.288547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/file_io.cpython-38.pyc
+-rw-r--r--   0        0        0     3051 2023-07-17 18:04:55.296547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/history_buffer.cpython-38.pyc
+-rw-r--r--   0        0        0     5883 2023-07-17 18:04:55.384548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/logger.cpython-38.pyc
+-rw-r--r--   0        0        0     4055 2023-07-17 18:04:55.376548 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/params.cpython-38.pyc
+-rw-r--r--   0        0        0     3603 2023-07-17 18:04:56.404559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/precision_bn.cpython-38.pyc
+-rw-r--r--   0        0        0     2267 2023-07-17 18:04:55.300547 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/registry.cpython-38.pyc
+-rw-r--r--   0        0        0     2258 2023-07-17 18:04:56.404559 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/timer.cpython-38.pyc
+-rw-r--r--   0        0        0    18277 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/checkpoint.py
+-rw-r--r--   0        0        0     4693 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/collect_env.py
+-rw-r--r--   0        0        0     7676 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/comm.py
+-rw-r--r--   0        0        0     6601 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/compute_dist.py
+-rw-r--r--   0        0        0     3699 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/env.py
+-rw-r--r--   0        0        0    16494 2023-07-17 15:11:01.086640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/events.py
+-rw-r--r--   0        0        0     3344 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/faiss_utils.py
+-rw-r--r--   0        0        0    19186 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/file_io.py
+-rw-r--r--   0        0        0     2273 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/history_buffer.py
+-rw-r--r--   0        0        0     7224 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/logger.py
+-rw-r--r--   0        0        0     4381 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/params.py
+-rw-r--r--   0        0        0     3726 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/precision_bn.py
+-rw-r--r--   0        0        0     2051 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/registry.py
+-rw-r--r--   0        0        0     4454 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/summary.py
+-rw-r--r--   0        0        0     1880 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/timer.py
+-rw-r--r--   0        0        0    11831 2023-07-17 15:11:01.090640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/visualizer.py
+-rw-r--r--   0        0        0     3530 2023-07-17 15:11:01.098640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/CrossDomainReID/README.md
+-rw-r--r--   0        0        0     3989 2023-07-17 15:11:01.106640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/DG-ReID/README.md
+-rw-r--r--   0        0        0     1111 2023-07-17 15:11:01.110640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/README.md
+-rw-r--r--   0        0        0     1054 2023-07-17 15:11:01.118640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/Base-attribute.yml
+-rw-r--r--   0        0        0      189 2023-07-17 15:11:01.126640 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/dukemtmc.yml
+-rw-r--r--   0        0        0      195 2023-07-17 15:11:01.134641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/market1501.yml
+-rw-r--r--   0        0        0      138 2023-07-17 15:11:01.138641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/pa100.yml
+-rw-r--r--   0        0        0      249 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/__init__.py
+-rw-r--r--   0        0        0     1188 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_dataset.py
+-rw-r--r--   0        0        0     3343 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_evaluation.py
+-rw-r--r--   0        0        0      293 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/config.py
+-rw-r--r--   0        0        0      215 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/__init__.py
+-rw-r--r--   0        0        0     3412 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/bases.py
+-rw-r--r--   0        0        0     2451 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/dukemtmcattr.py
+-rw-r--r--   0        0        0     3137 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/market1501attr.py
+-rw-r--r--   0        0        0     2088 2023-07-17 15:11:01.142641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/pa100k.py
+-rw-r--r--   0        0        0      205 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/__init__.py
+-rw-r--r--   0        0        0     1285 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_baseline.py
+-rw-r--r--   0        0        0     1171 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_head.py
+-rw-r--r--   0        0        0      974 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/bce_loss.py
+-rw-r--r--   0        0        0     3949 2023-07-17 15:11:01.146641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/train_net.py
+-rw-r--r--   0        0        0      574 2023-07-17 15:11:01.154641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/README.md
+-rw-r--r--   0        0        0     1144 2023-07-17 15:11:01.158641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/configs/base-clas.yaml
+-rw-r--r--   0        0        0      206 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/__init__.py
+-rw-r--r--   0        0        0     1441 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/bee_ant.py
+-rw-r--r--   0        0        0     1477 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/dataset.py
+-rw-r--r--   0        0        0     2824 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/trainer.py
+-rw-r--r--   0        0        0     1812 2023-07-17 15:11:01.166641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/train_net.py
+-rw-r--r--   0        0        0     1655 2023-07-17 15:11:01.174641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/README.md
+-rw-r--r--   0        0        0      415 2023-07-17 15:11:01.178641 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/Base-kd.yml
+-rw-r--r--   0        0        0      407 2023-07-17 15:11:01.190642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/kd-sbs_r101ibn-sbs_r34.yml
+-rw-r--r--   0        0        0      188 2023-07-17 15:11:01.198642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/sbs_r101ibn.yml
+-rw-r--r--   0        0        0      201 2023-07-17 15:11:01.202642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/configs/sbs_r34.yml
+-rw-r--r--   0        0        0      181 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/__init__.py
+-rw-r--r--   0        0        0     4547 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/overhaul.py
+-rw-r--r--   0        0        0    11483 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/resnet_distill.py
+-rw-r--r--   0        0        0     1340 2023-07-17 15:11:01.206642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/train_net.py
+-rw-r--r--   0        0        0     1200 2023-07-17 15:11:01.214642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/README.md
+-rw-r--r--   0        0        0     1169 2023-07-17 15:11:01.218642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/configs/face_base.yml
+-rw-r--r--   0        0        0      239 2023-07-17 15:11:01.226642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/configs/r101_ir.yml
+-rw-r--r--   0        0        0      198 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/configs/r50_ir.yml
+-rw-r--r--   0        0        0      198 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/config.py
+-rw-r--r--   0        0        0      139 2023-07-17 15:11:01.234642 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/__init__.py
+-rw-r--r--   0        0        0     1042 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/ms1mv2.py
+-rw-r--r--   0        0        0     1479 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/test_dataset.py
+-rw-r--r--   0        0        0     2382 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_data.py
+-rw-r--r--   0        0        0     2247 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_evaluator.py
+-rw-r--r--   0        0        0      234 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/__init__.py
+-rw-r--r--   0        0        0     1481 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_baseline.py
+-rw-r--r--   0        0        0     1097 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_head.py
+-rw-r--r--   0        0        0     6407 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/iresnet.py
+-rw-r--r--   0        0        0     6976 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/partial_fc.py
+-rw-r--r--   0        0        0     3042 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/pfc_checkpointer.py
+-rw-r--r--   0        0        0     8528 2023-07-17 15:11:01.238643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/trainer.py
+-rw-r--r--   0        0        0     3261 2023-07-17 15:11:01.242643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/utils_amp.py
+-rw-r--r--   0        0        0     7666 2023-07-17 15:11:01.242643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/verification.py
+-rw-r--r--   0        0        0     1339 2023-07-17 15:11:01.242643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/train_net.py
+-rwxr-xr-x   0        0        0       34 2023-07-17 15:11:01.250643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/.gitignore
+-rwxr-xr-x   0        0        0     2613 2023-07-17 15:11:01.254643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/CMakeLists.txt
+-rwxr-xr-x   0        0        0     9609 2023-07-17 15:11:01.262643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/README.md
+-rw-r--r--   0        0        0     1060 2023-07-17 15:11:01.262643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/demo/CMakeLists.txt
+-rwxr-xr-x   0        0        0     5398 2023-07-17 15:11:01.266643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/demo/inference.cpp
+-rw-r--r--   0        0        0      290 2023-07-17 15:11:01.274643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/docker/trt7cu100/Dockerfile
+-rw-r--r--   0        0        0     1019 2023-07-17 15:11:01.278643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/docker/trt7cu102/Dockerfile
+-rwxr-xr-x   0        0        0     1219 2023-07-17 15:11:01.286643 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/CMakeLists.txt
+-rw-r--r--   0        0        0       85 2023-07-17 15:11:01.290644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/backbones/CMakeLists.txt
+-rwxr-xr-x   0        0        0    19621 2023-07-17 15:11:01.298644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/backbones/sbs_resnet.cpp
+-rwxr-xr-x   0        0        0     2782 2023-07-17 15:11:01.306644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/calibrator.cpp
+-rw-r--r--   0        0        0     3694 2023-07-17 15:11:01.310644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/utils.cpp
+-rw-r--r--   0        0        0       90 2023-07-17 15:11:01.318644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/engine/CMakeLists.txt
+-rwxr-xr-x   0        0        0     3852 2023-07-17 15:11:01.322644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/engine/InferenceEngine.cpp
+-rw-r--r--   0        0        0      135 2023-07-17 15:11:01.326644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/factory/CMakeLists.txt
+-rwxr-xr-x   0        0        0     3559 2023-07-17 15:11:01.330644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/factory/factory.cpp
+-rw-r--r--   0        0        0       89 2023-07-17 15:11:01.338644 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/heads/CMakeLists.txt
+-rw-r--r--   0        0        0     1722 2023-07-17 15:11:01.346645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/heads/embedding_head.cpp
+-rw-r--r--   0        0        0      177 2023-07-17 15:11:01.350645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/CMakeLists.txt
+-rw-r--r--   0        0        0    22672 2023-07-17 15:11:01.354645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/layers.cpp
+-rw-r--r--   0        0        0     1580 2023-07-17 15:11:01.362645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.cpp
+-rw-r--r--   0        0        0     1207 2023-07-17 15:11:01.366645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.h
+-rw-r--r--   0        0        0      123 2023-07-17 15:11:01.370645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/CMakeLists.txt
+-rwxr-xr-x   0        0        0     1031 2023-07-17 15:11:01.374645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/baseline.cpp
+-rwxr-xr-x   0        0        0     5605 2023-07-17 15:11:01.382645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/model.cpp
+-rw-r--r--   0        0        0      405 2023-07-17 15:11:01.386645 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/IPoolingLayerRT.h
+-rwxr-xr-x   0        0        0     2106 2023-07-17 15:11:01.394646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/InferenceEngine.h
+-rw-r--r--   0        0        0      660 2023-07-17 15:11:01.398646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/baseline.h
+-rwxr-xr-x   0        0        0     1173 2023-07-17 15:11:01.406646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/calibrator.h
+-rwxr-xr-x   0        0        0      139 2023-07-17 15:11:01.414646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/config.h.in
+-rwxr-xr-x   0        0        0      417 2023-07-17 15:11:01.418646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/cuda_utils.h
+-rw-r--r--   0        0        0      675 2023-07-17 15:11:01.426646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/embedding_head.h
+-rw-r--r--   0        0        0      584 2023-07-17 15:11:01.430646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/factory.h
+-rwxr-xr-x   0        0        0     1060 2023-07-17 15:11:01.438646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/holder.h
+-rw-r--r--   0        0        0     3175 2023-07-17 15:11:01.442646 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/layers.h
+-rw-r--r--   0        0        0    16550 2023-07-17 15:11:01.446647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/logging.h
+-rwxr-xr-x   0        0        0     2081 2023-07-17 15:11:01.454647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/model.h
+-rw-r--r--   0        0        0      376 2023-07-17 15:11:01.458647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/module.h
+-rwxr-xr-x   0        0        0     2086 2023-07-17 15:11:01.466647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/sbs_resnet.h
+-rwxr-xr-x   0        0        0     1932 2023-07-17 15:11:01.470647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/struct.h
+-rwxr-xr-x   0        0        0     2151 2023-07-17 15:11:01.470647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/utils.h
+-rwxr-xr-x   0        0        0      960 2023-07-17 15:11:01.478647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/CMakeLists.txt
+-rw-r--r--   0        0        0     1064 2023-07-17 15:11:01.482647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/docker/trt7cu100/Dockerfile
+-rwxr-xr-x   0        0        0      325 2023-07-17 15:11:01.490647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/docker/trt7cu102_torch160/Dockerfile
+-rwxr-xr-x   0        0        0     1765 2023-07-17 15:11:01.490647 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/market_benchmark.py
+-rwxr-xr-x   0        0        0     4977 2023-07-17 15:11:01.494648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/reid.cpp
+-rwxr-xr-x   0        0        0      550 2023-07-17 15:11:01.494648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/test.py
+-rw-r--r--   0        0        0     1053 2023-07-17 15:11:01.502648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/CMakeLists.txt
+-rw-r--r--   0        0        0     1073 2023-07-17 15:11:01.506648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/LICENSE
+-rw-r--r--   0        0        0     2103 2023-07-17 15:11:01.510648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/README.md
+-rw-r--r--   0        0        0    11468 2023-07-17 15:11:01.518648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.cpp
+-rw-r--r--   0        0        0    10917 2023-07-17 15:11:01.522648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.h
+-rw-r--r--   0        0        0     1961 2023-07-17 15:11:01.530648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/example1.cpp
+-rw-r--r--   0        0        0      333 2023-07-17 15:11:01.538648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/mat2npz
+-rw-r--r--   0        0        0      253 2023-07-17 15:11:01.542648 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/npy2mat
+-rwxr-xr-x   0        0        0      271 2023-07-17 15:11:01.550649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/npz2mat
+-rw-r--r--   0        0        0     2941 2023-07-17 15:11:01.554649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/tools/How_to_Generate.md
+-rw-r--r--   0        0        0     3206 2023-07-17 15:11:01.554649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/tools/gen_wts.py
+-rw-r--r--   0        0        0     2422 2023-07-17 15:11:01.566649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/README.md
+-rw-r--r--   0        0        0     1202 2023-07-17 15:11:01.570649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/base-image_retri.yml
+-rw-r--r--   0        0        0      451 2023-07-17 15:11:01.578649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/cars.yml
+-rw-r--r--   0        0        0      457 2023-07-17 15:11:01.582649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/cub.yml
+-rw-r--r--   0        0        0      324 2023-07-17 15:11:01.586649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/inshop.yml
+-rw-r--r--   0        0        0      263 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/sop.yml
+-rw-r--r--   0        0        0      189 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/config.py
+-rw-r--r--   0        0        0     2548 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/datasets.py
+-rw-r--r--   0        0        0     4726 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/retri_evaluator.py
+-rw-r--r--   0        0        0     1656 2023-07-17 15:11:01.594649 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/train_net.py
+-rw-r--r--   0        0        0      572 2023-07-17 15:11:01.602650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/README.md
+-rw-r--r--   0        0        0      123 2023-07-17 15:11:01.602650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/autotuner/__init__.py
+-rw-r--r--   0        0        0     1850 2023-07-17 15:11:01.602650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/autotuner/tune_hooks.py
+-rw-r--r--   0        0        0     1520 2023-07-17 15:11:01.606650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/configs/search_trial.yml
+-rw-r--r--   0        0        0     8384 2023-07-17 15:11:01.610650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/tune_net.py
+-rw-r--r--   0        0        0     1497 2023-07-17 15:11:01.614650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/HAA/Readme.md
+-rw-r--r--   0        0        0     3135 2023-07-17 15:11:01.618650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/README.md
+-rw-r--r--   0        0        0     1514 2023-07-17 15:11:01.626650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/Base-naic.yml
+-rw-r--r--   0        0        0      179 2023-07-17 15:11:01.630650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/nest101-base.yml
+-rw-r--r--   0        0        0      194 2023-07-17 15:11:01.638650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/r34-ibn.yml
+-rw-r--r--   0        0        0      412 2023-07-17 15:11:01.642650 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/submit.yml
+-rw-r--r--   0        0        0  1342300 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/label.txt
+-rw-r--r--   0        0        0      189 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/__init__.py
+-rw-r--r--   0        0        0      187 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/config.py
+-rw-r--r--   0        0        0     7671 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_dataset.py
+-rw-r--r--   0        0        0     3922 2023-07-17 15:11:01.686651 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_evaluator.py
+-rw-r--r--   0        0        0  3757537 2023-07-17 15:11:01.794653 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic20r2_train_list_clean.txt
+-rw-r--r--   0        0        0  1090705 2023-07-17 15:11:01.830654 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/train_list_clean.txt
+-rw-r--r--   0        0        0     2192 2023-07-17 15:11:01.830654 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/train_net.py
+-rw-r--r--   0        0        0   353057 2023-07-17 15:11:01.846654 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/val_gallery.txt
+-rw-r--r--   0        0        0    48120 2023-07-17 15:11:01.854654 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/val_query.txt
+-rw-r--r--   0        0        0     3019 2023-07-17 15:11:01.862655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/README.md
+-rw-r--r--   0        0        0     1170 2023-07-17 15:11:01.866655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/configs/partial_market.yml
+-rw-r--r--   0        0        0      274 2023-07-17 15:11:01.870655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/__init__.py
+-rw-r--r--   0        0        0      224 2023-07-17 15:11:01.882655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/config.py
+-rw-r--r--   0        0        0     1883 2023-07-17 15:11:01.890655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_distance.py
+-rw-r--r--   0        0        0     4413 2023-07-17 15:11:01.898655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_evaluation.py
+-rw-r--r--   0        0        0     5947 2023-07-17 15:11:01.906655 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_head.py
+-rw-r--r--   0        0        0     2266 2023-07-17 15:11:01.918656 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partial_dataset.py
+-rw-r--r--   0        0        0     1502 2023-07-17 15:11:01.926656 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partialbaseline.py
+-rw-r--r--   0        0        0     2416 2023-07-17 15:11:01.930656 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/train_net.py
+-rw-r--r--   0        0        0     1602 2023-07-17 15:11:01.946656 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/README.md
+-rw-r--r--   0        0        0       80 2023-07-17 15:11:01.950656 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/__init__.py
+-rw-r--r--   0        0        0     1414 2023-07-17 15:11:01.958656 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/dataset_test.py
+-rw-r--r--   0        0        0     1226 2023-07-17 15:11:01.966657 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/feature_align.py
+-rw-r--r--   0        0        0      676 2023-07-17 15:11:01.982657 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/interp_test.py
+-rw-r--r--   0        0        0      646 2023-07-17 15:11:01.990657 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/lr_scheduler_test.py
+-rw-r--r--   0        0        0     1217 2023-07-17 15:11:01.998657 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/model_test.py
+-rw-r--r--   0        0        0      375 2023-07-17 15:11:02.006657 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/sampler_test.py
+-rw-r--r--   0        0        0      804 2023-07-17 15:11:02.014658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/test_repvgg.py
+-rw-r--r--   0        0        0     1369 2023-07-17 15:11:02.046658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/ReadMe.md
+-rw-r--r--   0        0        0        0 2023-07-17 15:11:02.050658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/__init__.py
+-rw-r--r--   0        0        0    93270 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe.proto
+-rw-r--r--   0        0        0      984 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_lmdb.py
+-rw-r--r--   0        0        0     4756 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_net.py
+-rw-r--r--   0        0        0   502318 2023-07-17 15:11:02.058658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_pb2.py
+-rw-r--r--   0        0        0     5605 2023-07-17 15:11:02.062658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/layer_param.py
+-rw-r--r--   0        0        0      100 2023-07-17 15:11:02.062658 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/net.py
+-rw-r--r--   0        0        0     5305 2023-07-17 15:11:02.066659 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/README.md
+-rw-r--r--   0        0        0     2282 2023-07-17 15:11:02.090659 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/caffe_export.py
+-rw-r--r--   0        0        0     2823 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/caffe_inference.py
+-rw-r--r--   0        0        0     4758 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/onnx_export.py
+-rw-r--r--   0        0        0     2384 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/onnx_inference.py
+-rw-r--r--   0        0        0    28802 2023-07-17 15:11:02.138660 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/pytorch_to_caffe.py
+-rw-r--r--   0        0        0     2223 2023-07-17 15:11:02.150660 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0022_c6s1_002976_01.jpg
+-rw-r--r--   0        0        0     2137 2023-07-17 15:11:02.162660 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0027_c2s2_091032_02.jpg
+-rw-r--r--   0        0        0     2640 2023-07-17 15:11:02.170661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0032_c6s1_002851_01.jpg
+-rw-r--r--   0        0        0     2149 2023-07-17 15:11:02.194661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0048_c1s1_005351_01.jpg
+-rw-r--r--   0        0        0     1890 2023-07-17 15:11:02.198661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0065_c6s1_009501_02.jpg
+-rw-r--r--   0        0        0     3554 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/trt_calibrator.py
+-rw-r--r--   0        0        0     5602 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/trt_export.py
+-rw-r--r--   0        0        0     6593 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/trt_inference.py
+-rw-r--r--   0        0        0     7297 2023-07-17 15:11:02.202661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/plain_train_net.py
+-rw-r--r--   0        0        0     1321 2023-07-17 15:11:02.206661 initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/train_net.py
+-rw-r--r--   0        0        0    11436 2023-07-18 15:18:02.865987 initor_bot_inference-2.0.2/src/initor_bot_inference/tools/__pycache__/demo.cpython-38.pyc
+-rw-r--r--   0        0        0    15899 2023-07-19 12:17:09.742698 initor_bot_inference-2.0.2/src/initor_bot_inference/tools/demo.py
+-rw-r--r--   0        0        0    18079 2023-07-17 15:12:35.360422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-02.txt
+-rw-r--r--   0        0        0    31683 2023-07-17 15:12:35.364422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-04.txt
+-rw-r--r--   0        0        0    25490 2023-07-17 15:12:35.372422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-05.txt
+-rw-r--r--   0        0        0    15909 2023-07-17 15:12:35.380422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-09.txt
+-rw-r--r--   0        0        0    19852 2023-07-17 15:12:35.384422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-10.txt
+-rw-r--r--   0        0        0    27360 2023-07-17 15:12:35.388422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-11.txt
+-rw-r--r--   0        0        0    23091 2023-07-17 15:12:35.396422 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-13.txt
+-rw-r--r--   0        0        0    27319 2023-07-17 15:12:35.404423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-01.txt
+-rw-r--r--   0        0        0    36372 2023-07-17 15:12:35.408423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-02.txt
+-rw-r--r--   0        0        0    91385 2023-07-17 15:12:35.420423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-03.txt
+-rw-r--r--   0        0        0    63832 2023-07-17 15:12:35.424423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-04.txt
+-rw-r--r--   0        0        0    51181 2023-07-17 15:12:35.432423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-05.txt
+-rw-r--r--   0        0        0    73362 2023-07-17 15:12:35.440423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-06.txt
+-rw-r--r--   0        0        0    30617 2023-07-17 15:12:35.448423 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-07.txt
+-rw-r--r--   0        0        0    37991 2023-07-17 15:12:35.452424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-08.txt
+-rw-r--r--   0        0        0    31899 2023-07-17 15:12:35.460424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-09.txt
+-rw-r--r--   0        0        0    39983 2023-07-17 15:12:35.468424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-10.txt
+-rw-r--r--   0        0        0    55004 2023-07-17 15:12:35.472424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-11.txt
+-rw-r--r--   0        0        0    55025 2023-07-17 15:12:35.480424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-12.txt
+-rw-r--r--   0        0        0    46217 2023-07-17 15:12:35.488424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-13.txt
+-rw-r--r--   0        0        0    46034 2023-07-17 15:12:35.496425 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-14.txt
+-rw-r--r--   0        0        0    25981 2023-07-17 15:12:35.500424 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-01.txt
+-rw-r--r--   0        0        0   170865 2023-07-17 15:12:35.520425 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-02.txt
+-rw-r--r--   0        0        0   147829 2023-07-17 15:12:35.536425 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-03.txt
+-rw-r--r--   0        0        0   127752 2023-07-17 15:12:35.544425 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-04.txt
+-rw-r--r--   0        0        0   204914 2023-07-17 15:12:35.556426 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-05.txt
+-rw-r--r--   0        0        0    61339 2023-07-17 15:12:35.564426 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-06.txt
+-rw-r--r--   0        0        0    35519 2023-07-17 15:12:35.568426 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-07.txt
+-rw-r--r--   0        0        0    49029 2023-07-17 15:12:35.576426 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-08.txt
+-rw-r--r--   0        0        0     2159 2023-07-17 18:04:55.260546 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/basetrack.cpython-38.pyc
+-rw-r--r--   0        0        0    12369 2023-07-17 18:04:54.908542 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/bot_sort.cpython-38.pyc
+-rw-r--r--   0        0        0     6224 2023-07-17 18:04:55.260546 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/gmc.cpython-38.pyc
+-rw-r--r--   0        0        0     8086 2023-07-17 18:04:55.256546 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/kalman_filter.cpython-38.pyc
+-rw-r--r--   0        0        0     6739 2023-07-17 18:04:54.908542 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/matching.cpython-38.pyc
+-rw-r--r--   0        0        0     1111 2023-07-17 15:12:35.624427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/basetrack.py
+-rw-r--r--   0        0        0    16778 2023-07-17 15:12:35.624427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/bot_sort.py
+-rw-r--r--   0        0        0    11753 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/gmc.py
+-rw-r--r--   0        0        0     9671 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/kalman_filter.py
+-rw-r--r--   0        0        0     6435 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/matching.py
+-rw-r--r--   0        0        0    17072 2023-07-17 15:12:35.628427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/mc_bot_sort.py
+-rw-r--r--   0        0        0     1158 2023-07-17 15:12:35.632427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-37.pyc
+-rw-r--r--   0        0        0     1139 2023-07-17 18:04:56.464560 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-38.pyc
+-rw-r--r--   0        0        0     4050 2023-07-17 15:12:35.640427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/evaluation.py
+-rw-r--r--   0        0        0     3627 2023-07-17 15:12:35.640427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/io.py
+-rw-r--r--   0        0        0      958 2023-07-17 15:12:35.640427 initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/timer.py
+-rwxr-xr-x   0        0        0  7620976 2023-07-17 15:12:35.860431 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/_C.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      126 2023-07-17 15:12:35.860431 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      152 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/core/__init__.py
+-rw-r--r--   0        0        0     7038 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/core/launch.py
+-rw-r--r--   0        0        0    10932 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/core/trainer.py
+-rw-r--r--   0        0        0      330 2023-07-17 15:12:35.888432 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-17 15:12:35.908432 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      456 2023-07-17 18:04:54.404537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7352 2023-07-17 15:12:35.932433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-37.pyc
+-rw-r--r--   0        0        0     7428 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-38.pyc
+-rw-r--r--   0        0        0     2524 2023-07-17 15:12:35.944433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-37.pyc
+-rw-r--r--   0        0        0     2553 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-38.pyc
+-rw-r--r--   0        0        0     5419 2023-07-17 15:12:35.960433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-37.pyc
+-rw-r--r--   0        0        0     5438 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-38.pyc
+-rw-r--r--   0        0        0     3992 2023-07-17 15:12:35.972433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-37.pyc
+-rw-r--r--   0        0        0     4035 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-38.pyc
+-rw-r--r--   0        0        0     9378 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/data_augment.py
+-rw-r--r--   0        0        0     2298 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/data_prefetcher.py
+-rw-r--r--   0        0        0     6231 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/dataloading.py
+-rw-r--r--   0        0        0      240 2023-07-17 15:12:35.980433 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__init__.py
+-rw-r--r--   0        0        0      356 2023-07-17 15:12:36.008434 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      355 2023-07-17 18:04:54.408537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4275 2023-07-17 15:12:36.024434 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-37.pyc
+-rw-r--r--   0        0        0     4246 2023-07-17 18:04:54.412537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0     6232 2023-07-17 15:12:36.036435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-37.pyc
+-rw-r--r--   0        0        0     6311 2023-07-17 18:04:54.412537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-38.pyc
+-rw-r--r--   0        0        0     4818 2023-07-17 18:04:54.412537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/mot.cpython-38.pyc
+-rw-r--r--   0        0        0     4250 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/datasets_wrapper.py
+-rw-r--r--   0        0        0    10196 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/mosaicdetection.py
+-rw-r--r--   0        0        0     4532 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/mot.py
+-rw-r--r--   0        0        0     3356 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/samplers.py
+-rw-r--r--   0        0        0      178 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/__init__.py
+-rw-r--r--   0        0        0     7476 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/coco_evaluator.py
+-rw-r--r--   0        0        0     6562 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/evaluation.py
+-rw-r--r--   0        0        0    31896 2023-07-17 15:12:36.052435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/mot_evaluator.py
+-rw-r--r--   0        0        0      191 2023-07-17 15:12:36.056435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-17 15:12:36.060435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      268 2023-07-17 18:04:54.896542 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2782 2023-07-17 15:12:36.076435 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-37.pyc
+-rw-r--r--   0        0        0     2843 2023-07-17 18:04:54.896542 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-38.pyc
+-rw-r--r--   0        0        0     1511 2023-07-17 15:12:36.088436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-37.pyc
+-rw-r--r--   0        0        0     1532 2023-07-17 18:04:54.900542 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-38.pyc
+-rw-r--r--   0        0        0     6032 2023-07-17 15:12:36.100436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-37.pyc
+-rw-r--r--   0        0        0     6045 2023-07-17 18:04:54.904543 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-38.pyc
+-rw-r--r--   0        0        0     2004 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/base_exp.py
+-rw-r--r--   0        0        0     1493 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/build.py
+-rw-r--r--   0        0        0     8227 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/yolox_base.py
+-rw-r--r--   0        0        0     1320 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/nano.py
+-rw-r--r--   0        0        0     3006 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolov3.py
+-rw-r--r--   0        0        0      355 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolox_l.py
+-rw-r--r--   0        0        0      357 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolox_m.py
+-rw-r--r--   0        0        0      357 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolox_s.py
+-rw-r--r--   0        0        0      496 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolox_tiny.py
+-rw-r--r--   0        0        0      357 2023-07-17 15:12:36.112436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolox_x.py
+-rw-r--r--   0        0        0     3381 2023-07-17 15:12:36.128436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_ablation.cpython-37.pyc
+-rw-r--r--   0        0        0     3383 2023-07-17 15:12:36.136436 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-37.pyc
+-rw-r--r--   0        0        0     3420 2023-07-18 15:12:13.551974 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-38.pyc
+-rw-r--r--   0        0        0     3384 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_mot20_ch.cpython-37.pyc
+-rw-r--r--   0        0        0     4352 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_l_mix_det.py
+-rw-r--r--   0        0        0     4354 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_m_mix_det.py
+-rw-r--r--   0        0        0     5189 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_nano_mix_det.py
+-rw-r--r--   0        0        0     4354 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_s_mix_det.py
+-rw-r--r--   0        0        0     4387 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_tiny_mix_det.py
+-rw-r--r--   0        0        0     4358 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ablation.py
+-rw-r--r--   0        0        0     4354 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ch.py
+-rw-r--r--   0        0        0     4605 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_det.py
+-rw-r--r--   0        0        0     4498 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_mot20_ch.py
+-rw-r--r--   0        0        0     4356 2023-07-17 15:12:36.148437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mot17_half.py
+-rw-r--r--   0        0        0      151 2023-07-17 15:12:36.152437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/__init__.py
+-rw-r--r--   0        0        0    20824 2023-07-17 15:12:36.160437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.cpp
+-rw-r--r--   0        0        0     3485 2023-07-17 15:12:36.164437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.h
+-rw-r--r--   0        0        0      524 2023-07-17 15:12:36.172437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/csrc/vision.cpp
+-rw-r--r--   0        0        0     5757 2023-07-17 15:12:36.172437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/fast_coco_eval_api.py
+-rw-r--r--   0        0        0      297 2023-07-17 15:12:36.172437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-17 15:12:36.184437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      414 2023-07-18 15:12:13.555975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4611 2023-07-17 15:12:36.196437 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-37.pyc
+-rw-r--r--   0        0        0     4579 2023-07-18 15:12:13.555975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-38.pyc
+-rw-r--r--   0        0        0     2903 2023-07-17 15:12:36.208438 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-37.pyc
+-rw-r--r--   0        0        0     2930 2023-07-18 15:12:13.559975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-38.pyc
+-rw-r--r--   0        0        0     6970 2023-07-17 15:12:36.220438 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-37.pyc
+-rw-r--r--   0        0        0     6954 2023-07-18 15:12:13.559975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-38.pyc
+-rw-r--r--   0        0        0     2557 2023-07-17 15:12:36.236438 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-37.pyc
+-rw-r--r--   0        0        0     2584 2023-07-18 15:12:13.559975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-38.pyc
+-rw-r--r--   0        0        0    11850 2023-07-17 15:12:36.248438 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-37.pyc
+-rw-r--r--   0        0        0    12118 2023-07-18 15:12:13.563975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-38.pyc
+-rw-r--r--   0        0        0     2495 2023-07-17 15:12:36.264439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-37.pyc
+-rw-r--r--   0        0        0     2556 2023-07-18 15:12:13.567975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-38.pyc
+-rw-r--r--   0        0        0     1300 2023-07-17 15:12:36.280439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-37.pyc
+-rw-r--r--   0        0        0     1315 2023-07-18 15:12:13.567975 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-38.pyc
+-rw-r--r--   0        0        0     6028 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/darknet.py
+-rw-r--r--   0        0        0     2900 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/losses.py
+-rw-r--r--   0        0        0     6102 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/network_blocks.py
+-rw-r--r--   0        0        0     2486 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolo_fpn.py
+-rw-r--r--   0        0        0    24140 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolo_head.py
+-rw-r--r--   0        0        0     3540 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolo_pafpn.py
+-rw-r--r--   0        0        0     1374 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolox.py
+-rw-r--r--   0        0        0     3437 2023-07-17 15:12:36.288439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/train.py
+-rw-r--r--   0        0        0      450 2023-07-17 15:12:36.292439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-17 15:12:36.296439 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      521 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3293 2023-07-17 15:12:36.308440 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-37.pyc
+-rw-r--r--   0        0        0     3328 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-38.pyc
+-rw-r--r--   0        0        0     3969 2023-07-17 15:12:36.324440 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-37.pyc
+-rw-r--r--   0        0        0     4012 2023-07-17 18:04:54.016533 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-38.pyc
+-rw-r--r--   0        0        0     1143 2023-07-17 15:12:36.332440 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-37.pyc
+-rw-r--r--   0        0        0     1160 2023-07-17 18:04:54.340536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-38.pyc
+-rw-r--r--   0        0        0     2601 2023-07-17 15:12:36.344440 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-37.pyc
+-rw-r--r--   0        0        0     2607 2023-07-17 18:04:54.340536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     6504 2023-07-17 15:12:36.360441 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-37.pyc
+-rw-r--r--   0        0        0     6511 2023-07-17 18:04:54.012533 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-38.pyc
+-rw-r--r--   0        0        0     2719 2023-07-17 15:12:36.372441 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-37.pyc
+-rw-r--r--   0        0        0     2736 2023-07-17 18:04:54.344536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-38.pyc
+-rw-r--r--   0        0        0     2888 2023-07-17 15:12:36.384441 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-37.pyc
+-rw-r--r--   0        0        0     2913 2023-07-17 18:04:54.344536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-38.pyc
+-rw-r--r--   0        0        0     3974 2023-07-17 15:12:36.396441 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-37.pyc
+-rw-r--r--   0        0        0     3982 2023-07-17 18:04:54.344536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-38.pyc
+-rw-r--r--   0        0        0     4477 2023-07-17 15:12:36.412441 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-37.pyc
+-rw-r--r--   0        0        0     4546 2023-07-17 18:04:54.348536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     2725 2023-07-17 15:12:36.424442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-37.pyc
+-rw-r--r--   0        0        0     2750 2023-07-17 18:04:54.348536 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     1336 2023-07-17 15:12:36.436442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-37.pyc
+-rw-r--r--   0        0        0     1345 2023-07-17 18:04:54.396537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-38.pyc
+-rw-r--r--   0        0        0     3636 2023-07-17 18:04:54.400537 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/visualize.cpython-38.pyc
+-rw-r--r--   0        0        0     2845 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/allreduce_norm.py
+-rw-r--r--   0        0        0     4269 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/boxes.py
+-rw-r--r--   0        0        0     1331 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/checkpoint.py
+-rw-r--r--   0        0        0     2806 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/demo_utils.py
+-rw-r--r--   0        0        0     7066 2023-07-17 15:12:36.448442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/dist.py
+-rw-r--r--   0        0        0     2533 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/ema.py
+-rw-r--r--   0        0        0     2751 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/logger.py
+-rw-r--r--   0        0        0     6561 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/lr_scheduler.py
+-rw-r--r--   0        0        0     3094 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/metric.py
+-rw-r--r--   0        0        0     3269 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/model_utils.py
+-rw-r--r--   0        0        0     1574 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/setup_env.py
+-rw-r--r--   0        0        0     4958 2023-07-17 15:12:36.452442 initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/visualize.py
+-rw-r--r--   0        0        0     7857 2023-07-19 12:17:24.543270 initor_bot_inference-2.0.2/setup.py
+-rw-r--r--   0        0        0     1373 2023-07-19 12:17:24.543720 initor_bot_inference-2.0.2/PKG-INFO
```

### Comparing `initor_bot_inference-2.0.1/pyproject.toml` & `initor_bot_inference-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "initor_bot_inference"
-version = "2.0.1"
+version = "2.0.2"
 description = ""
 authors = ["s"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "1.23.5"
 opencv-python = "^4.8.0"
```

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/FastReID-Logo.png` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/FastReID-Logo.png`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/bugs.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/bugs.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/questions-help-support.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/questions-help-support.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/unexpected-problems-bugs.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/ISSUE_TEMPLATE/unexpected-problems-bugs.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/wechat_group.png` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/wechat_group.png`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/workflows/issue_auto_close.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/workflows/issue_auto_close.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/.github/workflows/lint_python.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/.github/workflows/lint_python.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/CHANGELOG.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/GETTING_STARTED.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/INSTALL.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/INSTALL.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/LICENSE` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/LICENSE`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/MODEL_ZOO.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/MODEL_ZOO.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/__pycache__/fast_reid_interfece.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/__pycache__/fast_reid_interfece.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Base-SBS.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Base-SBS.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Base-bagtricks.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Base-bagtricks.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_vit.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/Market1501/bagtricks_vit.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/VERIWild/bagtricks_R50-ibn.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/VERIWild/bagtricks_R50-ibn.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/configs/VehicleID/bagtricks_R50-ibn.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/configs/VehicleID/bagtricks_R50-ibn.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/datasets/generate_mot_patches.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/datasets/generate_mot_patches.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/demo.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/demo.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/plot_roc_with_pickle.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/plot_roc_with_pickle.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/predictor.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/predictor.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/demo/visualize_result.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/demo/visualize_result.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docker/Dockerfile` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docker/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docker/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/Makefile` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/Makefile`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/conf.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/conf.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/data.rst` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/data.rst`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/modeling.rst` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/modeling.rst`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/docs/modules/utils.rst` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/docs/modules/utils.rst`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fast_reid_interfece.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fast_reid_interfece.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/config.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/defaults.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/__pycache__/defaults.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/config.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/config.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/config/defaults.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/config/defaults.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/common.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/data_utils.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/__pycache__/data_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/common.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/common.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/data_utils.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/AirportALERT.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/AirportALERT.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__init__.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/AirportALERT.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/AirportALERT.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/bases.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/bases.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/caviara.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/caviara.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk03.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk03.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk_sysu.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/cuhk_sysu.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/dukemtmcreid.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/dukemtmcreid.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/grid.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/grid.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/iLIDS.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/iLIDS.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/lpw.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/lpw.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/market1501.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/market1501.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot17.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot17.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot20.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/mot20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/msmt17.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/msmt17.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pes3d.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pes3d.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pku.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/pku.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prai.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prai.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prid.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/prid.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/saivt.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/saivt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sensereid.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sensereid.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/shinpuhkan.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/shinpuhkan.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sysu_mm.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/sysu_mm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/thermalworld.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/thermalworld.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/vehicleid.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/vehicleid.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veri.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veri.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veriwild.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/veriwild.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/viper.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/viper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/wildtracker.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/__pycache__/wildtracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/bases.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/bases.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/caviara.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/caviara.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk03.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk03.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk_sysu.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/cuhk_sysu.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/dukemtmcreid.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/dukemtmcreid.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/grid.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/grid.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/iLIDS.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/iLIDS.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/lpw.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/lpw.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/market1501.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/market1501.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot17.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot17.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20_.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/mot20_.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/msmt17.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/msmt17.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pes3d.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pes3d.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pku.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/pku.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prai.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prai.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prid.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/prid.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/saivt.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/saivt.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sensereid.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sensereid.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/shinpuhkan.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/shinpuhkan.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sysu_mm.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/sysu_mm.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/thermalworld.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/thermalworld.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/vehicleid.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/vehicleid.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veri.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veri.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veriwild.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/veriwild.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/viper.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/viper.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/datasets/wildtracker.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/datasets/wildtracker.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/data_sampler.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/data_sampler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/imbalance_sampler.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/imbalance_sampler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/triplet_sampler.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/__pycache__/triplet_sampler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/data_sampler.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/imbalance_sampler.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/imbalance_sampler.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/samplers/triplet_sampler.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/samplers/triplet_sampler.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/autoaugment.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/autoaugment.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/functional.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/functional.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/transforms.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/__pycache__/transforms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/autoaugment.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/autoaugment.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/functional.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/functional.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/data/transforms/transforms.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/data/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/defaults.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/defaults.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/hooks.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/hooks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/launch.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/launch.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/train_loop.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/__pycache__/train_loop.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/defaults.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/hooks.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/launch.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/launch.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/engine/train_loop.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/clas_evaluator.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/clas_evaluator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/evaluator.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/evaluator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/query_expansion.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/query_expansion.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/reid_evaluation.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/reid_evaluation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/testing.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/__pycache__/testing.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/clas_evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/clas_evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/query_expansion.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/query_expansion.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.c` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.c`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.pyx` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/rank_cy.pyx`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.c` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.c`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.pyx` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/roc_cy.pyx`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/setup.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/setup.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/test_cython.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rank_cylib/test_cython.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/reid_evaluation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/reid_evaluation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/rerank.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/rerank.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/roc.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/roc.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/evaluation/testing.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__init__.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/activation.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/activation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/any_softmax.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/any_softmax.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/batch_norm.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/batch_norm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/context_block.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/context_block.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/drop.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/drop.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/frn.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/frn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/gather_layer.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/gather_layer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/helpers.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/non_local.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/non_local.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/pooling.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/pooling.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/se_layer.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/se_layer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/splat.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/splat.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/weight_init.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/__pycache__/weight_init.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/activation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/activation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/any_softmax.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/any_softmax.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/batch_norm.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/context_block.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/context_block.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/drop.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/drop.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/frn.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/frn.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/gather_layer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/gather_layer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/helpers.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/helpers.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/non_local.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/non_local.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/pooling.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/se_layer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/se_layer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/splat.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/splat.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/layers/weight_init.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__init__.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenetv3.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/mobilenetv3.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/osnet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/osnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/repvgg.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/repvgg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnest.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnest.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnext.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/resnext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/shufflenet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/shufflenet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/vision_transformer.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/__pycache__/vision_transformer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenetv3.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/osnet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/osnet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/config.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/effnet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/effnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/regnet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/__pycache__/regnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/config.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/config.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/effnet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/regnet/regnet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/repvgg.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/repvgg.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnest.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnext.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/shufflenet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/shufflenet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/vision_transformer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/backbones/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/clas_head.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/clas_head.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/embedding_head.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/__pycache__/embedding_head.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/clas_head.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/clas_head.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/embedding_head.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/heads/embedding_head.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/circle_loss.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/circle_loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/cross_entroy_loss.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/cross_entroy_loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/focal_loss.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/focal_loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/triplet_loss.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/triplet_loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/utils.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/circle_loss.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/cross_entroy_loss.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/cross_entroy_loss.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/focal_loss.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/triplet_loss.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/utils.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/losses/utils.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/baseline.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/baseline.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/distiller.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/distiller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/mgn.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/mgn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/moco.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/__pycache__/moco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/baseline.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/baseline.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/distiller.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/distiller.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/mgn.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/mgn.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/moco.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/modeling/meta_arch/moco.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/lr_scheduler.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/__pycache__/lr_scheduler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/lr_scheduler.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/lamb.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/lamb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/radam.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/radam.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/swa.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/__pycache__/swa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/lamb.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/lamb.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/radam.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/radam.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/solver/optim/swa.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/solver/optim/swa.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/checkpoint.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/checkpoint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/collect_env.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/collect_env.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/comm.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/comm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/compute_dist.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/compute_dist.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/env.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/env.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/events.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/events.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/faiss_utils.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/faiss_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/file_io.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/file_io.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/history_buffer.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/history_buffer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/logger.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/params.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/params.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/precision_bn.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/precision_bn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/registry.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/registry.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/timer.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/__pycache__/timer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/checkpoint.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/collect_env.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/comm.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/comm.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/compute_dist.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/compute_dist.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/env.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/env.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/events.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/events.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/faiss_utils.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/faiss_utils.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/file_io.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/history_buffer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/history_buffer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/logger.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/logger.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/params.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/params.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/precision_bn.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/precision_bn.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/registry.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/registry.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/summary.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/summary.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/timer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/fastreid/utils/visualizer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/fastreid/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/CrossDomainReID/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/CrossDomainReID/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/DG-ReID/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/DG-ReID/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/Base-attribute.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/configs/Base-attribute.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_dataset.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_dataset.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_evaluation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/attr_evaluation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/bases.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/bases.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/dukemtmcattr.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/dukemtmcattr.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/market1501attr.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/market1501attr.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/pa100k.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/datasets/pa100k.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_baseline.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_baseline.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_head.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/attr_head.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/bce_loss.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/fastattr/modeling/bce_loss.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastAttr/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastAttr/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/configs/base-clas.yaml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/configs/base-clas.yaml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/bee_ant.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/bee_ant.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/dataset.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/dataset.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/trainer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/fastclas/trainer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastClas/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastClas/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/overhaul.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/overhaul.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/resnet_distill.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/fastdistill/resnet_distill.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastDistill/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastDistill/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/configs/face_base.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/configs/face_base.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/ms1mv2.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/ms1mv2.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/test_dataset.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/datasets/test_dataset.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_data.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_data.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/face_evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_baseline.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_baseline.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_head.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/face_head.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/iresnet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/iresnet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/partial_fc.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/modeling/partial_fc.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/pfc_checkpointer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/pfc_checkpointer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/trainer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/trainer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/utils_amp.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/utils_amp.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/verification.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/fastface/verification.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastFace/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastFace/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/CMakeLists.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/demo/CMakeLists.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/demo/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/demo/inference.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/demo/inference.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/docker/trt7cu102/Dockerfile` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/docker/trt7cu102/Dockerfile`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/CMakeLists.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/backbones/sbs_resnet.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/backbones/sbs_resnet.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/calibrator.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/calibrator.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/utils.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/common/utils.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/engine/InferenceEngine.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/engine/InferenceEngine.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/factory/factory.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/factory/factory.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/heads/embedding_head.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/heads/embedding_head.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/layers.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/layers.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/layers/poolingLayerRT.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/baseline.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/baseline.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/model.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/fastrt/meta_arch/model.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/InferenceEngine.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/InferenceEngine.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/baseline.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/baseline.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/calibrator.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/calibrator.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/embedding_head.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/embedding_head.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/factory.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/factory.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/holder.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/holder.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/layers.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/layers.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/logging.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/logging.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/model.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/model.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/sbs_resnet.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/sbs_resnet.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/struct.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/struct.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/utils.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/include/fastrt/utils.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/CMakeLists.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/docker/trt7cu100/Dockerfile` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/docker/trt7cu100/Dockerfile`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/market_benchmark.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/market_benchmark.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/reid.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/reid.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/test.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/pybind_interface/test.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/CMakeLists.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/LICENSE` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/LICENSE`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/cnpy.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/example1.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/third_party/cnpy/example1.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/tools/How_to_Generate.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/tools/How_to_Generate.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRT/tools/gen_wts.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRT/tools/gen_wts.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/base-image_retri.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/configs/base-image_retri.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/datasets.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/datasets.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/retri_evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/fastretri/retri_evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastRetri/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastRetri/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/autotuner/tune_hooks.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/autotuner/tune_hooks.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/configs/search_trial.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/configs/search_trial.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/FastTune/tune_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/FastTune/tune_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/HAA/Readme.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/HAA/Readme.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/Base-naic.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/configs/Base-naic.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/label.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/label.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_dataset.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_dataset.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic/naic_evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/naic20r2_train_list_clean.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/naic20r2_train_list_clean.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/train_list_clean.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/train_list_clean.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/val_gallery.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/val_gallery.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/NAIC20/val_query.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/NAIC20/val_query.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/configs/partial_market.yml` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/configs/partial_market.yml`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_distance.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_distance.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_evaluation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_evaluation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_head.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/dsr_head.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partial_dataset.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partial_dataset.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partialbaseline.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/partialreid/partialbaseline.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/PartialReID/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/PartialReID/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/projects/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/projects/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/dataset_test.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/dataset_test.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/feature_align.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/feature_align.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/interp_test.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/interp_test.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/lr_scheduler_test.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/lr_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/model_test.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tests/test_repvgg.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tests/test_repvgg.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/ReadMe.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/ReadMe.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe.proto` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe.proto`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_lmdb.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_lmdb.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_pb2.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/caffe_pb2.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/layer_param.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/Caffe/layer_param.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/README.md` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/README.md`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/caffe_export.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/caffe_export.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/caffe_inference.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/caffe_inference.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/onnx_export.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/onnx_export.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/onnx_inference.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/onnx_inference.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/pytorch_to_caffe.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/pytorch_to_caffe.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0022_c6s1_002976_01.jpg` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0022_c6s1_002976_01.jpg`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0027_c2s2_091032_02.jpg` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0027_c2s2_091032_02.jpg`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0032_c6s1_002851_01.jpg` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0032_c6s1_002851_01.jpg`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0048_c1s1_005351_01.jpg` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0048_c1s1_005351_01.jpg`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0065_c6s1_009501_02.jpg` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/test_data/0065_c6s1_009501_02.jpg`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/trt_calibrator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/trt_calibrator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/trt_export.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/trt_export.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/deploy/trt_inference.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/deploy/trt_inference.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/plain_train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/plain_train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/fast_reid/tools/train_net.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/fast_reid/tools/train_net.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tools/__pycache__/demo.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tools/__pycache__/demo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tools/demo.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tools/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import cv2
 import torch
 import json
 from loguru import logger
 
 sys.path.append('.')
 
-from yolox.data.data_augment import preproc
-from yolox.exp import get_exp
-from yolox.utils import fuse_model, get_model_info, postprocess
-from yolox.utils.visualize import plot_tracking
-from tracker.bot_sort import BoTSORT
-from tracker.tracking_utils.timer import Timer
+from ..yolox.data.data_augment import preproc
+from ..yolox.exp import get_exp
+from ..yolox.utils import fuse_model, get_model_info, postprocess
+from ..yolox.utils.visualize import plot_tracking
+from ..tracker.bot_sort import BoTSORT
+from ..tracker.tracking_utils.timer import Timer
 
 IMAGE_EXT = [".jpg", ".jpeg", ".webp", ".bmp", ".png", ".PNG"]
 
 class params:
      
     # constructor
     def __init__(self, dict1):
```

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-02.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-02.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-04.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-04.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-05.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-05.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-09.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-09.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-10.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-10.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-11.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-11.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-13.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOT17_ablation/GMC-MOT17-13.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-01.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-01.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-02.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-02.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-03.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-03.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-04.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-04.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-05.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-05.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-06.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-06.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-07.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-07.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-08.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-08.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-09.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-09.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-10.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-10.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-11.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-11.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-12.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-12.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-13.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-13.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-14.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT17-14.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-01.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-01.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-02.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-02.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-03.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-03.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-04.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-04.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-05.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-05.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-06.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-06.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-07.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-07.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-08.txt` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/GMC_files/MOTChallenge/GMC-MOT20-08.txt`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/basetrack.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/basetrack.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/bot_sort.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/bot_sort.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/gmc.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/gmc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/kalman_filter.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/kalman_filter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/__pycache__/matching.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/__pycache__/matching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/basetrack.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/bot_sort.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/bot_sort.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/gmc.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/gmc.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/kalman_filter.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/matching.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/mc_bot_sort.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/mc_bot_sort.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/__pycache__/timer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/evaluation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/io.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/io.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/tracker/tracking_utils/timer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/tracker/tracking_utils/timer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/_C.cpython-38-x86_64-linux-gnu.so` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/_C.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/core/launch.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/core/launch.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/core/trainer.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/core/trainer.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_augment.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/data_prefetcher.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/dataloading.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/__pycache__/samplers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/data_augment.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/data_augment.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/data_prefetcher.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/dataloading.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/dataloading.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/datasets_wrapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/mosaicdetection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/__pycache__/mot.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/__pycache__/mot.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/datasets_wrapper.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/datasets_wrapper.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/mosaicdetection.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/mosaicdetection.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/datasets/mot.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/datasets/mot.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/data/samplers.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/data/samplers.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/coco_evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/coco_evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/evaluation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/evaluation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/evaluators/mot_evaluator.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/evaluators/mot_evaluator.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/base_exp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/build.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/__pycache__/yolox_base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/base_exp.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/base_exp.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/build.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/build.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exp/yolox_base.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exp/yolox_base.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/nano.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/nano.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/default/yolov3.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/default/yolov3.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_ablation.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_ablation.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_det.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_mot20_ch.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/__pycache__/yolox_x_mix_mot20_ch.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_l_mix_det.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_l_mix_det.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_m_mix_det.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_m_mix_det.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_nano_mix_det.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_nano_mix_det.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_s_mix_det.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_s_mix_det.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_tiny_mix_det.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_tiny_mix_det.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ablation.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ablation.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ch.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_ch.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_det.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_det.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_mot20_ch.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mix_mot20_ch.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mot17_half.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/exps/example/mot/yolox_x_mot17_half.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.h` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/csrc/cocoeval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/csrc/vision.cpp` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/csrc/vision.cpp`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/layers/fast_coco_eval_api.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/layers/fast_coco_eval_api.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/darknet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/losses.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/network_blocks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_fpn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_head.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolo_pafpn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/__pycache__/yolox.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/darknet.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/losses.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/network_blocks.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolo_fpn.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolo_head.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolo_pafpn.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/models/yolox.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/train.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/train.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/allreduce_norm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/boxes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/checkpoint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/demo_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/dist.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/ema.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/lr_scheduler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/metric.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/model_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-37.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/setup_env.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/__pycache__/visualize.cpython-38.pyc` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/__pycache__/visualize.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/allreduce_norm.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/allreduce_norm.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/boxes.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/checkpoint.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/demo_utils.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/demo_utils.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/dist.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/dist.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/ema.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/ema.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/logger.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/logger.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/lr_scheduler.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/metric.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/metric.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/model_utils.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/setup_env.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/src/initor_bot_inference/yolox/utils/visualize.py` & `initor_bot_inference-2.0.2/src/initor_bot_inference/yolox/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `initor_bot_inference-2.0.1/setup.py` & `initor_bot_inference-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
  'thop>=0.1.1,<0.2.0',
  'torchvision==0.12.0',
  'tqdm>=4.65.0,<5.0.0',
  'yacs>=0.1.8,<0.2.0']
 
 setup_kwargs = {
     'name': 'initor-bot-inference',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': '',
     'long_description': None,
     'author': 's',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `initor_bot_inference-2.0.1/PKG-INFO` & `initor_bot_inference-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: initor-bot-inference
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 Author: s
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

