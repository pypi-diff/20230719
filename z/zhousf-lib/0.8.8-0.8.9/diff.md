# Comparing `tmp/zhousf-lib-0.8.8.tar.gz` & `tmp/zhousf-lib-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.8.8.tar", last modified: Tue Jul 18 09:40:11 2023, max compression
+gzip compressed data, was "zhousf-lib-0.8.9.tar", last modified: Wed Jul 19 06:05:03 2023, max compression
```

## Comparing `zhousf-lib-0.8.8.tar` & `zhousf-lib-0.8.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.829461 zhousf-lib-0.8.8/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.8.8/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-07-18 09:40:11.828461 zhousf-lib-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.8.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 09:40:11.829461 zhousf-lib-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-07-18 09:39:58.000000 zhousf-lib-0.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.753463 zhousf-lib-0.8.8/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-07-18 09:40:11.000000 zhousf-lib-0.8.8/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2257 2023-07-18 09:40:11.000000 zhousf-lib-0.8.8/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 09:40:11.000000 zhousf-lib-0.8.8/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 09:40:11.000000 zhousf-lib-0.8.8/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.754461 zhousf-lib-0.8.8/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.8.8/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.755463 zhousf-lib-0.8.8/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.8.8/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.757461 zhousf-lib-0.8.8/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.8.8/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.762461 zhousf-lib-0.8.8/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       73 2023-07-11 01:24:38.000000 zhousf-lib-0.8.8/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.767461 zhousf-lib-0.8.8/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.769461 zhousf-lib-0.8.8/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.8.8/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.771461 zhousf-lib-0.8.8/zhousflib/db/
--rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.8.8/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.8.8/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.773463 zhousf-lib-0.8.8/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.8/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-18 05:47:21.000000 zhousf-lib-0.8.8/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.775461 zhousf-lib-0.8.8/zhousflib/download/
--rw-rw-rw-   0        0        0       60 2023-06-16 08:05:46.000000 zhousf-lib-0.8.8/zhousflib/download/__init__.py
--rw-rw-rw-   0        0        0     4646 2023-06-16 08:07:58.000000 zhousf-lib-0.8.8/zhousflib/download/download_util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.790461 zhousf-lib-0.8.8/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.8.8/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.8.8/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.8.8/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.791463 zhousf-lib-0.8.8/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.8.8/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.794463 zhousf-lib-0.8.8/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.8.8/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4761 2023-06-19 03:04:32.000000 zhousf-lib-0.8.8/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     5872 2023-06-19 03:04:56.000000 zhousf-lib-0.8.8/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.797463 zhousf-lib-0.8.8/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.8.8/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.799492 zhousf-lib-0.8.8/zhousflib/so/
--rw-rw-rw-   0        0        0       85 2023-06-29 06:08:24.000000 zhousf-lib-0.8.8/zhousflib/so/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-06-27 03:01:19.000000 zhousf-lib-0.8.8/zhousflib/so/project_to_so.py
--rw-rw-rw-   0        0        0      273 2023-06-27 03:01:19.000000 zhousf-lib-0.8.8/zhousflib/so/py_to_so.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.823462 zhousf-lib-0.8.8/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     3103 2023-07-07 08:39:29.000000 zhousf-lib-0.8.8/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0     2067 2023-06-27 02:49:36.000000 zhousf-lib-0.8.8/zhousflib/util/char_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2609 2023-06-16 08:07:58.000000 zhousf-lib-0.8.8/zhousflib/util/dict_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.8.8/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0     1593 2023-06-29 06:32:27.000000 zhousf-lib-0.8.8/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0    13590 2023-07-18 09:25:11.000000 zhousf-lib-0.8.8/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0     1564 2023-06-26 06:05:28.000000 zhousf-lib-0.8.8/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1432 2023-06-16 08:43:33.000000 zhousf-lib-0.8.8/zhousflib/util/math_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.8.8/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      502 2023-06-16 08:10:19.000000 zhousf-lib-0.8.8/zhousflib/util/random_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.8.8/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     2209 2023-06-16 08:11:27.000000 zhousf-lib-0.8.8/zhousflib/util/thread_util.py
--rw-rw-rw-   0        0        0      794 2023-06-16 08:11:54.000000 zhousf-lib-0.8.8/zhousflib/util/threadpool_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.8.8/zhousflib/util/time_util.py
--rw-rw-rw-   0        0        0     3122 2023-06-16 08:43:33.000000 zhousf-lib-0.8.8/zhousflib/util/zip_util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:40:11.827461 zhousf-lib-0.8.8/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.8.8/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.8.8/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.8.8/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.757655 zhousf-lib-0.8.9/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0     2073 2023-07-19 06:05:03.757655 zhousf-lib-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.8.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 06:05:03.757655 zhousf-lib-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-07-19 06:05:01.000000 zhousf-lib-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.681665 zhousf-lib-0.8.9/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-07-19 06:05:03.000000 zhousf-lib-0.8.9/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2257 2023-07-19 06:05:03.000000 zhousf-lib-0.8.9/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 06:05:03.000000 zhousf-lib-0.8.9/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-19 06:05:03.000000 zhousf-lib-0.8.9/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.682672 zhousf-lib-0.8.9/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.8.9/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.684683 zhousf-lib-0.8.9/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.8.9/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.686652 zhousf-lib-0.8.9/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.8.9/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.691654 zhousf-lib-0.8.9/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       73 2023-07-11 01:24:38.000000 zhousf-lib-0.8.9/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.696678 zhousf-lib-0.8.9/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.698654 zhousf-lib-0.8.9/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.8.9/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.700654 zhousf-lib-0.8.9/zhousflib/db/
+-rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.8.9/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.8.9/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.704654 zhousf-lib-0.8.9/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.8.9/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-18 05:47:21.000000 zhousf-lib-0.8.9/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.705654 zhousf-lib-0.8.9/zhousflib/download/
+-rw-rw-rw-   0        0        0       60 2023-06-16 08:05:46.000000 zhousf-lib-0.8.9/zhousflib/download/__init__.py
+-rw-rw-rw-   0        0        0     4646 2023-06-16 08:07:58.000000 zhousf-lib-0.8.9/zhousflib/download/download_util.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.720654 zhousf-lib-0.8.9/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.8.9/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.8.9/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.8.9/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.722655 zhousf-lib-0.8.9/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.8.9/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.724683 zhousf-lib-0.8.9/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.8.9/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4761 2023-06-19 03:04:32.000000 zhousf-lib-0.8.9/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     5872 2023-06-19 03:04:56.000000 zhousf-lib-0.8.9/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.727676 zhousf-lib-0.8.9/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.8.9/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.730655 zhousf-lib-0.8.9/zhousflib/so/
+-rw-rw-rw-   0        0        0       85 2023-06-29 06:08:24.000000 zhousf-lib-0.8.9/zhousflib/so/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-06-27 03:01:19.000000 zhousf-lib-0.8.9/zhousflib/so/project_to_so.py
+-rw-rw-rw-   0        0        0      273 2023-06-27 03:01:19.000000 zhousf-lib-0.8.9/zhousflib/so/py_to_so.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.752656 zhousf-lib-0.8.9/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     3151 2023-07-19 06:01:50.000000 zhousf-lib-0.8.9/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0     2067 2023-06-27 02:49:36.000000 zhousf-lib-0.8.9/zhousflib/util/char_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2609 2023-06-16 08:07:58.000000 zhousf-lib-0.8.9/zhousflib/util/dict_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.8.9/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0     1593 2023-06-29 06:32:27.000000 zhousf-lib-0.8.9/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0    13590 2023-07-18 09:25:11.000000 zhousf-lib-0.8.9/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0     1564 2023-06-26 06:05:28.000000 zhousf-lib-0.8.9/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1432 2023-06-16 08:43:33.000000 zhousf-lib-0.8.9/zhousflib/util/math_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.8.9/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      502 2023-06-16 08:10:19.000000 zhousf-lib-0.8.9/zhousflib/util/random_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.8.9/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     2209 2023-06-16 08:11:27.000000 zhousf-lib-0.8.9/zhousflib/util/thread_util.py
+-rw-rw-rw-   0        0        0      794 2023-06-16 08:11:54.000000 zhousf-lib-0.8.9/zhousflib/util/threadpool_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.8.9/zhousflib/util/time_util.py
+-rw-rw-rw-   0        0        0     3122 2023-06-16 08:43:33.000000 zhousf-lib-0.8.9/zhousflib/util/zip_util.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:05:03.756656 zhousf-lib-0.8.9/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.8.9/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.8.9/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.8.9/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.8.8/LICENSE` & `zhousf-lib-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/PKG-INFO` & `zhousf-lib-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.8.8
+Version: 0.8.9
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.8.8/README.md` & `zhousf-lib-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/setup.py` & `zhousf-lib-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.8.8'
+VERSION = '0.8.9'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.8.8/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.8.9/zhousf_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.8.8
+Version: 0.8.9
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.8.8/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.8.9/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-0.8.9/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.8.9/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.8.9/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.8.9/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.8.9/zhousflib/db/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.8.9/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/download/download_util.py` & `zhousf-lib-0.8.9/zhousflib/download/download_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.8.9/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.8.9/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/font/__init__.py` & `zhousf-lib-0.8.9/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.8.9/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-0.8.9/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.8.9/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/pdf/export_image.py` & `zhousf-lib-0.8.9/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.8.9/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/so/project_to_so.py` & `zhousf-lib-0.8.9/zhousflib/so/project_to_so.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/calculater_util.py` & `zhousf-lib-0.8.9/zhousflib/util/calculater_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if number_str[0] in ["*", "/"]:
             union_symbol = number_str[0]
             number_str = number_str[1:]
     try:
         num = eval("".join(number_str))
     except Exception as e:
         num = number_str
-    if isinstance(type(num), int) or isinstance(type(num), float):
+    if isinstance(num, int) or isinstance(num, float):
         number_str_cal_result = round(num, 8) if len(number_str) > 0 else ""
     else:
         number_str_cal_result = num if len(number_str) > 0 else ""
     not_number_str = ["{0}".format(not_number) for not_number in not_number_list]
     if number_is_first:
         result_union = str(number_str_cal_result) + union_symbol + "".join(not_number_str)
     else:
@@ -76,11 +76,13 @@
     # print(cal(".+250+320+200+200+200"))
     # print(cal("*250+200"))
     # print(cal("+752+2+"))
     # print(cal("+05+120"))
     # print(cal("100*2/4"))
     # print(cal("60.3+733.9"))
     # print(cal("1811-(137+350)"))
-    print(cal("10+20+均353.5"))
+    # print(cal("10+20+均353.5"))
     # print(round(eval("均353.5"), 8))
+    print(cal("811-846.6"))
+    print(cal("846.6-811"))
     pass
```

### Comparing `zhousf-lib-0.8.8/zhousflib/util/char_util.py` & `zhousf-lib-0.8.9/zhousflib/util/char_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/cv_util.py` & `zhousf-lib-0.8.9/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/dict_util.py` & `zhousf-lib-0.8.9/zhousflib/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.8.9/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/img_util.py` & `zhousf-lib-0.8.9/zhousflib/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/iou_util.py` & `zhousf-lib-0.8.9/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/json_util.py` & `zhousf-lib-0.8.9/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/list_util.py` & `zhousf-lib-0.8.9/zhousflib/util/list_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/math_util.py` & `zhousf-lib-0.8.9/zhousflib/util/math_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/permission_util.py` & `zhousf-lib-0.8.9/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/poly_util.py` & `zhousf-lib-0.8.9/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/re_util.py` & `zhousf-lib-0.8.9/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/singleton.py` & `zhousf-lib-0.8.9/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/string_util.py` & `zhousf-lib-0.8.9/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/thread_util.py` & `zhousf-lib-0.8.9/zhousflib/util/thread_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/threadpool_util.py` & `zhousf-lib-0.8.9/zhousflib/util/threadpool_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/time_util.py` & `zhousf-lib-0.8.9/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/util/zip_util.py` & `zhousf-lib-0.8.9/zhousflib/util/zip_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/web/log_util.py` & `zhousf-lib-0.8.9/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/web/logger.py` & `zhousf-lib-0.8.9/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.8.8/zhousflib/web/response.py` & `zhousf-lib-0.8.9/zhousflib/web/response.py`

 * *Files identical despite different names*

