# Comparing `tmp/kingsoftcloud-sdk-python-1.1.4.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.1.4.tar", last modified: Mon Jul 17 06:44:14 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.5.tar", last modified: Wed Jul 19 02:15:54 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.1.4.tar` & `kingsoftcloud-sdk-python-1.1.5.tar`

### file list

```diff
@@ -1,165 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   124863 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.158770 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80297 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123172 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/LICENSE` & `kingsoftcloud-sdk-python-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.4
+Version: 1.1.5
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/README.rst` & `kingsoftcloud-sdk-python-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.4
+Version: 1.1.5
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,24 @@
 ksyun/client/kls/v20170101/__init__.py
 ksyun/client/kls/v20170101/client.py
 ksyun/client/kls/v20170101/models.py
 ksyun/client/mongodb/__init__.py
 ksyun/client/mongodb/v20170101/__init__.py
 ksyun/client/mongodb/v20170101/client.py
 ksyun/client/mongodb/v20170101/models.py
+ksyun/client/monitor/__init__.py
+ksyun/client/monitor/v20100525/__init__.py
+ksyun/client/monitor/v20100525/client.py
+ksyun/client/monitor/v20100525/models.py
+ksyun/client/monitor/v20210101/__init__.py
+ksyun/client/monitor/v20210101/client.py
+ksyun/client/monitor/v20210101/models.py
+ksyun/client/monitor/v20220101/__init__.py
+ksyun/client/monitor/v20220101/client.py
+ksyun/client/monitor/v20220101/models.py
 ksyun/client/resourcemanager/__init__.py
 ksyun/client/resourcemanager/v20210320/__init__.py
 ksyun/client/resourcemanager/v20210320/client.py
 ksyun/client/resourcemanager/v20210320/models.py
 ksyun/client/sks/__init__.py
 ksyun/client/sks/v20151101/__init__.py
 ksyun/client/sks/v20151101/client.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.1.4'
+__version__ = '1.1.5'
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1338,60 +1338,14 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
-    def DescribeImageSharePermission(self, request):
-        """镜像共享的账户列表
-        :param request: Request instance for DescribeImageSharePermission.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeImageSharePermissionRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeImageSharePermission", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
-    def DescribeRegions(self, request):
-        """用户有权限机房
-        :param request: Request instance for DescribeRegions.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeRegionsRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeRegions", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
     def AttachKey(self, request):
         """主机绑定密钥
         :param request: Request instance for AttachKey.
         :type request: :class:`ksyun.client.kec.v20160304.models.AttachKeyRequest`
         """
         try:
             params = request._serialize()
@@ -1430,37 +1384,14 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
-    def DescribeAvailabilityZones(self, request):
-        """查询可用区列表
-        :param request: Request instance for DescribeAvailabilityZones.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeAvailabilityZonesRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeAvailabilityZones", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
     def DescribeInstanceTypeConfigs(self, request):
         """查询机型套餐配置信息
         :param request: Request instance for DescribeInstanceTypeConfigs.
         :type request: :class:`ksyun.client.kec.v20160304.models.DescribeInstanceTypeConfigsRequest`
         """
         try:
             params = request._serialize()
@@ -2135,83 +2066,14 @@
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
-    def DescribeInstanceKmr(self, request):
-        """DescribeInstanceKmr
-        :param request: Request instance for DescribeInstanceKmr.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeInstanceKmrRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeInstanceKmr", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
-    def DescribeMinFlavorCount(self, request):
-        """DescribeMinFlavorCount
-        :param request: Request instance for DescribeMinFlavorCount.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeMinFlavorCountRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeMinFlavorCount", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
-    def DescribeProjectMaxNum(self, request):
-        """查询项目制最大数量限制
-        :param request: Request instance for DescribeProjectMaxNum.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeProjectMaxNumRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeProjectMaxNum", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
                 raise KsyunSDKException(code, message, req_id)
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2097,43 +2097,14 @@
             self.ImageId = params.get("ImageId")
         if params.get("AccountId"):
             self.AccountId = params.get("AccountId")
         if params.get("Permission"):
             self.Permission = params.get("Permission")
 
 
-class DescribeImageSharePermissionRequest(AbstractModel):
-    """DescribeImageSharePermission请求参数结构体
-    """
-
-    def __init__(self):
-        r"""镜像共享的账户列表
-        :param ImageId: 共享的镜像ID。
-标准UUID格式，形如^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$
-        :type PathPrefix: String
-        """
-        self.ImageId = None
-
-    def _deserialize(self, params):
-        if params.get("ImageId"):
-            self.ImageId = params.get("ImageId")
-
-
-class DescribeRegionsRequest(AbstractModel):
-    """DescribeRegions请求参数结构体
-    """
-
-    def __init__(self):
-        r"""用户有权限机房
-        """
-
-    def _deserialize(self, params):
-        return
-
-
 class AttachKeyRequest(AbstractModel):
     """AttachKey请求参数结构体
     """
 
     def __init__(self):
         r"""主机绑定密钥
         :param Action: 动作
@@ -2182,26 +2153,14 @@
             self.Action = params.get("Action")
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
         if params.get("KeyId"):
             self.KeyId = params.get("KeyId")
 
 
-class DescribeAvailabilityZonesRequest(AbstractModel):
-    """DescribeAvailabilityZones请求参数结构体
-    """
-
-    def __init__(self):
-        r"""查询可用区列表
-        """
-
-    def _deserialize(self, params):
-        return
-
-
 class DescribeInstanceTypeConfigsRequest(AbstractModel):
     """DescribeInstanceTypeConfigs请求参数结构体
     """
 
     def __init__(self):
         r"""查询机型套餐配置信息
         """
@@ -3147,43 +3106,7 @@
         self.InstanceId = None
 
     def _deserialize(self, params):
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
 
 
-class DescribeInstanceKmrRequest(AbstractModel):
-    """DescribeInstanceKmr请求参数结构体
-    """
-
-    def __init__(self):
-        r"""DescribeInstanceKmr
-        """
-
-    def _deserialize(self, params):
-        return
-
-
-class DescribeMinFlavorCountRequest(AbstractModel):
-    """DescribeMinFlavorCount请求参数结构体
-    """
-
-    def __init__(self):
-        r"""DescribeMinFlavorCount
-        """
-
-    def _deserialize(self, params):
-        return
-
-
-class DescribeProjectMaxNumRequest(AbstractModel):
-    """DescribeProjectMaxNum请求参数结构体
-    """
-
-    def __init__(self):
-        r"""查询项目制最大数量限制
-        """
-
-    def _deserialize(self, params):
-        return
-
-
```

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.5/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.4/setup.py` & `kingsoftcloud-sdk-python-1.1.5/setup.py`

 * *Files identical despite different names*

