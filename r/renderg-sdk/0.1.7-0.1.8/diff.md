# Comparing `tmp/renderg-sdk-0.1.7.tar.gz` & `tmp/renderg-sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\renderg-sdk-0.1.7.tar", last modified: Tue Jul 18 07:18:59 2023, max compression
+gzip compressed data, was "dist\renderg-sdk-0.1.8.tar", last modified: Wed Jul 19 03:14:25 2023, max compression
```

## Comparing `renderg-sdk-0.1.7.tar` & `renderg-sdk-0.1.8.tar`

### file list

```diff
@@ -1,104 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/
--rw-rw-rw-   0        0        0     3341 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:54.000000 renderg-sdk-0.1.7/analyze_houdini/
--rw-rw-rw-   0        0        0       52 2023-06-20 02:05:27.000000 renderg-sdk-0.1.7/analyze_houdini/__init__.py
--rw-rw-rw-   0        0        0     4084 2023-07-12 07:52:09.000000 renderg-sdk-0.1.7/analyze_houdini/analyze.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:55.000000 renderg-sdk-0.1.7/analyze_houdini/houdini/
--rw-rw-rw-   0        0        0   942080 2023-05-22 08:30:57.000000 renderg-sdk-0.1.7/analyze_houdini/houdini/HoudiniAnalyze.pyd
--rw-rw-rw-   0        0        0  1128448 2023-05-22 08:30:57.000000 renderg-sdk-0.1.7/analyze_houdini/houdini/HoudiniAnalyze_py37.pyd
--rw-rw-rw-   0        0        0   820224 2023-05-22 08:30:57.000000 renderg-sdk-0.1.7/analyze_houdini/houdini/HoudiniAnalyze_py39.pyd
--rw-rw-rw-   0        0        0      708 2023-05-26 09:16:22.000000 renderg-sdk-0.1.7/analyze_houdini/houdini/run.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:55.000000 renderg-sdk-0.1.7/ascp/
--rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.7/ascp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/ascp/bin/
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-file-l1-2-0.dll
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-file-l2-1-0.dll
--rw-rw-rw-   0        0        0    25176 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-localization-l1-2-0.dll
--rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-synch-l1-2-0.dll
--rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll
--rw-rw-rw-   0        0        0    26704 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll
--rw-rw-rw-   0        0        0    24656 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll
--rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll
--rw-rw-rw-   0        0        0    33360 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-math-l1-1-0.dll
--rw-rw-rw-   0        0        0    30800 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll
--rw-rw-rw-   0        0        0    75344 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-private-l1-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-process-l1-1-0.dll
--rw-rw-rw-   0        0        0    27216 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll
--rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll
--rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-string-l1-1-0.dll
--rw-rw-rw-   0        0        0    25168 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-time-l1-1-0.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll
--rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll
--rwxrwxrwx   0        0        0  3075664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/ascp.exe
--rwxrwxrwx   0        0        0  2299472 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/ascp4.exe
--rw-rw-rw-   0        0        0   870103 2023-06-20 02:06:37.000000 renderg-sdk-0.1.7/ascp/bin/aspera-scp-transfer.0.log
--rw-rw-rw-   0        0        0    58519 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/aspera-scp-transfer.log
--rwxrwxrwx   0        0        0  8328272 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/aspera.exe
--rw-rw-rw-   0        0        0   246864 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/concrt140.dll
--rw-rw-rw-   0        0        0  1444944 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/fasp3_shared.dll
--rw-rw-rw-   0        0        0  1292880 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/libeay32.dll
--rw-rw-rw-   0        0        0   434768 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/msvcp100.dll
--rw-rw-rw-   0        0        0   442968 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/msvcp140.dll
--rw-rw-rw-   0        0        0   783952 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/msvcr100.dll
--rw-rw-rw-   0        0        0   293976 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/ssleay32.dll
--rw-rw-rw-   0        0        0   886872 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/ucrtbase.dll
--rw-rw-rw-   0        0        0   270928 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/vccorlib140.dll
--rw-rw-rw-   0        0        0    88664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/bin/vcruntime140.dll
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/ascp/etc/
--rw-rw-rw-   0        0        0     1622 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/etc/aspera-license
--rw-rw-rw-   0        0        0      121 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/etc/aspera.conf
--rw-rw-rw-   0        0        0     3380 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/etc/aspera_tokenauth_id_rsa
--rw-rw-rw-   0        0        0      680 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/etc/asperaweb_id_dsa.openssh
--rw-rw-rw-   0        0        0      806 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/etc/asperaweb_id_dsa.putty
--rw-rw-rw-   0        0        0   218894 2023-06-16 07:10:02.000000 renderg-sdk-0.1.7/ascp/etc/curl-ca-bundle.crt
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_api/
--rw-rw-rw-   0        0        0       39 2023-06-15 06:53:33.000000 renderg-sdk-0.1.7/renderg_api/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_api/connect.py
--rw-rw-rw-   0        0        0      518 2023-07-12 07:50:32.000000 renderg-sdk-0.1.7/renderg_api/constants.py
--rw-rw-rw-   0        0        0     1183 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_api/core.py
--rw-rw-rw-   0        0        0      393 2023-06-15 01:37:04.000000 renderg-sdk-0.1.7/renderg_api/exception.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_api/operators/
--rw-rw-rw-   0        0        0      328 2023-06-15 02:47:54.000000 renderg-sdk-0.1.7/renderg_api/operators/__init__.py
--rw-rw-rw-   0        0        0      989 2023-06-15 08:50:33.000000 renderg-sdk-0.1.7/renderg_api/operators/env.py
--rw-rw-rw-   0        0        0     2496 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_api/operators/job.py
--rw-rw-rw-   0        0        0      245 2023-07-18 07:15:32.000000 renderg-sdk-0.1.7/renderg_api/operators/project.py
--rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.7/renderg_api/operators/task.py
--rw-rw-rw-   0        0        0     1059 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_api/operators/transfer.py
--rw-rw-rw-   0        0        0      382 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_api/operators/user.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_api/param_check/
--rw-rw-rw-   0        0        0       61 2023-06-15 06:14:24.000000 renderg-sdk-0.1.7/renderg_api/param_check/__init__.py
--rw-rw-rw-   0        0        0     3195 2023-07-12 07:52:09.000000 renderg-sdk-0.1.7/renderg_api/param_check/check.py
--rw-rw-rw-   0        0        0      879 2023-07-18 07:11:11.000000 renderg-sdk-0.1.7/renderg_api/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_sdk.egg-info/
--rw-rw-rw-   0        0        0     3341 2023-07-18 07:18:54.000000 renderg-sdk-0.1.7/renderg_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2927 2023-07-18 07:18:54.000000 renderg-sdk-0.1.7/renderg_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 07:18:54.000000 renderg-sdk-0.1.7/renderg_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-18 07:18:54.000000 renderg-sdk-0.1.7/renderg_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 07:18:54.000000 renderg-sdk-0.1.7/renderg_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_upload/
--rw-rw-rw-   0        0        0        0 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_upload/__init__.py
--rw-rw-rw-   0        0        0      159 2023-07-18 07:07:52.000000 renderg-sdk-0.1.7/renderg_upload/asperaTransfer.py
--rw-rw-rw-   0        0        0     1474 2023-07-18 07:07:52.000000 renderg-sdk-0.1.7/renderg_upload/asperaTransferHelper.py
--rw-rw-rw-   0        0        0     3920 2023-07-18 07:07:52.000000 renderg-sdk-0.1.7/renderg_upload/assetsPathHelper.py
--rw-rw-rw-   0        0        0     2309 2023-07-18 07:09:09.000000 renderg-sdk-0.1.7/renderg_upload/rgUpload.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_upload - 副本/
--rw-rw-rw-   0        0        0     3910 2023-07-18 06:52:19.000000 renderg-sdk-0.1.7/renderg_upload - 副本/AssetsPathHelper.py
--rw-rw-rw-   0        0        0     5909 2023-07-18 06:52:19.000000 renderg-sdk-0.1.7/renderg_upload - 副本/RGDownload.py
--rw-rw-rw-   0        0        0     3240 2023-07-18 07:03:35.000000 renderg-sdk-0.1.7/renderg_upload - 副本/RGUpload.py
--rw-rw-rw-   0        0        0     1743 2023-07-18 06:52:19.000000 renderg-sdk-0.1.7/renderg_upload - 副本/TransferHelper.py
--rw-rw-rw-   0        0        0       99 2023-07-18 05:53:28.000000 renderg-sdk-0.1.7/renderg_upload - 副本/__init__.py
--rw-rw-rw-   0        0        0      141 2023-07-18 05:53:28.000000 renderg-sdk-0.1.7/renderg_upload - 副本/mqConnect.py
--rw-rw-rw-   0        0        0     1908 2023-07-18 06:52:19.000000 renderg-sdk-0.1.7/renderg_upload - 副本/mqttSubscriber.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/renderg_utils/
--rw-rw-rw-   0        0        0      113 2023-07-12 07:50:32.000000 renderg-sdk-0.1.7/renderg_utils/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.7/renderg_utils/constants.py
--rw-rw-rw-   0        0        0     1131 2023-07-12 07:50:32.000000 renderg-sdk-0.1.7/renderg_utils/exception.py
--rw-rw-rw-   0        0        0     2655 2023-07-12 07:50:32.000000 renderg-sdk-0.1.7/renderg_utils/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-18 07:18:59.000000 renderg-sdk-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      980 2023-07-18 07:18:53.000000 renderg-sdk-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/
+-rw-rw-rw-   0        0        0     4312 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3931 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/analyze_houdini/
+-rw-rw-rw-   0        0        0       52 2023-06-20 02:05:27.000000 renderg-sdk-0.1.8/analyze_houdini/__init__.py
+-rw-rw-rw-   0        0        0     4075 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/analyze_houdini/analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/analyze_houdini/houdini/
+-rw-rw-rw-   0        0        0   991744 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/analyze_houdini/houdini/HoudiniAnalyze.pyd
+-rw-rw-rw-   0        0        0  1188352 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/analyze_houdini/houdini/HoudiniAnalyze_py37.pyd
+-rw-rw-rw-   0        0        0   859136 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/analyze_houdini/houdini/HoudiniAnalyze_py39.pyd
+-rw-rw-rw-   0        0        0      708 2023-05-26 09:16:22.000000 renderg-sdk-0.1.8/analyze_houdini/houdini/run.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/ascp/
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.8/ascp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/ascp/bin/
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-file-l1-2-0.dll
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-file-l2-1-0.dll
+-rw-rw-rw-   0        0        0    25176 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-localization-l1-2-0.dll
+-rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-synch-l1-2-0.dll
+-rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll
+-rw-rw-rw-   0        0        0    26704 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll
+-rw-rw-rw-   0        0        0    24656 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll
+-rw-rw-rw-   0        0        0    33360 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-math-l1-1-0.dll
+-rw-rw-rw-   0        0        0    30800 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll
+-rw-rw-rw-   0        0        0    75344 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-private-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-process-l1-1-0.dll
+-rw-rw-rw-   0        0        0    27216 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll
+-rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll
+-rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-string-l1-1-0.dll
+-rw-rw-rw-   0        0        0    25168 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-time-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll
+-rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll
+-rwxrwxrwx   0        0        0  3075664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/ascp.exe
+-rwxrwxrwx   0        0        0  2299472 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/ascp4.exe
+-rw-rw-rw-   0        0        0   870103 2023-06-20 02:06:37.000000 renderg-sdk-0.1.8/ascp/bin/aspera-scp-transfer.0.log
+-rw-rw-rw-   0        0        0    58519 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/aspera-scp-transfer.log
+-rwxrwxrwx   0        0        0  8328272 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/aspera.exe
+-rw-rw-rw-   0        0        0   246864 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/concrt140.dll
+-rw-rw-rw-   0        0        0  1444944 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/fasp3_shared.dll
+-rw-rw-rw-   0        0        0  1292880 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/libeay32.dll
+-rw-rw-rw-   0        0        0   434768 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/msvcp100.dll
+-rw-rw-rw-   0        0        0   442968 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/msvcp140.dll
+-rw-rw-rw-   0        0        0   783952 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/msvcr100.dll
+-rw-rw-rw-   0        0        0   293976 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/ssleay32.dll
+-rw-rw-rw-   0        0        0   886872 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/ucrtbase.dll
+-rw-rw-rw-   0        0        0   270928 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/vccorlib140.dll
+-rw-rw-rw-   0        0        0    88664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/bin/vcruntime140.dll
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/ascp/etc/
+-rw-rw-rw-   0        0        0     1622 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/etc/aspera-license
+-rw-rw-rw-   0        0        0      121 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/etc/aspera.conf
+-rw-rw-rw-   0        0        0     3380 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/etc/aspera_tokenauth_id_rsa
+-rw-rw-rw-   0        0        0      680 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/etc/asperaweb_id_dsa.openssh
+-rw-rw-rw-   0        0        0      806 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/etc/asperaweb_id_dsa.putty
+-rw-rw-rw-   0        0        0   218894 2023-06-16 07:10:02.000000 renderg-sdk-0.1.8/ascp/etc/curl-ca-bundle.crt
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/renderg_api/
+-rw-rw-rw-   0        0        0       39 2023-06-15 06:53:33.000000 renderg-sdk-0.1.8/renderg_api/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-07-19 03:03:11.000000 renderg-sdk-0.1.8/renderg_api/connect.py
+-rw-rw-rw-   0        0        0      554 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_api/constants.py
+-rw-rw-rw-   0        0        0     1274 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_api/core.py
+-rw-rw-rw-   0        0        0      393 2023-06-15 01:37:04.000000 renderg-sdk-0.1.8/renderg_api/exception.py
+-rw-rw-rw-   0        0        0      145 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_api/mqConnect.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/renderg_api/operators/
+-rw-rw-rw-   0        0        0      328 2023-06-15 02:47:54.000000 renderg-sdk-0.1.8/renderg_api/operators/__init__.py
+-rw-rw-rw-   0        0        0      989 2023-06-15 08:50:33.000000 renderg-sdk-0.1.8/renderg_api/operators/env.py
+-rw-rw-rw-   0        0        0     2620 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_api/operators/job.py
+-rw-rw-rw-   0        0        0      245 2023-07-19 03:02:32.000000 renderg-sdk-0.1.8/renderg_api/operators/project.py
+-rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.8/renderg_api/operators/task.py
+-rw-rw-rw-   0        0        0     1277 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_api/operators/transfer.py
+-rw-rw-rw-   0        0        0      382 2023-07-19 03:02:32.000000 renderg-sdk-0.1.8/renderg_api/operators/user.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/renderg_api/param_check/
+-rw-rw-rw-   0        0        0       61 2023-06-15 06:14:24.000000 renderg-sdk-0.1.8/renderg_api/param_check/__init__.py
+-rw-rw-rw-   0        0        0     3195 2023-07-12 07:52:09.000000 renderg-sdk-0.1.8/renderg_api/param_check/check.py
+-rw-rw-rw-   0        0        0      982 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_api/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/renderg_sdk.egg-info/
+-rw-rw-rw-   0        0        0     4312 2023-07-19 03:14:24.000000 renderg-sdk-0.1.8/renderg_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2706 2023-07-19 03:14:24.000000 renderg-sdk-0.1.8/renderg_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 03:14:24.000000 renderg-sdk-0.1.8/renderg_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-19 03:14:24.000000 renderg-sdk-0.1.8/renderg_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       64 2023-07-19 03:14:24.000000 renderg-sdk-0.1.8/renderg_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/renderg_transfer/
+-rw-rw-rw-   0        0        0     3706 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_transfer/AssetsPathHelper.py
+-rw-rw-rw-   0        0        0     1850 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_transfer/MQClient.py
+-rw-rw-rw-   0        0        0     4711 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_transfer/RGDownload.py
+-rw-rw-rw-   0        0        0     2091 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_transfer/RGUpload.py
+-rw-rw-rw-   0        0        0     3811 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_transfer/TransferHelper.py
+-rw-rw-rw-   0        0        0       48 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_transfer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/renderg_utils/
+-rw-rw-rw-   0        0        0      113 2023-07-12 07:50:32.000000 renderg-sdk-0.1.8/renderg_utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.8/renderg_utils/constants.py
+-rw-rw-rw-   0        0        0     1131 2023-07-12 07:50:32.000000 renderg-sdk-0.1.8/renderg_utils/exception.py
+-rw-rw-rw-   0        0        0     2886 2023-07-19 03:02:47.000000 renderg-sdk-0.1.8/renderg_utils/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 03:14:25.000000 renderg-sdk-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-07-19 03:07:35.000000 renderg-sdk-0.1.8/setup.py
```

### Comparing `renderg-sdk-0.1.7/PKG-INFO` & `renderg-sdk-0.1.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderg-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: www.renderg.com
 Home-page: https://github.com/renderg-repo/renderg-sdk.git
 Author: RenderG
 Author-email: support@renderg.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,17 @@
 
 ```python
 from renderg_utils import utils
 from analyze_houdini import AnalyzeHoudini
 from renderg_api import RenderGAPI
 from renderg_api.constants import TransferLines
 from renderg_api.param_check import RenderGParamChecker
-from renderg_upload.rgUpload import RendergUpload
+from renderg_transfer.RGUpload import RenderGUpload
+from renderg_transfer.RGDownload import RenderGDownload
+
 # ========分析资产和渲染参数==========
 # 1. 读取配置文件
 config = utils.read_json("./config.json")
 
 api = RenderGAPI(auth_key=config["AUTH_KEY"], cluster_id=config["CLUSTER_ID"])
 
 # 2.  创建任务信息
@@ -96,21 +98,50 @@
 
 # 2. 配置上传任务信息 
 upload_kwargs = {
     "api": api,
     "job_id": job_id,
     "info_path": info_path,
     "line": TransferLines.LINE_RENDERG,
-    "spend": 200 # 上传速度限制，单位为 Mbps
+    "speed": 200  # 上传速度限制，单位为 Mbps
 }
 # 3. 开始上传
-renderg_upload = RendergUpload(**upload_kwargs)
+renderg_upload = RenderGUpload(**upload_kwargs)
 renderg_upload.upload()
 
 # 4. 上传完成，提交任务，开始渲染
 submit = api.job.submit_job(job_id)
 print(submit["msg"])
 
+# 5. 下载
+# 等待任务完成下载
+download_kwargs = {
+    "api": api,
+    "job_id": job_id,
+    "download_path": "d:/test",  # 下载保存到本地路径
+    "line": TransferLines.LINE_RENDERG,
+    "cluster_id": config["CLUSTER_ID"],
+    "speed": 500  # 上传速度限制，单位为 Mbps
+}
+renderg_sync = RenderGDownload(**download_kwargs)
+result = renderg_sync.auto_download_after_job_completed()
+
+'''
+# 自定义下载
+download_others_json = {
+    "api": api,
+    "job_id": None,
+    "download_path": "d:/test",  # 下载保存到本地路径
+    "line": TransferLines.LINE_RENDERG,
+    "cluster_id": config["CLUSTER_ID"],
+    "speed": 3000  # 上传速度限制，单位为 Mbps
+}
+server_path = {
+    "/{job_id}".format(job_id=job_id)
+}  # 提供待下载目录列表
+renderg_sync = RenderGDownload(**download_others_json)
+renderg_sync.custom_download(server_path)
+'''
 ```
```

### Comparing `renderg-sdk-0.1.7/README.md` & `renderg-sdk-0.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 
 ```python
 from renderg_utils import utils
 from analyze_houdini import AnalyzeHoudini
 from renderg_api import RenderGAPI
 from renderg_api.constants import TransferLines
 from renderg_api.param_check import RenderGParamChecker
-from renderg_upload.rgUpload import RendergUpload
+from renderg_transfer.RGUpload import RenderGUpload
+from renderg_transfer.RGDownload import RenderGDownload
+
 # ========分析资产和渲染参数==========
 # 1. 读取配置文件
 config = utils.read_json("./config.json")
 
 api = RenderGAPI(auth_key=config["AUTH_KEY"], cluster_id=config["CLUSTER_ID"])
 
 # 2.  创建任务信息
@@ -84,21 +86,50 @@
 
 # 2. 配置上传任务信息 
 upload_kwargs = {
     "api": api,
     "job_id": job_id,
     "info_path": info_path,
     "line": TransferLines.LINE_RENDERG,
-    "spend": 200 # 上传速度限制，单位为 Mbps
+    "speed": 200  # 上传速度限制，单位为 Mbps
 }
 # 3. 开始上传
-renderg_upload = RendergUpload(**upload_kwargs)
+renderg_upload = RenderGUpload(**upload_kwargs)
 renderg_upload.upload()
 
 # 4. 上传完成，提交任务，开始渲染
 submit = api.job.submit_job(job_id)
 print(submit["msg"])
 
+# 5. 下载
+# 等待任务完成下载
+download_kwargs = {
+    "api": api,
+    "job_id": job_id,
+    "download_path": "d:/test",  # 下载保存到本地路径
+    "line": TransferLines.LINE_RENDERG,
+    "cluster_id": config["CLUSTER_ID"],
+    "speed": 500  # 上传速度限制，单位为 Mbps
+}
+renderg_sync = RenderGDownload(**download_kwargs)
+result = renderg_sync.auto_download_after_job_completed()
+
+'''
+# 自定义下载
+download_others_json = {
+    "api": api,
+    "job_id": None,
+    "download_path": "d:/test",  # 下载保存到本地路径
+    "line": TransferLines.LINE_RENDERG,
+    "cluster_id": config["CLUSTER_ID"],
+    "speed": 3000  # 上传速度限制，单位为 Mbps
+}
+server_path = {
+    "/{job_id}".format(job_id=job_id)
+}  # 提供待下载目录列表
+renderg_sync = RenderGDownload(**download_others_json)
+renderg_sync.custom_download(server_path)
+'''
 ```
```

### Comparing `renderg-sdk-0.1.7/analyze_houdini/analyze.py` & `renderg-sdk-0.1.8/analyze_houdini/analyze.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         self.env_id = env_id
         self.job_id = job_id
 
         if not job_id:
             self.job_id = self.api.job.new_job(self.dcc_file, self.project_id, self.env_id)
 
         self.workspace = os.path.join(renderg_utils.get_workspace(workspace), str(self.job_id))
-        if not os.path.isdir(self.workspace):
-            os.makedirs(self.workspace)
+        renderg_utils.check_path(self.workspace)
 
         self.info_path = os.path.join(self.workspace, "info.cfg")
         self.warning_path = os.path.join(self.workspace, "warning.json")
 
         self.warning_info = {}
 
     def add_warning(self, warn, *args):
@@ -75,30 +74,30 @@
                     winreg.HKEY_LOCAL_MACHINE, r'SOFTWARE\Side Effects Software\Houdini ' + self.dcc_version
                 )
                 regedit_dcc_exe_path, _ = winreg.QueryValueEx(key, "InstallPath")
                 dcc_exe_path = os.path.join(regedit_dcc_exe_path, r'bin\hython.exe')
             except BaseException as err:
                 print(err.__str__())
         if not dcc_exe_path or not os.path.isfile(dcc_exe_path):
-            raise DCCExeNotFoundError(ErrorCode.DCCExeNotFoundError, dcc_exe_path)
+            raise DCCExeNotFoundError(ErrorCode.DCCExeNotFoundError, self.dcc_version)
 
         return dcc_exe_path
 
     def analyze(self, cmd=None):
         self.check_file_version()
         if not self.dcc_exe_path:
             self.dcc_exe_path = self.find_dcc_exe()
 
         self._update_analyze_status(JobStatus.STATUS_ANALYZE_DOING)
         script_path = os.path.join(os.path.dirname(__file__), "houdini/run.py")
         cmd = cmd or [self.dcc_exe_path, script_path, "-input", self.dcc_file, "-output", self.info_path]
-        code = renderg_utils.run_cmd(cmd, shell=True)
+        code, stderr = renderg_utils.run_cmd(cmd, shell=True)
         if code != 0:
             self._update_analyze_status(JobStatus.STATUS_ANALYZE_FAILED)
-            raise AnalyzeFailError(ErrorCode.AnalyzeFailError, "analyze exits unexpectedly")
+            raise AnalyzeFailError(ErrorCode.AnalyzeFailError, stderr.read() or "analyze exits unexpectedly")
 
         if not os.path.isfile(self.info_path):
             self._update_analyze_status(JobStatus.STATUS_ANALYZE_FAILED)
             raise AnalyzeFailError(ErrorCode.AnalyzeFailError, "info.cfg not found.")
 
         self._update_analyze_status(JobStatus.STATUS_ANALYZED)
         return self
```

### Comparing `renderg-sdk-0.1.7/analyze_houdini/houdini/run.py` & `renderg-sdk-0.1.8/analyze_houdini/houdini/run.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-file-l1-2-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-file-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-file-l2-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-file-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-localization-l1-2-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-localization-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-synch-l1-2-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-synch-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-math-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-math-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-private-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-private-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-process-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-process-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-string-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-string-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-time-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-time-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll` & `renderg-sdk-0.1.8/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/ascp.exe` & `renderg-sdk-0.1.8/ascp/bin/ascp.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/ascp4.exe` & `renderg-sdk-0.1.8/ascp/bin/ascp4.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/aspera-scp-transfer.0.log` & `renderg-sdk-0.1.8/ascp/bin/aspera-scp-transfer.0.log`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/aspera-scp-transfer.log` & `renderg-sdk-0.1.8/ascp/bin/aspera-scp-transfer.log`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/aspera.exe` & `renderg-sdk-0.1.8/ascp/bin/aspera.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/concrt140.dll` & `renderg-sdk-0.1.8/ascp/bin/concrt140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/fasp3_shared.dll` & `renderg-sdk-0.1.8/ascp/bin/fasp3_shared.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/libeay32.dll` & `renderg-sdk-0.1.8/ascp/bin/libeay32.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/msvcp100.dll` & `renderg-sdk-0.1.8/ascp/bin/msvcp100.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/msvcp140.dll` & `renderg-sdk-0.1.8/ascp/bin/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/msvcr100.dll` & `renderg-sdk-0.1.8/ascp/bin/msvcr100.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/ssleay32.dll` & `renderg-sdk-0.1.8/ascp/bin/ssleay32.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/ucrtbase.dll` & `renderg-sdk-0.1.8/ascp/bin/ucrtbase.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/vccorlib140.dll` & `renderg-sdk-0.1.8/ascp/bin/vccorlib140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/bin/vcruntime140.dll` & `renderg-sdk-0.1.8/ascp/bin/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/etc/aspera-license` & `renderg-sdk-0.1.8/ascp/etc/aspera-license`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/etc/aspera_tokenauth_id_rsa` & `renderg-sdk-0.1.8/ascp/etc/aspera_tokenauth_id_rsa`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/etc/asperaweb_id_dsa.openssh` & `renderg-sdk-0.1.8/ascp/etc/asperaweb_id_dsa.openssh`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/etc/asperaweb_id_dsa.putty` & `renderg-sdk-0.1.8/ascp/etc/asperaweb_id_dsa.putty`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/ascp/etc/curl-ca-bundle.crt` & `renderg-sdk-0.1.8/ascp/etc/curl-ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/renderg_api/connect.py` & `renderg-sdk-0.1.8/renderg_api/connect.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/renderg_api/core.py` & `renderg-sdk-0.1.8/renderg_api/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 from renderg_api.connect import Connect
 from renderg_api.operators import UserOperator, TaskOperator, JobOperator, ProjectOperator, EnvOperator, \
     TransferOperator
+from renderg_api.mqConnect import MqConnect
 
 
 class RenderGAPI(object):
 
     def __init__(self, auth_key=None, protocol='https', domain="v.renderg.com", cluster_id=None):
         auth_key = auth_key or os.getenv("RENDERG_AUTH_KEY")
         if not auth_key:
@@ -19,13 +20,14 @@
 
         self.user = UserOperator(self._connect)
         self.job = JobOperator(self._connect)
         self.task = TaskOperator(self._connect)
         self.project = ProjectOperator(self._connect)
         self.env = EnvOperator(self._connect)
         self.transfer = TransferOperator(self._connect)
+        self.mqConnect = MqConnect(auth_key)
 
     def generate_job(self, dcc_file_path, project_name=None, env_name=None):
         pass
 
     def set_hardware_config(self, job_id, zone=None, ram=None):
         self.job.set_job_config(job_id, zone, ram)
```

### Comparing `renderg-sdk-0.1.7/renderg_api/operators/env.py` & `renderg-sdk-0.1.8/renderg_api/operators/env.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/renderg_api/operators/job.py` & `renderg-sdk-0.1.8/renderg_api/operators/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,7 +62,10 @@
 
     def submit_job(self, job_id):
         params = {
             'job_id': job_id,
             'submit_version': "2"
         }
         return self._connect.post(self._connect.urls.SubmitJob, params)
+
+    def get_jobs_info(self, job_id):
+        return self._connect.get(self._connect.urls.JobInfo,None,True,str(job_id))
```

### Comparing `renderg-sdk-0.1.7/renderg_api/operators/transfer.py` & `renderg-sdk-0.1.8/renderg_api/operators/transfer.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,7 +23,12 @@
         if not host or not port:
             raise TypeError('Required "host" or "port" not specified. host: "{}", port: "{}"'.format(host, port))
         return host, port
 
     def get_transfer_config(self, job_id):
         params = {'job_id': str(job_id)}
         return self._connect.post(self._connect.urls.GetTransferConfig, params).get('data')
+
+    def get_transfer_cluster(self, cluster_id):
+        params = {'cluster_id': str(cluster_id)}
+        data = self._connect.post(self._connect.urls.GetTransferByCluster, params).get('data')
+        return data
```

### Comparing `renderg-sdk-0.1.7/renderg_api/param_check/check.py` & `renderg-sdk-0.1.8/renderg_api/param_check/check.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/renderg_api/urls.py` & `renderg-sdk-0.1.8/renderg_api/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,7 +20,9 @@
     GetZoneList = "/api/v1/front/zone/list"
 
     GetEnvList = "/api/v1/front/environment/list"
     GetProjectList = "/api/v2/front/project/all"
 
     GetTransferLine = "/api/v1/front/transfer/lines"
     GetTransferConfig = "/api/v1/front/job/transfer_plus"
+    GetTransferByCluster = "/api/v1/front/transfer/transfer_plus"
+    JobInfo = "/api/v1/front/job/{}"
```

### Comparing `renderg-sdk-0.1.7/renderg_sdk.egg-info/PKG-INFO` & `renderg-sdk-0.1.8/renderg_sdk.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderg-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: www.renderg.com
 Home-page: https://github.com/renderg-repo/renderg-sdk.git
 Author: RenderG
 Author-email: support@renderg.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,17 @@
 
 ```python
 from renderg_utils import utils
 from analyze_houdini import AnalyzeHoudini
 from renderg_api import RenderGAPI
 from renderg_api.constants import TransferLines
 from renderg_api.param_check import RenderGParamChecker
-from renderg_upload.rgUpload import RendergUpload
+from renderg_transfer.RGUpload import RenderGUpload
+from renderg_transfer.RGDownload import RenderGDownload
+
 # ========分析资产和渲染参数==========
 # 1. 读取配置文件
 config = utils.read_json("./config.json")
 
 api = RenderGAPI(auth_key=config["AUTH_KEY"], cluster_id=config["CLUSTER_ID"])
 
 # 2.  创建任务信息
@@ -96,21 +98,50 @@
 
 # 2. 配置上传任务信息 
 upload_kwargs = {
     "api": api,
     "job_id": job_id,
     "info_path": info_path,
     "line": TransferLines.LINE_RENDERG,
-    "spend": 200 # 上传速度限制，单位为 Mbps
+    "speed": 200  # 上传速度限制，单位为 Mbps
 }
 # 3. 开始上传
-renderg_upload = RendergUpload(**upload_kwargs)
+renderg_upload = RenderGUpload(**upload_kwargs)
 renderg_upload.upload()
 
 # 4. 上传完成，提交任务，开始渲染
 submit = api.job.submit_job(job_id)
 print(submit["msg"])
 
+# 5. 下载
+# 等待任务完成下载
+download_kwargs = {
+    "api": api,
+    "job_id": job_id,
+    "download_path": "d:/test",  # 下载保存到本地路径
+    "line": TransferLines.LINE_RENDERG,
+    "cluster_id": config["CLUSTER_ID"],
+    "speed": 500  # 上传速度限制，单位为 Mbps
+}
+renderg_sync = RenderGDownload(**download_kwargs)
+result = renderg_sync.auto_download_after_job_completed()
+
+'''
+# 自定义下载
+download_others_json = {
+    "api": api,
+    "job_id": None,
+    "download_path": "d:/test",  # 下载保存到本地路径
+    "line": TransferLines.LINE_RENDERG,
+    "cluster_id": config["CLUSTER_ID"],
+    "speed": 3000  # 上传速度限制，单位为 Mbps
+}
+server_path = {
+    "/{job_id}".format(job_id=job_id)
+}  # 提供待下载目录列表
+renderg_sync = RenderGDownload(**download_others_json)
+renderg_sync.custom_download(server_path)
+'''
 ```
```

### Comparing `renderg-sdk-0.1.7/renderg_sdk.egg-info/SOURCES.txt` & `renderg-sdk-0.1.8/renderg_sdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 ascp/etc/asperaweb_id_dsa.putty
 ascp/etc/curl-ca-bundle.crt
 renderg_api/__init__.py
 renderg_api/connect.py
 renderg_api/constants.py
 renderg_api/core.py
 renderg_api/exception.py
+renderg_api/mqConnect.py
 renderg_api/urls.py
 renderg_api/operators/__init__.py
 renderg_api/operators/env.py
 renderg_api/operators/job.py
 renderg_api/operators/project.py
 renderg_api/operators/task.py
 renderg_api/operators/transfer.py
@@ -67,23 +68,17 @@
 renderg_api/param_check/__init__.py
 renderg_api/param_check/check.py
 renderg_sdk.egg-info/PKG-INFO
 renderg_sdk.egg-info/SOURCES.txt
 renderg_sdk.egg-info/dependency_links.txt
 renderg_sdk.egg-info/requires.txt
 renderg_sdk.egg-info/top_level.txt
-renderg_upload/__init__.py
-renderg_upload/asperaTransfer.py
-renderg_upload/asperaTransferHelper.py
-renderg_upload/assetsPathHelper.py
-renderg_upload/rgUpload.py
-renderg_upload - 副本/AssetsPathHelper.py
-renderg_upload - 副本/RGDownload.py
-renderg_upload - 副本/RGUpload.py
-renderg_upload - 副本/TransferHelper.py
-renderg_upload - 副本/__init__.py
-renderg_upload - 副本/mqConnect.py
-renderg_upload - 副本/mqttSubscriber.py
+renderg_transfer/AssetsPathHelper.py
+renderg_transfer/MQClient.py
+renderg_transfer/RGDownload.py
+renderg_transfer/RGUpload.py
+renderg_transfer/TransferHelper.py
+renderg_transfer/__init__.py
 renderg_utils/__init__.py
 renderg_utils/constants.py
 renderg_utils/exception.py
 renderg_utils/utils.py
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `renderg-sdk-0.1.7/renderg_upload/assetsPathHelper.py` & `renderg-sdk-0.1.8/renderg_transfer/AssetsPathHelper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,86 @@
 import os
-
-from renderg_upload.asperaTransfer import AsperaTransfer
-from renderg_upload.asperaTransferHelper import AsperaTransferHelper
+from renderg_transfer.TransferHelper import TransferConstants, TransferHelper
 
 
 class AssetsPathHelper:
 
-
     @staticmethod
     def get_file_list_for_info_cfg(info_path, job_id):
         source_paths = []
         dest_paths = []
 
         if os.path.isfile(info_path):
-            info_json = AsperaTransferHelper.read_json(info_path)
+            info_json = TransferHelper.read_json(info_path)
             if info_json:
                 source_paths, dest_paths = AssetsPathHelper.__get_file_list_for_info_cfg(
-                    job_id, info_json, AsperaTransfer.ASSETS, info_path)
+                    job_id, info_json, TransferConstants.ASSETS, info_path)
 
         return source_paths, dest_paths
 
     @staticmethod
     def __get_file_list_for_info_cfg(job_id, info_json, key, info_path=None):
         source_paths = []
         dest_paths = []
-        has_cfg_file = False
 
         assets_list = info_json.get(key)
         for path_dict in assets_list:
-            full_path = AsperaTransferHelper.handing_local_paths(
-                path_dict.get(AsperaTransfer.FULL_PATH)
+            full_path = TransferHelper.handing_local_paths(
+                path_dict.get(TransferConstants.FULL_PATH)
             )
-            remote_name = AsperaTransferHelper.handing_local_paths(
-                path_dict.get(AsperaTransfer.REMOTE_NAME)
+            remote_name = TransferHelper.handing_local_paths(
+                path_dict.get(TransferConstants.REMOTE_NAME)
             )
-            file_type = int(path_dict.get(AsperaTransfer.FILE_TYPE))
-            missing = int(path_dict.get(AsperaTransfer.MISSING))
-            if file_type == 1:
-                if missing == 0:
+            file_type = int(path_dict.get(TransferConstants.FILE_TYPE))
+            missing = int(path_dict.get(TransferConstants.MISSING))
+            if missing == 0:
+                if file_type == 1:
                     source_paths.append(full_path)
                     dest_paths.append(
                         AssetsPathHelper.assemble_server_cfg_path(job_id, full_path)
                     )
-            elif file_type == 2:
-                if missing == 0:
+                elif file_type == 2:
                     local_paths, server_paths = \
                         AssetsPathHelper.assemble_server_input_path(full_path, remote_name)
                     source_paths.append(local_paths)
                     dest_paths.append(server_paths)
 
         if os.path.isfile(info_path):
             source_paths.insert(0, info_path)
             dest_paths.insert(0, AssetsPathHelper.assemble_server_cfg_path(job_id, info_path))
 
         return source_paths, dest_paths
 
     @staticmethod
     def assemble_server_cfg_path(job_id, path):
         filename = os.path.basename(path)
-        cfg_path = f'cfg/{job_id}/{filename}'
+        cfg_path = 'cfg/{job_id}/{filename}'.format(job_id=job_id, filename=filename)
         return cfg_path.replace('\\', '/')
 
     @staticmethod
     def assemble_server_input_path(local_path, remote_name):
-        norma_path = AsperaTransferHelper.handing_local_paths(os.path.normpath(local_path))
-        norma_name = AsperaTransferHelper.handing_local_paths(os.path.normpath(remote_name))
+        norma_path = TransferHelper.handing_local_paths(os.path.normpath(local_path))
+        norma_name = TransferHelper.handing_local_paths(os.path.normpath(remote_name))
 
         split_path = norma_name.split(':')
         if len(split_path) == 2:
             driver = split_path[0].upper().strip('/')
             file = split_path[1].strip('/')
-            server_path = f'input/{driver}/{file}'
+            server_path = 'input/{driver}/{file}'.format(driver=driver, file=file)
         else:
             split_path = norma_name.split('/')
             if len(split_path) >= 2:
                 driver_name = split_path[0].split('_')
                 if len(driver_name) == 2:
                     driver = driver_name[1].upper().strip('/')
                     file = '/'.join(split_path[1:])
                     file = file.strip('/')
-                    server_path = f'input/{driver}/{file}'
+                    server_path = 'input/{driver}/{file}'.format(driver=driver, file=file)
                 else:
-                    if AsperaTransferHelper.is_unc_path(norma_name):
-                        server_path = f'input/UNC/{norma_name.strip("/")}'
+                    if TransferHelper.is_unc_path(norma_name):
+                        server_path = 'input/UNC/{}'.format(norma_name.strip("/"))
                     else:
-                        server_path = f'input/{norma_name.strip("/")}'
+                        server_path = 'input/{}'.format(norma_name.strip("/"))
             else:
-                server_path = os.path.join(f'input/{norma_name.strip("/")}')
+                server_path = os.path.join('input/{}'.format(norma_name.strip("/")))
 
         return norma_path.replace('\\', '/'), server_path.replace('\\', '/')
-
-    @staticmethod
-    def get_root_dir():
-        current_dir = os.path.dirname(os.path.abspath(__file__))
-        root_dir = os.path.abspath(os.path.join(current_dir, ".."))
-        return root_dir
-
```

### Comparing `renderg-sdk-0.1.7/renderg_upload/rgUpload.py` & `renderg-sdk-0.1.8/renderg_transfer/RGUpload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,55 @@
+
 import os
-import subprocess
-import time
 
 from renderg_api.constants import JobStatus
-from renderg_upload.assetsPathHelper import AssetsPathHelper
+from renderg_transfer.AssetsPathHelper import AssetsPathHelper
+from renderg_transfer.TransferHelper import TransferHelper
+
+import renderg_utils
 
 
-class RendergUpload:
+class RenderGUpload:
 
-    def __init__(self,api,job_id,info_path,line,spend):
+    def __init__(self, api, job_id, info_path, line, speed, workspace=None):
         self.api = api
         self.transfer_config = api.transfer.get_transfer_config(job_id)
         self.transfer_lines = api.transfer.get_transfer_line(line)
         self.info_path = info_path
         self.job_id = job_id
-        if spend is not None:
-            self.spend = spend
+        if speed is not None:
+            self.speed = speed
         else:
-            self.spend = 1000
+            self.speed = 1000
+        self.workspace = os.path.join(renderg_utils.get_workspace(workspace), str(self.job_id))
+        self.log_path = os.path.join(renderg_utils.get_workspace(workspace), 'log')
+        renderg_utils.check_path(self.workspace)
+        renderg_utils.check_path(self.log_path)
 
     def upload(self):
         self.api.job.update_job_status(self.job_id, JobStatus.STATUS_UPLOAD)
-        source_paths,dest_paths = AssetsPathHelper.get_file_list_for_info_cfg(self.info_path,self.job_id)
+        source_paths, dest_paths = AssetsPathHelper.get_file_list_for_info_cfg(self.info_path, self.job_id)
 
         host, port = self.transfer_lines
         username = self.transfer_config.get("username")
         password = self.transfer_config.get("password")
 
-        root_dir = AssetsPathHelper.get_root_dir()
-        ascp_dir = f"{root_dir}/ascp/bin/ascp.exe".replace('\\', '/')
-        timestamp = time.time()
-
-        formatted_time = time.strftime('%Y%m%d%H%M%S', time.localtime(timestamp))
-        workspace = self.info_path.replace('info.cfg', '')
-        filepairlist_dir = os.path.join(workspace, f'{self.job_id}_{formatted_time}.txt')
-        print(filepairlist_dir)
-
-        with open(filepairlist_dir, 'w') as f:
-            for index, source in enumerate(source_paths, 0):
-                dest = dest_paths[index]
-                print("source:", source)
-                print("dest:", dest)
-                f.write(f"{source}\n")
-                f.write(f"{dest}\n")
-
-        cmd_pass = f"set ASPERA_SCP_PASS={password}"
-        cmd = f'{cmd_pass}&& {ascp_dir} -P {port} -O {port} -T -l{self.spend}m --mode=send -k2 --overwrite=diff --user={username} -d --host={host} -L {workspace} --file-pair-list={filepairlist_dir} .'
-
-        try:
-            process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True)
-            while True:
-                line = process.stdout.readline()
-                if not line:
-                    break
-                print(line.decode('gbk').strip())
-        except Exception as e:
-            print('Error:',e)
+        file_pair_list_path = TransferHelper.create_file_pair_list_file(
+            self.workspace, source_paths, dest_paths
+        )
+
+        cmd_pass = "set ASPERA_SCP_PASS={password}".format(password=password)
+        cmd = TransferHelper.create_ascp_command(
+            cmd_pass=cmd_pass,
+            mode="send",
+            host=host,
+            port=port,
+            username=username,
+            max_speed=self.speed,
+            log_dir=self.log_path,
+            pair_list_file=file_pair_list_path
+        )
+        print(cmd)
+        code, stderr = renderg_utils.run_cmd(cmd, shell=True)
+        print("cmd return code: {}".format(code))
+        if code != 0:
+            raise Exception("{} 上传失败。 error={}".format(self.job_id, stderr))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `renderg-sdk-0.1.7/renderg_upload - 副本/mqttSubscriber.py` & `renderg-sdk-0.1.8/renderg_transfer/MQClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,29 @@
         if MqttClient.client is None:
             broker_address = "v.renderg.com"
             port = 1883
 
             MqttClient.client = mqtt.Client(username)
             MqttClient.client.on_connect = MqttClient.on_connect
             MqttClient.client.on_message = MqttClient.on_message
-            MqttClient.client.connect(broker_address, port)
             if username and password:
                 MqttClient.client.username_pw_set(username, password)
+            MqttClient.client.connect(broker_address, port)
             MqttClient.client.loop_start()
-            time.sleep(5)
 
     @staticmethod
     def on_connect(client, userdata, flags, rc):
         if rc == 0:
             print("Connected successfully")
         else:
             print("Connection failed with code {rc}".format(rc=rc))
         MqttClient.rc = rc
 
     @staticmethod
     def on_message(client, userdata, message):
-        print('收到消息')
         topic = message.topic
         payload = message.payload.decode('utf-8')
         if topic in MqttClient.callbacks:
             callback = MqttClient.callbacks[topic]
             callback(payload)
 
     @staticmethod
```

### Comparing `renderg-sdk-0.1.7/renderg_utils/exception.py` & `renderg-sdk-0.1.8/renderg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.7/renderg_utils/utils.py` & `renderg-sdk-0.1.8/renderg_utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,22 +25,33 @@
     with codecs.open(file_path, 'w', encoding=encoding) as f:
         if PY_VERSION == 3:
             json.dump(data, f, ensure_ascii=ensure_ascii, indent=4)
         else:
             f.write(str(json.dumps(data, ensure_ascii=ensure_ascii, indent=4)))
 
 
+def check_path(path):
+    """
+    check the system path, create path if it's not exists
+
+    :param path: a system path
+    :return: None
+    """
+    if not os.path.isdir(path):
+        os.makedirs(path)
+
+
 def run_cmd(cmd, shell=False):
     if PY_VERSION == 2:
         cmd = str(cmd).encode(sys.getfilesystemencoding())
 
     popen = subprocess.Popen(cmd, stderr=subprocess.PIPE, shell=shell)
     popen.wait()
 
-    return popen.returncode
+    return popen.returncode, popen.stderr
 
 
 def get_dcc_file_version(file_path, regex):
     version = ''
 
     with open(file_path, 'rb') as read_obj:
         while True:
```

### Comparing `renderg-sdk-0.1.7/setup.py` & `renderg-sdk-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,25 +8,26 @@
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
     return long_description
 
 
 setup(
     name='renderg-sdk',
-    version='0.1.7',
+    version='0.1.8',
     url='https://github.com/renderg-repo/renderg-sdk.git',
     author='RenderG',
     author_email='support@renderg.com',
     description='www.renderg.com',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),    
     install_requires=[
         'requests',
-        'tenacity'
+        'tenacity',
+        'paho-mqtt'
     ],
     package_data={
         'analyze_houdini': ["./houdini/*"],
         'ascp': ["./*/*"],
     },
     classifiers=[
         "Programming Language :: Python",
```

