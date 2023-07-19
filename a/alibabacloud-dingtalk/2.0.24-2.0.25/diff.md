# Comparing `tmp/alibabacloud_dingtalk-2.0.24.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.24.tar", last modified: Mon Jul 17 04:23:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.25.tar", last modified: Wed Jul 19 03:10:17 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.24.tar` & `alibabacloud_dingtalk-2.0.25.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/
--rw-r--r--   0 root         (0) root         (0)    20207 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90914 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139242 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202090 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   576378 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142048 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346941 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39942 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106288 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126888 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172646 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23872 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33155 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57073 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    75811 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219916 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   278738 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269893 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95111 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139534 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302740 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379213 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14366 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   177099 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   419073 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12289 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89958 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   102471 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19158 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32757 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32014 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    34941 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12583 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/
+-rw-r--r--   0 root         (0) root         (0)    20272 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202090 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   576378 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39942 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106288 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23872 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33155 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57073 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    75811 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95111 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139534 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106806 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19158 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32757 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 03:10:17.000000 alibabacloud_dingtalk-2.0.25/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-07-19 03:10:16.000000 alibabacloud_dingtalk-2.0.25/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.24/ChangeLog.md` & `alibabacloud_dingtalk-2.0.25/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-17 Version: 2.0.24
+- Update AddOfficialAccountFollower.
+
 2023-07-12 Version: 2.0.23
 - Update AddOfficialAccountFollower.
 
 2023-07-05 Version: 2.0.22
 - Update AddOfficialAccountFollower.
 
 2023-06-16 Version: 2.0.21
```

### Comparing `alibabacloud_dingtalk-2.0.24/LICENSE` & `alibabacloud_dingtalk-2.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/PKG-INFO` & `alibabacloud_dingtalk-2.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.24
+Version: 2.0.25
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.24/README-CN.md` & `alibabacloud_dingtalk-2.0.25/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/README.md` & `alibabacloud_dingtalk-2.0.25/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,14 +577,112 @@
         self,
         request: dingtalkrobot__1__0_models.ClearRobotPluginRequest,
     ) -> dingtalkrobot__1__0_models.ClearRobotPluginResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkrobot__1__0_models.ClearRobotPluginHeaders()
         return await self.clear_robot_plugin_with_options_async(request, headers, runtime)
 
+    def execute_robot_ai_skill_with_options(
+        self,
+        request: dingtalkrobot__1__0_models.ExecuteRobotAiSkillRequest,
+        headers: dingtalkrobot__1__0_models.ExecuteRobotAiSkillHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrobot__1__0_models.ExecuteRobotAiSkillResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.context):
+            body['context'] = request.context
+        if not UtilClient.is_unset(request.input):
+            body['input'] = request.input
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        if not UtilClient.is_unset(request.skill_id):
+            body['skillId'] = request.skill_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ExecuteRobotAiSkill',
+            version='robot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/robot/aiSkill/execute',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrobot__1__0_models.ExecuteRobotAiSkillResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def execute_robot_ai_skill_with_options_async(
+        self,
+        request: dingtalkrobot__1__0_models.ExecuteRobotAiSkillRequest,
+        headers: dingtalkrobot__1__0_models.ExecuteRobotAiSkillHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrobot__1__0_models.ExecuteRobotAiSkillResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.context):
+            body['context'] = request.context
+        if not UtilClient.is_unset(request.input):
+            body['input'] = request.input
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        if not UtilClient.is_unset(request.skill_id):
+            body['skillId'] = request.skill_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ExecuteRobotAiSkill',
+            version='robot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/robot/aiSkill/execute',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrobot__1__0_models.ExecuteRobotAiSkillResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def execute_robot_ai_skill(
+        self,
+        request: dingtalkrobot__1__0_models.ExecuteRobotAiSkillRequest,
+    ) -> dingtalkrobot__1__0_models.ExecuteRobotAiSkillResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrobot__1__0_models.ExecuteRobotAiSkillHeaders()
+        return self.execute_robot_ai_skill_with_options(request, headers, runtime)
+
+    async def execute_robot_ai_skill_async(
+        self,
+        request: dingtalkrobot__1__0_models.ExecuteRobotAiSkillRequest,
+    ) -> dingtalkrobot__1__0_models.ExecuteRobotAiSkillResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrobot__1__0_models.ExecuteRobotAiSkillHeaders()
+        return await self.execute_robot_ai_skill_with_options_async(request, headers, runtime)
+
     def get_bot_list_in_group_with_options(
         self,
         request: dingtalkrobot__1__0_models.GetBotListInGroupRequest,
         headers: dingtalkrobot__1__0_models.GetBotListInGroupHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkrobot__1__0_models.GetBotListInGroupResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -929,14 +929,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ClearRobotPluginResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ExecuteRobotAiSkillHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ExecuteRobotAiSkillRequest(TeaModel):
+    def __init__(
+        self,
+        context: Dict[str, Any] = None,
+        input: str = None,
+        robot_code: str = None,
+        skill_id: str = None,
+    ):
+        self.context = context
+        self.input = input
+        self.robot_code = robot_code
+        self.skill_id = skill_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.context is not None:
+            result['context'] = self.context
+        if self.input is not None:
+            result['input'] = self.input
+        if self.robot_code is not None:
+            result['robotCode'] = self.robot_code
+        if self.skill_id is not None:
+            result['skillId'] = self.skill_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('context') is not None:
+            self.context = m.get('context')
+        if m.get('input') is not None:
+            self.input = m.get('input')
+        if m.get('robotCode') is not None:
+            self.robot_code = m.get('robotCode')
+        if m.get('skillId') is not None:
+            self.skill_id = m.get('skillId')
+        return self
+
+
+class ExecuteRobotAiSkillResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: str = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class ExecuteRobotAiSkillResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ExecuteRobotAiSkillResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ExecuteRobotAiSkillResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetBotListInGroupHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.24
+Version: 2.0.25
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.25/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.24/setup.py` & `alibabacloud_dingtalk-2.0.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 17/07/2023
+Created on 19/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

