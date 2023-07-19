# Comparing `tmp/pyvmomi-8.0.1.0.1.tar.gz` & `tmp/pyvmomi-8.0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvmomi-8.0.1.0.1.tar", last modified: Thu May 25 15:14:36 2023, max compression
+gzip compressed data, was "pyvmomi-8.0.1.0.2.tar", last modified: Wed Jul 19 08:40:02 2023, max compression
```

## Comparing `pyvmomi-8.0.1.0.1.tar` & `pyvmomi-8.0.1.0.2.tar`

### file list

```diff
@@ -1,222 +1,247 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.673256 pyvmomi-8.0.1.0.1/
--rw-rw-rw-   0        0        0    11510 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      172 2023-05-05 22:57:58.000000 pyvmomi-8.0.1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      238 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0.1/NOTICE.txt
--rw-rw-rw-   0        0        0     4867 2023-05-25 15:14:36.674343 pyvmomi-8.0.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3258 2023-04-27 12:08:03.000000 pyvmomi-8.0.1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:35.974528 pyvmomi-8.0.1.0.1/pyVim/
--rw-rw-rw-   0        0        0      163 2022-11-24 20:53:17.000000 pyvmomi-8.0.1.0.1/pyVim/__init__.py
--rw-rw-rw-   0        0        0    38332 2023-03-09 21:15:31.000000 pyvmomi-8.0.1.0.1/pyVim/connect.py
--rw-rw-rw-   0        0        0    62300 2023-02-06 16:32:40.000000 pyvmomi-8.0.1.0.1/pyVim/sso.py
--rw-rw-rw-   0        0        0    12028 2023-04-28 08:19:44.000000 pyvmomi-8.0.1.0.1/pyVim/task.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.200574 pyvmomi-8.0.1.0.1/pyVmomi/
--rw-rw-rw-   0        0        0      836 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Cache.py
--rw-rw-rw-   0        0        0     9634 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Differ.py
--rw-rw-rw-   0        0        0      932 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Feature.py
--rw-rw-rw-   0        0        0    12510 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Iso8601.py
--rw-rw-rw-   0        0        0     1470 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Security.py
--rw-rw-rw-   0        0        0    74293 2023-05-03 19:43:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/SoapAdapter.py
--rw-rw-rw-   0        0        0     2165 2023-05-03 19:30:54.000000 pyvmomi-8.0.1.0.1/pyVmomi/StubAdapterAccessorImpl.py
--rw-rw-rw-   0        0        0      644 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Version.py
--rw-rw-rw-   0        0        0     5752 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/VmomiJSONEncoder.py
--rw-rw-rw-   0        0        0    72988 2023-05-16 12:11:40.000000 pyvmomi-8.0.1.0.1/pyVmomi/VmomiSupport.py
--rw-rw-rw-   0        0        0     3002 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/__init__.py
--rw-rw-rw-   0        0        0     5225 2023-05-03 19:34:10.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_core.py
--rw-rw-rw-   0        0        0    88121 2023-05-03 19:34:17.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_eam.py
--rw-rw-rw-   0        0        0   121683 2023-05-03 19:38:39.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_pbm.py
--rw-rw-rw-   0        0        0    12391 2023-05-03 19:39:45.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_query.py
--rw-rw-rw-   0        0        0   136338 2023-05-03 19:39:58.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_sms.py
--rw-rw-rw-   0        0        0  1319281 2023-05-14 19:31:15.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_vim.py
--rw-rw-rw-   0        0        0      692 2023-05-03 19:33:57.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfos.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.206172 pyvmomi-8.0.1.0.1/pyVmomi/eam/
--rw-rw-rw-   0        0        0    15066 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.208230 pyvmomi-8.0.1.0.1/pyVmomi/eam/fault/
--rw-rw-rw-   0        0        0     2426 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.212198 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/
--rw-rw-rw-   0        0        0     8674 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.214791 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/
--rw-rw-rw-   0        0        0       19 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.217852 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/agent/
--rw-rw-rw-   0        0        0     1971 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/agent/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.220796 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/
--rw-rw-rw-   0        0        0       20 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.224301 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/agency/
--rw-rw-rw-   0        0        0      205 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/agency/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.227309 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/
--rw-rw-rw-   0        0        0       27 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.230325 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agency/
--rw-rw-rw-   0        0        0     1204 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agency/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.233339 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agent/
--rw-rw-rw-   0        0        0      166 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agent/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.235968 pyvmomi-8.0.1.0.1/pyVmomi/eam/lccm/
--rw-rw-rw-   0        0        0    16188 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/lccm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.240979 pyvmomi-8.0.1.0.1/pyVmomi/eam/vib/
--rw-rw-rw-   0        0        0     1336 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/vib/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.244056 pyvmomi-8.0.1.0.1/pyVmomi/pbm/
--rw-rw-rw-   0        0        0     5081 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.247612 pyvmomi-8.0.1.0.1/pyVmomi/pbm/auth/
--rw-rw-rw-   0        0        0       92 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/auth/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.250625 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/
--rw-rw-rw-   0        0        0     4437 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.255106 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/provider/
--rw-rw-rw-   0        0        0     4965 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.260100 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/types/
--rw-rw-rw-   0        0        0     1231 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/types/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.265305 pyvmomi-8.0.1.0.1/pyVmomi/pbm/compliance/
--rw-rw-rw-   0        0        0     6060 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/compliance/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.269310 pyvmomi-8.0.1.0.1/pyVmomi/pbm/fault/
--rw-rw-rw-   0        0        0     3064 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.272529 pyvmomi-8.0.1.0.1/pyVmomi/pbm/placement/
--rw-rw-rw-   0        0        0     4175 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/placement/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.278055 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/
--rw-rw-rw-   0        0        0    11494 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.282076 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/provider/
--rw-rw-rw-   0        0        0     1318 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.286576 pyvmomi-8.0.1.0.1/pyVmomi/pbm/provider/
--rw-rw-rw-   0        0        0       86 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.289562 pyvmomi-8.0.1.0.1/pyVmomi/pbm/replication/
--rw-rw-rw-   0        0        0      881 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/replication/__init__.pyi
--rw-rw-rw-   0        0        0        0 2023-05-05 22:57:58.000000 pyvmomi-8.0.1.0.1/pyVmomi/py.typed
--rw-rw-rw-   0        0        0      244 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pyVmomiSettings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.292564 pyvmomi-8.0.1.0.1/pyVmomi/sms/
--rw-rw-rw-   0        0        0     7021 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.296077 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/
--rw-rw-rw-   0        0        0     5403 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.299078 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/replication/
--rw-rw-rw-   0        0        0     1081 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/replication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.301079 pyvmomi-8.0.1.0.1/pyVmomi/sms/provider/
--rw-rw-rw-   0        0        0    10967 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.305666 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/
--rw-rw-rw-   0        0        0    16413 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.309635 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/replication/
--rw-rw-rw-   0        0        0    19257 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/replication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.312635 pyvmomi-8.0.1.0.1/pyVmomi/vim/
--rw-rw-rw-   0        0        0   297305 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.316153 pyvmomi-8.0.1.0.1/pyVmomi/vim/action/
--rw-rw-rw-   0        0        0     2202 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/action/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.319198 pyvmomi-8.0.1.0.1/pyVmomi/vim/alarm/
--rw-rw-rw-   0        0        0    15604 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/alarm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.322153 pyvmomi-8.0.1.0.1/pyVmomi/vim/cluster/
--rw-rw-rw-   0        0        0    63584 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.325243 pyvmomi-8.0.1.0.1/pyVmomi/vim/dvs/
--rw-rw-rw-   0        0        0   100848 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/dvs/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.328273 pyvmomi-8.0.1.0.1/pyVmomi/vim/encryption/
--rw-rw-rw-   0        0        0    19092 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/encryption/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.332312 pyvmomi-8.0.1.0.1/pyVmomi/vim/event/
--rw-rw-rw-   0        0        0   106110 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/event/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.334746 pyvmomi-8.0.1.0.1/pyVmomi/vim/ext/
--rw-rw-rw-   0        0        0     2402 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/ext/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.337752 pyvmomi-8.0.1.0.1/pyVmomi/vim/fault/
--rw-rw-rw-   0        0        0   143157 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.340846 pyvmomi-8.0.1.0.1/pyVmomi/vim/host/
--rw-rw-rw-   0        0        0   437042 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.344396 pyvmomi-8.0.1.0.1/pyVmomi/vim/net/
--rw-rw-rw-   0        0        0    11910 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/net/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.347363 pyvmomi-8.0.1.0.1/pyVmomi/vim/option/
--rw-rw-rw-   0        0        0     4185 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/option/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.350374 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/
--rw-rw-rw-   0        0        0    20853 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.354878 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/cluster/
--rw-rw-rw-   0        0        0     1372 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.358893 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/
--rw-rw-rw-   0        0        0    36486 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.361935 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/profileEngine/
--rw-rw-rw-   0        0        0      190 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/profileEngine/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.366492 pyvmomi-8.0.1.0.1/pyVmomi/vim/scheduler/
--rw-rw-rw-   0        0        0     9113 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/scheduler/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.369503 pyvmomi-8.0.1.0.1/pyVmomi/vim/storageDrs/
--rw-rw-rw-   0        0        0    24800 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/storageDrs/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.372496 pyvmomi-8.0.1.0.1/pyVmomi/vim/tenant/
--rw-rw-rw-   0        0        0      414 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/tenant/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.376024 pyvmomi-8.0.1.0.1/pyVmomi/vim/vcha/
--rw-rw-rw-   0        0        0    12321 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vcha/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.380061 pyvmomi-8.0.1.0.1/pyVmomi/vim/view/
--rw-rw-rw-   0        0        0     1417 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/view/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.383022 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/
--rw-rw-rw-   0        0        0   188045 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.386550 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/check/
--rw-rw-rw-   0        0        0     2058 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/check/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.390560 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/customization/
--rw-rw-rw-   0        0        0    12143 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/customization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.394098 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/device/
--rw-rw-rw-   0        0        0    85963 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/device/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.398109 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/guest/
--rw-rw-rw-   0        0        0    17968 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/guest/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.401105 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/replication/
--rw-rw-rw-   0        0        0     1024 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/replication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.404103 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/
--rw-rw-rw-   0        0        0       27 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.406649 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/cluster/
--rw-rw-rw-   0        0        0     1168 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.408643 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/host/
--rw-rw-rw-   0        0        0     9828 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.411654 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/
--rw-rw-rw-   0        0        0    12685 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.416150 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/host/
--rw-rw-rw-   0        0        0     3294 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.419154 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/vcenter/
--rw-rw-rw-   0        0        0     5459 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/vcenter/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.422157 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/
--rw-rw-rw-   0        0        0     2287 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.424267 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/fault/
--rw-rw-rw-   0        0        0     2055 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.428321 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/query/
--rw-rw-rw-   0        0        0    10309 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/query/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.444571 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/
--rw-rw-rw-   0        0        0     4867 2023-05-25 15:14:34.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4798 2023-05-25 15:14:35.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:14:34.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-25 15:14:35.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 15:14:35.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 20:22:03.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/zip-safe
--rw-rw-rw-   0        0        0       12 2022-11-24 21:14:55.000000 pyvmomi-8.0.1.0.1/requirements.txt
--rw-rw-rw-   0        0        0      112 2023-05-25 15:14:36.676003 pyvmomi-8.0.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3006 2023-05-25 15:03:35.000000 pyvmomi-8.0.1.0.1/setup.py
--rw-rw-rw-   0        0        0       42 2023-02-06 15:29:30.000000 pyvmomi-8.0.1.0.1/test-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.546796 pyvmomi-8.0.1.0.1/tests/
--rw-rw-rw-   0        0        0      485 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/README.rst
--rw-rw-rw-   0        0        0     1581 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.590707 pyvmomi-8.0.1.0.1/tests/files/
--rw-rw-rw-   0        0        0    72751 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_datacenter_explode.expect
--rw-rw-rw-   0        0        0     7005 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_datastore_explode.expect
--rw-rw-rw-   0        0        0  1403229 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_host_explode.expect
--rw-rw-rw-   0        0        0     1120 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_network_explode.expect
--rw-rw-rw-   0        0        0    83829 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_default.expect
--rw-rw-rw-   0        0        0    84925 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_objs_match.expect
--rw-rw-rw-   0        0        0    67681 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_strip_dynamic.expect
--rw-rw-rw-   0        0        0   138420 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_type_match.expect
--rw-rw-rw-   0        0        0     3881 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/unknown_method.xml
-drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.669274 pyvmomi-8.0.1.0.1/tests/fixtures/
--rw-rw-rw-   0        0        0    19046 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection.yaml
--rw-rw-rw-   0        0        0     6611 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection_bad_password.yaml
--rw-rw-rw-   0        0        0    24770 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/basic_container_view.yaml
--rw-rw-rw-   0        0        0      619 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/http_proxy.yaml
--rw-rw-rw-   0        0        0    25823 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/iso8601_set_datetime.yaml
--rw-rw-rw-   0        0        0    30887 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/pbm_check_compatibility.yaml
--rw-rw-rw-   0        0        0    23423 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/root_folder_parent.yaml
--rw-rw-rw-   0        0        0    22129 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/smart_connection.yaml
--rw-rw-rw-   0        0        0      329 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/ssl_tunnel.yaml
--rw-rw-rw-   0        0        0      605 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/ssl_tunnel_http_failure.yaml
--rw-rw-rw-   0        0        0    19039 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/sspi_connection.yaml
--rw-rw-rw-   0        0        0   128012 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datacenter_explode.yaml
--rw-rw-rw-   0        0        0    72776 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datastore_explode.yaml
--rw-rw-rw-   0        0        0  1229165 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_host_explode.yaml
--rw-rw-rw-   0        0        0    59413 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_network_explode.yaml
--rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_default.yaml
--rw-rw-rw-   0        0        0   201173 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_objs.yaml
--rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml
--rw-rw-rw-   0        0        0   272726 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_type.yaml
--rw-rw-rw-   0        0        0     3233 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_simple_request_serializer.yaml
--rw-rw-rw-   0        0        0    22674 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_vm_config_iso8601.yaml
--rw-rw-rw-   0        0        0   236577 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/vm_nic_data.yaml
--rw-rw-rw-   0        0        0     5839 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_connect.py
--rw-rw-rw-   0        0        0     1740 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_container_view.py
--rw-rw-rw-   0        0        0     1389 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_deserializer.py
--rw-rw-rw-   0        0        0     4360 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_iso8601.py
--rw-rw-rw-   0        0        0     7305 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_json.py
--rw-rw-rw-   0        0        0     1396 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_managed_object.py
--rw-rw-rw-   0        0        0     2592 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_pbm_check_compatibility.py
--rw-rw-rw-   0        0        0     5051 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_serializer.py
--rw-rw-rw-   0        0        0      432 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_vim_session_oriented_stub.py
--rw-rw-rw-   0        0        0     3086 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_virtual_machine_object.py
--rw-rw-rw-   0        0        0      103 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.367943 pyvmomi-8.0.1.0.2/
+-rw-rw-rw-   0        0        0    11510 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      172 2023-05-05 22:57:58.000000 pyvmomi-8.0.1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      238 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0.2/NOTICE.txt
+-rw-rw-rw-   0        0        0     4716 2023-07-19 08:40:02.368943 pyvmomi-8.0.1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3107 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:01.928684 pyvmomi-8.0.1.0.2/pyVim/
+-rw-rw-rw-   0        0        0      175 2023-06-08 13:13:41.000000 pyvmomi-8.0.1.0.2/pyVim/__init__.py
+-rw-rw-rw-   0        0        0    39785 2023-07-18 17:44:58.000000 pyvmomi-8.0.1.0.2/pyVim/connect.py
+-rw-rw-rw-   0        0        0    62319 2023-06-08 15:36:53.000000 pyvmomi-8.0.1.0.2/pyVim/sso.py
+-rw-rw-rw-   0        0        0    12133 2023-06-08 15:11:39.000000 pyvmomi-8.0.1.0.2/pyVim/task.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.013733 pyvmomi-8.0.1.0.2/pyVmomi/
+-rw-rw-rw-   0        0        0      836 2023-03-10 18:54:35.000000 pyvmomi-8.0.1.0.2/pyVmomi/Cache.py
+-rw-rw-rw-   0        0        0     9634 2023-03-10 18:54:35.000000 pyvmomi-8.0.1.0.2/pyVmomi/Differ.py
+-rw-rw-rw-   0        0        0      932 2023-03-10 18:54:35.000000 pyvmomi-8.0.1.0.2/pyVmomi/Feature.py
+-rw-rw-rw-   0        0        0    12510 2023-03-10 18:54:35.000000 pyvmomi-8.0.1.0.2/pyVmomi/Iso8601.py
+-rw-rw-rw-   0        0        0     1470 2023-03-10 18:54:35.000000 pyvmomi-8.0.1.0.2/pyVmomi/Security.py
+-rw-rw-rw-   0        0        0    74790 2023-07-18 17:40:14.000000 pyvmomi-8.0.1.0.2/pyVmomi/SoapAdapter.py
+-rw-rw-rw-   0        0        0     2187 2023-07-05 20:44:17.000000 pyvmomi-8.0.1.0.2/pyVmomi/StubAdapterAccessorImpl.py
+-rw-rw-rw-   0        0        0      644 2023-03-10 18:54:36.000000 pyvmomi-8.0.1.0.2/pyVmomi/Version.py
+-rw-rw-rw-   0        0        0     5752 2023-03-10 18:54:36.000000 pyvmomi-8.0.1.0.2/pyVmomi/VmomiJSONEncoder.py
+-rw-rw-rw-   0        0        0    73114 2023-06-21 09:48:26.000000 pyvmomi-8.0.1.0.2/pyVmomi/VmomiSupport.py
+-rw-rw-rw-   0        0        0     2769 2023-07-17 11:20:50.000000 pyvmomi-8.0.1.0.2/pyVmomi/__init__.py
+-rw-rw-rw-   0        0        0     5225 2023-07-18 18:14:32.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_core.py
+-rw-rw-rw-   0        0        0    88121 2023-07-18 18:17:26.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_eam.py
+-rw-rw-rw-   0        0        0   121683 2023-07-18 18:16:29.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_pbm.py
+-rw-rw-rw-   0        0        0    12391 2023-07-18 18:17:19.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_query.py
+-rw-rw-rw-   0        0        0   136338 2023-07-18 18:16:22.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_sms.py
+-rw-rw-rw-   0        0        0  1319281 2023-07-18 18:15:24.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_vim.py
+-rw-rw-rw-   0        0        0   506659 2022-07-21 18:24:04.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_vsan.py
+-rw-rw-rw-   0        0        0    89187 2023-07-18 18:13:26.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_vslm.py
+-rw-rw-rw-   0        0        0     1230 2023-07-18 18:16:03.000000 pyvmomi-8.0.1.0.2/pyVmomi/_typeinfos.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.016738 pyvmomi-8.0.1.0.2/pyVmomi/eam/
+-rw-rw-rw-   0        0        0    15173 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.019737 pyvmomi-8.0.1.0.2/pyVmomi/eam/fault/
+-rw-rw-rw-   0        0        0     2426 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.022243 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/
+-rw-rw-rw-   0        0        0     8741 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.024263 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/cluster/
+-rw-rw-rw-   0        0        0       28 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.027257 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/cluster/agent/
+-rw-rw-rw-   0        0        0     1971 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/cluster/agent/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.029266 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/integrity/
+-rw-rw-rw-   0        0        0       30 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/integrity/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.031261 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/integrity/agency/
+-rw-rw-rw-   0        0        0      205 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/integrity/agency/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.034295 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/
+-rw-rw-rw-   0        0        0       60 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.036312 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/agency/
+-rw-rw-rw-   0        0        0     1204 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/agency/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.038304 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/agent/
+-rw-rw-rw-   0        0        0      166 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/agent/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.041295 pyvmomi-8.0.1.0.2/pyVmomi/eam/lccm/
+-rw-rw-rw-   0        0        0    16188 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/lccm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.043822 pyvmomi-8.0.1.0.2/pyVmomi/eam/vib/
+-rw-rw-rw-   0        0        0     1336 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/eam/vib/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.045825 pyvmomi-8.0.1.0.2/pyVmomi/pbm/
+-rw-rw-rw-   0        0        0     5328 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.048839 pyvmomi-8.0.1.0.2/pyVmomi/pbm/auth/
+-rw-rw-rw-   0        0        0       92 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/auth/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.050835 pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/
+-rw-rw-rw-   0        0        0     4472 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.053371 pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/provider/
+-rw-rw-rw-   0        0        0     4965 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.055362 pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/types/
+-rw-rw-rw-   0        0        0     1231 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/types/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.057371 pyvmomi-8.0.1.0.2/pyVmomi/pbm/compliance/
+-rw-rw-rw-   0        0        0     6060 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/compliance/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.060374 pyvmomi-8.0.1.0.2/pyVmomi/pbm/fault/
+-rw-rw-rw-   0        0        0     3064 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.062372 pyvmomi-8.0.1.0.2/pyVmomi/pbm/placement/
+-rw-rw-rw-   0        0        0     4175 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/placement/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.064910 pyvmomi-8.0.1.0.2/pyVmomi/pbm/profile/
+-rw-rw-rw-   0        0        0    11518 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/profile/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.066904 pyvmomi-8.0.1.0.2/pyVmomi/pbm/profile/provider/
+-rw-rw-rw-   0        0        0     1318 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/profile/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.068910 pyvmomi-8.0.1.0.2/pyVmomi/pbm/provider/
+-rw-rw-rw-   0        0        0       86 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.070910 pyvmomi-8.0.1.0.2/pyVmomi/pbm/replication/
+-rw-rw-rw-   0        0        0      904 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/pbm/replication/__init__.pyi
+-rw-rw-rw-   0        0        0        0 2023-05-05 22:57:58.000000 pyvmomi-8.0.1.0.2/pyVmomi/py.typed
+-rw-rw-rw-   0        0        0      244 2023-07-17 11:20:45.000000 pyvmomi-8.0.1.0.2/pyVmomi/pyVmomiSettings.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.073445 pyvmomi-8.0.1.0.2/pyVmomi/sms/
+-rw-rw-rw-   0        0        0     7156 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/sms/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.076434 pyvmomi-8.0.1.0.2/pyVmomi/sms/fault/
+-rw-rw-rw-   0        0        0     5472 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/sms/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.078433 pyvmomi-8.0.1.0.2/pyVmomi/sms/fault/replication/
+-rw-rw-rw-   0        0        0     1119 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/sms/fault/replication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.081443 pyvmomi-8.0.1.0.2/pyVmomi/sms/provider/
+-rw-rw-rw-   0        0        0    10967 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/sms/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.082950 pyvmomi-8.0.1.0.2/pyVmomi/sms/storage/
+-rw-rw-rw-   0        0        0    16428 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/sms/storage/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.085958 pyvmomi-8.0.1.0.2/pyVmomi/sms/storage/replication/
+-rw-rw-rw-   0        0        0    19644 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/sms/storage/replication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.087958 pyvmomi-8.0.1.0.2/pyVmomi/vim/
+-rw-rw-rw-   0        0        0   298858 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.090972 pyvmomi-8.0.1.0.2/pyVmomi/vim/action/
+-rw-rw-rw-   0        0        0     2202 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/action/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.093508 pyvmomi-8.0.1.0.2/pyVmomi/vim/alarm/
+-rw-rw-rw-   0        0        0    15604 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/alarm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.095498 pyvmomi-8.0.1.0.2/pyVmomi/vim/cluster/
+-rw-rw-rw-   0        0        0    63652 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.097507 pyvmomi-8.0.1.0.2/pyVmomi/vim/dvs/
+-rw-rw-rw-   0        0        0   100848 2023-07-18 18:36:39.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/dvs/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.099507 pyvmomi-8.0.1.0.2/pyVmomi/vim/encryption/
+-rw-rw-rw-   0        0        0    19092 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/encryption/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.102506 pyvmomi-8.0.1.0.2/pyVmomi/vim/event/
+-rw-rw-rw-   0        0        0   106110 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/event/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.104041 pyvmomi-8.0.1.0.2/pyVmomi/vim/ext/
+-rw-rw-rw-   0        0        0     2402 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/ext/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.107044 pyvmomi-8.0.1.0.2/pyVmomi/vim/fault/
+-rw-rw-rw-   0        0        0   143445 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.110042 pyvmomi-8.0.1.0.2/pyVmomi/vim/host/
+-rw-rw-rw-   0        0        0   437163 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.112042 pyvmomi-8.0.1.0.2/pyVmomi/vim/net/
+-rw-rw-rw-   0        0        0    11910 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/net/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.114186 pyvmomi-8.0.1.0.2/pyVmomi/vim/option/
+-rw-rw-rw-   0        0        0     4185 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/option/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.116186 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/
+-rw-rw-rw-   0        0        0    20886 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.119194 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/cluster/
+-rw-rw-rw-   0        0        0     1372 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.121198 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/host/
+-rw-rw-rw-   0        0        0    36566 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.123720 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/host/profileEngine/
+-rw-rw-rw-   0        0        0      190 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/host/profileEngine/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.125710 pyvmomi-8.0.1.0.2/pyVmomi/vim/scheduler/
+-rw-rw-rw-   0        0        0     9113 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/scheduler/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.127719 pyvmomi-8.0.1.0.2/pyVmomi/vim/storageDrs/
+-rw-rw-rw-   0        0        0    24800 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/storageDrs/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.129719 pyvmomi-8.0.1.0.2/pyVmomi/vim/tenant/
+-rw-rw-rw-   0        0        0      414 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/tenant/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.132228 pyvmomi-8.0.1.0.2/pyVmomi/vim/vcha/
+-rw-rw-rw-   0        0        0    12321 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vcha/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.134245 pyvmomi-8.0.1.0.2/pyVmomi/vim/view/
+-rw-rw-rw-   0        0        0     1417 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/view/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.137246 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/
+-rw-rw-rw-   0        0        0   188329 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.139244 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/check/
+-rw-rw-rw-   0        0        0     2058 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/check/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.142244 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/customization/
+-rw-rw-rw-   0        0        0    12143 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/customization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.143780 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/device/
+-rw-rw-rw-   0        0        0    85963 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/device/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.145779 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/guest/
+-rw-rw-rw-   0        0        0    17968 2023-07-18 18:36:40.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/guest/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.148779 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/replication/
+-rw-rw-rw-   0        0        0     1024 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/replication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.150770 pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/
+-rw-rw-rw-   0        0        0       60 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.153292 pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/cluster/
+-rw-rw-rw-   0        0        0     1168 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.155301 pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/host/
+-rw-rw-rw-   0        0        0     9872 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.157301 pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/
+-rw-rw-rw-   0        0        0    12718 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.159301 pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/host/
+-rw-rw-rw-   0        0        0     3294 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.162301 pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/vcenter/
+-rw-rw-rw-   0        0        0     5459 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/vcenter/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.163838 pyvmomi-8.0.1.0.2/pyVmomi/vmodl/
+-rw-rw-rw-   0        0        0     2319 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vmodl/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.165829 pyvmomi-8.0.1.0.2/pyVmomi/vmodl/fault/
+-rw-rw-rw-   0        0        0     2055 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vmodl/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.168830 pyvmomi-8.0.1.0.2/pyVmomi/vmodl/query/
+-rw-rw-rw-   0        0        0    10309 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vmodl/query/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.170828 pyvmomi-8.0.1.0.2/pyVmomi/vslm/
+-rw-rw-rw-   0        0        0     8060 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vslm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.173358 pyvmomi-8.0.1.0.2/pyVmomi/vslm/auth/
+-rw-rw-rw-   0        0        0      206 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vslm/auth/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.175357 pyvmomi-8.0.1.0.2/pyVmomi/vslm/event/
+-rw-rw-rw-   0        0        0      295 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vslm/event/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.178357 pyvmomi-8.0.1.0.2/pyVmomi/vslm/fault/
+-rw-rw-rw-   0        0        0      366 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vslm/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.180348 pyvmomi-8.0.1.0.2/pyVmomi/vslm/vso/
+-rw-rw-rw-   0        0        0    10539 2023-07-18 18:36:41.000000 pyvmomi-8.0.1.0.2/pyVmomi/vslm/vso/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.194414 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/
+-rw-rw-rw-   0        0        0     4716 2023-07-19 08:40:01.000000 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5601 2023-07-19 08:40:01.000000 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:40:01.000000 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-19 08:40:01.000000 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-19 08:40:01.000000 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 20:22:03.000000 pyvmomi-8.0.1.0.2/pyvmomi.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       12 2022-11-24 21:14:55.000000 pyvmomi-8.0.1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      112 2023-07-19 08:40:02.369943 pyvmomi-8.0.1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3006 2023-07-19 08:35:46.000000 pyvmomi-8.0.1.0.2/setup.py
+-rw-rw-rw-   0        0        0       25 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/test-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.237445 pyvmomi-8.0.1.0.2/tests/
+-rw-rw-rw-   0        0        0      485 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/README.rst
+-rw-rw-rw-   0        0        0     1581 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-07-05 20:48:00.000000 pyvmomi-8.0.1.0.2/tests/__init__.pyc
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.286051 pyvmomi-8.0.1.0.2/tests/__pycache__/
+-rw-rw-rw-   0        0        0     1300 2023-07-05 18:11:58.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4431 2023-07-18 18:45:56.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_connect.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1125 2023-07-05 18:12:05.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_container_view.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1160 2023-07-05 23:49:47.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_deserializer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2995 2023-07-05 18:12:05.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_iso8601.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5470 2023-07-05 23:49:47.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_json.cpython-310.pyc
+-rw-rw-rw-   0        0        0      972 2023-07-05 18:12:05.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_managed_object.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2182 2023-07-05 23:49:47.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_pbm_check_compatibility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5001 2023-07-05 23:49:47.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_serializer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1056 2023-07-05 23:49:47.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_vim_session_oriented_stub.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2269 2023-07-05 18:12:06.000000 pyvmomi-8.0.1.0.2/tests/__pycache__/test_virtual_machine_object.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.311113 pyvmomi-8.0.1.0.2/tests/files/
+-rw-rw-rw-   0        0        0    72751 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_datacenter_explode.expect
+-rw-rw-rw-   0        0        0     7005 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_datastore_explode.expect
+-rw-rw-rw-   0        0        0  1403229 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_host_explode.expect
+-rw-rw-rw-   0        0        0     1120 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_network_explode.expect
+-rw-rw-rw-   0        0        0    83829 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_default.expect
+-rw-rw-rw-   0        0        0    84925 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_objs_match.expect
+-rw-rw-rw-   0        0        0    67681 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_strip_dynamic.expect
+-rw-rw-rw-   0        0        0   138420 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_type_match.expect
+-rw-rw-rw-   0        0        0     3881 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/files/unknown_method.xml
+drwxrwxrwx   0        0        0        0 2023-07-19 08:40:02.365943 pyvmomi-8.0.1.0.2/tests/fixtures/
+-rw-rw-rw-   0        0        0    19046 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/basic_connection.yaml
+-rw-rw-rw-   0        0        0     6611 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/basic_connection_bad_password.yaml
+-rw-rw-rw-   0        0        0    24770 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/basic_container_view.yaml
+-rw-rw-rw-   0        0        0      619 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/http_proxy.yaml
+-rw-rw-rw-   0        0        0    25823 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/iso8601_set_datetime.yaml
+-rw-rw-rw-   0        0        0    30887 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/pbm_check_compatibility.yaml
+-rw-rw-rw-   0        0        0    23423 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/root_folder_parent.yaml
+-rw-rw-rw-   0        0        0    22129 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/smart_connection.yaml
+-rw-rw-rw-   0        0        0      329 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/ssl_tunnel.yaml
+-rw-rw-rw-   0        0        0      605 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/ssl_tunnel_http_failure.yaml
+-rw-rw-rw-   0        0        0    19039 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/sspi_connection.yaml
+-rw-rw-rw-   0        0        0   128012 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_datacenter_explode.yaml
+-rw-rw-rw-   0        0        0    72776 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_datastore_explode.yaml
+-rw-rw-rw-   0        0        0  1229165 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_host_explode.yaml
+-rw-rw-rw-   0        0        0    59413 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_network_explode.yaml
+-rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_default.yaml
+-rw-rw-rw-   0        0        0   201173 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_objs.yaml
+-rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml
+-rw-rw-rw-   0        0        0   272726 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_type.yaml
+-rw-rw-rw-   0        0        0     3233 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_simple_request_serializer.yaml
+-rw-rw-rw-   0        0        0    22674 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/test_vm_config_iso8601.yaml
+-rw-rw-rw-   0        0        0   236577 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/fixtures/vm_nic_data.yaml
+-rw-rw-rw-   0        0        0     5851 2023-07-18 18:44:19.000000 pyvmomi-8.0.1.0.2/tests/test_connect.py
+-rw-rw-rw-   0        0        0     1740 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/test_container_view.py
+-rw-rw-rw-   0        0        0     1343 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/tests/test_deserializer.py
+-rw-rw-rw-   0        0        0     4360 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/test_iso8601.py
+-rw-rw-rw-   0        0        0     7103 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/tests/test_json.py
+-rw-rw-rw-   0        0        0     1396 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/test_managed_object.py
+-rw-rw-rw-   0        0        0     2713 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/tests/test_pbm_check_compatibility.py
+-rw-rw-rw-   0        0        0     5204 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/tests/test_serializer.py
+-rw-rw-rw-   0        0        0      485 2023-07-05 23:48:08.000000 pyvmomi-8.0.1.0.2/tests/test_vim_session_oriented_stub.py
+-rw-rw-rw-   0        0        0     3086 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.2/tests/test_virtual_machine_object.py
+-rw-rw-rw-   0        0        0      115 2023-07-18 18:42:07.000000 pyvmomi-8.0.1.0.2/tox.ini
```

### Comparing `pyvmomi-8.0.1.0.1/LICENSE.txt` & `pyvmomi-8.0.1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/PKG-INFO` & `pyvmomi-8.0.1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvmomi
-Version: 8.0.1.0.1
+Version: 8.0.1.0.2
 Summary: VMware vSphere Python SDK
 Home-page: https://github.com/vmware/pyvmomi
 Author: VMware, Inc.
 Author-email: jhu@vmware.com
 License: License :: OSI Approved :: Apache Software License
 Keywords: pyvmomi,vsphere,vmware,esx
 Platform: Windows
@@ -36,18 +36,14 @@
 Requires-Python: >=2.7.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Provides-Extra: sso
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 pyvmomi
 ------------
-.. image:: https://travis-ci.org/vmware/pyvmomi.svg?branch=v6.0.0.2016.4
-    :target: https://travis-ci.org/vmware/pyvmomi
-    :alt: Build Status
-
 .. image:: https://img.shields.io/pypi/dm/pyvmomi.svg
     :target: https://pypi.python.org/pypi/pyvmomi/
     :alt: Downloads
 
 pyVmomi is the Python SDK for the VMware vSphere API that allows you to manage 
 ESX, ESXi, and vCenter.
```

### Comparing `pyvmomi-8.0.1.0.1/README.rst` & `pyvmomi-8.0.1.0.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 pyvmomi
 ------------
-.. image:: https://travis-ci.org/vmware/pyvmomi.svg?branch=v6.0.0.2016.4
-    :target: https://travis-ci.org/vmware/pyvmomi
-    :alt: Build Status
-
 .. image:: https://img.shields.io/pypi/dm/pyvmomi.svg
     :target: https://pypi.python.org/pypi/pyvmomi/
     :alt: Downloads
 
 pyVmomi is the Python SDK for the VMware vSphere API that allows you to manage 
 ESX, ESXi, and vCenter.
```

### Comparing `pyvmomi-8.0.1.0.1/pyVim/connect.py` & `pyvmomi-8.0.1.0.2/pyVim/connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #############################################################
 # Copyright (c) 2005-2023 VMware, Inc.
 #############################################################
 
-## @file connect.py
-## @brief Connect to a VMOMI ServiceInstance.
-##
-## Detailed description (for Doxygen goes here)
+# @file connect.py
+# @brief Connect to a VMOMI ServiceInstance.
+#
+# Detailed description (for Doxygen goes here)
 """
 Connect to a VMOMI ServiceInstance.
 
 Detailed description (for [e]pydoc goes here).
 """
 
 import re
@@ -35,15 +35,15 @@
 TOKEN_TYPE_OAUTH_BEARER = 'oauth-bearer'
 TOKEN_TYPE_SAML = 'saml'
 TOKEN_TYPE_SSPI = 'sspi'
 TOKEN_TYPES = [TOKEN_TYPE_OAUTH_BEARER, TOKEN_TYPE_SAML, TOKEN_TYPE_SSPI]
 
 """
 Global regular expression for parsing host and port connection
-See http://www.ietf.org/rfc/rfc3986.txt sec 3.2.2
+See https://www.ietf.org/rfc/rfc3986.txt sec 3.2.2
 """
 _rx = re.compile(r"(^\[.+\]|[^:]+)(:\d+)?$")
 
 _si = None
 """
 Global (thread-shared) ServiceInstance
 
@@ -78,60 +78,60 @@
         return self.obj
 
     def __exit__(self, *exc_info):
         self.obj.close()
 
 
 class VimSessionOrientedStub(SessionOrientedStub):
-    '''A vim-specific SessionOrientedStub.  See the SessionOrientedStub class
+    """A vim-specific SessionOrientedStub.  See the SessionOrientedStub class
     in pyVmomi/SoapAdapter.py for more information.
-    '''
+    """
 
     # The set of exceptions that should trigger a relogin by the session stub.
     SESSION_EXCEPTIONS = (vim.fault.NotAuthenticated, )
 
     @staticmethod
     def makeUserLoginMethod(username, password, locale=None):
-        '''Return a function that will call the vim.SessionManager.Login() method
+        """Return a function that will call the vim.SessionManager.Login() method
         with the given parameters.  The result of this function can be passed as
         the "loginMethod" to a SessionOrientedStub constructor.
-        '''
+        """
         def _doLogin(soapStub):
             si = vim.ServiceInstance("ServiceInstance", soapStub)
             sm = si.content.sessionManager
             if not sm.currentSession:
                 si.content.sessionManager.Login(username, password, locale)
 
         return _doLogin
 
     @staticmethod
     def makeExtensionLoginMethod(extensionKey):
-        '''Return a function that will call the vim.SessionManager.Login() method
+        """Return a function that will call the vim.SessionManager.Login() method
         with the given parameters.  The result of this function can be passed as
         the "loginMethod" to a SessionOrientedStub constructor.
-        '''
+        """
         def _doLogin(soapStub):
             si = vim.ServiceInstance("ServiceInstance", soapStub)
             sm = si.content.sessionManager
             if not sm.currentSession:
                 si.content.sessionManager.LoginExtensionByCertificate(
                     extensionKey)
 
         return _doLogin
 
     @staticmethod
     def makeCertHokTokenLoginMethod(stsUrl, stsCert=None, ssl_context=None):
-        '''Return a function that will call the vim.SessionManager.LoginByToken()
+        """Return a function that will call the vim.SessionManager.LoginByToken()
         after obtaining a HoK SAML token from the STS. The result of this function
         can be passed as the "loginMethod" to a SessionOrientedStub constructor.
 
         @param stsUrl: URL of the SAML Token issuing service. (i.e. SSO server).
         @param stsCert: public key of the STS service.
         @param ssl_context: SSL context
-        '''
+        """
         assert (stsUrl)
 
         def _doLogin(soapStub):
             from . import sso
             cert = soapStub.schemeArgs['cert_file']
             key = soapStub.schemeArgs['key_file']
             authenticator = sso.SsoAuthenticator(sts_url=stsUrl,
@@ -157,24 +157,24 @@
 
     @staticmethod
     def makeCredBearerTokenLoginMethod(username,
                                        password,
                                        stsUrl,
                                        stsCert=None,
                                        ssl_context=None):
-        '''Return a function that will call the vim.SessionManager.LoginByToken()
+        """Return a function that will call the vim.SessionManager.LoginByToken()
         after obtaining a Bearer token from the STS. The result of this function
         can be passed as the "loginMethod" to a SessionOrientedStub constructor.
 
         @param username: username of the user/service registered with STS.
         @param password: password of the user/service registered with STS.
         @param stsUrl: URL of the SAML Token issueing service. (i.e. SSO server).
         @param stsCert: public key of the STS service.
         @param ssl_context: SSL context
-        '''
+        """
         assert (username)
         assert (password)
         assert (stsUrl)
 
         def _doLogin(soapStub):
             from . import sso
             cert = soapStub.schemeArgs['cert_file']
@@ -252,15 +252,15 @@
     @param keyFile: ssl key file path
     @type  keyFile: string
     @param certFile: ssl cert file path
     @type  certFile: string
     @param httpProxyHost The host name of the proxy server.
     @type  httpProxyHost: string
     @param httpProxyPort The proxy server port.
-    @type  httpProxyPort: string
+    @type  httpProxyPort: int
     @param thumbprint: host cert thumbprint
     @type  thumbprint: string
     @param sslContext: SSL Context describing the various SSL options. It is only
                         supported in Python 2.7.9 or higher.
     @type  sslContext: SSL.Context
     @param httpConnectionTimeout: Timeout in secs for http requests.
     @type  httpConnectionTimeout: int
@@ -270,15 +270,15 @@
     @type  token: string
     @param token: Authentication and Authorization token to use for the connection.
                     The presence of this token overrides the user and pwd parameters.
     @type  tokenType: string
     @param tokenType: Select which type of Authentication and Authorization token to use.
     @type  disableSslCertValidation: bool
     @param disableSslCertValidation: Creates an unverified SSL context when True.
-    @type  customHeaders: dictionary
+    @type  customHeaders: dict
     @param customHeaders: Dictionary with custom HTTP headers.
     @param b64token: base64 encoded token
            *** Deprecated: Use token instead ***
     @type  b64token: string
     @param mechanism: authentication mechanism: userpass or sspi
            *** Deprecated: Use tokenType instead ***
     @type  mechanism: string
@@ -335,18 +335,18 @@
                        tokenType=tokenType,
                        customHeaders=customHeaders)
     SetSi(si)
 
     return si
 
 
-def Disconnect(si = None):
+def Disconnect(si=None):
     """
     Logout and disconnect the service instance
-    @param si: Service instance (returned from Connect)
+    @param si: The service instance (returned from Connect)
                Defaults to the saved service instance
     """
     if not si:
         si = GetSi()
 
     if not si:
         return
@@ -359,15 +359,15 @@
 
     si._stub.DropConnections()
 
     if si == GetSi():
         SetSi(None)
 
 
-## Method that gets a local ticket for the specified user
+# Method that gets a local ticket for the specified user
 def GetLocalTicket(si, user):
     try:
         sessionManager = si.content.sessionManager
     except Exception as e:
         if type(e).__name__ == 'ExpatError':
             msg = 'Malformed response while querying for local ticket: "%s"' % e
             raise vim.fault.HostConnectFault(msg=msg)
@@ -376,16 +376,16 @@
             raise vim.fault.HostConnectFault(msg=msg)
     localTicket = sessionManager.AcquireLocalTicket(userName=user)
     with open(localTicket.passwordFilePath) as f:
         content = f.read()
     return localTicket.userName, content
 
 
-## Private method that performs the actual Connect and returns a
-## connected service instance object.
+# Private method that performs the actual Connect and returns a
+# connected service instance object.
 
 
 def __Login(host,
             port,
             user,
             pwd,
             # TODO Remove service
@@ -427,15 +427,15 @@
     @param keyFile: ssl key file path
     @type  keyFile: string
     @param certFile: ssl cert file path
     @type  certFile: string
     @param httpProxyHost The host name of the proxy server.
     @type  httpProxyHost: string
     @param httpProxyPort The proxy server port.
-    @type  httpProxyPort: string
+    @type  httpProxyPort: int
     @param thumbprint: host cert thumbprint
     @type  thumbprint: string
     @param sslContext: SSL Context describing the various SSL options. It is only
                         supported in Python 2.7.9 or higher.
     @type  sslContext: SSL.Context
     @param httpConnectionTimeout: Timeout in secs for http requests.
     @type  httpConnectionTimeout: int
@@ -443,15 +443,15 @@
                                     negative numbers for never closing the connections
     @type  connectionPoolTimeout: int
     @type  token: string
     @param token: Authentication and Authorization token to use for the connection.
                     The presence of this token overrides the user and pwd parameters.
     @type  tokenType: string
     @param tokenType: Select which type of Authentication and Authorization token to use.
-    @type  customHeaders: dictionary
+    @type  customHeaders: dict
     @param customHeaders: Dictionary with custom HTTP headers.
     """
 
     # XXX remove the adapter and service arguments once dependent code is fixed
     if adapter != "SOAP":
         raise ValueError(adapter)
 
@@ -522,44 +522,44 @@
             content.sessionManager.LoginBySSPI(token)
         else:
             raise Exception("'{0}' token type is not supported. "
                             "Supported types are: {1}".format(tokenType, TOKEN_TYPES))
     return si, stub
 
 
-## Get the saved service instance.
+# Get the saved service instance.
 
 
 def GetSi():
     """ Get the saved service instance. """
     return _si
 
 
-## Set the saved service instance.
+# Set the saved service instance.
 
 
 def SetSi(si):
     """ Set the saved service instance. """
 
     global _si
     _si = si
 
 
-## Get the global saved stub
+# Get the global saved stub
 
 
 def GetStub():
     """ Get the global saved stub. """
     si = GetSi()
     if si:
         return si._GetStub()
     return None
 
 
-## RAII-style class for managing connections
+# RAII-style class for managing connections
 
 
 class Connection(object):
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
         self.si = None
@@ -586,15 +586,15 @@
 
     def __exit__(self, *exc_info):
         if self.si:
             Disconnect(self.si)
             self.si = None
 
 
-## Deprecated, use __GetElementTree method instead
+# Deprecated, use __GetElementTree method instead
 def __GetElementTreeFromUrl(url, sslContext):
     """
     Private method that returns an ElementTree for the XML document referenced by
     the url.
 
     @param url: URL
     @type  url: string
@@ -619,64 +619,73 @@
                 return tree
     except ExpatError:
         pass
     return None
 
 
 def __GetElementTree(protocol, server, port, path, sslContext,
-                     httpProxyHost, httpProxyPort):
+                     httpProxyHost, httpProxyPort,
+                     customHeaders):
     """
     Private method that returns ElementTree for a remote XML document.
 
     @param protocol: What protocol to use for the connection (e.g. https or http).
     @type  protocol: string
     @param server: Which server to connect to.
     @type  server: string
     @param port: Port
     @type  port: int
     @param path: Path
     @type  path: string
     @param sslContext: SSL Context describing the various SSL options. It is only
                         supported in Python 2.7.9 or higher.
     @type  sslContext: SSL.Context
+    @param httpProxyHost The host name of the proxy server.
+    @type  httpProxyHost: string
+    @param httpProxyPort The proxy server port.
+    @type  httpProxyPort: int
+    @type  customHeaders: dict
+    @param customHeaders: Dictionary with custom HTTP headers.
     """
     tree = ElementTree()
+    headers = customHeaders if customHeaders else {}
 
     if httpProxyHost:
         kwargs = {"context": sslContext} if sslContext else {}
         conn = http_client.HTTPSConnection(httpProxyHost, port=httpProxyPort, **kwargs)
-        conn.set_tunnel(server, port)
+        conn.set_tunnel(server, port, headers)
     elif protocol == "https":
         kwargs = {"context": sslContext} if sslContext else {}
         conn = http_client.HTTPSConnection(server, port=port, **kwargs)
     elif protocol == "http":
         conn = http_client.HTTPConnection(server, port=port)
     else:
         raise Exception("Protocol " + protocol + " not supported.")
-    conn.request("GET", path)
+    conn.request(method="GET", url=path, headers=headers)
     try:
         response = conn.getresponse()
         if response.status == 200:
             try:
                 tree.parse(response)
                 return tree
             except ExpatError:
                 pass
         return None
     finally:
         conn.close()
 
 
-## Private method that returns an ElementTree describing the API versions
-## supported by the specified server.  The result will be vimServiceVersions.xml
-## if it exists, otherwise None.
+# Private method that returns an ElementTree describing the API versions
+# supported by the specified server.  The result will be vimServiceVersions.xml
+# if it exists, otherwise None.
 
 
 def __GetServiceVersionDescription(protocol, server, port, path, sslContext,
-                                   httpProxyHost, httpProxyPort):
+                                   httpProxyHost, httpProxyPort,
+                                   customHeaders):
     """
     Private method that returns an ElementTree describing the API versions
     supported by the specified server.  The result will be vimServiceVersions.xml
     if it exists, otherwise vimService.wsdl if it exists, otherwise None.
 
     @param protocol: What protocol to use for the connection (e.g. https or http).
     @type  protocol: string
@@ -685,23 +694,29 @@
     @param port: Port
     @type  port: int
     @param path: Path
     @type  path: string
     @param sslContext: SSL Context describing the various SSL options. It is only
                         supported in Python 2.7.9 or higher.
     @type  sslContext: SSL.Context
+    @param httpProxyHost The host name of the proxy server.
+    @type  httpProxyHost: string
+    @param httpProxyPort The proxy server port.
+    @type  httpProxyPort: int
+    @type  customHeaders: dict
+    @param customHeaders: Dictionary with custom HTTP headers.
     """
 
     return __GetElementTree(protocol, server, port,
                             path + "/vimServiceVersions.xml", sslContext,
-                            httpProxyHost, httpProxyPort)
+                            httpProxyHost, httpProxyPort, customHeaders)
 
 
-## Private method that returns true if the service version description document
-##  indicates that the desired version is supported
+# Private method that returns true if the service version description document
+#  indicates that the desired version is supported
 
 
 def __VersionIsSupported(desiredVersion, serviceVersionDescription):
     """
     Private method that returns true if the service version description document
     indicates that the desired version is supported
 
@@ -729,20 +744,21 @@
             else:
                 for versionId in namespace.findall('priorVersions/version'):
                     if versionId.text == desiredVersionId:
                         return True
     return False
 
 
-## Private method that returns the most preferred API version supported by the
-## specified server,
+# Private method that returns the most preferred API version supported by the
+# specified server,
 
 
 def __FindSupportedVersion(protocol, server, port, path, preferredApiVersions,
-                           sslContext, httpProxyHost, httpProxyPort):
+                           sslContext, httpProxyHost, httpProxyPort,
+                           customHeaders):
     """
     Private method that returns the most preferred API version supported by the
     specified server,
 
     @param protocol: What protocol to use for the connection (e.g. https or http).
     @type  protocol: string
     @param server: Which server to connect to.
@@ -754,18 +770,25 @@
     @param preferredApiVersions: Acceptable API version(s) (e.g. vim.version.version9)
                                     If a list of versions is specified the versions should
                                     be ordered from most to least preferred.
     @type  preferredApiVersions: string or string list
     @param sslContext: SSL Context describing the various SSL options. It is only
                         supported in Python 2.7.9 or higher.
     @type  sslContext: SSL.Context
+    @param httpProxyHost The host name of the proxy server.
+    @type  httpProxyHost: string
+    @param httpProxyPort The proxy server port.
+    @type  httpProxyPort: int
+    @type  customHeaders: dict
+    @param customHeaders: Dictionary with custom HTTP headers.
     """
 
     serviceVersionDescription = __GetServiceVersionDescription(
-        protocol, server, port, path, sslContext, httpProxyHost, httpProxyPort)
+        protocol, server, port, path, sslContext, httpProxyHost,
+        httpProxyPort, customHeaders)
     if serviceVersionDescription is None:
         return None
 
     if not isinstance(preferredApiVersions, list):
         preferredApiVersions = [preferredApiVersions]
 
     for desiredVersion in preferredApiVersions:
@@ -789,40 +812,44 @@
                      cacertsFile=None,
                      preferredApiVersions=None,
                      acceptCompressedResponses=True,
                      samlToken=None,
                      sslContext=None,
                      httpConnectionTimeout=None,
                      connectionPoolTimeout=CONNECTION_POOL_IDLE_TIMEOUT_SEC,
-                     disableSslCertValidation=False):
+                     disableSslCertValidation=False,
+                     customHeaders=None):
     """
     Determine the most preferred API version supported by the specified server,
     then create a soap stub adapter using that version
 
     The parameters are the same as for pyVmomi.SoapStubAdapter except for
     version which is renamed to prefferedApiVersions
 
     @param preferredApiVersions: Acceptable API version(s) (e.g. vim.version.version9)
                                     If a list of versions is specified the versions should
                                     be ordered from most to least preferred.  If None is
                                     specified, the list of versions support by pyVmomi will
                                     be used.
     @type  preferredApiVersions: string or string list
-    @type disableSslCertValidation: bool
+    @type  disableSslCertValidation: bool
     @param disableSslCertValidation: Creates an unverified SSL context when True.
+    @type  customHeaders: dict
+    @param customHeaders: Dictionary with custom HTTP headers.
     """
     if preferredApiVersions is None:
         preferredApiVersions = GetServiceVersions('vim25')
 
     sslContext = getSslContext(host, sslContext, disableSslCertValidation)
 
     supportedVersion = __FindSupportedVersion('https' if port > 0 else 'http',
                                               host, port, path,
                                               preferredApiVersions, sslContext,
-                                              httpProxyHost, httpProxyPort)
+                                              httpProxyHost, httpProxyPort,
+                                              customHeaders)
     if supportedVersion is None:
         raise Exception("{0}:{1} is down or is not a VIM server"
                         .format(host, port))
 
     return SoapStubAdapter(host=host,
                            port=port,
                            path=path,
@@ -837,15 +864,16 @@
                            thumbprint=thumbprint,
                            cacertsFile=cacertsFile,
                            version=supportedVersion,
                            acceptCompressedResponses=acceptCompressedResponses,
                            samlToken=samlToken,
                            sslContext=sslContext,
                            httpConnectionTimeout=httpConnectionTimeout,
-                           connectionPoolTimeout=connectionPoolTimeout)
+                           connectionPoolTimeout=connectionPoolTimeout,
+                           customHeaders=customHeaders)
 
 
 def SmartConnect(protocol='https',
                  host='localhost',
                  port=443,
                  user='root',
                  pwd='',
@@ -903,15 +931,15 @@
     @param keyFile: ssl key file path
     @type  keyFile: string
     @param certFile: ssl cert file path
     @type  certFile: string
     @param httpProxyHost The host name of the proxy server.
     @type  httpProxyHost: string
     @param httpProxyPort The proxy server port.
-    @type  httpProxyPort: string
+    @type  httpProxyPort: int
     @param thumbprint: host cert thumbprint
     @type  thumbprint: string
     @param sslContext: SSL Context describing the various SSL options. It is only
                         supported in Python 2.7.9 or higher.
     @type  sslContext: SSL.Context
     @param httpConnectionTimeout: Timeout in secs for http requests.
     @type  httpConnectionTimeout: int
@@ -919,14 +947,16 @@
                                     negative numbers for never closing the connections
     @type  connectionPoolTimeout: int
     @type  token: string
     @param token: Authentication and Authorization token to use for the connection.
                     The presence of this token overrides the user and pwd parameters.
     @type disableSslCertValidation: bool
     @param disableSslCertValidation: Creates an unverified SSL context when True.
+    @type  customHeaders: dict
+    @param customHeaders: Dictionary with custom HTTP headers.
     @param b64token: base64 encoded token
            *** Deprecated: Use token instead ***
     @type  b64token: string
     @param mechanism: authentication mechanism: userpass or sspi
            *** Deprecated: Use tokenType instead ***
     @type  mechanism: string
     """
@@ -934,15 +964,16 @@
     if preferredApiVersions is None:
         preferredApiVersions = GetServiceVersions('vim25')
 
     sslContext = getSslContext(host, sslContext, disableSslCertValidation)
 
     supportedVersion = __FindSupportedVersion(protocol, host, port, path,
                                               preferredApiVersions, sslContext,
-                                              httpProxyHost, httpProxyPort)
+                                              httpProxyHost, httpProxyPort,
+                                              customHeaders)
     if supportedVersion is None:
         raise Exception("{0}:{1} is down or is not a VIM server"
                         .format(host, port))
 
     portNumber = protocol == "http" and -int(port) or int(port)
 
     return Connect(host=host,
```

### Comparing `pyvmomi-8.0.1.0.1/pyVim/sso.py` & `pyvmomi-8.0.1.0.2/pyVim/sso.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #############################################################
-# Copyright (c) 2012-2022 VMware, Inc.
+# Copyright (c) 2012-2023 VMware, Inc.
 # A python helper module to do SSO related operations.
 #############################################################
 __author__ = 'VMware, Inc.'
 
 #Standard library imports.
 import six.moves.http_client
 import re
@@ -35,23 +35,23 @@
 SHA512 = 'sha512'
 
 # add default parser to etree with resolve_entities set to False
 default_parser = etree.XMLParser(resolve_entities=False)
 etree.set_default_parser(default_parser)
 
 def _extract_certificate(cert):
-    '''
+    """
     Extract DER certificate/private key from DER/base64-ed DER/PEM string.
 
     @type           cert: C{str}
     @param          cert: Certificate/private key in one of three supported formats.
 
     @rtype: C{str}
     @return: Certificate/private key in DER (binary ASN.1) format.
-    '''
+    """
     if not cert:
         raise IOError('Empty certificate')
     signature = cert[0]
     # DER certificate is sequence.  ASN.1 sequence is 0x30.
     if signature == '\x30':
         return cert
     # PEM without preamble.  Base64-encoded 0x30 is 0x4D.
@@ -67,170 +67,171 @@
 #time.strftime() method returns 6 digit millisecond
 #Formatting time with 3 digit milliseconds
 def format_time(time):
     return time[:-3] + 'Z'
 
 
 class SoapException(Exception):
-    '''
+    """
     Exception raised in case of STS request failure.
-    '''
+    """
     def __init__(self, soap_msg, fault_code, fault_string):
-        '''
+        """
         Initializer for SoapException.
 
         @type      soap_msg: C{str}
         @param     soap_msg: the soap fault XML returned by STS
         @type    fault_code: C{str}
         @param   fault_code: The fault code returned by STS.
         @type  fault_string: C{str}
         @param fault_string: The fault string returned by STS.
-        '''
+        """
         self._soap_msg = soap_msg
         self._fault_code = fault_code
         self._fault_string = fault_string
         Exception.__init__(self)
 
     def __str__(self):
-        '''
+        """
         Returns the string representation of SoapException.
 
         @rtype: C{str}
         @return: string representation of SoapException
-        '''
+        """
         return ("SoapException:\nfaultcode: %(_fault_code)s\n"
                 "faultstring: %(_fault_string)s\n"
                 "faultxml: %(_soap_msg)s" % self.__dict__)
 
 
 class SSOHTTPConnection(six.moves.http_client.HTTPConnection):
-    '''
+    """
     A class that establishes HTTP Connection.
     Only intened to be used for calls routing through
     a local sidecar proxy (localhost:1080).
-    '''
+    """
     def __init__(self, *args, **kwargs):
-        '''
+        """
         Initializer.  See httplib.HTTPConnection for other arguments
-        '''
+        """
         tmpKwargs = {}
         httpConn = six.moves.http_client.HTTPConnection
         for key in httpConn.__init__.__code__.co_varnames:
             if key in kwargs and key != 'self':
                 tmpKwargs[key] = kwargs[key]
         self.host = kwargs.pop('host')
         six.moves.http_client.HTTPConnection.__init__(self, *args, **tmpKwargs)
 
+
 class SSOHTTPSConnection(six.moves.http_client.HTTPSConnection):
-    '''
+    """
     An HTTPS class that verifies server's certificate on connect.
-    '''
+    """
     def __init__(self, *args, **kwargs):
-        '''
+        """
         Initializer.  See httplib.HTTPSConnection for other arguments
         than thumbprint and server_cert.
 
         At least one of thumbprint, server_cert should be provided,
         otherwise server certificate is not validated.
 
         @type           thumbprint: C(str)
         @param          thumbprint: Expected SHA-1 thumbprint of the server
                                     certificate.  May be None.
 
         @type          server_cert: C(str)
         @param         server_cert: File with expected server certificate.
                                     May be None.
-        '''
+        """
         self.server_thumbprint = kwargs.pop('thumbprint')
         if self.server_thumbprint is not None:
             self.server_thumbprint = re.sub(':', '',
                                             self.server_thumbprint.lower())
         server_cert_path = kwargs.pop('server_cert')
         if server_cert_path is not None:
             with open(server_cert_path, 'rb') as f:
                 server_cert = f.read().decode(UTF_8)
             self.server_cert = _extract_certificate(server_cert)
         else:
             self.server_cert = None
         six.moves.http_client.HTTPSConnection.__init__(self, *args, **kwargs)
 
     def _check_cert(self, peerCert):
-        '''
+        """
         Verify that peer certificate matches one we expect.
 
         @type             peerCert: C(str)
         @param            peerCert: Server certificate in DER format.
 
         @rtype: boolean
         @return: True if peerCert is acceptable.  False otherwise.
-        '''
+        """
         try:
             if self.server_cert is not None:
                 if peerCert != self.server_cert:
                     raise Exception("Invalid certificate")
             if self.server_thumbprint:
                 VerifyCertThumbprint(peerCert, self.server_thumbprint)
         except Exception:
             self.sock.close()
             self.sock = None
             raise
 
     def connect(self):
-        '''
+        """
         Connect method: connects to the remote system, and upon
         successful connection validates certificate.
 
         Throws an exception when something is wrong.  See
         httplib.HTTPSConnection.connect() for details.
-        '''
+        """
         six.moves.http_client.HTTPSConnection.connect(self)
 
         self._check_cert(self.sock.getpeercert(True))
 
 
 def is_sidecar_request(scheme, host):
-    '''
+    """
     Check if the request is through
     local sidecar (localhost:1080)
-    '''
+    """
     if scheme == "http" and host == "localhost:1080":
-        return True;
+        return True
 
 
 class SsoAuthenticator(object):
-    '''
+    """
     A class to handle the transport layer communication between the client and
     the STS service.
-    '''
+    """
     def __init__(self, sts_url, sts_cert=None, thumbprint=None):
-        '''
+        """
         Initializer for SsoAuthenticator.
 
         @type           sts_url: C{str}
         @param          sts_url: URL for the Security Token Service. Usually
                                  obtained by querying Component Manager.
         @type          sts_cert: C{str}
         @param         sts_cert: The file with public key of the Security
                                  Token Service.  Usually obtained from
                                  Component Manager and written to the file.
         @type        thumbprint: C{str}
         @param       thumbprint: The SHA-1 thumbprint of the certificate used
                                  by the Security Token Service.  It is same
                                  thumbprint you can pass to pyVmomi SoapAdapter.
-        '''
+        """
         self._sts_cert = sts_cert
         self._sts_url = sts_url
         self._sts_thumbprint = thumbprint
 
     def perform_request(self,
                         soap_message,
                         public_key=None,
                         private_key=None,
                         ssl_context=None):
-        '''
+        """
         Performs a Holder-of-Key SAML token request using the service user's
         certificates or a bearer token request using the user credentials.
 
         @type      soap_message: C{str}
         @param     soap_message: Authentication SOAP request.
         @type        public_key: C{str}
         @param       public_key: File containing the public key for the service
@@ -239,24 +240,24 @@
         @param      private_key: File containing the private key for the service
                                  user registered with SSO, in PEM format.
         @type       ssl_context: C{ssl.SSLContext}
         @param      ssl_context: SSL context describing the various SSL options.
                                  It is only supported in Python 2.7.9 or higher.
         @rtype: C{str}
         @return: Response received from the STS after the HoK request.
-        '''
+        """
         parsed = urlparse(self._sts_url)
         host = parsed.netloc  # pylint: disable=E1101
         scheme = parsed.scheme
         encoded_message = soap_message.encode(UTF_8)
 
-        '''
+        """
         Allow creation of HTTPConnection, only for calls routing
         through local sidecar (localhost:1080)
-        '''
+        """
         if is_sidecar_request(scheme, host):
             webservice = SSOHTTPConnection(host=host)
         elif hasattr(ssl, '_create_unverified_context'):
             # Python 2.7.9 has stronger SSL certificate validation, so we need
             # to pass in a context when dealing with self-signed certificates.
             webservice = SSOHTTPSConnection(host=host,
                                             key_file=private_key,
@@ -307,15 +308,15 @@
                                   public_key=None,
                                   private_key=None,
                                   request_duration=60,
                                   token_duration=600,
                                   delegatable=False,
                                   renewable=False,
                                   ssl_context=None):
-        '''
+        """
         Extracts the assertion from the Bearer Token received from the Security
         Token Service.
 
         @type          username: C{str}
         @param         username: Username for the user for which bearer token
                                  needs to be requested.
         @type          password: C{str}
@@ -341,15 +342,15 @@
         @param      delegatable: Whether the generated token is delegatable or not
                                  The default value is False
         @type       ssl_context: C{ssl.SSLContext}
         @param      ssl_context: SSL context describing the various SSL options.
                                  It is only supported in Python 2.7.9 or higher.
         @rtype: C{str}
         @return: The SAML assertion in Unicode.
-        '''
+        """
         request = SecurityTokenRequest(username=username,
                                        password=password,
                                        public_key=public_key,
                                        private_key=private_key,
                                        request_duration=request_duration,
                                        token_duration=token_duration)
         soap_message = request.construct_bearer_token_request(
@@ -364,15 +365,15 @@
     def _get_gss_soap_response(self,
                                binary_token,
                                request_duration=60,
                                token_duration=600,
                                delegatable=False,
                                renewable=False,
                                ssl_context=None):
-        '''
+        """
         Extracts the assertion from the Bearer Token received from the Security
         Token Service using the binary token generated using either sspi or gss module.
 
         @type  binary_token: C{str}
         @param binary_token: The security token in base64 encoded format
 
         @type  request_duration: C{long}
@@ -391,29 +392,29 @@
         @param        renewable: Whether the generated token is renewable or not
                                  The default value is False
         @type       ssl_context: C{ssl.SSLContext}
         @param      ssl_context: SSL context describing the various SSL options.
                                  It is only supported in Python 2.7.9 or higher.
         @rtype: C{str}
         @return: The SAML assertion.
-        '''
+        """
         request = SecurityTokenRequest(request_duration=request_duration,
                                        token_duration=token_duration,
                                        gss_binary_token=binary_token)
         soap_message = request.construct_bearer_token_request_with_binary_token(
             delegatable=delegatable, renewable=renewable)
         return self.perform_request(soap_message, ssl_context=ssl_context)
 
     def _get_bearer_saml_assertion_win(self,
                                        request_duration=60,
                                        token_duration=600,
                                        delegatable=False,
                                        renewable=False,
                                        ssl_context=None):
-        '''
+        """
         Extracts the assertion from the Bearer Token received from the Security
         Token Service using the SSPI module.
 
         @type  request_duration: C{long}
         @param request_duration: The duration for which the request is valid. If
                                  the STS receives this request after this
                                  duration, it is assumed to have expired. The
@@ -429,15 +430,15 @@
         @param        renewable: Whether the generated token is renewable or not
                                  The default value is False
         @type       ssl_context: C{ssl.SSLContext}
         @param      ssl_context: SSL context describing the various SSL options.
                                  It is only supported in Python 2.7.9 or higher.
         @rtype: C{str}
         @return: The SAML assertion.
-        '''
+        """
         import sspi, win32api
         spn = "sts/%s.com" % win32api.GetDomainName()
         sspiclient = sspi.ClientAuth("Kerberos", targetspn=spn)
         in_buf = None
         err = True
         # The following will keep running unless we receive a saml token or an error
         while True:
@@ -466,15 +467,15 @@
         return saml_token
 
     def _get_bearer_saml_assertion_lin(self,
                                        request_duration=60,
                                        token_duration=600,
                                        delegatable=False,
                                        renewable=False):
-        '''
+        """
         Extracts the assertion from the Bearer Token received from the Security
         Token Service using kerberos.
 
         @type  request_duration: C{long}
         @param request_duration: The duration for which the request is valid. If
                                  the STS receives this request after this
                                  duration, it is assumed to have expired. The
@@ -487,15 +488,15 @@
         @param      delegatable: Whether the generated token is delegatable or not
                                  The default value is False
         @type         renewable: C{boolean}
         @param        renewable: Whether the generated token is renewable or not
                                  The default value is False
         @rtype: C{str}
         @return: The SAML assertion in Unicode.
-        '''
+        """
         import kerberos, platform
         service = 'host@%s' % platform.node()
         _, context = kerberos.authGSSClientInit(service, 0)
         challenge = ''
         # The following will keep running unless we receive a saml token or an error
         while True:
             # Call GSS step
@@ -525,15 +526,15 @@
         return saml_token
 
     def get_bearer_saml_assertion_gss_api(self,
                                           request_duration=60,
                                           token_duration=600,
                                           delegatable=False,
                                           renewable=False):
-        '''
+        """
         Extracts the assertion from the Bearer Token received from the Security
         Token Service using the GSS API.
 
         @type  request_duration: C{long}
         @param request_duration: The duration for which the request is valid. If
                                  the STS receives this request after this
                                  duration, it is assumed to have expired. The
@@ -546,35 +547,35 @@
         @param      delegatable: Whether the generated token is delegatable or not
                                  The default value is False
         @type         renewable: C{boolean}
         @param        renewable: Whether the generated token is renewable or not
                                  The default value is False
         @rtype: C{str}
         @return: The SAML assertion.
-        '''
+        """
         if sys.platform == "win32":
             saml_token = self._get_bearer_saml_assertion_win(
                 request_duration, token_duration, delegatable, renewable)
         else:
             raise Exception("Currently, not supported on this platform")
-            ## TODO Remove this exception once SSO supports validation of tickets
+            # TODO Remove this exception once SSO supports validation of tickets
             #       generated against host machines
             # saml_token = self._get_bearer_saml_assertion_lin(request_duration, token_duration, delegatable)
         return saml_token
 
     def get_hok_saml_assertion(self,
                                public_key,
                                private_key,
                                request_duration=60,
                                token_duration=600,
                                act_as_token=None,
                                delegatable=False,
                                renewable=False,
                                ssl_context=None):
-        '''
+        """
         Extracts the assertion from the response received from the Security
         Token Service.
 
         @type        public_key: C{str}
         @param       public_key: File containing the public key for the service
                                  user registered with SSO, in PEM format.
         @type       private_key: C{str}
@@ -597,15 +598,15 @@
         @param        renewable: Whether the generated token is renewable or not
                                  The default value is False
         @type       ssl_context: C{ssl.SSLContext}
         @param      ssl_context: SSL context describing the various SSL options.
                                  It is only supported in Python 2.7.9 or higher.
         @rtype: C{str}
         @return: The SAML assertion in Unicode.
-        '''
+        """
         request = SecurityTokenRequest(public_key=public_key,
                                        private_key=private_key,
                                        request_duration=request_duration,
                                        token_duration=token_duration)
         soap_message = request.construct_hok_request(delegatable=delegatable,
                                                      act_as_token=act_as_token,
                                                      renewable=renewable)
@@ -669,30 +670,30 @@
         return etree.tostring(_extract_element(
             etree.fromstring(hok_token), 'Assertion',
             {'saml2': "urn:oasis:names:tc:SAML:2.0:assertion"}),
                               pretty_print=False).decode(UTF_8)
 
 
 class SecurityTokenRequest(object):
-    '''
+    """
     SecurityTokenRequest class handles the serialization of request to the STS
     for a SAML token.
-    '''
+    """
 
     #pylint: disable=R0902
     def __init__(self,
                  username=None,
                  password=None,
                  public_key=None,
                  private_key=None,
                  request_duration=60,
                  token_duration=600,
                  gss_binary_token=None,
                  hok_token=None):
-        '''
+        """
         Initializer for the SecurityToken Request class.
 
         @type          username: C{str}
         @param         username: Username for the user for which bearer token
                                  needs to be requested.
         @type          password: C{str}
         @param         password: Password for the user for which bearer token
@@ -709,15 +710,15 @@
                                  duration, it is assumed to have expired. The
                                  duration is specified in seconds and default is
                                  60s.
         @type    token_duration: C{long}
         @param   token_duraiton: The duration for which the SAML token is issued
                                  for. The duration is specified in seconds and
                                  the default is 600s.
-        '''
+        """
         self._timestamp_id = _generate_id()
         self._signature_id = _generate_id()
         self._request_id = _generate_id()
         self._security_token_id = _generate_id()
         current = datetime.datetime.utcnow()
         self._created = format_time(current.strftime(TIME_FORMAT))
         self._expires = format_time(
@@ -763,66 +764,66 @@
         if self._public_key_file:
             with open(self._public_key_file) as fp:
                 self._public_key = fp.read()
 
     def construct_bearer_token_request(self,
                                        delegatable=False,
                                        renewable=False):
-        '''
+        """
         Constructs the actual Bearer token SOAP request.
 
         @type  delegatable: C{boolean}
         @param delegatable: Whether the generated token is delegatable or not
         @type    renewable: C{boolean}
         @param   renewable: Whether the generated token is renewable or not
                             The default value is False
         @rtype:  C{str}
         @return: Bearer token SOAP request.
-        '''
+        """
         self._key_type = "http://docs.oasis-open.org/ws-sx/ws-trust/200512/Bearer"
         self._security_token = USERNAME_TOKEN_TEMPLATE % self.__dict__
         self._delegatable = str(delegatable).lower()
         self._renewable = str(renewable).lower()
         return _canonicalize(REQUEST_TEMPLATE % self.__dict__)
 
     def construct_bearer_token_request_with_binary_token(
             self, delegatable=False, renewable=False):
-        '''
+        """
         Constructs the actual Bearer token SOAP request using the binary exchange GSS/SSPI token.
 
         @type  delegatable: C{boolean}
         @param delegatable: Whether the generated token is delegatable or not
         @type    renewable: C{boolean}
         @param   renewable: Whether the generated token is renewable or not
                             The default value is False
         @rtype:  C{str}
         @return: Bearer token SOAP request.
-        '''
+        """
         self._key_type = "http://docs.oasis-open.org/ws-sx/ws-trust/200512/Bearer"
         self._delegatable = str(delegatable).lower()
         self._renewable = str(renewable).lower()
         return _canonicalize(GSS_REQUEST_TEMPLATE % self.__dict__)
 
     def construct_hok_request(self,
                               delegatable=False,
                               act_as_token=None,
                               renewable=False):
-        '''
+        """
         Constructs the actual HoK token SOAP request.
 
         @type   delegatable: C{boolean}
         @param  delegatable: Whether the generated token is delegatable or not
         @type  act_as_token: C{str}
         @param act_as_token: Bearer/Hok token which is delegatable
         @type    renewable: C{boolean}
         @param   renewable: Whether the generated token is renewable or not
                             The default value is False
         @rtype: C{str}
         @return: HoK token SOAP request in Unicode.
-        '''
+        """
         self._binary_security_token = base64.b64encode(
             _extract_certificate(self._public_key)).decode(UTF_8)
         self._use_key = USE_KEY_TEMPLATE % self.__dict__
         self._security_token = BINARY_SECURITY_TOKEN_TEMPLATE % self.__dict__
         self._key_type = "http://docs.oasis-open.org/ws-sx/ws-trust/200512/PublicKey"
         self._renewable = str(renewable).lower()
         self._delegatable = str(delegatable).lower()
@@ -847,19 +848,19 @@
         """
         self._delegatable = str(delegatable).lower()
         self._renewable = str(renewable).lower()
         self._key_type = "http://docs.oasis-open.org/ws-sx/ws-trust/200512/PublicKey"
         return _canonicalize(REQUEST_TEMPLATE_TOKEN_BY_TOKEN) % self.__dict__
 
     def sign_request(self):
-        '''
+        """
         Calculates the signature to the header of the SOAP request which can be
         used by the STS to verify that the SOAP message originated from a
         trusted service.
-        '''
+        """
         base_xml = etree.fromstring(self._xml_text)
         request_tree = _extract_element(
             base_xml, 'Body',
             {'SOAP-ENV': "http://schemas.xmlsoap.org/soap/envelope/"})
         request = _canonicalize(etree.tostring(request_tree))
         request_tree = _extract_element(
             base_xml, 'Timestamp', {
@@ -875,17 +876,17 @@
         self._signature_value = _sign(self._private_key,
                                       self._signed_info).decode(UTF_8)
         self._signature_text = _canonicalize(SIGNATURE_TEMPLATE %
                                              self.__dict__)
         self.embed_signature()
 
     def embed_signature(self):
-        '''
+        """
         Embeds the signature in to the header of the SOAP request.
-        '''
+        """
         self._xml = etree.fromstring(self._xml_text)
         security = _extract_element(
             self._xml, 'Security', {
                 'ns6':
                 "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd"
             })
         self._signature = etree.fromstring(self._signature_text)
@@ -893,15 +894,15 @@
         self._xml_text = etree.tostring(self._xml).decode(UTF_8)
 
 
 def add_saml_context(serialized_request,
                      saml_token,
                      private_key_file,
                      request_duration=60):
-    '''
+    """
     A helper method provided to sign the outgoing LoginByToken requests with the
     HoK token.
 
     @type       serialized_request: C{str}
     @param      serialized_request: SOAP request which needs to be signed.
     @type               saml_token: C{str}
     @param              saml_token: SAML assertion that will be added to the SOAP
@@ -912,15 +913,15 @@
     @type         request_duration: C{long}
     @param request_duration: The duration for which the request is valid. If
                                  the STS receives this request after this
                                  duration, it is assumed to have expired. The
                                  duration is in seconds and the default is 60s.
     @rtype: C{str}
     @return: signed SOAP request in Unicode.
-    '''
+    """
     with open(private_key_file) as fp:
         private_key = fp.read()
     xml = etree.fromstring(serialized_request)
     value_map = {}
     value_map['_request_id'] = _generate_id()
     request_body = _extract_element(
         xml, 'Body', {'soapenv': "http://schemas.xmlsoap.org/soap/envelope/"})
@@ -957,33 +958,33 @@
     signature = etree.fromstring(
         _canonicalize(REQUEST_SIGNATURE_TEMPLATE % value_map))
     security.append(signature)
     return etree.tostring(xml, pretty_print=False).decode(UTF_8)
 
 
 def _generate_id():
-    '''
+    """
     An internal helper method to generate UUIDs.
 
     @rtype: C{str}
     @return: UUID
-    '''
+    """
     return "_%s" % uuid4()
 
 
 def _load_private_key(der_key):
-    '''
+    """
     An internal helper to load private key.
 
     @type  der_key: C{str}
     @param der_key: The private key, in DER format.
 
     @rtype: crypto.privatekey
     @return: Loaded private key.
-    '''
+    """
 
     # OpenSSL 0.9.8 does not handle correctly PKCS8 keys passed in DER format
     # (only PKCS1 keys are understood in DER format).
 
     # Unencrypted PKCS8, or PKCS1 for OpenSSL 1.0.1, PKCS1 for OpenSSL 0.9.8
     try:
         return crypto.load_privatekey(crypto.FILETYPE_ASN1, der_key, b'')
@@ -999,110 +1000,110 @@
         except (crypto.Error, ValueError):
             pass
     # We could try 'ENCRYPTED PRIVATE KEY' here - but we do not know passphrase.
     raise
 
 
 def _sign(private_key, data, digest=SHA256):
-    '''
+    """
     An internal helper method to sign the 'data' with the 'private_key'.
 
     @type  private_key: C{str}
     @param private_key: The private key used to sign the 'data', in one of
                         supported formats.
     @type         data: C{str}
     @param        data: The data that needs to be signed.
     @type       digest: C{str}
     @param      digest: Digest is a str naming a supported message digest type,
                         for example 'sha256'.
 
     @rtype: C{str}
     @return: Signed string.
-    '''
+    """
     # Convert private key in arbitrary format into DER (DER is binary format
     # so we get rid of \n / \r\n differences, and line breaks in PEM).
     pkey = _load_private_key(_extract_certificate(private_key))
     return base64.b64encode(crypto.sign(pkey, data.encode(UTF_8), digest))
 
 
 def _canonicalize(xml_string):
-    '''
+    """
     Given an xml string, canonicalize the string per
     U{http://www.w3.org/2001/10/xml-exc-c14n#}
 
     @type  xml_string: C{str}
     @param xml_string: The XML string that needs to be canonicalized.
 
     @rtype: C{str}
     @return: Canonicalized string in Unicode.
-    '''
+    """
     # TODO: keep the parser between _canonicalize() invocations.
     parser = etree.XMLParser(remove_blank_text=True, resolve_entities=False)
     tree = etree.fromstring(xml_string, parser=parser).getroottree()
     string = BytesIO()
     tree.write_c14n(string, exclusive=True, with_comments=False)
     return string.getvalue().decode(UTF_8)
 
 
 def _extract_element(xml, element_name, namespace):
-    '''
+    """
     An internal method provided to extract an element from the given XML.
 
     @type           xml: C{str}
     @param          xml: The XML string from which the element will be extracted.
     @type  element_name: C{str}
     @param element_name: The element that needs to be extracted from the XML.
     @type     namespace: dict
     @param    namespace: A dict containing the namespace of the element to be
                          extracted.
 
     @rtype: etree element.
     @return: The extracted element.
-    '''
+    """
     assert (len(namespace) == 1)
     result = xml.xpath("//{0}:{1}".format(list(namespace.keys())[0], element_name),
                        namespaces=namespace)
     if result:
         return result[0]
     else:
         raise KeyError("%s does not seem to be present in the XML." %
                        element_name)
 
 
 def _make_hash(data):
-    '''
+    """
     An internal method to calculate the sha256 hash of the data.
 
     @type  data: C{str}
     @param data: The data for which the hash needs to be calculated.
 
     @rtype: C{str}
     @return: Base64 encoded sha256 hash.
-    '''
+    """
     return base64.b64encode(hashlib.sha256(data).digest())  # pylint: disable=E1101
 
 
 def _make_hash_sha512(data):
-    '''
+    """
     An internal method to calculate the sha512 hash of the data.
 
     @type  data:      C{str}
     @param data:      The data for which the hash needs to be calculated.
 
     @rtype: C{str}
     @return: Base64 encoded sha512 hash.
-    '''
+    """
     return base64.b64encode(hashlib.sha512(data).digest())  # pylint: disable=E1101
 
 
 TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%f"
 
-#The SAML token requests usually contain an xmldsig which guarantees that the
-#message hasn't been tampered with during the transport. The following
-#SIGNED_INFO_TEMPLATE is used to construct the signedinfo part of the signature.
+# The SAML token requests usually contain an xmldsig which guarantees that the
+# message hasn't been tampered with during the transport. The following
+# SIGNED_INFO_TEMPLATE is used to construct the signedinfo part of the signature.
 SIGNED_INFO_TEMPLATE = """\
 <ds:SignedInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
 <ds:CanonicalizationMethod Algorithm="http://www.w3.org/2001/10/xml-exc-c14n#"/>
 <ds:SignatureMethod Algorithm="http://www.w3.org/2001/04/xmldsig-more#rsa-%(_algorithm)s"/>
 <ds:Reference URI="#%(_request_id)s">
 <ds:Transforms>
 <ds:Transform Algorithm="http://www.w3.org/2001/10/xml-exc-c14n#"/>
@@ -1116,47 +1117,47 @@
 </ds:Transforms>
 <ds:DigestMethod Algorithm="http://www.w3.org/2001/04/xmlenc#%(_algorithm)s"/>
 <ds:DigestValue>%(_timestamp_digest)s</ds:DigestValue>
 </ds:Reference>
 </ds:SignedInfo>
 """
 
-#The following template is used as the container for signed info in WS-Trust
-#SOAP requests signed with the SAML token. It contains the digest of the
-#signed info, signed with the private key of the Solution user and contains a
-#reference to the actual SAML token which contains the solution user's public
-#key.
+# The following template is used as the container for signed info in WS-Trust
+# SOAP requests signed with the SAML token. It contains the digest of the
+# signed info, signed with the private key of the Solution user and contains a
+# reference to the actual SAML token which contains the solution user's public
+# key.
 REQUEST_SIGNATURE_TEMPLATE = """\
 <ds:Signature xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
 %(_signed_info)s
 <ds:SignatureValue>%(_signature_value)s</ds:SignatureValue>
 <ds:KeyInfo>
 <ns2:SecurityTokenReference xmlns:ns2="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd"
                             xmlns:wsse11="http://docs.oasis-open.org/wss/oasis-wss-wssecurity-secext-1.1.xsd"
                             wsse11:TokenType="http://docs.oasis-open.org/wss/oasis-wss-saml-token-profile-1.1#SAMLV2.0">
 <ns2:KeyIdentifier ValueType="http://docs.oasis-open.org/wss/oasis-wss-saml-token-profile-1.1#SAMLID">%(samlId)s</ns2:KeyIdentifier>
 </ns2:SecurityTokenReference>
 </ds:KeyInfo>
 </ds:Signature>"""
 
-#The following template is used as a signed info container for the actual SAML
-#token requests requesting a SAML token. It contains the digest of the signed
-#info signed with the Service User's private key.
+# The following template is used as a signed info container for the actual SAML
+# token requests requesting a SAML token. It contains the digest of the signed
+# info signed with the Service User's private key.
 SIGNATURE_TEMPLATE = """\
 <ds:Signature xmlns:ds="http://www.w3.org/2000/09/xmldsig#" Id="%(_signature_id)s">
 %(_signed_info)s
 <ds:SignatureValue>%(_signature_value)s</ds:SignatureValue>
 <ds:KeyInfo>
 <ns2:SecurityTokenReference xmlns:ns2="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd">
 <ns2:Reference URI="#%(_security_token_id)s" ValueType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-x509-token-profile-1.0#X509v3"/>
 </ns2:SecurityTokenReference>
 </ds:KeyInfo>
 </ds:Signature>"""
 
-#The following template is used to construct the token requests to the STS.
+# The following template is used to construct the token requests to the STS.
 REQUEST_TEMPLATE = """\
 <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
 <SOAP-ENV:Header>
 <ns6:Security xmlns="http://docs.oasis-open.org/ws-sx/ws-trust/200512"
               xmlns:ns2="http://www.w3.org/2005/08/addressing"
               xmlns:ns3="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd"
               xmlns:ns6="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd">
@@ -1178,15 +1179,15 @@
 <Renewing Allow="%(_renewable)s" OK="%(_renewable)s"/>
 <Delegatable>%(_delegatable)s</Delegatable>
 <KeyType>%(_key_type)s</KeyType>
 <SignatureAlgorithm>http://www.w3.org/2001/04/xmldsig-more#rsa-sha256</SignatureAlgorithm>%(_use_key)s</RequestSecurityToken>
 </SOAP-ENV:Body>
 </SOAP-ENV:Envelope>"""
 
-#The following template is used to construct the token-by-token requests to the STS.
+# The following template is used to construct the token-by-token requests to the STS.
 REQUEST_TEMPLATE_TOKEN_BY_TOKEN = """\
 <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
 <SOAP-ENV:Header>
 <ns5:Security xmlns="http://docs.oasis-open.org/ws-sx/ws-trust/200512"
               xmlns:ns3="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd"
               xmlns:ns5="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd">
 %(_hok_token)s
@@ -1235,37 +1236,37 @@
 <KeyType>%(_key_type)s</KeyType>
 <SignatureAlgorithm>http://www.w3.org/2001/04/xmldsig-more#rsa-sha256</SignatureAlgorithm>
 %(_binary_exchange)s
 %(_use_key)s</RequestSecurityToken>
 </SOAP-ENV:Body>
 </SOAP-ENV:Envelope>"""
 
-#Template container for the service user's public key when requesting an HoK
-#token.
+# Template container for the service user's public key when requesting an HoK
+# token.
 BINARY_SECURITY_TOKEN_TEMPLATE = """\
 <ns2:BinarySecurityToken xmlns:ns1="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd"
                          xmlns:ns2="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd"
                          EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary"
                          ValueType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-x509-token-profile-1.0#X509v3"
                          ns1:Id="%(_security_token_id)s">%(_binary_security_token)s</ns2:BinarySecurityToken>
 """
 
-#Template container for user's credentials when requesting a bearer token.
+# Template container for user's credentials when requesting a bearer token.
 USERNAME_TOKEN_TEMPLATE = """\
 <ns2:UsernameToken xmlns:ns2="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd">
 <ns2:Username>%(_username)s</ns2:Username>
 <ns2:Password>%(_password)s</ns2:Password>
 </ns2:UsernameToken>"""
 
-#Template containing the anchor to the signature.
+# Template containing the anchor to the signature.
 USE_KEY_TEMPLATE = """\
 <UseKey Sig="%(_signature_id)s"/>"""
 
-#The follwoing template is used to create a timestamp for the various messages.
-#The timestamp is used to indicate the duration of the request itself.
+# The follwoing template is used to create a timestamp for the various messages.
+# The timestamp is used to indicate the duration of the request itself.
 TIMESTAMP_TEMPLATE = """\
 <ns3:Timestamp xmlns:ns3="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd" ns3:Id="%(_timestamp_id)s">
 <ns3:Created>%(_created)s</ns3:Created><ns3:Expires>%(_request_expires)s</ns3:Expires></ns3:Timestamp>"""
 
 BINARY_EXCHANGE_TEMPLATE = """\
 <BinaryExchange EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary" ValueType="http://schemas.xmlsoap.org/ws/2005/02/trust/spnego">%s</BinaryExchange>"""
```

### Comparing `pyvmomi-8.0.1.0.1/pyVim/task.py` & `pyvmomi-8.0.1.0.2/pyVim/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #############################################################
 # Copyright (c) 2005-2023 VMware, Inc.
 #############################################################
 
-## @file task.py
-## @brief Task functions
-##
-## This module provies synchronization of client/server operations
-## since many VIM operations return 'tasks' which can have
-## varying completion times.
+# @file task.py
+# @brief Task functions
+#
+# This module provies synchronization of client/server operations
+# since many VIM operations return 'tasks' which can have
+# varying completion times.
 """
 Task functions
 
 This module provies synchronization of client/server operations since
 many VIM operations return 'tasks' which can have varying completion
 times.
 """
@@ -19,22 +19,22 @@
 __author__ = 'VMware, Inc'
 
 from pyVmomi import vmodl, vim
 
 import time
 
 
-##
-## @brief Exception class to represent when task is blocked (e.g.:
-## waiting for an answer to a question.
-##
+#
+# @brief Exception class to represent when task is blocked (e.g.:
+# waiting for an answer to a question.
+#
 class TaskBlocked(Exception):
     """
-    Exception class to represent when task is blocked (e.g.: waiting
-    for an answer to a question.
+    Exception class to represent when task is blocked
+    e.g.: waiting for an answer to a question
     """
     pass
 
 
 #
 # TaskUpdates
 #     verbose information about task progress
@@ -55,35 +55,35 @@
     global globalTaskUpdate
     if verbose:
         globalTaskUpdate = TaskUpdatesVerbose
     else:
         globalTaskUpdate = None
 
 
-##
-## @param raiseOnError [in] Any exception thrown is thrown up to the caller if
-## raiseOnError is set to true
-## @param si [in] ServiceInstance to use. If set to None, use the default one.
-## @param pc [in] property collector to use else retrieve one from cache
-## @param maxWaitTime [in] The maximum amount of time the task is allowed to
-## run. Throws an exception if raiseOnError is True.
-## @param onProgressUpdate [in] callable to call with task progress updates.
-##    For example:
-##
-##    def OnTaskProgressUpdate(task, percentDone):
-##       sys.stderr.write('# Task {}: {:.0f}% complete ...\n'
-##                        .format(task, percentDone))
-##
-## Given a task object and a service instance, wait for the task completion
-##
-## @return state as either "success" or "error". To look at any errors, the
-## user should reexamine the task object.
-##
-## NOTE: This is a blocking call.
-##
+#
+# @param raiseOnError [in] Any exception thrown is thrown up to the caller if
+# raiseOnError is set to true
+# @param si [in] ServiceInstance to use. If set to None, use the default one.
+# @param pc [in] property collector to use else retrieve one from cache
+# @param maxWaitTime [in] The maximum amount of time the task is allowed to
+# run. Throws an exception if raiseOnError is True.
+# @param onProgressUpdate [in] callable to call with task progress updates.
+#    For example:
+#
+#    def OnTaskProgressUpdate(task, percentDone):
+#       sys.stderr.write('# Task {}: {:.0f}% complete ...\n'
+#                        .format(task, percentDone))
+#
+# Given a task object and a service instance, wait for the task completion
+#
+# @return state as either "success" or "error". To look at any errors, the
+# user should reexamine the task object.
+#
+# NOTE: This is a blocking call.
+#
 def WaitForTask(task,
                 raiseOnError=True,
                 si=None,
                 pc=None,
                 maxWaitTime=None,
                 onProgressUpdate=None,
                 log=None,
@@ -100,15 +100,15 @@
     @type  pc                : ManagedObjectReference to a PropertyCollector.
     @param pc                : Property collector to use. If None, get it from
                                 the ServiceInstance.
     @type  maxWaitTime       : numeric value
     @param maxWaitTime       : The maximum amount of time the task is allowed to
                                 run. Throws an exception if raiseOnError is True.
     @type  onProgressUpdate  : callable
-    @param onProgressUpdate  : Callable to call with task progress updates.
+    @param onProgressUpdate  : The callable to call with task progress updates.
     @type  log               : Optional logger.
     @param log               : Logging.
     @type  getAllUpdates     : Optional bool value. Default is False.
     @param getAllUpdates     : Get all updates for the task.
 
         For example::
 
@@ -142,15 +142,15 @@
                 if raiseOnError is True:
                     raise Exception(err)
                 break
         except vmodl.fault.ManagedObjectNotFound as e:
             print("Task object has been deleted: %s" % e.obj)
             break
 
-    filter.Destroy()
+    DestroyFilter(filter)
 
     info = task.info
     if state == "error":
         progressUpdater.Update("error: %s" % info.error)
         if raiseOnError:
             raise info.error
         else:
@@ -163,15 +163,15 @@
     else:  # state = running
         _LogMsg(log, "Task reports as still running: %s" % info)
         progressUpdater.UpdateIfNeeded()
 
     return state
 
 
-## Wait for multiple tasks to complete
+# Wait for multiple tasks to complete
 #  See WaitForTask for detail
 #
 #  Difference: WaitForTasks won't return the state of tasks. User can check
 #  tasks state directly with task.info.state
 #
 #  TODO: Did not check for question pending
 def WaitForTasks(tasks,
@@ -244,15 +244,15 @@
                         else:
                             if onProgressUpdate:
                                 progressUpdater.UpdateIfNeeded()
             # Move to next version
             version = update.version
     finally:
         if filter:
-            filter.Destroy()
+            DestroyFilter(filter)
     return
 
 
 def GetTaskStatus(task, version, pc):
     update = pc.WaitForUpdates(version)
     info = task.info
     state = info.state
@@ -289,14 +289,21 @@
     filterspec.objectSet = objspecs
     filterspec.propSet = [propspec]
 
     # Create the filter
     return pc.CreateFilter(filterspec, True)
 
 
+def DestroyFilter(filter):
+    try:
+        filter.Destroy()
+    except vmodl.fault.ManagedObjectNotFound:
+        pass
+
+
 def CheckForQuestionPending(info):
     """ Check to see if VM needs to ask a question, throw exception """
 
     vm = info.entity
     if vm is not None and isinstance(vm, vim.VirtualMachine):
         qst = vm.runtime.question
         if qst is not None:
@@ -307,18 +314,18 @@
     """Helper logging a message with logger or print depending on the flag."""
     if log:
         log(message)
     else:
         print(message)
 
 
-##
-## @brief Class that keeps track of task percentage complete and calls
-## a provided callback when it changes.
-##
+#
+# @brief Class that keeps track of task percentage complete and calls
+# a provided callback when it changes.
+#
 class ProgressUpdater(object):
     """
     Class that keeps track of task percentage complete and calls a
     provided callback when it changes.
     """
     def __init__(self, task, onProgressUpdate, getAllUpdates=False):
         self.task = task
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/Cache.py` & `pyvmomi-8.0.1.0.2/pyVmomi/Cache.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/Differ.py` & `pyvmomi-8.0.1.0.2/pyVmomi/Differ.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/Feature.py` & `pyvmomi-8.0.1.0.2/pyVmomi/Feature.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/Iso8601.py` & `pyvmomi-8.0.1.0.2/pyVmomi/Iso8601.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/Security.py` & `pyvmomi-8.0.1.0.2/pyVmomi/Security.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/SoapAdapter.py` & `pyvmomi-8.0.1.0.2/pyVmomi/SoapAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import socket
 import subprocess
 import sys
 import threading
 import time
 from datetime import datetime
 from xml.parsers.expat import ExpatError, ParserCreate
-# For Visor, space is very limited. Import xml.sax pull in too many junk.
+# For Visor, space is very limited. Import xml.sax pull in too much junk.
 # Define our own xml escape instead
 # from xml.sax.saxutils import escape
 
 import six
 from six import PY3
 from six.moves import StringIO, zip
 from six.moves.urllib.parse import urlparse
@@ -187,15 +187,15 @@
 # @param val the value to serialize
 # @param info the field
 # @param version the version
 # @param nsMap a dict of xml ns -> prefix
 # @return the serialized object as bytes
 # @param encoding Deprecated this is not used during serialization since we
 #        always use utf-8 to encode a request message. We didn't remove the
-#        parameter so it is still compatible with clients that are still
+#        parameter, so it is still compatible with clients that are still
 #        using it.
 def Serialize(val,
               info=None,
               version=None,
               nsMap=None,
               encoding=None,
               hidepasswd=False):
@@ -301,15 +301,15 @@
     # Serializer constructor
     #
     # @param writer File writer
     # @param version the version
     # @param nsMap a dict of xml ns -> prefix
     # @param encoding Deprecated this is not used during serialization since we
     #                 always use utf-8 to encode a request message. We didn't
-    #                 remove the parameter so it is still compatible with
+    #                 remove the parameter, so it is still compatible with
     #                 clients that are still using it.
     def __init__(self, writer, version, nsMap, encoding=None):
         """ Constructor """
         self.writer = writer
         self.version = version
         self.nsMap = nsMap and nsMap or {}
         for ns, prefix in six.iteritems(self.nsMap):
@@ -562,15 +562,15 @@
                 # encoding than UTF-8, you cannot serialize it again once more.
                 # That's feature, nota bug.
                 val = val.decode('UTF-8')
             result = XmlEscape(val)
             self.writer.write(u'<{0}{1}>{2}</{0}>'.format(
                 info.name, attr, result))
 
-    # Serialize a a data object (internal)
+    # Serialize a data object (internal)
     #
     # @param val the value to serialize
     # @param info the field
     # @param attr attributes to serialized in the outermost elementt
     # @param currDefNS the current default namespace
     def _SerializeDataObject(self, val, info, attr, currDefNS):
         if info.flags & F_LINK:
@@ -601,15 +601,15 @@
 
 
 # Deserialize an object from a file or string
 #
 # This function will deserialize one top-level XML node.
 # @param data the data to deserialize (a file object or string)
 # @param resultType expected result type
-# @param stub stub for moRef deserialization
+# @param stub the stub for moRef deserialization
 # @return the deserialized object
 def Deserialize(data, resultType=object, stub=None):
     parser = ParserCreate(namespace_separator=NS_SEP)
     ds = SoapDeserializer(stub)
     ds.Deserialize(parser, resultType)
     # Many existing tests pass in str directly in python2 for testing purpose.
     # But in python3 the input become unicode and the handling will fall into
@@ -668,30 +668,30 @@
         self.nsMap[prefix].pop()
 
 
 # SOAP -> Python Deserializer
 class SoapDeserializer(ExpatDeserializerNSHandlers):
     # Constructor
     #
-    # @param self self
-    # @param stub Stub adapter to use for deserializing moRefs
+    # @param self The object pointer
+    # @param stub The stub adapter to use for deserializing moRefs
     def __init__(self, stub=None, version=None):
         ExpatDeserializerNSHandlers.__init__(self)
         self.stub = stub
         if version:
             self.version = version
         elif self.stub:
             self.version = self.stub.version
         else:
             self.version = None
         self.result = None
 
     # Deserialize a SOAP object
     #
-    # @param self self
+    # @param self The object pointer
     # @param parser an expat parser
     # @param resultType the static type of the result
     # @param isFault true if the response is a fault response
     # @param nsMap a dict of prefix -> [xml ns stack]
     # @return the deserialized object
     def Deserialize(self,
                     parser,
@@ -908,25 +908,25 @@
         self.data += data
 
 
 # SOAP Response Deserializer class
 class SoapResponseDeserializer(ExpatDeserializerNSHandlers):
     # Constructor
     #
-    # @param self self
-    # @param stub Stub adapter to use for deserializing moRefs
+    # @param self The object pointer
+    # @param stub The stub adapter to use for deserializing moRefs
     def __init__(self, stub):
         ExpatDeserializerNSHandlers.__init__(self)
         self.stub = stub
         self.deser = SoapDeserializer(stub)
         self.soapFaultTag = XMLNS_SOAPENV + NS_SEP + "Fault"
 
     # Deserialize a SOAP response
     #
-    # @param self self
+    # @param self The object pointer
     # @param response the response (a file object or a string)
     # @param resultType expected result type
     # @param nsMap a dict of prefix -> [xml ns stack]
     # @return the deserialized object
     def Deserialize(self, response, resultType, nsMap=None):
         self.resultType = resultType
         self.stack = []
@@ -990,15 +990,15 @@
         StubAdapterAccessorMixin.__init__(self)
         self.ComputeVersionInfo(version)
 
     # Compute the version information for the specified namespace
     #
     # @param ns the namespace
     def ComputeVersionInfo(self, version):
-        # Make sure we do NOT fallback to an older version
+        # Make sure we do NOT fall back to an older version
         if hasattr(self, 'version') and IsChildVersion(self.version, version):
             # print("WARNING: stub degrading: " +
             #       self.version + " -> " + version)
             return
 
         versionNS = GetVersionNamespace(version)
         if versionNS.find("/") >= 0:
@@ -1091,18 +1091,18 @@
         # as HTTPConnection.connect, which puts the socket in self.sock.
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.connect(self.path)
         self.sock = sock
 
 
 def _VerifyThumbprint(thumbprint, connection):
-    '''If there is a thumbprint, connect to the server and verify that the
+    """If there is a thumbprint, connect to the server and verify that the
     SSL certificate matches the given thumbprint.  An exception is thrown
     if there is a mismatch.
-    '''
+    """
     if thumbprint and isinstance(connection,
                                  six.moves.http_client.HTTPSConnection):
         if not connection.sock:
             connection.connect()
         derCert = connection.sock.getpeercert(True)
         VerifyCertThumbprint(derCert, thumbprint)
 
@@ -1163,16 +1163,18 @@
         #      # pemcert = ssl.DER_cert_to_PEM_cert(dercert)
 
 
 # Stand-in for the HTTPSConnection class that will connect to a proxy and
 # issue a CONNECT command to start an SSL tunnel.
 class SSLTunnelConnection(object):
     # @param proxyPath The path to pass to the CONNECT command.
-    def __init__(self, proxyPath):
+    # @param customHeaders Dictionary with custom HTTP headers.
+    def __init__(self, proxyPath, customHeaders=None):
         self.proxyPath = proxyPath
+        self.customHeaders = customHeaders if customHeaders else {}
 
     # Connects to a proxy server and initiates a tunnel to the destination
     # specified by proxyPath. If successful, a new HTTPSConnection is returned.
     # For Python Version < 2.7.9. cert_reqs=CERT_OPTIONAL to verify
     # server certificate
     #
     # @param path The destination URL path.
@@ -1224,15 +1226,15 @@
                 retval._context.check_hostname = False
             if 'ca_certs' in kwargs and kwargs['ca_certs']:
                 retval._context.load_verify_locations(kwargs['ca_certs'])
             # Call set_tunnel when proxyPath is a stand alone proxy host.
             proxyHost = splitport(self.proxyPath)[0]
             if (_CheckIPv4(proxyHost) or _CheckIPv6(proxyHost)
                     or _CheckHostname(proxyHost)):
-                retval.set_tunnel(self.proxyPath)
+                retval.set_tunnel(self.proxyPath, headers=self.customHeaders)
             # Call wrap_socket if ProxyPath is VC inbuilt proxyPath
             # ex: /sdkTunnel
             else:
                 retval.sock = retval._context.wrap_socket(sock=tunnel.sock,
                                                           server_hostname=host)
         else:
             if host in ['localhost', '127.0.0.1', '::1']:
@@ -1244,27 +1246,29 @@
         return retval
 
 
 # Stand-in for the HTTPSConnection class that will connect to a regular HTTP
 # proxy.
 class HTTPProxyConnection(object):
     # @param proxyPath The path to pass to the CONNECT command.
-    def __init__(self, proxyPath):
+    # @param customHeaders Dictionary with custom HTTP headers.
+    def __init__(self, proxyPath, customHeaders=None):
         self.proxyPath = proxyPath
+        self.customHeaders = customHeaders if customHeaders else {}
 
     # Connects to an HTTP proxy server and initiates a tunnel to the destination
     # specified by proxyPath. If successful, a new HTTPSConnection is returned.
     #
     # @param path The destination URL path.
     # @param args Arguments are ignored
     # @param kwargs Arguments for HTTPSConnection
     def __call__(self, path, **kwargs):
         httpsConnArgs = {k: kwargs[k] for k in kwargs if k not in SOAP_ADAPTER_ARGS}
         conn = six.moves.http_client.HTTPSConnection(path, **httpsConnArgs)
-        conn.set_tunnel(self.proxyPath)
+        conn.set_tunnel(self.proxyPath, headers=self.customHeaders)
         return conn
 
 
 class GzipReader:
     GZIP = 1
     DEFLATE = 2
 
@@ -1320,15 +1324,15 @@
                 break
 
         if bufSize <= bytes or bytes == -1:
             leftoverBytes = 0
             leftoverChunks = []
         else:
             leftoverBytes = bufSize - bytes
-            # Adjust last chunk to hold only the left over bytes
+            # Adjust last chunk to hold only the leftover bytes
             lastChunk = chunks.pop()
             chunks.append(lastChunk[:-leftoverBytes])
             leftoverChunks = [lastChunk[-leftoverBytes:]]
 
         self.chunks = leftoverChunks
         self.bufSize = leftoverBytes
 
@@ -1338,15 +1342,15 @@
 
 # SOAP stub adapter object
 class SoapStubAdapter(SoapStubAdapterBase):
     # Constructor
     #
     # The endpoint can be specified individually as either a host/port
     # combination, or with a URL (using a url= keyword).
-    # @param self self
+    # @param self The object pointer
     # @param host host
     # @param port port (pass negative port number for no SSL)
     # @param **** Deprecated. Please use version instead **** ns API namespace
     # @param path location of SOAP VMOMI service
     # @param url URL (overrides host, port, path if set)
     # @param sock unix domain socket path (overrides host, port, url if set)
     # @param poolSize size of HTTP connection pool
@@ -1437,18 +1441,18 @@
                 raise Exception(
                     "Invalid SHA thumbprint -- {0}".format(thumbprint))
         else:
             self.thumbprint = None
 
         self.is_tunnel = False
         if sslProxyPath:
-            self.scheme = SSLTunnelConnection(sslProxyPath)
+            self.scheme = SSLTunnelConnection(sslProxyPath, customHeaders)
             self.is_tunnel = True
         elif httpProxyHost:
-            self.scheme = HTTPProxyConnection(self.host)
+            self.scheme = HTTPProxyConnection(self.host, customHeaders)
             self.is_tunnel = True
 
             # Is httpProxyHost IPv6
             if httpProxyHost.find(':') != -1 and httpProxyHost[0] != '[':
                 httpProxyHost = '[' + httpProxyHost + ']'
 
             # Swap the actual host with the proxy.
@@ -1476,27 +1480,27 @@
         self.samlToken = samlToken
         self.requestContext = requestContext
         self.requestModifierList = []
         self._acceptCompressedResponses = acceptCompressedResponses
 
     # Context modifier used to modify the SOAP request.
     # @param func The func that takes in the serialized message and
-    #   modifies the the request. The func is appended to the
+    #   modifies the request. The func is appended to the
     #   requestModifierList and then popped after the request is modified.
     @contextlib.contextmanager
     def requestModifier(self, func):
         self.requestModifierList.append(func)
         try:
             yield
         finally:
             self.requestModifierList.pop()
 
     # Invoke a managed method
     #
-    # @param self self
+    # @param self The object pointer
     # @param mo the 'this'
     # @param info method info
     # @param args arguments
     # @param outerStub If not-None, this should be a reference to the wrapping
     #   stub adapter.  Any ManagedObject references returned from this method
     #   will have outerStub in their _stub field.  Note that this also changes
     #   the return type to a tuple containing the HTTP status and the
@@ -1525,15 +1529,15 @@
         for modifier in self.requestModifierList:
             req = modifier(req)
         conn = self.GetConnection()
         try:
             conn.request('POST', self.path, req, headers)
             resp = conn.getresponse()
         except (socket.error, six.moves.http_client.HTTPException):
-            # The server is probably sick, drop all of the cached connections.
+            # The server is probably sick, drop all the cached connections.
             self.DropConnections()
             raise
         cookie = resp.getheader('Set-Cookie')
         if cookie is None:
             # try lower-case header for backwards compat. with old vSphere
             cookie = resp.getheader('set-cookie')
         status = resp.status
@@ -1550,15 +1554,15 @@
                 elif encoding == 'deflate':
                     fd = GzipReader(resp, encoding=GzipReader.DEFLATE)
                 obj = SoapResponseDeserializer(outerStub).Deserialize(
                     fd, info.result)
             # TODO Add specific exception(s)
             except:  # noqa: E722
                 conn.close()
-                # The server might be sick, drop all of the cached connections.
+                # The server might be sick, drop all the cached connections.
                 self.DropConnections()
                 raise
             else:
                 resp.read()
                 self.ReturnConnection(conn)
             if outerStub != self:
                 return (status, obj)
@@ -1595,15 +1599,15 @@
                     idleConnections = self.pool[i:]
                     self.pool = self.pool[:i]
                     break
 
             for conn, _ in idleConnections:
                 conn.close()
 
-    # Get a HTTP connection from the pool
+    # Get an HTTP connection from the pool
     def GetConnection(self):
         self.lock.acquire()
         self._CloseIdleConnections()
         if self.pool:
             result, _ = self.pool.pop(0)
             self.lock.release()
         else:
@@ -1619,15 +1623,15 @@
         self.lock.acquire()
         oldConnections = self.pool
         self.pool = []
         self.lock.release()
         for conn, _ in oldConnections:
             conn.close()
 
-    # Return a HTTP connection to the pool
+    # Return an HTTP connection to the pool
     def ReturnConnection(self, conn):
         self.lock.acquire()
         self._CloseIdleConnections()
         # In case of ssl tunneling, only add the conn if the conn has
         # not been closed
         if len(self.pool) < self.poolSize and (not self.is_tunnel
                                                or conn.sock):
@@ -1656,19 +1660,19 @@
     headerEnd += len(HEADER_SECTION_END)
     headerText = httpResponse[:headerEnd]
     bodyText = httpResponse[headerEnd:]
     return (headerText, bodyText)
 
 
 class SessionOrientedStub(StubAdapterBase):
-    '''A session-oriented stub adapter that will relogin to the destination if
+    """A session-oriented stub adapter that will relogin to the destination if
     a session-oriented exception is thrown.
 
 
-    Here's an example.  First, we setup the communication substrate:
+    Here's an example.  First, we set up the communication substrate:
 
     >>> soapStub = SoapStubAdapter(host="192.168.1.2", ns="vim25/5.5")
 
     Create a SessionOrientedStub that uses the stub we just created for talking
     to the server:
 
     >>> from pyVim.connect import VimSessionOrientedStub
@@ -1678,23 +1682,23 @@
 
     Perform some privileged operations without needing to explicitly login:
 
     >>> si = Vim.ServiceInstance("ServiceInstance", sessionStub)
     >>> si.content.sessionManager.sessionList
     >>> si.content.sessionManager.Logout()
     >>> si.content.sessionManager.sessionList
-    '''
+    """
 
     STATE_UNAUTHENTICATED = 0
     STATE_AUTHENTICATED = 1
 
     SESSION_EXCEPTIONS = tuple()
 
     def __init__(self, soapStub, loginMethod, retryDelay=0.1, retryCount=4):
-        '''Construct a SessionOrientedStub.
+        """Construct a SessionOrientedStub.
 
         The stub starts off in the "unauthenticated" state, so it will
         call the loginMethod on the first invocation of a method.  If a
         communication error is encountered, the stub will wait for
         retryDelay seconds and then try to call the method again.  If
         the server throws an exception that is in the SESSION_EXCEPTIONS
         tuple, it will be caught and the stub will transition back into
@@ -1705,15 +1709,15 @@
         @param loginMethod A function that takes a single parameter,
             soapStub, and performs the necessary operations to authenticate
             with the server.
         @param retryDelay The amount of time to sleep before retrying after a
             communication error.
         @param retryCount The number of times to retry connecting to the
             server.
-        '''
+        """
         assert callable(loginMethod)
         assert retryCount >= 0
         StubAdapterBase.__init__(self, version=soapStub.version)
 
         self.lock = threading.Lock()
         self.soapStub = soapStub
         self.DropConnections = soapStub.DropConnections
@@ -1759,15 +1763,15 @@
             else:
                 # It's an exception from the method that was called,
                 # send it up.
                 raise obj
 
     # Retrieve a managed property
     #
-    # @param self self
+    # @param self The object pointer
     # @param mo managed object
     # @param info property info
     def InvokeAccessor(self, mo, info):
         # This retry logic is replicated in InvokeMethod and the two
         # copies need to be in sync
         retriesLeft = self.retryCount
         while True:
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/StubAdapterAccessorImpl.py` & `pyvmomi-8.0.1.0.2/pyVmomi/StubAdapterAccessorImpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     "PropertyPath": "string",
     "type[]": "string[]",
     "ManagedMethod[]": "string[]",
     "PropertyPath[]": "string[]"
 }
 
 
-class StubAdapterAccessorMixin:
+class StubAdapterAccessorMixin(object):
 
     # Retrieve a managed property
     #
-    # @param self self
+    # @param self The object pointer
     # @param mo managed object
     # @param info property info
     def InvokeAccessor(self, mo, info):
         prop = info.name
         param = Object(name="prop", type=str, version=self.version, flags=0)
 
         # Emulate legacy behavior for backward compatibility
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/Version.py` & `pyvmomi-8.0.1.0.2/pyVmomi/Version.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/VmomiJSONEncoder.py` & `pyvmomi-8.0.1.0.2/pyVmomi/VmomiJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/VmomiSupport.py` & `pyvmomi-8.0.1.0.2/pyVmomi/VmomiSupport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2005-2022 VMware, Inc.
+# Copyright (c) 2005-2023 VMware, Inc.
 """VMOMI support code
 
 This module contains support for VMOMI abstractions such as VMODL types,
 Versions, etc.
 """
 
 import base64
@@ -357,15 +357,15 @@
         object.__setattr__(self, "_moId", moId)
         object.__setattr__(self, "_stub", stub)
         object.__setattr__(self, "_serverGuid", serverGuid)
 
     # Invoke a managed method
     #
     # @param info method info
-    # @param self self
+    # @param self The object pointer
     # @param ... arguments
     def _InvokeMethod(info, self, *posargs, **kwargs):
         if len(posargs) > len(info.params):
             s = "s" * (len(info.params) != 1)
             raise TypeError(
                 "%s() takes at most %d argument%s (%d given)" %
                 (Capitalize(info.name), len(info.params), s, len(posargs)))
@@ -388,15 +388,15 @@
         return self._stub.InvokeMethod(self, info, args)
 
     _InvokeMethod = staticmethod(_InvokeMethod)
 
     # Invoke a managed property accessor
     #
     # @param info property info
-    # @param self self
+    # @param self The object pointer
     def _InvokeAccessor(info, self):
         return self._stub.InvokeAccessor(self, info)
 
     _InvokeAccessor = staticmethod(_InvokeAccessor)
 
     # Get the ID of a managed object
     def _GetMoId(self):
@@ -576,15 +576,15 @@
 # Class for curried function objects
 #
 # Instances of this class are curried python function objects.
 # If g = Curry(f, a1,...,an), then g(b1,...,bm) = f(a1,...,an, b1,...,bm)
 class Curry(object):
     # Constructor
     #
-    # @param self self
+    # @param self The object pointer
     # @param f the function object
     # @param args arguments to fix
     def __init__(self, f, *args):
         self.f = f
         self.args = args
 
     def __call__(self, *args, **kwargs):
@@ -599,15 +599,15 @@
         return self
 
 
 # Class for managed object methods
 class ManagedMethod(Curry):
     # Constructor
     #
-    # @param self self
+    # @param self The object pointer
     # @param info method info
     def __init__(self, info):
         Curry.__init__(self, ManagedObject._InvokeMethod, info)
         self.info = info
 
 
 # __setattr__ implementation for MethodFault object.
@@ -1973,24 +1973,24 @@
     return _threadLocalContext.__dict__.setdefault('httpCtx', dict())
 
 
 # Class that resolves links
 class LinkResolver:
     # Constructor
     #
-    # @param self self
+    # @param self The object pointer
     # @param scope DataObject to be used against for resolving links
     def __init__(self, scope):
         self.linkables = {}
         self._VisitDataObject(scope)
 
     # Visit a DataObject and add it to linkable if it is one. Also
     # visit its properties that are DataObjects
     #
-    # @param self self
+    # @param self The object pointer
     # @param obj DataObject to be visited
     def _VisitDataObject(self, obj):
         if isinstance(obj, DataObject):
             for prop in obj._GetPropertyList():
                 if issubclass(prop.type, list):
                     for dataObj in getattr(obj, prop.name):
                         if (prop.flags & F_LINKABLE):
@@ -2003,15 +2003,15 @@
                     self._VisitDataObject(dataObj)
         elif isinstance(obj, list):
             for dataObj in obj:
                 self._VisitDataObject(dataObj)
 
     # Adds a DataObject to linkable dictionary using its key
     #
-    # @param self self
+    # @param self The object pointer
     # @param obj DataObject to be added to linkable
     def _AddLinkable(self, obj):
         key = getattr(obj, "key")
         if key and key != '':
             if key in self.linkables:
                 # duplicate key present
                 raise AttributeError(key)
@@ -2019,23 +2019,23 @@
                 self.linkables[key] = obj
         else:
             # empty key
             raise AttributeError(key)
 
     # Resolves a key by looking up linkable dictionary
     #
-    # @param self self
+    # @param self The object pointer
     # @param key Key to be resolved
     def ResolveLink(self, key):
         val = self.linkables[key]
         return val
 
     # Resolves a list of keys by resolving each key
     #
-    # @param self self
+    # @param self The object pointer
     # @param keys keys to be resolved
     def ResolveLinks(self, keys):
         val = [self.linkables[k] for k in keys]
         return val
 
 
 # Resolves a link key using the object provided as its scope by creating a
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/__init__.py` & `pyvmomi-8.0.1.0.2/pyVmomi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # **********************************************************
-# Copyright (c) 2005-2022 VMware, Inc.
+# Copyright (c) 2005-2023 VMware, Inc.
 # **********************************************************
 
 import sys
 import importlib
 
 if sys.version_info < (2, 7, 9):
     sys.stderr.write("pyVmomi requires Python 2.7.9 or newer")
@@ -15,26 +15,14 @@
 # Definition precedes pyVmomi modules imports to escape circular
 # dependency error if modules import _assert_not_initialized()
 def _assert_not_initialized():
     if _initialized:
         raise RuntimeError("pyVmomi is already initialized!")
 
 
-def _import_typeinfo(typeinfo):
-    try:
-        __import__('_typeinfo_' + typeinfo, globals(), level=1)
-    except ImportError:
-        pass
-
-
-def _load_typeinfos():
-    from ._typeinfos import typeinfos
-    for typeinfo in typeinfos:
-        _import_typeinfo(typeinfo)
-
 try:
     settings = importlib.import_module('.pyVmomiSettings', 'pyVmomi')
 except ImportError:
     settings = None
 
 # set default settings
 _allowGetSet = getattr(settings, 'allowGetSet', True)
@@ -44,16 +32,16 @@
     getattr(settings, 'binaryIsBytearray', False)
 _legacyThumbprintException = \
     getattr(settings, 'legacyThumbprintException', False)
 
 
 from . import VmomiSupport  # noqa: E402
 from . import Feature  # noqa: E402
-
-_load_typeinfos()
+from ._typeinfos import load_typeinfos  # noqa: E402
+load_typeinfos()
 
 # All data object types and fault types have DynamicData as an ancestor
 # As well load it proactively.
 # Note: This should be done before importing SoapAdapter as it uses
 # some fault types
 VmomiSupport.GetVmodlType("vmodl.DynamicData")
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_core.py` & `pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_core.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_eam.py` & `pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_eam.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_pbm.py` & `pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_pbm.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_query.py` & `pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_query.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_sms.py` & `pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_sms.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_vim.py` & `pyvmomi-8.0.1.0.2/pyVmomi/_typeinfo_vim.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import List, Literal
 from enum import Enum
 from pyVmomi import eam, vim, vmodl
 from pyVmomi.VmomiSupport import ManagedObject, NoneType
-from . import fault, issue, lccm, vib
+from . import fault as fault
+from . import issue as issue
+from . import lccm as lccm
+from . import vib as vib
 
 
 class Agency(EamObject):
     @property
     def solutionId(self) -> str: ...
     @property
     def owner(self) -> str: ...
@@ -23,15 +26,15 @@
     def QueryAgent(self) -> List[Agent]: ...
     def RegisterAgentVm(self, agentVm: vim.VirtualMachine) -> Agent: ...
     def UnregisterAgentVm(self, agentVm: vim.VirtualMachine) -> NoneType: ...
     def Enable(self) -> NoneType: ...
     def Disable(self) -> NoneType: ...
     def Uninstall(self) -> NoneType: ...
     def DestroyAgency(self) -> NoneType: ...
-    def AddIssue(self, issue: issue.Issue) -> issue.Issue: ...
+    def AddIssue(self, issue: eam.issue.Issue) -> eam.issue.Issue: ...
 
 
     class ComputeResourceScope(Agency.Scope):
         @property
         def computeResource(self) -> List[vim.ComputeResource]: ...
         @computeResource.setter
         def computeResource(self, value: List[vim.ComputeResource]):
@@ -298,17 +301,17 @@
             self._esxAgentFolder = value
         @property
         def installedBulletin(self) -> List[str]: ...
         @installedBulletin.setter
         def installedBulletin(self, value: List[str]):
             self._installedBulletin = value
         @property
-        def installedVibs(self) -> List[vib.VibInfo]: ...
+        def installedVibs(self) -> List[eam.vib.VibInfo]: ...
         @installedVibs.setter
-        def installedVibs(self, value: List[vib.VibInfo]):
+        def installedVibs(self, value: List[eam.vib.VibInfo]):
             self._installedVibs = value
         @property
         def agency(self) -> Agency: ...
         @agency.setter
         def agency(self, value: Agency):
             self._agency = value
         @property
@@ -360,27 +363,27 @@
         def profileId(self, value: str):
             self._profileId = value
 
 
 class EamObject(ManagedObject):
     def Resolve(self, issueKey: List[int]) -> List[int]: ...
     def ResolveAll(self) -> NoneType: ...
-    def QueryIssue(self, issueKey: List[int]) -> List[issue.Issue]: ...
+    def QueryIssue(self, issueKey: List[int]) -> List[eam.issue.Issue]: ...
 
 
     class RuntimeInfo(vmodl.DynamicData):
         @property
         def status(self) -> str: ...
         @status.setter
         def status(self, value: str):
             self._status = value
         @property
-        def issue(self) -> List[issue.Issue]: ...
+        def issue(self) -> List[eam.issue.Issue]: ...
         @issue.setter
-        def issue(self, value: List[issue.Issue]):
+        def issue(self, value: List[eam.issue.Issue]):
             self._issue = value
         @property
         def goalState(self) -> str: ...
         @goalState.setter
         def goalState(self, value: str):
             self._goalState = value
         @property
@@ -402,15 +405,15 @@
             red = "red"
 
 
 class EsxAgentManager(EamObject):
     @property
     def agency(self) -> List[Agency]: ...
     @property
-    def issue(self) -> List[issue.Issue]: ...
+    def issue(self) -> List[eam.issue.Issue]: ...
     def QueryAgency(self) -> List[Agency]: ...
     def CreateAgency(self, agencyConfigInfo: Agency.ConfigInfo, initialGoalState: str) -> Agency: ...
     def ScanForUnknownAgentVm(self) -> NoneType: ...
     def SetMaintenanceModePolicy(self, policy: str) -> NoneType: ...
     def GetMaintenanceModePolicy(self) -> str: ...
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/fault/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/fault/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List
 from pyVmomi import eam, vim, vmodl
 from datetime import datetime
-from . import cluster, integrity, personality
+from . import cluster as cluster
+from . import integrity as integrity
+from . import personality as personality
 
 
 class AgencyDisabled(AgencyIssue): ...
 
 
 class AgencyIssue(Issue):
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/agent/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/cluster/agent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agency/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/issue/personality/agency/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/lccm/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/lccm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/eam/vib/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/eam/vib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from typing import List
 from enum import Enum
-from pyVmomi import vmodl
+from pyVmomi import pbm, vmodl
 from pyVmomi.VmomiSupport import ManagedObject
-from . import auth, capability, compliance, fault, placement, profile, provider, replication
+from . import auth as auth
+from . import capability as capability
+from . import compliance as compliance
+from . import fault as fault
+from . import placement as placement
+from . import profile as profile
+from . import provider as provider
+from . import replication as replication
 
 
 class ServiceInstance(ManagedObject):
     @property
     def content(self) -> ServiceInstanceContent: ...
     def RetrieveContent(self) -> ServiceInstanceContent: ...
 
@@ -127,42 +134,42 @@
 class ServiceInstanceContent(vmodl.DynamicData):
     @property
     def aboutInfo(self) -> AboutInfo: ...
     @aboutInfo.setter
     def aboutInfo(self, value: AboutInfo):
         self._aboutInfo = value
     @property
-    def sessionManager(self) -> auth.SessionManager: ...
+    def sessionManager(self) -> pbm.auth.SessionManager: ...
     @sessionManager.setter
-    def sessionManager(self, value: auth.SessionManager):
+    def sessionManager(self, value: pbm.auth.SessionManager):
         self._sessionManager = value
     @property
-    def capabilityMetadataManager(self) -> capability.CapabilityMetadataManager: ...
+    def capabilityMetadataManager(self) -> pbm.capability.CapabilityMetadataManager: ...
     @capabilityMetadataManager.setter
-    def capabilityMetadataManager(self, value: capability.CapabilityMetadataManager):
+    def capabilityMetadataManager(self, value: pbm.capability.CapabilityMetadataManager):
         self._capabilityMetadataManager = value
     @property
-    def profileManager(self) -> profile.ProfileManager: ...
+    def profileManager(self) -> pbm.profile.ProfileManager: ...
     @profileManager.setter
-    def profileManager(self, value: profile.ProfileManager):
+    def profileManager(self, value: pbm.profile.ProfileManager):
         self._profileManager = value
     @property
-    def complianceManager(self) -> compliance.ComplianceManager: ...
+    def complianceManager(self) -> pbm.compliance.ComplianceManager: ...
     @complianceManager.setter
-    def complianceManager(self, value: compliance.ComplianceManager):
+    def complianceManager(self, value: pbm.compliance.ComplianceManager):
         self._complianceManager = value
     @property
-    def placementSolver(self) -> placement.PlacementSolver: ...
+    def placementSolver(self) -> pbm.placement.PlacementSolver: ...
     @placementSolver.setter
-    def placementSolver(self, value: placement.PlacementSolver):
+    def placementSolver(self, value: pbm.placement.PlacementSolver):
         self._placementSolver = value
     @property
-    def replicationManager(self) -> replication.ReplicationManager: ...
+    def replicationManager(self) -> pbm.replication.ReplicationManager: ...
     @replicationManager.setter
-    def replicationManager(self, value: replication.ReplicationManager):
+    def replicationManager(self, value: pbm.replication.ReplicationManager):
         self._replicationManager = value
 
 
 class PbmDebugManager():
 
 
     class KeystoreName(Enum):
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
 from pyVmomi import pbm, vmodl
 from pyVmomi.VmomiSupport import ManagedObject
-from . import provider, types
+from . import provider as provider
+from . import types as types
 
 
 class CapabilityMetadataManager(ManagedObject): ...
 
 
 class CapabilityInstance(vmodl.DynamicData):
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/provider/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/provider/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/types/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/capability/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/compliance/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/compliance/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/fault/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/fault/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/placement/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/placement/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/profile/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 from enum import Enum
 from pyVmomi import pbm, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedObject, NoneType, long
-from . import provider
+from . import provider as provider
 
 
 class ProfileManager(ManagedObject):
     def FetchResourceType(self) -> List[ResourceType]: ...
     def FetchVendorInfo(self, resourceType: ResourceType) -> List[pbm.capability.provider.CapabilityObjectSchema.VendorResourceTypeInfo]: ...
     def FetchCapabilityMetadata(self, resourceType: ResourceType, vendorUuid: str) -> List[pbm.capability.provider.CapabilityObjectMetadataPerCategory]: ...
     def FetchCapabilitySchema(self, vendorUuid: str, lineOfService: List[str]) -> List[pbm.capability.provider.CapabilityObjectSchema]: ...
@@ -21,15 +21,15 @@
     def QueryAssociatedEntity(self, profile: ProfileId, entityType: str) -> List[pbm.ServerObjectRef]: ...
     def QueryDefaultRequirementProfile(self, hub: pbm.placement.PlacementHub) -> ProfileId: ...
     def ResetDefaultRequirementProfile(self, profile: ProfileId) -> NoneType: ...
     def AssignDefaultRequirementProfile(self, profile: ProfileId, datastores: List[pbm.placement.PlacementHub]) -> NoneType: ...
     def FindApplicableDefaultProfile(self, datastores: List[pbm.placement.PlacementHub]) -> List[Profile]: ...
     def QueryDefaultRequirementProfiles(self, datastores: List[pbm.placement.PlacementHub]) -> List[DefaultProfileInfo]: ...
     def ResetVSanDefaultProfile(self) -> NoneType: ...
-    def QuerySpaceStatsForStorageContainer(self, datastore: pbm.ServerObjectRef, capabilityProfileId: List[ProfileId]) -> List[provider.DatastoreSpaceStatistics]: ...
+    def QuerySpaceStatsForStorageContainer(self, datastore: pbm.ServerObjectRef, capabilityProfileId: List[ProfileId]) -> List[pbm.profile.provider.DatastoreSpaceStatistics]: ...
     def QueryAssociatedEntities(self, profiles: List[ProfileId]) -> List[QueryProfileResult]: ...
 
 
 class CapabilityBasedProfile(Profile):
     @property
     def profileCategory(self) -> str: ...
     @profileCategory.setter
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/provider/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/profile/provider/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/pbm/replication/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/pbm/replication/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List
-from pyVmomi import ReplicationGroupId, pbm, vmodl
+from pyVmomi import pbm, vim, vmodl
 from pyVmomi.VmomiSupport import ManagedObject
 
 
 class ReplicationManager(ManagedObject):
     def QueryReplicationGroups(self, entities: List[pbm.ServerObjectRef]) -> List[QueryReplicationGroupResult]: ...
 
 
 class QueryReplicationGroupResult(vmodl.DynamicData):
     @property
     def object(self) -> pbm.ServerObjectRef: ...
     @object.setter
     def object(self, value: pbm.ServerObjectRef):
         self._object = value
     @property
-    def replicationGroupId(self) -> ReplicationGroupId: ...
+    def replicationGroupId(self) -> vim.vm.replication.ReplicationGroupId: ...
     @replicationGroupId.setter
-    def replicationGroupId(self, value: ReplicationGroupId):
+    def replicationGroupId(self, value: vim.vm.replication.ReplicationGroupId):
         self._replicationGroupId = value
     @property
     def fault(self) -> vmodl.MethodFault: ...
     @fault.setter
     def fault(self, value: vmodl.MethodFault):
         self._fault = value
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/sms/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/sms/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from typing import List, Literal
 from enum import Enum
-from pyVmomi import auth, vim, vmodl
+from pyVmomi import sms, vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedObject
-from . import fault, provider, storage
+from . import fault as fault
+from . import provider as provider
+from . import storage as storage
 
 
 class ServiceInstance(ManagedObject):
     def QueryStorageManager(self) -> StorageManager: ...
-    def QuerySessionManager(self) -> auth.SessionManager: ...
+    def QuerySessionManager(self) -> sms.auth.SessionManager: ...
     def QueryAboutInfo(self) -> AboutInfo: ...
 
 
 class StorageManager(ManagedObject):
-    def RegisterProvider(self, providerSpec: provider.ProviderSpec) -> Task: ...
+    def RegisterProvider(self, providerSpec: sms.provider.ProviderSpec) -> Task: ...
     def UnregisterProvider(self, providerId: str) -> Task: ...
-    def QueryProvider(self) -> List[provider.Provider]: ...
-    def QueryArray(self, providerId: List[str]) -> List[storage.StorageArray]: ...
-    def QueryProcessorAssociatedWithArray(self, arrayId: str) -> List[storage.StorageProcessor]: ...
-    def QueryPortAssociatedWithArray(self, arrayId: str) -> List[storage.StoragePort]: ...
-    def QueryPortAssociatedWithLun(self, scsi3Id: str, arrayId: str) -> storage.StoragePort: ...
-    def QueryLunAssociatedWithPort(self, portId: str, arrayId: str) -> List[storage.StorageLun]: ...
-    def QueryArrayAssociatedWithLun(self, canonicalName: str) -> storage.StorageArray: ...
-    def QueryPortAssociatedWithProcessor(self, processorId: str, arrayId: str) -> List[storage.StoragePort]: ...
-    def QueryLunAssociatedWithArray(self, arrayId: str) -> List[storage.StorageLun]: ...
-    def QueryFileSystemAssociatedWithArray(self, arrayId: str) -> List[storage.StorageFileSystem]: ...
-    def QueryDatastoreCapability(self, datastore: vim.Datastore) -> storage.StorageCapability: ...
+    def QueryProvider(self) -> List[sms.provider.Provider]: ...
+    def QueryArray(self, providerId: List[str]) -> List[sms.storage.StorageArray]: ...
+    def QueryProcessorAssociatedWithArray(self, arrayId: str) -> List[sms.storage.StorageProcessor]: ...
+    def QueryPortAssociatedWithArray(self, arrayId: str) -> List[sms.storage.StoragePort]: ...
+    def QueryPortAssociatedWithLun(self, scsi3Id: str, arrayId: str) -> sms.storage.StoragePort: ...
+    def QueryLunAssociatedWithPort(self, portId: str, arrayId: str) -> List[sms.storage.StorageLun]: ...
+    def QueryArrayAssociatedWithLun(self, canonicalName: str) -> sms.storage.StorageArray: ...
+    def QueryPortAssociatedWithProcessor(self, processorId: str, arrayId: str) -> List[sms.storage.StoragePort]: ...
+    def QueryLunAssociatedWithArray(self, arrayId: str) -> List[sms.storage.StorageLun]: ...
+    def QueryFileSystemAssociatedWithArray(self, arrayId: str) -> List[sms.storage.StorageFileSystem]: ...
+    def QueryDatastoreCapability(self, datastore: vim.Datastore) -> sms.storage.StorageCapability: ...
     def QueryHostAssociatedWithLun(self, scsi3Id: str, arrayId: str) -> List[vim.HostSystem]: ...
     def QueryVmfsDatastoreAssociatedWithLun(self, scsi3Id: str, arrayId: str) -> vim.Datastore: ...
     def QueryNfsDatastoreAssociatedWithFileSystem(self, fileSystemId: str, arrayId: str) -> vim.Datastore: ...
     def QueryDrsMigrationCapabilityForPerformance(self, srcDatastore: vim.Datastore, dstDatastore: vim.Datastore) -> bool: ...
-    def QueryDrsMigrationCapabilityForPerformanceEx(self, datastore: List[vim.Datastore]) -> storage.DrsMigrationCapabilityResult: ...
-    def QueryStorageContainer(self, containerSpec: storage.StorageContainerSpec) -> storage.StorageContainerResult: ...
-    def QueryAssociatedBackingStoragePool(self, entityId: str, entityType: str) -> List[storage.BackingStoragePool]: ...
-    def QueryDatastoreBackingPoolMapping(self, datastore: List[vim.Datastore]) -> List[storage.DatastoreBackingPoolMapping]: ...
+    def QueryDrsMigrationCapabilityForPerformanceEx(self, datastore: List[vim.Datastore]) -> sms.storage.DrsMigrationCapabilityResult: ...
+    def QueryStorageContainer(self, containerSpec: sms.storage.StorageContainerSpec) -> sms.storage.StorageContainerResult: ...
+    def QueryAssociatedBackingStoragePool(self, entityId: str, entityType: str) -> List[sms.storage.BackingStoragePool]: ...
+    def QueryDatastoreBackingPoolMapping(self, datastore: List[vim.Datastore]) -> List[sms.storage.DatastoreBackingPoolMapping]: ...
     def RefreshCACertificatesAndCRLs(self, providerId: List[str]) -> Task: ...
     def QueryFaultDomain(self, filter: FaultDomainFilter) -> List[vim.vm.replication.FaultDomainId]: ...
-    def QueryReplicationGroupInfo(self, rgFilter: ReplicationGroupFilter) -> List[storage.replication.GroupOperationResult]: ...
+    def QueryReplicationGroupInfo(self, rgFilter: ReplicationGroupFilter) -> List[sms.storage.replication.GroupOperationResult]: ...
 
 
 class Task(ManagedObject):
     def QueryResult(self) -> object: ...
     def QueryInfo(self) -> TaskInfo: ...
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/sms/fault/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Literal
 from pyVmomi import sms, vim, vmodl
 from pyVmomi.VmomiSupport import long
-from . import replication
+from . import replication as replication
 
 
-class AuthConnectionFailed(NoPermission): ...
+class AuthConnectionFailed(vim.fault.NoPermission): ...
 
 
 class CertificateAuthorityFault(ProviderRegistrationFault):
     @property
     def faultCode(self) -> int: ...
     @faultCode.setter
     def faultCode(self, value: int):
@@ -61,15 +61,15 @@
 
 class InvalidLogin(vmodl.MethodFault): ...
 
 
 class InvalidProfile(vmodl.MethodFault): ...
 
 
-class InvalidSession(NoPermission):
+class InvalidSession(vim.fault.NoPermission):
     @property
     def sessionCookie(self) -> str: ...
     @sessionCookie.setter
     def sessionCookie(self, value: str):
         self._sessionCookie = value
 
 
@@ -77,15 +77,15 @@
     @property
     def url(self) -> str: ...
     @url.setter
     def url(self, value: str):
         self._url = value
 
 
-class MultipleSortSpecsNotSupported(InvalidArgument): ...
+class MultipleSortSpecsNotSupported(vmodl.fault.InvalidArgument): ...
 
 
 class NoCommonProviderForAllBackings(QueryExecutionFault): ...
 
 
 class NotSupportedByProvider(vmodl.MethodFault): ...
 
@@ -144,28 +144,28 @@
 
 class ProxyRegistrationFailed(vmodl.RuntimeFault): ...
 
 
 class QueryExecutionFault(vmodl.MethodFault): ...
 
 
-class QueryNotSupported(InvalidArgument):
+class QueryNotSupported(vmodl.fault.InvalidArgument):
     @property
     def entityType(self) -> sms.EntityReference.EntityType | Literal['datacenter', 'resourcePool', 'storagePod', 'cluster', 'vm', 'datastore', 'host', 'vmFile', 'scsiPath', 'scsiTarget', 'scsiVolume', 'scsiAdapter', 'nasMount']: ...
     @entityType.setter
     def entityType(self, value: sms.EntityReference.EntityType | Literal['datacenter', 'resourcePool', 'storagePod', 'cluster', 'vm', 'datastore', 'host', 'vmFile', 'scsiPath', 'scsiTarget', 'scsiVolume', 'scsiAdapter', 'nasMount']):
         self._entityType = value
     @property
     def relatedEntityType(self) -> sms.EntityReference.EntityType | Literal['datacenter', 'resourcePool', 'storagePod', 'cluster', 'vm', 'datastore', 'host', 'vmFile', 'scsiPath', 'scsiTarget', 'scsiVolume', 'scsiAdapter', 'nasMount']: ...
     @relatedEntityType.setter
     def relatedEntityType(self, value: sms.EntityReference.EntityType | Literal['datacenter', 'resourcePool', 'storagePod', 'cluster', 'vm', 'datastore', 'host', 'vmFile', 'scsiPath', 'scsiTarget', 'scsiVolume', 'scsiAdapter', 'nasMount']):
         self._relatedEntityType = value
 
 
-class ResourceInUse(ResourceInUse):
+class ResourceInUse(vim.fault.ResourceInUse):
     @property
     def deviceIds(self) -> List[sms.storage.replication.DeviceId]: ...
     @deviceIds.setter
     def deviceIds(self, value: List[sms.storage.replication.DeviceId]):
         self._deviceIds = value
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/replication/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/sms/fault/replication/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from pyVmomi import DeviceId, sms, vmodl
+from pyVmomi import sms, vmodl
 
 
 class AlreadyDone(ReplicationFault): ...
 
 
 class InvalidFunctionTarget(ReplicationFault): ...
 
@@ -22,17 +22,17 @@
 
 
 class NoReplicationTarget(ReplicationFault): ...
 
 
 class NoValidReplica(ReplicationFault):
     @property
-    def deviceId(self) -> DeviceId: ...
+    def deviceId(self) -> sms.storage.replication.DeviceId: ...
     @deviceId.setter
-    def deviceId(self, value: DeviceId):
+    def deviceId(self, value: sms.storage.replication.DeviceId):
         self._deviceId = value
 
 
 class PeerNotReachable(ReplicationFault): ...
 
 
 class ReplicationFault(vmodl.MethodFault): ...
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/sms/provider/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/sms/provider/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/sms/storage/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 from enum import Enum
 from pyVmomi import sms, vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import long
-from . import replication
+from . import replication as replication
 
 
 class BackingConfig(vmodl.DynamicData):
     @property
     def thinProvisionBackingIdentifier(self) -> str: ...
     @thinProvisionBackingIdentifier.setter
     def thinProvisionBackingIdentifier(self, value: str):
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/replication/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/sms/storage/replication/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from pyVmomi import DeviceGroupId, FaultDomainId, ReplicationGroupId, sms, vim, vmodl
+from pyVmomi import sms, vim, vmodl
 from datetime import datetime
 
 
 class DeviceId(vmodl.DynamicData): ...
 
 
 class FailoverParam(vmodl.DynamicData):
@@ -45,17 +45,17 @@
         @datastore.setter
         def datastore(self, value: vim.Datastore):
             self._datastore = value
 
 
     class ReplicationGroupData(vmodl.DynamicData):
         @property
-        def groupId(self) -> ReplicationGroupId: ...
+        def groupId(self) -> vim.vm.replication.ReplicationGroupId: ...
         @groupId.setter
-        def groupId(self, value: ReplicationGroupId):
+        def groupId(self, value: vim.vm.replication.ReplicationGroupId):
             self._groupId = value
         @property
         def pitId(self) -> PointInTimeReplicaId: ...
         @pitId.setter
         def pitId(self, value: PointInTimeReplicaId):
             self._pitId = value
 
@@ -145,15 +145,15 @@
         @property
         def diskPath(self) -> str: ...
         @diskPath.setter
         def diskPath(self, value: str):
             self._diskPath = value
 
 
-class FaultDomainInfo(FaultDomainId):
+class FaultDomainInfo(vim.vm.replication.FaultDomainId):
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, value: str):
         self._name = value
     @property
     def description(self) -> str: ...
@@ -162,17 +162,17 @@
         self._description = value
     @property
     def storageArrayId(self) -> str: ...
     @storageArrayId.setter
     def storageArrayId(self, value: str):
         self._storageArrayId = value
     @property
-    def children(self) -> List[FaultDomainId]: ...
+    def children(self) -> List[vim.vm.replication.FaultDomainId]: ...
     @children.setter
-    def children(self, value: List[FaultDomainId]):
+    def children(self, value: List[vim.vm.replication.FaultDomainId]):
         self._children = value
     @property
     def provider(self) -> sms.provider.Provider: ...
     @provider.setter
     def provider(self, value: sms.provider.Provider):
         self._provider = value
 
@@ -183,25 +183,25 @@
     @error.setter
     def error(self, value: List[vmodl.MethodFault]):
         self._error = value
 
 
 class GroupInfo(vmodl.DynamicData):
     @property
-    def groupId(self) -> ReplicationGroupId: ...
+    def groupId(self) -> vim.vm.replication.ReplicationGroupId: ...
     @groupId.setter
-    def groupId(self, value: ReplicationGroupId):
+    def groupId(self, value: vim.vm.replication.ReplicationGroupId):
         self._groupId = value
 
 
 class GroupOperationResult(vmodl.DynamicData):
     @property
-    def groupId(self) -> ReplicationGroupId: ...
+    def groupId(self) -> vim.vm.replication.ReplicationGroupId: ...
     @groupId.setter
-    def groupId(self, value: ReplicationGroupId):
+    def groupId(self, value: vim.vm.replication.ReplicationGroupId):
         self._groupId = value
     @property
     def warning(self) -> List[vmodl.MethodFault]: ...
     @warning.setter
     def warning(self, value: List[vmodl.MethodFault]):
         self._warning = value
 
@@ -217,17 +217,17 @@
 class PromoteParam(vmodl.DynamicData):
     @property
     def isPlanned(self) -> bool: ...
     @isPlanned.setter
     def isPlanned(self, value: bool):
         self._isPlanned = value
     @property
-    def replicationGroupsToPromote(self) -> List[ReplicationGroupId]: ...
+    def replicationGroupsToPromote(self) -> List[vim.vm.replication.ReplicationGroupId]: ...
     @replicationGroupsToPromote.setter
-    def replicationGroupsToPromote(self, value: List[ReplicationGroupId]):
+    def replicationGroupsToPromote(self, value: List[vim.vm.replication.ReplicationGroupId]):
         self._replicationGroupsToPromote = value
 
 
 class QueryPointInTimeReplicaParam(vmodl.DynamicData):
     @property
     def replicaTimeQueryParam(self) -> QueryPointInTimeReplicaParam.ReplicaQueryIntervalParam: ...
     @replicaTimeQueryParam.setter
@@ -331,22 +331,22 @@
     @rgInfo.setter
     def rgInfo(self, value: GroupInfo):
         self._rgInfo = value
 
 
 class QueryReplicationPeerResult(vmodl.DynamicData):
     @property
-    def sourceDomain(self) -> FaultDomainId: ...
+    def sourceDomain(self) -> vim.vm.replication.FaultDomainId: ...
     @sourceDomain.setter
-    def sourceDomain(self, value: FaultDomainId):
+    def sourceDomain(self, value: vim.vm.replication.FaultDomainId):
         self._sourceDomain = value
     @property
-    def targetDomain(self) -> List[FaultDomainId]: ...
+    def targetDomain(self) -> List[vim.vm.replication.FaultDomainId]: ...
     @targetDomain.setter
-    def targetDomain(self, value: List[FaultDomainId]):
+    def targetDomain(self, value: List[vim.vm.replication.FaultDomainId]):
         self._targetDomain = value
     @property
     def error(self) -> List[vmodl.MethodFault]: ...
     @error.setter
     def error(self, value: List[vmodl.MethodFault]):
         self._error = value
     @property
@@ -370,17 +370,17 @@
     @id.setter
     def id(self, value: str):
         self._id = value
 
 
 class ReverseReplicationSuccessResult(GroupOperationResult):
     @property
-    def newGroupId(self) -> DeviceGroupId: ...
+    def newGroupId(self) -> vim.vm.replication.DeviceGroupId: ...
     @newGroupId.setter
-    def newGroupId(self, value: DeviceGroupId):
+    def newGroupId(self, value: vim.vm.replication.DeviceGroupId):
         self._newGroupId = value
 
 
 class SourceGroupInfo(GroupInfo):
     @property
     def name(self) -> str: ...
     @name.setter
@@ -406,17 +406,17 @@
     @memberInfo.setter
     def memberInfo(self, value: List[SourceGroupMemberInfo]):
         self._memberInfo = value
 
 
     class ReplicationTargetInfo(vmodl.DynamicData):
         @property
-        def targetGroupId(self) -> ReplicationGroupId: ...
+        def targetGroupId(self) -> vim.vm.replication.ReplicationGroupId: ...
         @targetGroupId.setter
-        def targetGroupId(self, value: ReplicationGroupId):
+        def targetGroupId(self, value: vim.vm.replication.ReplicationGroupId):
             self._targetGroupId = value
         @property
         def replicationAgreementDescription(self) -> str: ...
         @replicationAgreementDescription.setter
         def replicationAgreementDescription(self, value: str):
             self._replicationAgreementDescription = value
 
@@ -432,17 +432,17 @@
     @targetId.setter
     def targetId(self, value: List[SourceGroupMemberInfo.TargetDeviceId]):
         self._targetId = value
 
 
     class TargetDeviceId(vmodl.DynamicData):
         @property
-        def domainId(self) -> FaultDomainId: ...
+        def domainId(self) -> vim.vm.replication.FaultDomainId: ...
         @domainId.setter
-        def domainId(self, value: FaultDomainId):
+        def domainId(self, value: vim.vm.replication.FaultDomainId):
             self._domainId = value
         @property
         def deviceId(self) -> ReplicaId: ...
         @deviceId.setter
         def deviceId(self, value: ReplicaId):
             self._deviceId = value
 
@@ -486,17 +486,17 @@
     @isPromoteCapable.setter
     def isPromoteCapable(self, value: bool):
         self._isPromoteCapable = value
 
 
     class TargetToSourceInfo(vmodl.DynamicData):
         @property
-        def sourceGroupId(self) -> ReplicationGroupId: ...
+        def sourceGroupId(self) -> vim.vm.replication.ReplicationGroupId: ...
         @sourceGroupId.setter
-        def sourceGroupId(self, value: ReplicationGroupId):
+        def sourceGroupId(self, value: vim.vm.replication.ReplicationGroupId):
             self._sourceGroupId = value
         @property
         def replicationAgreementDescription(self) -> str: ...
         @replicationAgreementDescription.setter
         def replicationAgreementDescription(self, value: str):
             self._replicationAgreementDescription = value
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 from typing import List, Literal
 from enum import Enum
 from pyVmomi import vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedMethod, ManagedObject, NoneType, byte, double, long, short
-from . import action, alarm, cluster, dvs, encryption, event, ext, fault, host, net, option, profile, scheduler, storageDrs, tenant, vcha, view, vm, vsan, vslm
+from . import action as action
+from . import alarm as alarm
+from . import cluster as cluster
+from . import dvs as dvs
+from . import encryption as encryption
+from . import event as event
+from . import ext as ext
+from . import fault as fault
+from . import host as host
+from . import net as net
+from . import option as option
+from . import profile as profile
+from . import scheduler as scheduler
+from . import storageDrs as storageDrs
+from . import tenant as tenant
+from . import vcha as vcha
+from . import view as view
+from . import vm as vm
+from . import vsan as vsan
+from . import vslm as vslm
 
 
 class AuthorizationManager(ManagedObject):
     @property
     def privilegeList(self) -> List[AuthorizationManager.Privilege]: ...
     @property
     def roleList(self) -> List[AuthorizationManager.Role]: ...
@@ -151,48 +170,48 @@
     def RefreshCACertificatesAndCRLs(self, host: List[HostSystem]) -> Task: ...
     def RefreshCertificates(self, host: List[HostSystem]) -> Task: ...
     def RevokeCertificates(self, host: List[HostSystem]) -> Task: ...
 
 
 class ClusterComputeResource(ComputeResource):
     @property
-    def configuration(self) -> cluster.ConfigInfo: ...
+    def configuration(self) -> vim.cluster.ConfigInfo: ...
     @property
-    def recommendation(self) -> List[cluster.Recommendation]: ...
+    def recommendation(self) -> List[vim.cluster.Recommendation]: ...
     @property
-    def drsRecommendation(self) -> List[cluster.DrsRecommendation]: ...
+    def drsRecommendation(self) -> List[vim.cluster.DrsRecommendation]: ...
     @property
     def summaryEx(self) -> ClusterComputeResource.Summary: ...
     @property
     def hciConfig(self) -> ClusterComputeResource.HCIConfigInfo: ...
     @property
-    def migrationHistory(self) -> List[cluster.DrsMigration]: ...
+    def migrationHistory(self) -> List[vim.cluster.DrsMigration]: ...
     @property
-    def actionHistory(self) -> List[cluster.ActionHistory]: ...
+    def actionHistory(self) -> List[vim.cluster.ActionHistory]: ...
     @property
-    def drsFault(self) -> List[cluster.DrsFaults]: ...
+    def drsFault(self) -> List[vim.cluster.DrsFaults]: ...
     def ConfigureHCI(self, clusterSpec: ClusterComputeResource.HCIConfigSpec, hostInputs: List[ClusterComputeResource.HostConfigurationInput]) -> Task: ...
     def ExtendHCI(self, hostInputs: List[ClusterComputeResource.HostConfigurationInput], vSanConfigSpec: SDDCBase) -> Task: ...
     def AbandonHciWorkflow(self) -> NoneType: ...
     def ValidateHCIConfiguration(self, hciConfigSpec: ClusterComputeResource.HCIConfigSpec, hosts: List[HostSystem]) -> List[ClusterComputeResource.ValidationResultBase]: ...
-    def Reconfigure(self, spec: cluster.ConfigSpec, modify: bool) -> Task: ...
+    def Reconfigure(self, spec: vim.cluster.ConfigSpec, modify: bool) -> Task: ...
     def ApplyRecommendation(self, key: str) -> NoneType: ...
     def CancelRecommendation(self, key: str) -> NoneType: ...
-    def RecommendHostsForVm(self, vm: VirtualMachine, pool: ResourcePool) -> List[cluster.HostRecommendation]: ...
-    def AddHost(self, spec: host.ConnectSpec, asConnected: bool, resourcePool: ResourcePool, license: str) -> Task: ...
+    def RecommendHostsForVm(self, vm: VirtualMachine, pool: ResourcePool) -> List[vim.cluster.HostRecommendation]: ...
+    def AddHost(self, spec: vim.host.ConnectSpec, asConnected: bool, resourcePool: ResourcePool, license: str) -> Task: ...
     def MoveInto(self, host: List[HostSystem]) -> Task: ...
     def MoveHostInto(self, host: HostSystem, resourcePool: ResourcePool) -> Task: ...
     def RefreshRecommendation(self) -> NoneType: ...
-    def EvcManager(self) -> cluster.EVCManager: ...
-    def RetrieveDasAdvancedRuntimeInfo(self) -> cluster.DasAdvancedRuntimeInfo: ...
-    def EnterMaintenanceMode(self, host: List[HostSystem], option: List[option.OptionValue]) -> cluster.EnterMaintenanceResult: ...
-    def PlaceVm(self, placementSpec: cluster.PlacementSpec) -> cluster.PlacementResult: ...
-    def FindRulesForVm(self, vm: VirtualMachine) -> List[cluster.RuleInfo]: ...
+    def EvcManager(self) -> vim.cluster.EVCManager: ...
+    def RetrieveDasAdvancedRuntimeInfo(self) -> vim.cluster.DasAdvancedRuntimeInfo: ...
+    def EnterMaintenanceMode(self, host: List[HostSystem], option: List[vim.option.OptionValue]) -> vim.cluster.EnterMaintenanceResult: ...
+    def PlaceVm(self, placementSpec: vim.cluster.PlacementSpec) -> vim.cluster.PlacementResult: ...
+    def FindRulesForVm(self, vm: VirtualMachine) -> List[vim.cluster.RuleInfo]: ...
     def StampAllRulesWithUuid(self) -> Task: ...
-    def GetResourceUsage(self) -> cluster.ResourceUsageSummary: ...
+    def GetResourceUsage(self) -> vim.cluster.ResourceUsageSummary: ...
     def SetCryptoMode(self, cryptoMode: str) -> NoneType: ...
     def GetSystemVMsRestrictedDatastores(self) -> List[Datastore]: ...
 
 
     class ClusterConfigResult(vmodl.DynamicData):
         @property
         def failedHosts(self) -> List[Folder.FailedHostResult]: ...
@@ -235,17 +254,17 @@
         @dvPortgroupSetting.setter
         def dvPortgroupSetting(self, value: List[ClusterComputeResource.DVSSetting.DVPortgroupToServiceMapping]):
             self._dvPortgroupSetting = value
 
 
         class DVPortgroupToServiceMapping(vmodl.DynamicData):
             @property
-            def dvPortgroup(self) -> dvs.DistributedVirtualPortgroup: ...
+            def dvPortgroup(self) -> vim.dvs.DistributedVirtualPortgroup: ...
             @dvPortgroup.setter
-            def dvPortgroup(self, value: dvs.DistributedVirtualPortgroup):
+            def dvPortgroup(self, value: vim.dvs.DistributedVirtualPortgroup):
                 self._dvPortgroup = value
             @property
             def service(self) -> str: ...
             @service.setter
             def service(self, value: str):
                 self._service = value
 
@@ -271,22 +290,22 @@
         @dvPortgroupMapping.setter
         def dvPortgroupMapping(self, value: List[ClusterComputeResource.DvsProfile.DVPortgroupSpecToServiceMapping]):
             self._dvPortgroupMapping = value
 
 
         class DVPortgroupSpecToServiceMapping(vmodl.DynamicData):
             @property
-            def dvPortgroupSpec(self) -> dvs.DistributedVirtualPortgroup.ConfigSpec: ...
+            def dvPortgroupSpec(self) -> vim.dvs.DistributedVirtualPortgroup.ConfigSpec: ...
             @dvPortgroupSpec.setter
-            def dvPortgroupSpec(self, value: dvs.DistributedVirtualPortgroup.ConfigSpec):
+            def dvPortgroupSpec(self, value: vim.dvs.DistributedVirtualPortgroup.ConfigSpec):
                 self._dvPortgroupSpec = value
             @property
-            def dvPortgroup(self) -> dvs.DistributedVirtualPortgroup: ...
+            def dvPortgroup(self) -> vim.dvs.DistributedVirtualPortgroup: ...
             @dvPortgroup.setter
-            def dvPortgroup(self, value: dvs.DistributedVirtualPortgroup):
+            def dvPortgroup(self, value: vim.dvs.DistributedVirtualPortgroup):
                 self._dvPortgroup = value
             @property
             def service(self) -> str: ...
             @service.setter
             def service(self, value: str):
                 self._service = value
 
@@ -353,22 +372,22 @@
         @allowedInNonMaintenanceMode.setter
         def allowedInNonMaintenanceMode(self, value: bool):
             self._allowedInNonMaintenanceMode = value
 
 
     class HostConfigurationProfile(vmodl.DynamicData):
         @property
-        def dateTimeConfig(self) -> host.DateTimeConfig: ...
+        def dateTimeConfig(self) -> vim.host.DateTimeConfig: ...
         @dateTimeConfig.setter
-        def dateTimeConfig(self, value: host.DateTimeConfig):
+        def dateTimeConfig(self, value: vim.host.DateTimeConfig):
             self._dateTimeConfig = value
         @property
-        def lockdownMode(self) -> host.HostAccessManager.LockdownMode | Literal['lockdownDisabled', 'lockdownNormal', 'lockdownStrict']: ...
+        def lockdownMode(self) -> vim.host.HostAccessManager.LockdownMode | Literal['lockdownDisabled', 'lockdownNormal', 'lockdownStrict']: ...
         @lockdownMode.setter
-        def lockdownMode(self, value: host.HostAccessManager.LockdownMode | Literal['lockdownDisabled', 'lockdownNormal', 'lockdownStrict']):
+        def lockdownMode(self, value: vim.host.HostAccessManager.LockdownMode | Literal['lockdownDisabled', 'lockdownNormal', 'lockdownStrict']):
             self._lockdownMode = value
 
 
     class HostConfigurationValidation(ClusterComputeResource.ValidationResultBase):
         @property
         def host(self) -> HostSystem: ...
         @host.setter
@@ -394,17 +413,17 @@
         @isLockdownModeValid.setter
         def isLockdownModeValid(self, value: bool):
             self._isLockdownModeValid = value
 
 
     class HostVmkNicInfo(vmodl.DynamicData):
         @property
-        def nicSpec(self) -> host.VirtualNic.Specification: ...
+        def nicSpec(self) -> vim.host.VirtualNic.Specification: ...
         @nicSpec.setter
-        def nicSpec(self, value: host.VirtualNic.Specification):
+        def nicSpec(self, value: vim.host.VirtualNic.Specification):
             self._nicSpec = value
         @property
         def service(self) -> str: ...
         @service.setter
         def service(self, value: str):
             self._service = value
 
@@ -412,17 +431,17 @@
     class Summary(ComputeResource.Summary):
         @property
         def currentFailoverLevel(self) -> int: ...
         @currentFailoverLevel.setter
         def currentFailoverLevel(self, value: int):
             self._currentFailoverLevel = value
         @property
-        def admissionControlInfo(self) -> cluster.DasAdmissionControlInfo: ...
+        def admissionControlInfo(self) -> vim.cluster.DasAdmissionControlInfo: ...
         @admissionControlInfo.setter
-        def admissionControlInfo(self, value: cluster.DasAdmissionControlInfo):
+        def admissionControlInfo(self, value: vim.cluster.DasAdmissionControlInfo):
             self._admissionControlInfo = value
         @property
         def numVmotions(self) -> int: ...
         @numVmotions.setter
         def numVmotions(self, value: int):
             self._numVmotions = value
         @property
@@ -442,32 +461,32 @@
             self._drsScore = value
         @property
         def numVmsPerDrsScoreBucket(self) -> List[int]: ...
         @numVmsPerDrsScoreBucket.setter
         def numVmsPerDrsScoreBucket(self, value: List[int]):
             self._numVmsPerDrsScoreBucket = value
         @property
-        def usageSummary(self) -> cluster.UsageSummary: ...
+        def usageSummary(self) -> vim.cluster.UsageSummary: ...
         @usageSummary.setter
-        def usageSummary(self, value: cluster.UsageSummary):
+        def usageSummary(self, value: vim.cluster.UsageSummary):
             self._usageSummary = value
         @property
         def currentEVCModeKey(self) -> str: ...
         @currentEVCModeKey.setter
         def currentEVCModeKey(self, value: str):
             self._currentEVCModeKey = value
         @property
         def currentEVCGraphicsModeKey(self) -> str: ...
         @currentEVCGraphicsModeKey.setter
         def currentEVCGraphicsModeKey(self, value: str):
             self._currentEVCGraphicsModeKey = value
         @property
-        def dasData(self) -> cluster.DasData: ...
+        def dasData(self) -> vim.cluster.DasData: ...
         @dasData.setter
-        def dasData(self, value: cluster.DasData):
+        def dasData(self, value: vim.cluster.DasData):
             self._dasData = value
         @property
         def clusterMaintenanceModeStatus(self) -> str: ...
         @clusterMaintenanceModeStatus.setter
         def clusterMaintenanceModeStatus(self, value: str):
             self._clusterMaintenanceModeStatus = value
         @property
@@ -480,17 +499,17 @@
         @vcsSlots.setter
         def vcsSlots(self, value: List[ClusterComputeResource.VcsSlots]):
             self._vcsSlots = value
 
 
     class VCProfile(vmodl.DynamicData):
         @property
-        def clusterSpec(self) -> cluster.ConfigSpecEx: ...
+        def clusterSpec(self) -> vim.cluster.ConfigSpecEx: ...
         @clusterSpec.setter
-        def clusterSpec(self, value: cluster.ConfigSpecEx):
+        def clusterSpec(self, value: vim.cluster.ConfigSpecEx):
             self._clusterSpec = value
         @property
         def evcModeKey(self) -> str: ...
         @evcModeKey.setter
         def evcModeKey(self, value: str):
             self._evcModeKey = value
         @property
@@ -774,19 +793,19 @@
     def networkFolder(self) -> Folder: ...
     @property
     def datastore(self) -> List[Datastore]: ...
     @property
     def network(self) -> List[Network]: ...
     @property
     def configuration(self) -> Datacenter.ConfigInfo: ...
-    def BatchQueryConnectInfo(self, hostSpecs: List[host.ConnectSpec]) -> List[Datacenter.BasicConnectInfo]: ...
-    def QueryConnectionInfo(self, hostname: str, port: int, username: str, password: str, sslThumbprint: str) -> host.ConnectInfo: ...
-    def QueryConnectionInfoViaSpec(self, spec: host.ConnectSpec) -> host.ConnectInfo: ...
-    def PowerOnVm(self, vm: List[VirtualMachine], option: List[option.OptionValue]) -> Task: ...
-    def QueryConfigOptionDescriptor(self) -> List[vm.ConfigOptionDescriptor]: ...
+    def BatchQueryConnectInfo(self, hostSpecs: List[vim.host.ConnectSpec]) -> List[Datacenter.BasicConnectInfo]: ...
+    def QueryConnectionInfo(self, hostname: str, port: int, username: str, password: str, sslThumbprint: str) -> vim.host.ConnectInfo: ...
+    def QueryConnectionInfoViaSpec(self, spec: vim.host.ConnectSpec) -> vim.host.ConnectInfo: ...
+    def PowerOnVm(self, vm: List[VirtualMachine], option: List[vim.option.OptionValue]) -> Task: ...
+    def QueryConfigOptionDescriptor(self) -> List[vim.vm.ConfigOptionDescriptor]: ...
     def Reconfigure(self, spec: Datacenter.ConfigSpec, modify: bool) -> Task: ...
 
 
     class BasicConnectInfo(vmodl.DynamicData):
         @property
         def hostname(self) -> str: ...
         @hostname.setter
@@ -861,15 +880,15 @@
     @property
     def summary(self) -> Datastore.Summary: ...
     @property
     def host(self) -> List[Datastore.HostMount]: ...
     @property
     def vm(self) -> List[VirtualMachine]: ...
     @property
-    def browser(self) -> host.DatastoreBrowser: ...
+    def browser(self) -> vim.host.DatastoreBrowser: ...
     @property
     def capability(self) -> Datastore.Capability: ...
     @property
     def iormConfiguration(self) -> StorageResourceManager.IORMConfigInfo: ...
     def Refresh(self) -> NoneType: ...
     def RefreshStorageInfo(self) -> NoneType: ...
     def UpdateVirtualMachineFiles(self, mountPathDatastoreMapping: List[Datastore.MountPathDatastorePair]) -> Task: ...
@@ -947,17 +966,17 @@
     class HostMount(vmodl.DynamicData):
         @property
         def key(self) -> HostSystem: ...
         @key.setter
         def key(self, value: HostSystem):
             self._key = value
         @property
-        def mountInfo(self) -> host.MountInfo: ...
+        def mountInfo(self) -> vim.host.MountInfo: ...
         @mountInfo.setter
-        def mountInfo(self, value: host.MountInfo):
+        def mountInfo(self, value: vim.host.MountInfo):
             self._mountInfo = value
 
 
     class Info(vmodl.DynamicData):
         @property
         def name(self) -> str: ...
         @name.setter
@@ -1226,40 +1245,40 @@
     @property
     def capability(self) -> DistributedVirtualSwitch.Capability: ...
     @property
     def summary(self) -> DistributedVirtualSwitch.Summary: ...
     @property
     def config(self) -> DistributedVirtualSwitch.ConfigInfo: ...
     @property
-    def networkResourcePool(self) -> List[dvs.NetworkResourcePool]: ...
+    def networkResourcePool(self) -> List[vim.dvs.NetworkResourcePool]: ...
     @property
-    def portgroup(self) -> List[dvs.DistributedVirtualPortgroup]: ...
+    def portgroup(self) -> List[vim.dvs.DistributedVirtualPortgroup]: ...
     @property
     def runtime(self) -> DistributedVirtualSwitch.RuntimeInfo: ...
-    def FetchPortKeys(self, criteria: dvs.PortCriteria) -> List[str]: ...
-    def FetchPorts(self, criteria: dvs.PortCriteria) -> List[dvs.DistributedVirtualPort]: ...
+    def FetchPortKeys(self, criteria: vim.dvs.PortCriteria) -> List[str]: ...
+    def FetchPorts(self, criteria: vim.dvs.PortCriteria) -> List[vim.dvs.DistributedVirtualPort]: ...
     def QueryUsedVlanId(self) -> List[int]: ...
     def Reconfigure(self, spec: DistributedVirtualSwitch.ConfigSpec) -> Task: ...
-    def PerformProductSpecOperation(self, operation: str, productSpec: dvs.ProductSpec) -> Task: ...
+    def PerformProductSpecOperation(self, operation: str, productSpec: vim.dvs.ProductSpec) -> Task: ...
     def Merge(self, dvs: DistributedVirtualSwitch) -> Task: ...
-    def AddPortgroups(self, spec: List[dvs.DistributedVirtualPortgroup.ConfigSpec]) -> Task: ...
+    def AddPortgroups(self, spec: List[vim.dvs.DistributedVirtualPortgroup.ConfigSpec]) -> Task: ...
     def MovePort(self, portKey: List[str], destinationPortgroupKey: str) -> Task: ...
     def UpdateCapability(self, capability: DistributedVirtualSwitch.Capability) -> NoneType: ...
-    def ReconfigurePort(self, port: List[dvs.DistributedVirtualPort.ConfigSpec]) -> Task: ...
+    def ReconfigurePort(self, port: List[vim.dvs.DistributedVirtualPort.ConfigSpec]) -> Task: ...
     def RefreshPortState(self, portKeys: List[str]) -> NoneType: ...
     def RectifyHost(self, hosts: List[HostSystem]) -> Task: ...
-    def UpdateNetworkResourcePool(self, configSpec: List[dvs.NetworkResourcePool.ConfigSpec]) -> NoneType: ...
-    def AddNetworkResourcePool(self, configSpec: List[dvs.NetworkResourcePool.ConfigSpec]) -> NoneType: ...
+    def UpdateNetworkResourcePool(self, configSpec: List[vim.dvs.NetworkResourcePool.ConfigSpec]) -> NoneType: ...
+    def AddNetworkResourcePool(self, configSpec: List[vim.dvs.NetworkResourcePool.ConfigSpec]) -> NoneType: ...
     def RemoveNetworkResourcePool(self, key: List[str]) -> NoneType: ...
-    def ReconfigureVmVnicNetworkResourcePool(self, configSpec: List[dvs.VmVnicNetworkResourcePool.ConfigSpec]) -> Task: ...
+    def ReconfigureVmVnicNetworkResourcePool(self, configSpec: List[vim.dvs.VmVnicNetworkResourcePool.ConfigSpec]) -> Task: ...
     def EnableNetworkResourceManagement(self, enable: bool) -> NoneType: ...
-    def Rollback(self, entityBackup: dvs.EntityBackup.Config) -> Task: ...
-    def AddPortgroup(self, spec: dvs.DistributedVirtualPortgroup.ConfigSpec) -> Task: ...
+    def Rollback(self, entityBackup: vim.dvs.EntityBackup.Config) -> Task: ...
+    def AddPortgroup(self, spec: vim.dvs.DistributedVirtualPortgroup.ConfigSpec) -> Task: ...
     def UpdateHealthCheckConfig(self, healthCheckConfig: List[DistributedVirtualSwitch.HealthCheckConfig]) -> Task: ...
-    def LookupPortgroup(self, portgroupKey: str) -> dvs.DistributedVirtualPortgroup: ...
+    def LookupPortgroup(self, portgroupKey: str) -> vim.dvs.DistributedVirtualPortgroup: ...
 
 
     class BackupRestoreCapability(vmodl.DynamicData):
         @property
         def backupRestoreSupported(self) -> bool: ...
         @backupRestoreSupported.setter
         def backupRestoreSupported(self, value: bool):
@@ -1279,17 +1298,17 @@
             self._dvPortGroupOperationSupported = value
         @property
         def dvPortOperationSupported(self) -> bool: ...
         @dvPortOperationSupported.setter
         def dvPortOperationSupported(self, value: bool):
             self._dvPortOperationSupported = value
         @property
-        def compatibleHostComponentProductInfo(self) -> List[dvs.HostProductSpec]: ...
+        def compatibleHostComponentProductInfo(self) -> List[vim.dvs.HostProductSpec]: ...
         @compatibleHostComponentProductInfo.setter
-        def compatibleHostComponentProductInfo(self, value: List[dvs.HostProductSpec]):
+        def compatibleHostComponentProductInfo(self, value: List[vim.dvs.HostProductSpec]):
             self._compatibleHostComponentProductInfo = value
         @property
         def featuresSupported(self) -> DistributedVirtualSwitch.FeatureCapability: ...
         @featuresSupported.setter
         def featuresSupported(self, value: DistributedVirtualSwitch.FeatureCapability):
             self._featuresSupported = value
 
@@ -1322,47 +1341,47 @@
             self._maxPorts = value
         @property
         def uplinkPortPolicy(self) -> DistributedVirtualSwitch.UplinkPortPolicy: ...
         @uplinkPortPolicy.setter
         def uplinkPortPolicy(self, value: DistributedVirtualSwitch.UplinkPortPolicy):
             self._uplinkPortPolicy = value
         @property
-        def uplinkPortgroup(self) -> List[dvs.DistributedVirtualPortgroup]: ...
+        def uplinkPortgroup(self) -> List[vim.dvs.DistributedVirtualPortgroup]: ...
         @uplinkPortgroup.setter
-        def uplinkPortgroup(self, value: List[dvs.DistributedVirtualPortgroup]):
+        def uplinkPortgroup(self, value: List[vim.dvs.DistributedVirtualPortgroup]):
             self._uplinkPortgroup = value
         @property
-        def defaultPortConfig(self) -> dvs.DistributedVirtualPort.Setting: ...
+        def defaultPortConfig(self) -> vim.dvs.DistributedVirtualPort.Setting: ...
         @defaultPortConfig.setter
-        def defaultPortConfig(self, value: dvs.DistributedVirtualPort.Setting):
+        def defaultPortConfig(self, value: vim.dvs.DistributedVirtualPort.Setting):
             self._defaultPortConfig = value
         @property
-        def host(self) -> List[dvs.HostMember]: ...
+        def host(self) -> List[vim.dvs.HostMember]: ...
         @host.setter
-        def host(self, value: List[dvs.HostMember]):
+        def host(self, value: List[vim.dvs.HostMember]):
             self._host = value
         @property
-        def productInfo(self) -> dvs.ProductSpec: ...
+        def productInfo(self) -> vim.dvs.ProductSpec: ...
         @productInfo.setter
-        def productInfo(self, value: dvs.ProductSpec):
+        def productInfo(self, value: vim.dvs.ProductSpec):
             self._productInfo = value
         @property
-        def targetInfo(self) -> dvs.ProductSpec: ...
+        def targetInfo(self) -> vim.dvs.ProductSpec: ...
         @targetInfo.setter
-        def targetInfo(self, value: dvs.ProductSpec):
+        def targetInfo(self, value: vim.dvs.ProductSpec):
             self._targetInfo = value
         @property
         def extensionKey(self) -> str: ...
         @extensionKey.setter
         def extensionKey(self, value: str):
             self._extensionKey = value
         @property
-        def vendorSpecificConfig(self) -> List[dvs.KeyedOpaqueBlob]: ...
+        def vendorSpecificConfig(self) -> List[vim.dvs.KeyedOpaqueBlob]: ...
         @vendorSpecificConfig.setter
-        def vendorSpecificConfig(self, value: List[dvs.KeyedOpaqueBlob]):
+        def vendorSpecificConfig(self, value: List[vim.dvs.KeyedOpaqueBlob]):
             self._vendorSpecificConfig = value
         @property
         def policy(self) -> DistributedVirtualSwitch.SwitchPolicy: ...
         @policy.setter
         def policy(self, value: DistributedVirtualSwitch.SwitchPolicy):
             self._policy = value
         @property
@@ -1417,17 +1436,17 @@
             self._netResourcePoolTrafficResourceConfig = value
         @property
         def networkResourceControlVersion(self) -> str: ...
         @networkResourceControlVersion.setter
         def networkResourceControlVersion(self, value: str):
             self._networkResourceControlVersion = value
         @property
-        def vmVnicNetworkResourcePool(self) -> List[dvs.VmVnicNetworkResourcePool]: ...
+        def vmVnicNetworkResourcePool(self) -> List[vim.dvs.VmVnicNetworkResourcePool]: ...
         @vmVnicNetworkResourcePool.setter
-        def vmVnicNetworkResourcePool(self, value: List[dvs.VmVnicNetworkResourcePool]):
+        def vmVnicNetworkResourcePool(self, value: List[vim.dvs.VmVnicNetworkResourcePool]):
             self._vmVnicNetworkResourcePool = value
         @property
         def pnicCapacityRatioForReservation(self) -> int: ...
         @pnicCapacityRatioForReservation.setter
         def pnicCapacityRatioForReservation(self, value: int):
             self._pnicCapacityRatioForReservation = value
 
@@ -1455,27 +1474,27 @@
             self._maxPorts = value
         @property
         def uplinkPortPolicy(self) -> DistributedVirtualSwitch.UplinkPortPolicy: ...
         @uplinkPortPolicy.setter
         def uplinkPortPolicy(self, value: DistributedVirtualSwitch.UplinkPortPolicy):
             self._uplinkPortPolicy = value
         @property
-        def uplinkPortgroup(self) -> List[dvs.DistributedVirtualPortgroup]: ...
+        def uplinkPortgroup(self) -> List[vim.dvs.DistributedVirtualPortgroup]: ...
         @uplinkPortgroup.setter
-        def uplinkPortgroup(self, value: List[dvs.DistributedVirtualPortgroup]):
+        def uplinkPortgroup(self, value: List[vim.dvs.DistributedVirtualPortgroup]):
             self._uplinkPortgroup = value
         @property
-        def defaultPortConfig(self) -> dvs.DistributedVirtualPort.Setting: ...
+        def defaultPortConfig(self) -> vim.dvs.DistributedVirtualPort.Setting: ...
         @defaultPortConfig.setter
-        def defaultPortConfig(self, value: dvs.DistributedVirtualPort.Setting):
+        def defaultPortConfig(self, value: vim.dvs.DistributedVirtualPort.Setting):
             self._defaultPortConfig = value
         @property
-        def host(self) -> List[dvs.HostMember.ConfigSpec]: ...
+        def host(self) -> List[vim.dvs.HostMember.ConfigSpec]: ...
         @host.setter
-        def host(self, value: List[dvs.HostMember.ConfigSpec]):
+        def host(self, value: List[vim.dvs.HostMember.ConfigSpec]):
             self._host = value
         @property
         def extensionKey(self) -> str: ...
         @extensionKey.setter
         def extensionKey(self, value: str):
             self._extensionKey = value
         @property
@@ -1485,17 +1504,17 @@
             self._description = value
         @property
         def policy(self) -> DistributedVirtualSwitch.SwitchPolicy: ...
         @policy.setter
         def policy(self, value: DistributedVirtualSwitch.SwitchPolicy):
             self._policy = value
         @property
-        def vendorSpecificConfig(self) -> List[dvs.KeyedOpaqueBlob]: ...
+        def vendorSpecificConfig(self) -> List[vim.dvs.KeyedOpaqueBlob]: ...
         @vendorSpecificConfig.setter
-        def vendorSpecificConfig(self, value: List[dvs.KeyedOpaqueBlob]):
+        def vendorSpecificConfig(self, value: List[vim.dvs.KeyedOpaqueBlob]):
             self._vendorSpecificConfig = value
         @property
         def contact(self) -> DistributedVirtualSwitch.ContactInfo: ...
         @contact.setter
         def contact(self, value: DistributedVirtualSwitch.ContactInfo):
             self._contact = value
         @property
@@ -1541,17 +1560,17 @@
     class CreateSpec(vmodl.DynamicData):
         @property
         def configSpec(self) -> DistributedVirtualSwitch.ConfigSpec: ...
         @configSpec.setter
         def configSpec(self, value: DistributedVirtualSwitch.ConfigSpec):
             self._configSpec = value
         @property
-        def productInfo(self) -> dvs.ProductSpec: ...
+        def productInfo(self) -> vim.dvs.ProductSpec: ...
         @productInfo.setter
-        def productInfo(self, value: dvs.ProductSpec):
+        def productInfo(self, value: vim.dvs.ProductSpec):
             self._productInfo = value
         @property
         def capability(self) -> DistributedVirtualSwitch.Capability: ...
         @capability.setter
         def capability(self, value: DistributedVirtualSwitch.Capability):
             self._capability = value
 
@@ -1715,38 +1734,38 @@
             self._usage = value
         @property
         def available(self) -> int: ...
         @available.setter
         def available(self, value: int):
             self._available = value
         @property
-        def allocatedResource(self) -> List[dvs.VmVnicNetworkResourcePool.VnicAllocatedResource]: ...
+        def allocatedResource(self) -> List[vim.dvs.VmVnicNetworkResourcePool.VnicAllocatedResource]: ...
         @allocatedResource.setter
-        def allocatedResource(self, value: List[dvs.VmVnicNetworkResourcePool.VnicAllocatedResource]):
+        def allocatedResource(self, value: List[vim.dvs.VmVnicNetworkResourcePool.VnicAllocatedResource]):
             self._allocatedResource = value
         @property
-        def vmVnicNetworkResourcePoolRuntime(self) -> List[dvs.VmVnicNetworkResourcePool.RuntimeInfo]: ...
+        def vmVnicNetworkResourcePoolRuntime(self) -> List[vim.dvs.VmVnicNetworkResourcePool.RuntimeInfo]: ...
         @vmVnicNetworkResourcePoolRuntime.setter
-        def vmVnicNetworkResourcePoolRuntime(self, value: List[dvs.VmVnicNetworkResourcePool.RuntimeInfo]):
+        def vmVnicNetworkResourcePoolRuntime(self, value: List[vim.dvs.VmVnicNetworkResourcePool.RuntimeInfo]):
             self._vmVnicNetworkResourcePoolRuntime = value
 
 
     class RollbackCapability(vmodl.DynamicData):
         @property
         def rollbackSupported(self) -> bool: ...
         @rollbackSupported.setter
         def rollbackSupported(self, value: bool):
             self._rollbackSupported = value
 
 
     class RuntimeInfo(vmodl.DynamicData):
         @property
-        def hostMemberRuntime(self) -> List[dvs.HostMember.RuntimeInfo]: ...
+        def hostMemberRuntime(self) -> List[vim.dvs.HostMember.RuntimeInfo]: ...
         @hostMemberRuntime.setter
-        def hostMemberRuntime(self, value: List[dvs.HostMember.RuntimeInfo]):
+        def hostMemberRuntime(self, value: List[vim.dvs.HostMember.RuntimeInfo]):
             self._hostMemberRuntime = value
         @property
         def resourceRuntimeInfo(self) -> DistributedVirtualSwitch.ResourceRuntimeInfo: ...
         @resourceRuntimeInfo.setter
         def resourceRuntimeInfo(self, value: DistributedVirtualSwitch.ResourceRuntimeInfo):
             self._resourceRuntimeInfo = value
 
@@ -1764,17 +1783,17 @@
             self._uuid = value
         @property
         def numPorts(self) -> int: ...
         @numPorts.setter
         def numPorts(self, value: int):
             self._numPorts = value
         @property
-        def productInfo(self) -> dvs.ProductSpec: ...
+        def productInfo(self) -> vim.dvs.ProductSpec: ...
         @productInfo.setter
-        def productInfo(self, value: dvs.ProductSpec):
+        def productInfo(self, value: vim.dvs.ProductSpec):
             self._productInfo = value
         @property
         def hostMember(self) -> List[HostSystem]: ...
         @hostMember.setter
         def hostMember(self, value: List[HostSystem]):
             self._hostMember = value
         @property
@@ -1863,20 +1882,20 @@
         notifyAvailableUpgrade = "notifyAvailableUpgrade"
         proceedWithUpgrade = "proceedWithUpgrade"
         updateBundleInfo = "updateBundleInfo"
 
 
 class EnvironmentBrowser(ManagedObject):
     @property
-    def datastoreBrowser(self) -> host.DatastoreBrowser: ...
-    def QueryConfigOptionDescriptor(self) -> List[vm.ConfigOptionDescriptor]: ...
-    def QueryConfigOption(self, key: str, host: HostSystem) -> vm.ConfigOption: ...
-    def QueryConfigOptionEx(self, spec: EnvironmentBrowser.ConfigOptionQuerySpec) -> vm.ConfigOption: ...
-    def QueryConfigTarget(self, host: HostSystem) -> vm.ConfigTarget: ...
-    def QueryTargetCapabilities(self, host: HostSystem) -> host.Capability: ...
+    def datastoreBrowser(self) -> vim.host.DatastoreBrowser: ...
+    def QueryConfigOptionDescriptor(self) -> List[vim.vm.ConfigOptionDescriptor]: ...
+    def QueryConfigOption(self, key: str, host: HostSystem) -> vim.vm.ConfigOption: ...
+    def QueryConfigOptionEx(self, spec: EnvironmentBrowser.ConfigOptionQuerySpec) -> vim.vm.ConfigOption: ...
+    def QueryConfigTarget(self, host: HostSystem) -> vim.vm.ConfigTarget: ...
+    def QueryTargetCapabilities(self, host: HostSystem) -> vim.host.Capability: ...
 
 
     class ConfigOptionQuerySpec(vmodl.DynamicData):
         @property
         def key(self) -> str: ...
         @key.setter
         def key(self, value: str):
@@ -1941,19 +1960,19 @@
     def childType(self) -> List[type]: ...
     @property
     def childEntity(self) -> List[ManagedEntity]: ...
     @property
     def namespace(self) -> str: ...
     def CreateFolder(self, name: str) -> Folder: ...
     def MoveInto(self, list: List[ManagedEntity]) -> Task: ...
-    def CreateVm(self, config: vm.ConfigSpec, pool: ResourcePool, host: HostSystem) -> Task: ...
+    def CreateVm(self, config: vim.vm.ConfigSpec, pool: ResourcePool, host: HostSystem) -> Task: ...
     def RegisterVm(self, path: str, name: str, asTemplate: bool, pool: ResourcePool, host: HostSystem) -> Task: ...
-    def CreateCluster(self, name: str, spec: cluster.ConfigSpec) -> ClusterComputeResource: ...
-    def CreateClusterEx(self, name: str, spec: cluster.ConfigSpecEx) -> ClusterComputeResource: ...
-    def AddStandaloneHost(self, spec: host.ConnectSpec, compResSpec: ComputeResource.ConfigSpec, addConnected: bool, license: str) -> Task: ...
+    def CreateCluster(self, name: str, spec: vim.cluster.ConfigSpec) -> ClusterComputeResource: ...
+    def CreateClusterEx(self, name: str, spec: vim.cluster.ConfigSpecEx) -> ClusterComputeResource: ...
+    def AddStandaloneHost(self, spec: vim.host.ConnectSpec, compResSpec: ComputeResource.ConfigSpec, addConnected: bool, license: str) -> Task: ...
     def CreateDatacenter(self, name: str) -> Datacenter: ...
     def UnregisterAndDestroy(self) -> Task: ...
     def CreateDistributedVirtualSwitch(self, spec: DistributedVirtualSwitch.CreateSpec) -> Task: ...
     def CreateStoragePod(self, name: str) -> StoragePod: ...
     def BatchAddStandaloneHosts(self, newHosts: List[Folder.NewHostSpec], compResSpec: ComputeResource.ConfigSpec, addConnected: bool) -> Task: ...
     def BatchAddHostsToCluster(self, cluster: ClusterComputeResource, newHosts: List[Folder.NewHostSpec], existingHosts: List[HostSystem], compResSpec: ComputeResource.ConfigSpec, desiredState: str) -> Task: ...
 
@@ -2010,17 +2029,17 @@
         @fault.setter
         def fault(self, value: vmodl.MethodFault):
             self._fault = value
 
 
     class NewHostSpec(vmodl.DynamicData):
         @property
-        def hostCnxSpec(self) -> host.ConnectSpec: ...
+        def hostCnxSpec(self) -> vim.host.ConnectSpec: ...
         @hostCnxSpec.setter
-        def hostCnxSpec(self, value: host.ConnectSpec):
+        def hostCnxSpec(self, value: vim.host.ConnectSpec):
             self._hostCnxSpec = value
         @property
         def esxLicense(self) -> str: ...
         @esxLicense.setter
         def esxLicense(self, value: str):
             self._esxLicense = value
 
@@ -2061,75 +2080,75 @@
     def Rewind(self) -> NoneType: ...
     def Reset(self) -> NoneType: ...
     def Remove(self) -> NoneType: ...
 
 
 class HostSystem(ManagedEntity):
     @property
-    def runtime(self) -> host.RuntimeInfo: ...
+    def runtime(self) -> vim.host.RuntimeInfo: ...
     @property
-    def summary(self) -> host.Summary: ...
+    def summary(self) -> vim.host.Summary: ...
     @property
-    def hardware(self) -> host.HardwareInfo: ...
+    def hardware(self) -> vim.host.HardwareInfo: ...
     @property
-    def capability(self) -> host.Capability: ...
+    def capability(self) -> vim.host.Capability: ...
     @property
     def licensableResource(self) -> LicenseManager.LicensableResourceInfo: ...
     @property
     def remediationState(self) -> HostSystem.RemediationState: ...
     @property
-    def precheckRemediationResult(self) -> profile.host.ProfileManager.ApplyHostConfigSpec: ...
+    def precheckRemediationResult(self) -> vim.profile.host.ProfileManager.ApplyHostConfigSpec: ...
     @property
-    def remediationResult(self) -> profile.host.ProfileManager.ApplyHostConfigResult: ...
+    def remediationResult(self) -> vim.profile.host.ProfileManager.ApplyHostConfigResult: ...
     @property
     def complianceCheckState(self) -> HostSystem.ComplianceCheckState: ...
     @property
-    def complianceCheckResult(self) -> profile.ComplianceResult: ...
+    def complianceCheckResult(self) -> vim.profile.ComplianceResult: ...
     @property
-    def configManager(self) -> host.ConfigManager: ...
+    def configManager(self) -> vim.host.ConfigManager: ...
     @property
-    def config(self) -> host.ConfigInfo: ...
+    def config(self) -> vim.host.ConfigInfo: ...
     @property
     def vm(self) -> List[VirtualMachine]: ...
     @property
     def datastore(self) -> List[Datastore]: ...
     @property
     def network(self) -> List[Network]: ...
     @property
-    def datastoreBrowser(self) -> host.DatastoreBrowser: ...
+    def datastoreBrowser(self) -> vim.host.DatastoreBrowser: ...
     @property
-    def systemResources(self) -> host.SystemResourceInfo: ...
+    def systemResources(self) -> vim.host.SystemResourceInfo: ...
     @property
-    def answerFileValidationState(self) -> profile.host.AnswerFileStatusResult: ...
+    def answerFileValidationState(self) -> vim.profile.host.AnswerFileStatusResult: ...
     @property
-    def answerFileValidationResult(self) -> profile.host.AnswerFileStatusResult: ...
-    def QueryTpmAttestationReport(self) -> host.TpmAttestationReport: ...
-    def QueryConnectionInfo(self) -> host.ConnectInfo: ...
-    def UpdateSystemResources(self, resourceInfo: host.SystemResourceInfo) -> NoneType: ...
-    def UpdateSystemSwapConfiguration(self, sysSwapConfig: host.SystemSwapConfiguration) -> NoneType: ...
-    def Reconnect(self, cnxSpec: host.ConnectSpec, reconnectSpec: HostSystem.ReconnectSpec) -> Task: ...
+    def answerFileValidationResult(self) -> vim.profile.host.AnswerFileStatusResult: ...
+    def QueryTpmAttestationReport(self) -> vim.host.TpmAttestationReport: ...
+    def QueryConnectionInfo(self) -> vim.host.ConnectInfo: ...
+    def UpdateSystemResources(self, resourceInfo: vim.host.SystemResourceInfo) -> NoneType: ...
+    def UpdateSystemSwapConfiguration(self, sysSwapConfig: vim.host.SystemSwapConfiguration) -> NoneType: ...
+    def Reconnect(self, cnxSpec: vim.host.ConnectSpec, reconnectSpec: HostSystem.ReconnectSpec) -> Task: ...
     def Disconnect(self) -> Task: ...
-    def EnterMaintenanceMode(self, timeout: int, evacuatePoweredOffVms: bool, maintenanceSpec: host.MaintenanceSpec) -> Task: ...
+    def EnterMaintenanceMode(self, timeout: int, evacuatePoweredOffVms: bool, maintenanceSpec: vim.host.MaintenanceSpec) -> Task: ...
     def ExitMaintenanceMode(self, timeout: int) -> Task: ...
     def Reboot(self, force: bool) -> Task: ...
     def Shutdown(self, force: bool) -> Task: ...
     def EnterStandbyMode(self, timeoutSec: int, evacuatePoweredOffVms: bool) -> Task: ...
     def ExitStandbyMode(self, timeoutSec: int) -> Task: ...
     def QueryOverhead(self, memorySize: long, videoRamSize: int, numVcpus: int) -> long: ...
-    def QueryOverheadEx(self, vmConfigInfo: vm.ConfigInfo) -> long: ...
+    def QueryOverheadEx(self, vmConfigInfo: vim.vm.ConfigInfo) -> long: ...
     def ReconfigureDAS(self) -> Task: ...
-    def UpdateFlags(self, flagInfo: host.FlagInfo) -> NoneType: ...
+    def UpdateFlags(self, flagInfo: vim.host.FlagInfo) -> NoneType: ...
     def EnterLockdownMode(self) -> NoneType: ...
     def ExitLockdownMode(self) -> NoneType: ...
     def AcquireCimServicesTicket(self) -> HostServiceTicket: ...
-    def UpdateIpmi(self, ipmiInfo: host.IpmiInfo) -> NoneType: ...
+    def UpdateIpmi(self, ipmiInfo: vim.host.IpmiInfo) -> NoneType: ...
     def RetrieveHardwareUptime(self) -> long: ...
     def PrepareCrypto(self) -> NoneType: ...
-    def EnableCrypto(self, keyPlain: encryption.CryptoKeyPlain) -> NoneType: ...
-    def ConfigureCryptoKey(self, keyId: encryption.CryptoKeyId) -> NoneType: ...
+    def EnableCrypto(self, keyPlain: vim.encryption.CryptoKeyPlain) -> NoneType: ...
+    def ConfigureCryptoKey(self, keyId: vim.encryption.CryptoKeyId) -> NoneType: ...
     def QueryProductLockerLocation(self) -> str: ...
     def UpdateProductLockerLocation(self, path: str) -> Task: ...
     def RetrieveFreeEpcMemory(self) -> long: ...
 
 
     class ComplianceCheckState(vmodl.DynamicData):
         @property
@@ -2435,15 +2454,15 @@
     def InstallIoFilter(self, vibUrl: str, compRes: ComputeResource) -> Task: ...
     def UninstallIoFilter(self, filterId: str, compRes: ComputeResource) -> Task: ...
     def UpgradeIoFilter(self, filterId: str, compRes: ComputeResource, vibUrl: str) -> Task: ...
     def QueryIssue(self, filterId: str, compRes: ComputeResource) -> IoFilterManager.QueryIssueResult: ...
     def QueryIoFilterInfo(self, compRes: ComputeResource) -> List[IoFilterManager.ClusterIoFilterInfo]: ...
     def ResolveInstallationErrorsOnHost(self, filterId: str, host: HostSystem) -> Task: ...
     def ResolveInstallationErrorsOnCluster(self, filterId: str, cluster: ClusterComputeResource) -> Task: ...
-    def QueryDisksUsingFilter(self, filterId: str, compRes: ComputeResource) -> List[vm.device.VirtualDiskId]: ...
+    def QueryDisksUsingFilter(self, filterId: str, compRes: ComputeResource) -> List[vim.vm.device.VirtualDiskId]: ...
 
 
     class ClusterIoFilterInfo(IoFilterManager.IoFilterInfo):
         @property
         def opType(self) -> str: ...
         @opType.setter
         def opType(self, value: str):
@@ -2975,29 +2994,29 @@
     @property
     def customValue(self) -> List[CustomFieldsManager.Value]: ...
     @property
     def overallStatus(self) -> ManagedEntity.Status | Literal['gray', 'green', 'yellow', 'red']: ...
     @property
     def configStatus(self) -> ManagedEntity.Status | Literal['gray', 'green', 'yellow', 'red']: ...
     @property
-    def configIssue(self) -> List[event.Event]: ...
+    def configIssue(self) -> List[vim.event.Event]: ...
     @property
     def effectiveRole(self) -> List[int]: ...
     @property
     def permission(self) -> List[AuthorizationManager.Permission]: ...
     @property
     def name(self) -> str: ...
     @property
     def disabledMethod(self) -> List[ManagedMethod]: ...
     @property
     def recentTask(self) -> List[Task]: ...
     @property
-    def declaredAlarmState(self) -> List[alarm.AlarmState]: ...
+    def declaredAlarmState(self) -> List[vim.alarm.AlarmState]: ...
     @property
-    def triggeredAlarmState(self) -> List[alarm.AlarmState]: ...
+    def triggeredAlarmState(self) -> List[vim.alarm.AlarmState]: ...
     @property
     def alarmActionsEnabled(self) -> bool: ...
     @property
     def tag(self) -> List[Tag]: ...
     def Reload(self) -> NoneType: ...
     def Rename(self, newName: str) -> Task: ...
     def Destroy(self) -> Task: ...
@@ -3048,15 +3067,15 @@
             self._ipPoolId = value
 
 
 class OpaqueNetwork(Network):
     @property
     def capability(self) -> OpaqueNetwork.Capability: ...
     @property
-    def extraConfig(self) -> List[option.OptionValue]: ...
+    def extraConfig(self) -> List[vim.option.OptionValue]: ...
 
 
     class Capability(vmodl.DynamicData):
         @property
         def networkReservationSupported(self) -> bool: ...
         @networkReservationSupported.setter
         def networkReservationSupported(self, value: bool):
@@ -3137,17 +3156,17 @@
             self._includeImageFiles = value
         @property
         def exportOption(self) -> List[str]: ...
         @exportOption.setter
         def exportOption(self, value: List[str]):
             self._exportOption = value
         @property
-        def snapshot(self) -> vm.Snapshot: ...
+        def snapshot(self) -> vim.vm.Snapshot: ...
         @snapshot.setter
-        def snapshot(self, value: vm.Snapshot):
+        def snapshot(self, value: vim.vm.Snapshot):
             self._snapshot = value
 
 
     class CreateDescriptorResult(vmodl.DynamicData):
         @property
         def ovfDescriptor(self) -> str: ...
         @ovfDescriptor.setter
@@ -3925,15 +3944,15 @@
     def childConfiguration(self) -> List[ResourceConfigSpec]: ...
     def UpdateConfig(self, name: str, config: ResourceConfigSpec) -> NoneType: ...
     def MoveInto(self, list: List[ManagedEntity]) -> NoneType: ...
     def UpdateChildResourceConfiguration(self, spec: List[ResourceConfigSpec]) -> NoneType: ...
     def CreateResourcePool(self, name: str, spec: ResourceConfigSpec) -> ResourcePool: ...
     def DestroyChildren(self) -> NoneType: ...
     def CreateVApp(self, name: str, resSpec: ResourceConfigSpec, configSpec: vApp.VAppConfigSpec, vmFolder: Folder) -> VirtualApp: ...
-    def CreateVm(self, config: vm.ConfigSpec, host: HostSystem) -> Task: ...
+    def CreateVm(self, config: vim.vm.ConfigSpec, host: HostSystem) -> Task: ...
     def RegisterVm(self, path: str, name: str, host: HostSystem) -> Task: ...
     def ImportVApp(self, spec: ImportSpec, folder: Folder, host: HostSystem) -> HttpNfcLease: ...
     def QueryResourceConfigOption(self) -> ResourceConfigOption: ...
     def RefreshRuntime(self) -> NoneType: ...
 
 
     class ResourceUsage(vmodl.DynamicData):
@@ -4115,15 +4134,15 @@
     def serverClock(self) -> datetime: ...
     @property
     def capability(self) -> Capability: ...
     @property
     def content(self) -> ServiceInstanceContent: ...
     def CurrentTime(self) -> datetime: ...
     def RetrieveContent(self) -> ServiceInstanceContent: ...
-    def ValidateMigration(self, vm: List[VirtualMachine], state: VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended'], testType: List[str], pool: ResourcePool, host: HostSystem) -> List[event.Event]: ...
+    def ValidateMigration(self, vm: List[VirtualMachine], state: VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended'], testType: List[str], pool: ResourcePool, host: HostSystem) -> List[vim.event.Event]: ...
     def QueryVMotionCompatibility(self, vm: VirtualMachine, host: List[HostSystem], compatibility: List[str]) -> List[ServiceInstance.HostVMotionCompatibility]: ...
     def RetrieveProductComponents(self) -> List[ServiceInstance.ProductComponentInfo]: ...
 
 
     class HostVMotionCompatibility(vmodl.DynamicData):
         @property
         def host(self) -> HostSystem: ...
@@ -4244,17 +4263,17 @@
             self._hostName = value
         @property
         def sslThumbprint(self) -> str: ...
         @sslThumbprint.setter
         def sslThumbprint(self, value: str):
             self._sslThumbprint = value
         @property
-        def certThumbprintList(self) -> List[vm.CertThumbprint]: ...
+        def certThumbprintList(self) -> List[vim.vm.CertThumbprint]: ...
         @certThumbprintList.setter
-        def certThumbprintList(self, value: List[vm.CertThumbprint]):
+        def certThumbprintList(self, value: List[vim.vm.CertThumbprint]):
             self._certThumbprintList = value
         @property
         def ticketType(self) -> str: ...
         @ticketType.setter
         def ticketType(self, value: str):
             self._ticketType = value
 
@@ -4390,17 +4409,17 @@
         @reservation.setter
         def reservation(self, value: int):
             self._reservation = value
 
 
     class IOAllocationOption(vmodl.DynamicData):
         @property
-        def limitOption(self) -> option.LongOption: ...
+        def limitOption(self) -> vim.option.LongOption: ...
         @limitOption.setter
-        def limitOption(self, value: option.LongOption):
+        def limitOption(self, value: vim.option.LongOption):
             self._limitOption = value
         @property
         def sharesOption(self) -> SharesOption: ...
         @sharesOption.setter
         def sharesOption(self, value: SharesOption):
             self._sharesOption = value
 
@@ -4446,32 +4465,32 @@
         @reservableIopsThreshold.setter
         def reservableIopsThreshold(self, value: int):
             self._reservableIopsThreshold = value
 
 
     class IORMConfigOption(vmodl.DynamicData):
         @property
-        def enabledOption(self) -> option.BoolOption: ...
+        def enabledOption(self) -> vim.option.BoolOption: ...
         @enabledOption.setter
-        def enabledOption(self, value: option.BoolOption):
+        def enabledOption(self, value: vim.option.BoolOption):
             self._enabledOption = value
         @property
-        def congestionThresholdOption(self) -> option.IntOption: ...
+        def congestionThresholdOption(self) -> vim.option.IntOption: ...
         @congestionThresholdOption.setter
-        def congestionThresholdOption(self, value: option.IntOption):
+        def congestionThresholdOption(self, value: vim.option.IntOption):
             self._congestionThresholdOption = value
         @property
-        def statsCollectionEnabledOption(self) -> option.BoolOption: ...
+        def statsCollectionEnabledOption(self) -> vim.option.BoolOption: ...
         @statsCollectionEnabledOption.setter
-        def statsCollectionEnabledOption(self, value: option.BoolOption):
+        def statsCollectionEnabledOption(self, value: vim.option.BoolOption):
             self._statsCollectionEnabledOption = value
         @property
-        def reservationEnabledOption(self) -> option.BoolOption: ...
+        def reservationEnabledOption(self) -> vim.option.BoolOption: ...
         @reservationEnabledOption.setter
-        def reservationEnabledOption(self, value: option.BoolOption):
+        def reservationEnabledOption(self, value: vim.option.BoolOption):
             self._reservationEnabledOption = value
 
 
     class IORMConfigSpec(vmodl.DynamicData):
         @property
         def enabled(self) -> bool: ...
         @enabled.setter
@@ -4517,27 +4536,27 @@
     class PodStorageDrsEntry(vmodl.DynamicData):
         @property
         def storageDrsConfig(self) -> storageDrs.ConfigInfo: ...
         @storageDrsConfig.setter
         def storageDrsConfig(self, value: storageDrs.ConfigInfo):
             self._storageDrsConfig = value
         @property
-        def recommendation(self) -> List[cluster.Recommendation]: ...
+        def recommendation(self) -> List[vim.cluster.Recommendation]: ...
         @recommendation.setter
-        def recommendation(self, value: List[cluster.Recommendation]):
+        def recommendation(self, value: List[vim.cluster.Recommendation]):
             self._recommendation = value
         @property
-        def drsFault(self) -> List[cluster.DrsFaults]: ...
+        def drsFault(self) -> List[vim.cluster.DrsFaults]: ...
         @drsFault.setter
-        def drsFault(self, value: List[cluster.DrsFaults]):
+        def drsFault(self, value: List[vim.cluster.DrsFaults]):
             self._drsFault = value
         @property
-        def actionHistory(self) -> List[cluster.ActionHistory]: ...
+        def actionHistory(self) -> List[vim.cluster.ActionHistory]: ...
         @actionHistory.setter
-        def actionHistory(self, value: List[cluster.ActionHistory]):
+        def actionHistory(self, value: List[vim.cluster.ActionHistory]):
             self._actionHistory = value
 
 
     class StoragePerformanceSummary(vmodl.DynamicData):
         @property
         def interval(self) -> int: ...
         @interval.setter
@@ -4706,26 +4725,26 @@
         starting = "starting"
         stopping = "stopping"
 
 
 class VirtualDiskManager(ManagedObject):
     def CreateVirtualDisk(self, name: str, datacenter: Datacenter, spec: VirtualDiskManager.VirtualDiskSpec) -> Task: ...
     def DeleteVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
-    def MoveVirtualDisk(self, sourceName: str, sourceDatacenter: Datacenter, destName: str, destDatacenter: Datacenter, force: bool, profile: List[vm.ProfileSpec]) -> Task: ...
+    def MoveVirtualDisk(self, sourceName: str, sourceDatacenter: Datacenter, destName: str, destDatacenter: Datacenter, force: bool, profile: List[vim.vm.ProfileSpec]) -> Task: ...
     def CopyVirtualDisk(self, sourceName: str, sourceDatacenter: Datacenter, destName: str, destDatacenter: Datacenter, destSpec: VirtualDiskManager.VirtualDiskSpec, force: bool) -> Task: ...
     def ExtendVirtualDisk(self, name: str, datacenter: Datacenter, newCapacityKb: long, eagerZero: bool) -> Task: ...
     def QueryVirtualDiskFragmentation(self, name: str, datacenter: Datacenter) -> int: ...
     def DefragmentVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
     def ShrinkVirtualDisk(self, name: str, datacenter: Datacenter, copy: bool) -> Task: ...
     def InflateVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
     def EagerZeroVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
     def ZeroFillVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
     def SetVirtualDiskUuid(self, name: str, datacenter: Datacenter, uuid: str) -> NoneType: ...
     def QueryVirtualDiskUuid(self, name: str, datacenter: Datacenter) -> str: ...
-    def QueryVirtualDiskGeometry(self, name: str, datacenter: Datacenter) -> host.DiskDimensions.Chs: ...
+    def QueryVirtualDiskGeometry(self, name: str, datacenter: Datacenter) -> vim.host.DiskDimensions.Chs: ...
     def ImportUnmanagedSnapshot(self, vdisk: str, datacenter: Datacenter, vvolId: str) -> NoneType: ...
     def ReleaseManagedSnapshot(self, vdisk: str, datacenter: Datacenter) -> NoneType: ...
 
 
     class DeviceBackedVirtualDiskSpec(VirtualDiskManager.VirtualDiskSpec):
         @property
         def device(self) -> str: ...
@@ -4737,22 +4756,22 @@
     class FileBackedVirtualDiskSpec(VirtualDiskManager.VirtualDiskSpec):
         @property
         def capacityKb(self) -> long: ...
         @capacityKb.setter
         def capacityKb(self, value: long):
             self._capacityKb = value
         @property
-        def profile(self) -> List[vm.ProfileSpec]: ...
+        def profile(self) -> List[vim.vm.ProfileSpec]: ...
         @profile.setter
-        def profile(self, value: List[vm.ProfileSpec]):
+        def profile(self, value: List[vim.vm.ProfileSpec]):
             self._profile = value
         @property
-        def crypto(self) -> encryption.CryptoSpec: ...
+        def crypto(self) -> vim.encryption.CryptoSpec: ...
         @crypto.setter
-        def crypto(self, value: encryption.CryptoSpec):
+        def crypto(self, value: vim.encryption.CryptoSpec):
             self._crypto = value
 
 
     class SeSparseVirtualDiskSpec(VirtualDiskManager.FileBackedVirtualDiskSpec):
         @property
         def grainSizeKb(self) -> int: ...
         @grainSizeKb.setter
@@ -4793,71 +4812,71 @@
         sparseMonolithic = "sparseMonolithic"
         flatMonolithic = "flatMonolithic"
         thick = "thick"
 
 
 class VirtualMachine(ManagedEntity):
     @property
-    def capability(self) -> vm.Capability: ...
+    def capability(self) -> vim.vm.Capability: ...
     @property
-    def config(self) -> vm.ConfigInfo: ...
+    def config(self) -> vim.vm.ConfigInfo: ...
     @property
-    def layout(self) -> vm.FileLayout: ...
+    def layout(self) -> vim.vm.FileLayout: ...
     @property
-    def layoutEx(self) -> vm.FileLayoutEx: ...
+    def layoutEx(self) -> vim.vm.FileLayoutEx: ...
     @property
-    def storage(self) -> vm.StorageInfo: ...
+    def storage(self) -> vim.vm.StorageInfo: ...
     @property
     def environmentBrowser(self) -> EnvironmentBrowser: ...
     @property
     def resourcePool(self) -> ResourcePool: ...
     @property
     def parentVApp(self) -> ManagedEntity: ...
     @property
     def resourceConfig(self) -> ResourceConfigSpec: ...
     @property
-    def runtime(self) -> vm.RuntimeInfo: ...
+    def runtime(self) -> vim.vm.RuntimeInfo: ...
     @property
-    def guest(self) -> vm.GuestInfo: ...
+    def guest(self) -> vim.vm.GuestInfo: ...
     @property
-    def summary(self) -> vm.Summary: ...
+    def summary(self) -> vim.vm.Summary: ...
     @property
     def datastore(self) -> List[Datastore]: ...
     @property
     def network(self) -> List[Network]: ...
     @property
-    def snapshot(self) -> vm.SnapshotInfo: ...
+    def snapshot(self) -> vim.vm.SnapshotInfo: ...
     @property
-    def rootSnapshot(self) -> List[vm.Snapshot]: ...
+    def rootSnapshot(self) -> List[vim.vm.Snapshot]: ...
     @property
     def guestHeartbeatStatus(self) -> ManagedEntity.Status | Literal['gray', 'green', 'yellow', 'red']: ...
     def RefreshStorageInfo(self) -> NoneType: ...
     def CreateSnapshot(self, name: str, description: str, memory: bool, quiesce: bool) -> Task: ...
-    def CreateSnapshotEx(self, name: str, description: str, memory: bool, quiesceSpec: vm.GuestQuiesceSpec) -> Task: ...
+    def CreateSnapshotEx(self, name: str, description: str, memory: bool, quiesceSpec: vim.vm.GuestQuiesceSpec) -> Task: ...
     def RevertToCurrentSnapshot(self, host: HostSystem, suppressPowerOn: bool) -> Task: ...
     def RemoveAllSnapshots(self, consolidate: bool) -> Task: ...
     def ConsolidateDisks(self) -> Task: ...
     def EstimateStorageRequirementForConsolidate(self) -> Task: ...
-    def Reconfigure(self, spec: vm.ConfigSpec) -> Task: ...
+    def Reconfigure(self, spec: vim.vm.ConfigSpec) -> Task: ...
     def UpgradeVirtualHardware(self, version: str) -> Task: ...
     def ExtractOvfEnvironment(self) -> str: ...
     def PowerOn(self, host: HostSystem) -> Task: ...
     def PowerOff(self) -> Task: ...
     def Suspend(self) -> Task: ...
     def Reset(self) -> Task: ...
     def ShutdownGuest(self) -> NoneType: ...
     def RebootGuest(self) -> NoneType: ...
     def StandbyGuest(self) -> NoneType: ...
     def Answer(self, questionId: str, answerChoice: str) -> NoneType: ...
-    def Customize(self, spec: vm.customization.Specification) -> Task: ...
-    def CheckCustomizationSpec(self, spec: vm.customization.Specification) -> NoneType: ...
+    def Customize(self, spec: vim.vm.customization.Specification) -> Task: ...
+    def CheckCustomizationSpec(self, spec: vim.vm.customization.Specification) -> NoneType: ...
     def Migrate(self, pool: ResourcePool, host: HostSystem, priority: VirtualMachine.MovePriority | Literal['lowPriority', 'highPriority', 'defaultPriority'], state: VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended']) -> Task: ...
-    def Relocate(self, spec: vm.RelocateSpec, priority: VirtualMachine.MovePriority | Literal['lowPriority', 'highPriority', 'defaultPriority']) -> Task: ...
-    def Clone(self, folder: Folder, name: str, spec: vm.CloneSpec) -> Task: ...
-    def InstantClone(self, spec: vm.InstantCloneSpec) -> Task: ...
+    def Relocate(self, spec: vim.vm.RelocateSpec, priority: VirtualMachine.MovePriority | Literal['lowPriority', 'highPriority', 'defaultPriority']) -> Task: ...
+    def Clone(self, folder: Folder, name: str, spec: vim.vm.CloneSpec) -> Task: ...
+    def InstantClone(self, spec: vim.vm.InstantCloneSpec) -> Task: ...
     def ExportVm(self) -> HttpNfcLease: ...
     def MarkAsTemplate(self) -> NoneType: ...
     def MarkAsVirtualMachine(self, pool: ResourcePool, host: HostSystem) -> NoneType: ...
     def Unregister(self) -> NoneType: ...
     def ResetGuestInformation(self) -> NoneType: ...
     def MountToolsInstaller(self) -> NoneType: ...
     def UnmountToolsInstaller(self) -> NoneType: ...
@@ -4865,38 +4884,38 @@
     def AcquireMksTicket(self) -> VirtualMachine.MksTicket: ...
     def QueryConnections(self) -> List[VirtualMachine.Connection]: ...
     def DropConnections(self, listOfConnections: List[VirtualMachine.Connection]) -> bool: ...
     def AcquireTicket(self, ticketType: str) -> VirtualMachine.Ticket: ...
     def SetScreenResolution(self, width: int, height: int) -> NoneType: ...
     def DefragmentAllDisks(self) -> NoneType: ...
     def CreateSecondary(self, host: HostSystem) -> Task: ...
-    def CreateSecondaryEx(self, host: HostSystem, spec: vm.FaultToleranceConfigSpec) -> Task: ...
+    def CreateSecondaryEx(self, host: HostSystem, spec: vim.vm.FaultToleranceConfigSpec) -> Task: ...
     def TurnOffFaultTolerance(self) -> Task: ...
     def MakePrimary(self, vm: VirtualMachine) -> Task: ...
     def TerminateFaultTolerantVM(self, vm: VirtualMachine) -> Task: ...
     def DisableSecondary(self, vm: VirtualMachine) -> Task: ...
     def EnableSecondary(self, vm: VirtualMachine, host: HostSystem) -> Task: ...
     def SetDisplayTopology(self, displays: List[VirtualMachine.DisplayTopology]) -> NoneType: ...
     def StartRecording(self, name: str, description: str) -> Task: ...
     def StopRecording(self) -> Task: ...
-    def StartReplaying(self, replaySnapshot: vm.Snapshot) -> Task: ...
+    def StartReplaying(self, replaySnapshot: vim.vm.Snapshot) -> Task: ...
     def StopReplaying(self) -> Task: ...
-    def PromoteDisks(self, unlink: bool, disks: List[vm.device.VirtualDisk]) -> Task: ...
+    def PromoteDisks(self, unlink: bool, disks: List[vim.vm.device.VirtualDisk]) -> Task: ...
     def CreateScreenshot(self) -> Task: ...
-    def PutUsbScanCodes(self, spec: vm.UsbScanCodeSpec) -> int: ...
-    def QueryChangedDiskAreas(self, snapshot: vm.Snapshot, deviceKey: int, startOffset: long, changeId: str) -> VirtualMachine.DiskChangeInfo: ...
+    def PutUsbScanCodes(self, spec: vim.vm.UsbScanCodeSpec) -> int: ...
+    def QueryChangedDiskAreas(self, snapshot: vim.vm.Snapshot, deviceKey: int, startOffset: long, changeId: str) -> VirtualMachine.DiskChangeInfo: ...
     def QueryUnownedFiles(self) -> List[str]: ...
     def ReloadFromPath(self, configurationPath: str) -> Task: ...
     def QueryFaultToleranceCompatibility(self) -> List[vmodl.MethodFault]: ...
     def QueryFaultToleranceCompatibilityEx(self, forLegacyFt: bool) -> List[vmodl.MethodFault]: ...
     def Terminate(self) -> NoneType: ...
     def SendNMI(self) -> NoneType: ...
-    def AttachDisk(self, diskId: vslm.ID, datastore: Datastore, controllerKey: int, unitNumber: int) -> Task: ...
-    def DetachDisk(self, diskId: vslm.ID) -> Task: ...
-    def ApplyEvcMode(self, mask: List[host.FeatureMask], completeMasks: bool) -> Task: ...
+    def AttachDisk(self, diskId: vim.vslm.ID, datastore: Datastore, controllerKey: int, unitNumber: int) -> Task: ...
+    def DetachDisk(self, diskId: vim.vslm.ID) -> Task: ...
+    def ApplyEvcMode(self, mask: List[vim.host.FeatureMask], completeMasks: bool) -> Task: ...
     def CryptoUnlock(self) -> Task: ...
 
 
     class Connection(vmodl.DynamicData):
         @property
         def label(self) -> str: ...
         @label.setter
@@ -5035,17 +5054,17 @@
             self._port = value
         @property
         def sslThumbprint(self) -> str: ...
         @sslThumbprint.setter
         def sslThumbprint(self, value: str):
             self._sslThumbprint = value
         @property
-        def certThumbprintList(self) -> List[vm.CertThumbprint]: ...
+        def certThumbprintList(self) -> List[vim.vm.CertThumbprint]: ...
         @certThumbprintList.setter
-        def certThumbprintList(self, value: List[vm.CertThumbprint]):
+        def certThumbprintList(self, value: List[vim.vm.CertThumbprint]):
             self._certThumbprintList = value
         @property
         def url(self) -> str: ...
         @url.setter
         def url(self, value: str):
             self._url = value
 
@@ -5182,17 +5201,17 @@
     class PreflightCheckResult(vmodl.DynamicData):
         @property
         def issues(self) -> List[VsanUpgradeSystem.PreflightCheckIssue]: ...
         @issues.setter
         def issues(self, value: List[VsanUpgradeSystem.PreflightCheckIssue]):
             self._issues = value
         @property
-        def diskMappingToRestore(self) -> vsan.host.DiskMapping: ...
+        def diskMappingToRestore(self) -> vim.vsan.host.DiskMapping: ...
         @diskMappingToRestore.setter
-        def diskMappingToRestore(self, value: vsan.host.DiskMapping):
+        def diskMappingToRestore(self, value: vim.vsan.host.DiskMapping):
             self._diskMappingToRestore = value
 
 
     class RogueHostsInClusterIssue(VsanUpgradeSystem.PreflightCheckIssue):
         @property
         def uuids(self) -> List[str]: ...
         @uuids.setter
@@ -5203,17 +5222,17 @@
     class UpgradeHistoryDiskGroupOp(VsanUpgradeSystem.UpgradeHistoryItem):
         @property
         def operation(self) -> str: ...
         @operation.setter
         def operation(self, value: str):
             self._operation = value
         @property
-        def diskMapping(self) -> vsan.host.DiskMapping: ...
+        def diskMapping(self) -> vim.vsan.host.DiskMapping: ...
         @diskMapping.setter
-        def diskMapping(self, value: vsan.host.DiskMapping):
+        def diskMapping(self, value: vim.vsan.host.DiskMapping):
             self._diskMapping = value
 
 
     class UpgradeHistoryItem(vmodl.DynamicData):
         @property
         def timestamp(self) -> datetime: ...
         @timestamp.setter
@@ -5529,17 +5548,17 @@
 class CustomizationSpecItem(vmodl.DynamicData):
     @property
     def info(self) -> CustomizationSpecInfo: ...
     @info.setter
     def info(self, value: CustomizationSpecInfo):
         self._info = value
     @property
-    def spec(self) -> vm.customization.Specification: ...
+    def spec(self) -> vim.vm.customization.Specification: ...
     @spec.setter
-    def spec(self, value: vm.customization.Specification):
+    def spec(self, value: vim.vm.customization.Specification):
         self._spec = value
 
 
 class Description(vmodl.DynamicData):
     @property
     def label(self) -> str: ...
     @label.setter
@@ -5602,32 +5621,32 @@
         @version.setter
         def version(self, value: str):
             self._version = value
 
 
 class EVCMode(ElementDescription):
     @property
-    def guaranteedCPUFeatures(self) -> List[host.CpuIdInfo]: ...
+    def guaranteedCPUFeatures(self) -> List[vim.host.CpuIdInfo]: ...
     @guaranteedCPUFeatures.setter
-    def guaranteedCPUFeatures(self, value: List[host.CpuIdInfo]):
+    def guaranteedCPUFeatures(self, value: List[vim.host.CpuIdInfo]):
         self._guaranteedCPUFeatures = value
     @property
-    def featureCapability(self) -> List[host.FeatureCapability]: ...
+    def featureCapability(self) -> List[vim.host.FeatureCapability]: ...
     @featureCapability.setter
-    def featureCapability(self, value: List[host.FeatureCapability]):
+    def featureCapability(self, value: List[vim.host.FeatureCapability]):
         self._featureCapability = value
     @property
-    def featureMask(self) -> List[host.FeatureMask]: ...
+    def featureMask(self) -> List[vim.host.FeatureMask]: ...
     @featureMask.setter
-    def featureMask(self, value: List[host.FeatureMask]):
+    def featureMask(self, value: List[vim.host.FeatureMask]):
         self._featureMask = value
     @property
-    def featureRequirement(self) -> List[vm.FeatureRequirement]: ...
+    def featureRequirement(self) -> List[vim.vm.FeatureRequirement]: ...
     @featureRequirement.setter
-    def featureRequirement(self, value: List[vm.FeatureRequirement]):
+    def featureRequirement(self, value: List[vim.vm.FeatureRequirement]):
         self._featureRequirement = value
     @property
     def vendor(self) -> str: ...
     @vendor.setter
     def vendor(self, value: str):
         self._vendor = value
     @property
@@ -5767,32 +5786,32 @@
         self._healthInfo = value
     @property
     def ovfConsumerInfo(self) -> Extension.OvfConsumerInfo: ...
     @ovfConsumerInfo.setter
     def ovfConsumerInfo(self, value: Extension.OvfConsumerInfo):
         self._ovfConsumerInfo = value
     @property
-    def extendedProductInfo(self) -> ext.ExtendedProductInfo: ...
+    def extendedProductInfo(self) -> vim.ext.ExtendedProductInfo: ...
     @extendedProductInfo.setter
-    def extendedProductInfo(self, value: ext.ExtendedProductInfo):
+    def extendedProductInfo(self, value: vim.ext.ExtendedProductInfo):
         self._extendedProductInfo = value
     @property
-    def managedEntityInfo(self) -> List[ext.ManagedEntityInfo]: ...
+    def managedEntityInfo(self) -> List[vim.ext.ManagedEntityInfo]: ...
     @managedEntityInfo.setter
-    def managedEntityInfo(self, value: List[ext.ManagedEntityInfo]):
+    def managedEntityInfo(self, value: List[vim.ext.ManagedEntityInfo]):
         self._managedEntityInfo = value
     @property
     def shownInSolutionManager(self) -> bool: ...
     @shownInSolutionManager.setter
     def shownInSolutionManager(self, value: bool):
         self._shownInSolutionManager = value
     @property
-    def solutionManagerInfo(self) -> ext.SolutionManagerInfo: ...
+    def solutionManagerInfo(self) -> vim.ext.SolutionManagerInfo: ...
     @solutionManagerInfo.setter
-    def solutionManagerInfo(self, value: ext.SolutionManagerInfo):
+    def solutionManagerInfo(self, value: vim.ext.SolutionManagerInfo):
         self._solutionManagerInfo = value
 
 
     class ClientInfo(vmodl.DynamicData):
         @property
         def version(self) -> str: ...
         @version.setter
@@ -5958,27 +5977,27 @@
     @faults.setter
     def faults(self, value: List[vmodl.MethodFault]):
         self._faults = value
 
 
 class FeatureEVCMode(ElementDescription):
     @property
-    def mask(self) -> List[host.FeatureMask]: ...
+    def mask(self) -> List[vim.host.FeatureMask]: ...
     @mask.setter
-    def mask(self, value: List[host.FeatureMask]):
+    def mask(self, value: List[vim.host.FeatureMask]):
         self._mask = value
     @property
-    def capability(self) -> List[host.FeatureCapability]: ...
+    def capability(self) -> List[vim.host.FeatureCapability]: ...
     @capability.setter
-    def capability(self, value: List[host.FeatureCapability]):
+    def capability(self, value: List[vim.host.FeatureCapability]):
         self._capability = value
     @property
-    def requirement(self) -> List[vm.FeatureRequirement]: ...
+    def requirement(self) -> List[vim.vm.FeatureRequirement]: ...
     @requirement.setter
-    def requirement(self, value: List[vm.FeatureRequirement]):
+    def requirement(self, value: List[vim.vm.FeatureRequirement]):
         self._requirement = value
 
 
 class HbrManager():
 
 
     class ReplicationVmInfo(vmodl.DynamicData):
@@ -6548,27 +6567,27 @@
         self._rootFolder = value
     @property
     def propertyCollector(self) -> vmodl.query.PropertyCollector: ...
     @propertyCollector.setter
     def propertyCollector(self, value: vmodl.query.PropertyCollector):
         self._propertyCollector = value
     @property
-    def viewManager(self) -> view.ViewManager: ...
+    def viewManager(self) -> vim.view.ViewManager: ...
     @viewManager.setter
-    def viewManager(self, value: view.ViewManager):
+    def viewManager(self, value: vim.view.ViewManager):
         self._viewManager = value
     @property
     def about(self) -> AboutInfo: ...
     @about.setter
     def about(self, value: AboutInfo):
         self._about = value
     @property
-    def setting(self) -> option.OptionManager: ...
+    def setting(self) -> vim.option.OptionManager: ...
     @setting.setter
-    def setting(self, value: option.OptionManager):
+    def setting(self, value: vim.option.OptionManager):
         self._setting = value
     @property
     def userDirectory(self) -> UserDirectory: ...
     @userDirectory.setter
     def userDirectory(self, value: UserDirectory):
         self._userDirectory = value
     @property
@@ -6588,27 +6607,27 @@
         self._serviceManager = value
     @property
     def perfManager(self) -> PerformanceManager: ...
     @perfManager.setter
     def perfManager(self, value: PerformanceManager):
         self._perfManager = value
     @property
-    def scheduledTaskManager(self) -> scheduler.ScheduledTaskManager: ...
+    def scheduledTaskManager(self) -> vim.scheduler.ScheduledTaskManager: ...
     @scheduledTaskManager.setter
-    def scheduledTaskManager(self, value: scheduler.ScheduledTaskManager):
+    def scheduledTaskManager(self, value: vim.scheduler.ScheduledTaskManager):
         self._scheduledTaskManager = value
     @property
-    def alarmManager(self) -> alarm.AlarmManager: ...
+    def alarmManager(self) -> vim.alarm.AlarmManager: ...
     @alarmManager.setter
-    def alarmManager(self, value: alarm.AlarmManager):
+    def alarmManager(self, value: vim.alarm.AlarmManager):
         self._alarmManager = value
     @property
-    def eventManager(self) -> event.EventManager: ...
+    def eventManager(self) -> vim.event.EventManager: ...
     @eventManager.setter
-    def eventManager(self, value: event.EventManager):
+    def eventManager(self, value: vim.event.EventManager):
         self._eventManager = value
     @property
     def taskManager(self) -> TaskManager: ...
     @taskManager.setter
     def taskManager(self, value: TaskManager):
         self._taskManager = value
     @property
@@ -6618,27 +6637,27 @@
         self._extensionManager = value
     @property
     def customizationSpecManager(self) -> CustomizationSpecManager: ...
     @customizationSpecManager.setter
     def customizationSpecManager(self, value: CustomizationSpecManager):
         self._customizationSpecManager = value
     @property
-    def guestCustomizationManager(self) -> vm.GuestCustomizationManager: ...
+    def guestCustomizationManager(self) -> vim.vm.GuestCustomizationManager: ...
     @guestCustomizationManager.setter
-    def guestCustomizationManager(self, value: vm.GuestCustomizationManager):
+    def guestCustomizationManager(self, value: vim.vm.GuestCustomizationManager):
         self._guestCustomizationManager = value
     @property
     def customFieldsManager(self) -> CustomFieldsManager: ...
     @customFieldsManager.setter
     def customFieldsManager(self, value: CustomFieldsManager):
         self._customFieldsManager = value
     @property
-    def accountManager(self) -> host.LocalAccountManager: ...
+    def accountManager(self) -> vim.host.LocalAccountManager: ...
     @accountManager.setter
-    def accountManager(self, value: host.LocalAccountManager):
+    def accountManager(self, value: vim.host.LocalAccountManager):
         self._accountManager = value
     @property
     def diagnosticManager(self) -> DiagnosticManager: ...
     @diagnosticManager.setter
     def diagnosticManager(self, value: DiagnosticManager):
         self._diagnosticManager = value
     @property
@@ -6668,72 +6687,72 @@
         self._virtualDiskManager = value
     @property
     def virtualizationManager(self) -> VirtualizationManager: ...
     @virtualizationManager.setter
     def virtualizationManager(self, value: VirtualizationManager):
         self._virtualizationManager = value
     @property
-    def snmpSystem(self) -> host.SnmpSystem: ...
+    def snmpSystem(self) -> vim.host.SnmpSystem: ...
     @snmpSystem.setter
-    def snmpSystem(self, value: host.SnmpSystem):
+    def snmpSystem(self, value: vim.host.SnmpSystem):
         self._snmpSystem = value
     @property
-    def vmProvisioningChecker(self) -> vm.check.ProvisioningChecker: ...
+    def vmProvisioningChecker(self) -> vim.vm.check.ProvisioningChecker: ...
     @vmProvisioningChecker.setter
-    def vmProvisioningChecker(self, value: vm.check.ProvisioningChecker):
+    def vmProvisioningChecker(self, value: vim.vm.check.ProvisioningChecker):
         self._vmProvisioningChecker = value
     @property
-    def vmCompatibilityChecker(self) -> vm.check.CompatibilityChecker: ...
+    def vmCompatibilityChecker(self) -> vim.vm.check.CompatibilityChecker: ...
     @vmCompatibilityChecker.setter
-    def vmCompatibilityChecker(self, value: vm.check.CompatibilityChecker):
+    def vmCompatibilityChecker(self, value: vim.vm.check.CompatibilityChecker):
         self._vmCompatibilityChecker = value
     @property
     def ovfManager(self) -> OvfManager: ...
     @ovfManager.setter
     def ovfManager(self, value: OvfManager):
         self._ovfManager = value
     @property
     def ipPoolManager(self) -> IpPoolManager: ...
     @ipPoolManager.setter
     def ipPoolManager(self, value: IpPoolManager):
         self._ipPoolManager = value
     @property
-    def dvSwitchManager(self) -> dvs.DistributedVirtualSwitchManager: ...
+    def dvSwitchManager(self) -> vim.dvs.DistributedVirtualSwitchManager: ...
     @dvSwitchManager.setter
-    def dvSwitchManager(self, value: dvs.DistributedVirtualSwitchManager):
+    def dvSwitchManager(self, value: vim.dvs.DistributedVirtualSwitchManager):
         self._dvSwitchManager = value
     @property
-    def hostProfileManager(self) -> profile.host.ProfileManager: ...
+    def hostProfileManager(self) -> vim.profile.host.ProfileManager: ...
     @hostProfileManager.setter
-    def hostProfileManager(self, value: profile.host.ProfileManager):
+    def hostProfileManager(self, value: vim.profile.host.ProfileManager):
         self._hostProfileManager = value
     @property
-    def clusterProfileManager(self) -> profile.cluster.ProfileManager: ...
+    def clusterProfileManager(self) -> vim.profile.cluster.ProfileManager: ...
     @clusterProfileManager.setter
-    def clusterProfileManager(self, value: profile.cluster.ProfileManager):
+    def clusterProfileManager(self, value: vim.profile.cluster.ProfileManager):
         self._clusterProfileManager = value
     @property
-    def complianceManager(self) -> profile.ComplianceManager: ...
+    def complianceManager(self) -> vim.profile.ComplianceManager: ...
     @complianceManager.setter
-    def complianceManager(self, value: profile.ComplianceManager):
+    def complianceManager(self, value: vim.profile.ComplianceManager):
         self._complianceManager = value
     @property
     def localizationManager(self) -> LocalizationManager: ...
     @localizationManager.setter
     def localizationManager(self, value: LocalizationManager):
         self._localizationManager = value
     @property
     def storageResourceManager(self) -> StorageResourceManager: ...
     @storageResourceManager.setter
     def storageResourceManager(self, value: StorageResourceManager):
         self._storageResourceManager = value
     @property
-    def guestOperationsManager(self) -> vm.guest.GuestOperationsManager: ...
+    def guestOperationsManager(self) -> vim.vm.guest.GuestOperationsManager: ...
     @guestOperationsManager.setter
-    def guestOperationsManager(self, value: vm.guest.GuestOperationsManager):
+    def guestOperationsManager(self, value: vim.vm.guest.GuestOperationsManager):
         self._guestOperationsManager = value
     @property
     def overheadMemoryManager(self) -> OverheadMemoryManager: ...
     @overheadMemoryManager.setter
     def overheadMemoryManager(self, value: OverheadMemoryManager):
         self._overheadMemoryManager = value
     @property
@@ -6743,47 +6762,47 @@
         self._certificateManager = value
     @property
     def ioFilterManager(self) -> IoFilterManager: ...
     @ioFilterManager.setter
     def ioFilterManager(self, value: IoFilterManager):
         self._ioFilterManager = value
     @property
-    def vStorageObjectManager(self) -> vslm.VStorageObjectManagerBase: ...
+    def vStorageObjectManager(self) -> vim.vslm.VStorageObjectManagerBase: ...
     @vStorageObjectManager.setter
-    def vStorageObjectManager(self, value: vslm.VStorageObjectManagerBase):
+    def vStorageObjectManager(self, value: vim.vslm.VStorageObjectManagerBase):
         self._vStorageObjectManager = value
     @property
-    def hostSpecManager(self) -> profile.host.HostSpecificationManager: ...
+    def hostSpecManager(self) -> vim.profile.host.HostSpecificationManager: ...
     @hostSpecManager.setter
-    def hostSpecManager(self, value: profile.host.HostSpecificationManager):
+    def hostSpecManager(self, value: vim.profile.host.HostSpecificationManager):
         self._hostSpecManager = value
     @property
-    def cryptoManager(self) -> encryption.CryptoManager: ...
+    def cryptoManager(self) -> vim.encryption.CryptoManager: ...
     @cryptoManager.setter
-    def cryptoManager(self, value: encryption.CryptoManager):
+    def cryptoManager(self, value: vim.encryption.CryptoManager):
         self._cryptoManager = value
     @property
     def healthUpdateManager(self) -> HealthUpdateManager: ...
     @healthUpdateManager.setter
     def healthUpdateManager(self, value: HealthUpdateManager):
         self._healthUpdateManager = value
     @property
-    def failoverClusterConfigurator(self) -> vcha.FailoverClusterConfigurator: ...
+    def failoverClusterConfigurator(self) -> vim.vcha.FailoverClusterConfigurator: ...
     @failoverClusterConfigurator.setter
-    def failoverClusterConfigurator(self, value: vcha.FailoverClusterConfigurator):
+    def failoverClusterConfigurator(self, value: vim.vcha.FailoverClusterConfigurator):
         self._failoverClusterConfigurator = value
     @property
-    def failoverClusterManager(self) -> vcha.FailoverClusterManager: ...
+    def failoverClusterManager(self) -> vim.vcha.FailoverClusterManager: ...
     @failoverClusterManager.setter
-    def failoverClusterManager(self, value: vcha.FailoverClusterManager):
+    def failoverClusterManager(self, value: vim.vcha.FailoverClusterManager):
         self._failoverClusterManager = value
     @property
-    def tenantManager(self) -> tenant.TenantManager: ...
+    def tenantManager(self) -> vim.tenant.TenantManager: ...
     @tenantManager.setter
-    def tenantManager(self, value: tenant.TenantManager):
+    def tenantManager(self, value: vim.tenant.TenantManager):
         self._tenantManager = value
     @property
     def siteInfoManager(self) -> SiteInfoManager: ...
     @siteInfoManager.setter
     def siteInfoManager(self, value: SiteInfoManager):
         self._siteInfoManager = value
     @property
@@ -6858,17 +6877,17 @@
         normal = "normal"
         high = "high"
         custom = "custom"
 
 
 class SharesOption(vmodl.DynamicData):
     @property
-    def sharesOption(self) -> option.IntOption: ...
+    def sharesOption(self) -> vim.option.IntOption: ...
     @sharesOption.setter
-    def sharesOption(self, value: option.IntOption):
+    def sharesOption(self, value: vim.option.IntOption):
         self._sharesOption = value
     @property
     def defaultLevel(self) -> SharesInfo.Level | Literal['low', 'normal', 'high', 'custom']: ...
     @defaultLevel.setter
     def defaultLevel(self, value: SharesInfo.Level | Literal['low', 'normal', 'high', 'custom']):
         self._defaultLevel = value
 
@@ -6957,22 +6976,22 @@
         self._activationId = value
     @property
     def state(self) -> List[TaskInfo.State]: ...
     @state.setter
     def state(self, value: List[TaskInfo.State]):
         self._state = value
     @property
-    def alarm(self) -> alarm.Alarm: ...
+    def alarm(self) -> vim.alarm.Alarm: ...
     @alarm.setter
-    def alarm(self, value: alarm.Alarm):
+    def alarm(self, value: vim.alarm.Alarm):
         self._alarm = value
     @property
-    def scheduledTask(self) -> scheduler.ScheduledTask: ...
+    def scheduledTask(self) -> vim.scheduler.ScheduledTask: ...
     @scheduledTask.setter
-    def scheduledTask(self, value: scheduler.ScheduledTask):
+    def scheduledTask(self, value: vim.scheduler.ScheduledTask):
         self._scheduledTask = value
     @property
     def eventChainId(self) -> List[int]: ...
     @eventChainId.setter
     def eventChainId(self, value: List[int]):
         self._eventChainId = value
     @property
@@ -7177,17 +7196,17 @@
 class TaskReasonAlarm(TaskReason):
     @property
     def alarmName(self) -> str: ...
     @alarmName.setter
     def alarmName(self, value: str):
         self._alarmName = value
     @property
-    def alarm(self) -> alarm.Alarm: ...
+    def alarm(self) -> vim.alarm.Alarm: ...
     @alarm.setter
-    def alarm(self, value: alarm.Alarm):
+    def alarm(self, value: vim.alarm.Alarm):
         self._alarm = value
     @property
     def entityName(self) -> str: ...
     @entityName.setter
     def entityName(self, value: str):
         self._entityName = value
     @property
@@ -7200,17 +7219,17 @@
 class TaskReasonSchedule(TaskReason):
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, value: str):
         self._name = value
     @property
-    def scheduledTask(self) -> scheduler.ScheduledTask: ...
+    def scheduledTask(self) -> vim.scheduler.ScheduledTask: ...
     @scheduledTask.setter
-    def scheduledTask(self, value: scheduler.ScheduledTask):
+    def scheduledTask(self, value: vim.scheduler.ScheduledTask):
         self._scheduledTask = value
 
 
 class TaskReasonSystem(TaskReason): ...
 
 
 class TaskReasonUser(TaskReason):
@@ -7864,15 +7883,15 @@
         @property
         def contents(self) -> str: ...
         @contents.setter
         def contents(self, value: str):
             self._contents = value
 
 
-    class OvfSectionSpec(option.ArrayUpdateSpec):
+    class OvfSectionSpec(vim.option.ArrayUpdateSpec):
         @property
         def info(self) -> vApp.OvfSectionInfo: ...
         @info.setter
         def info(self, value: vApp.OvfSectionInfo):
             self._info = value
 
 
@@ -7925,15 +7944,15 @@
         @property
         def appUrl(self) -> str: ...
         @appUrl.setter
         def appUrl(self, value: str):
             self._appUrl = value
 
 
-    class ProductSpec(option.ArrayUpdateSpec):
+    class ProductSpec(vim.option.ArrayUpdateSpec):
         @property
         def info(self) -> vApp.ProductInfo: ...
         @info.setter
         def info(self, value: vApp.ProductInfo):
             self._info = value
 
 
@@ -7996,15 +8015,15 @@
         @property
         def description(self) -> str: ...
         @description.setter
         def description(self, value: str):
             self._description = value
 
 
-    class PropertySpec(option.ArrayUpdateSpec):
+    class PropertySpec(vim.option.ArrayUpdateSpec):
         @property
         def info(self) -> vApp.PropertyInfo: ...
         @info.setter
         def info(self, value: vApp.PropertyInfo):
             self._info = value
 
 
@@ -8021,17 +8040,17 @@
             self._annotation = value
         @property
         def instanceUuid(self) -> str: ...
         @instanceUuid.setter
         def instanceUuid(self, value: str):
             self._instanceUuid = value
         @property
-        def managedBy(self) -> ext.ManagedByInfo: ...
+        def managedBy(self) -> vim.ext.ManagedByInfo: ...
         @managedBy.setter
-        def managedBy(self, value: ext.ManagedByInfo):
+        def managedBy(self, value: vim.ext.ManagedByInfo):
             self._managedBy = value
 
 
     class VAppConfigSpec(vApp.VmConfigSpec):
         @property
         def entityConfig(self) -> List[vApp.EntityConfigInfo]: ...
         @entityConfig.setter
@@ -8044,17 +8063,17 @@
             self._annotation = value
         @property
         def instanceUuid(self) -> str: ...
         @instanceUuid.setter
         def instanceUuid(self, value: str):
             self._instanceUuid = value
         @property
-        def managedBy(self) -> ext.ManagedByInfo: ...
+        def managedBy(self) -> vim.ext.ManagedByInfo: ...
         @managedBy.setter
-        def managedBy(self, value: ext.ManagedByInfo):
+        def managedBy(self, value: vim.ext.ManagedByInfo):
             self._managedBy = value
 
 
     class VAppImportSpec(ImportSpec):
         @property
         def name(self) -> str: ...
         @name.setter
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/action/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/action/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/alarm/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/cluster/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/cluster/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -234,17 +234,17 @@
         self._dpmConfigInfo = value
     @property
     def dpmHostConfig(self) -> List[DpmHostConfigInfo]: ...
     @dpmHostConfig.setter
     def dpmHostConfig(self, value: List[DpmHostConfigInfo]):
         self._dpmHostConfig = value
     @property
-    def vsanConfigInfo(self) -> ConfigInfo: ...
+    def vsanConfigInfo(self) -> vim.vsan.cluster.ConfigInfo: ...
     @vsanConfigInfo.setter
-    def vsanConfigInfo(self, value: ConfigInfo):
+    def vsanConfigInfo(self, value: vim.vsan.cluster.ConfigInfo):
         self._vsanConfigInfo = value
     @property
     def vsanHostConfig(self) -> List[vim.vsan.host.ConfigInfo]: ...
     @vsanHostConfig.setter
     def vsanHostConfig(self, value: List[vim.vsan.host.ConfigInfo]):
         self._vsanHostConfig = value
     @property
@@ -345,17 +345,17 @@
         self._dpmConfig = value
     @property
     def dpmHostConfigSpec(self) -> List[DpmHostConfigSpec]: ...
     @dpmHostConfigSpec.setter
     def dpmHostConfigSpec(self, value: List[DpmHostConfigSpec]):
         self._dpmHostConfigSpec = value
     @property
-    def vsanConfig(self) -> ConfigInfo: ...
+    def vsanConfig(self) -> vim.vsan.cluster.ConfigInfo: ...
     @vsanConfig.setter
-    def vsanConfig(self, value: ConfigInfo):
+    def vsanConfig(self, value: vim.vsan.cluster.ConfigInfo):
         self._vsanConfig = value
     @property
     def vsanHostConfigSpec(self) -> List[vim.vsan.host.ConfigInfo]: ...
     @vsanHostConfigSpec.setter
     def vsanHostConfigSpec(self, value: List[vim.vsan.host.ConfigInfo]):
         self._vsanHostConfigSpec = value
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/dvs/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/dvs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/encryption/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/encryption/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/event/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/event/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/ext/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/ext/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/fault/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/fault/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1072,15 +1072,15 @@
 
 class ExpiredAddonLicense(ExpiredFeatureLicense): ...
 
 
 class ExpiredEditionLicense(ExpiredFeatureLicense): ...
 
 
-class ExpiredFeatureLicense(NotEnoughLicenses):
+class ExpiredFeatureLicense(vmodl.fault.NotEnoughLicenses):
     @property
     def feature(self) -> str: ...
     @feature.setter
     def feature(self, value: str):
         self._feature = value
     @property
     def count(self) -> int: ...
@@ -1103,15 +1103,15 @@
     @property
     def data(self) -> List[vim.KeyValue]: ...
     @data.setter
     def data(self, value: List[vim.KeyValue]):
         self._data = value
 
 
-class FailToEnableSPBM(NotEnoughLicenses):
+class FailToEnableSPBM(vmodl.fault.NotEnoughLicenses):
     @property
     def cs(self) -> vim.ComputeResource: ...
     @cs.setter
     def cs(self, value: vim.ComputeResource):
         self._cs = value
     @property
     def csName(self) -> str: ...
@@ -1520,15 +1520,15 @@
 
 class HAErrorsAtDest(MigrationFault): ...
 
 
 class HeterogenousHostsBlockingEVC(EVCConfigFault): ...
 
 
-class HostAccessRestrictedToManagementServer(NotSupported):
+class HostAccessRestrictedToManagementServer(vmodl.fault.NotSupported):
     @property
     def managementServer(self) -> str: ...
     @managementServer.setter
     def managementServer(self, value: str):
         self._managementServer = value
 
 
@@ -1593,15 +1593,15 @@
     @property
     def reason(self) -> str: ...
     @reason.setter
     def reason(self, value: str):
         self._reason = value
 
 
-class HostInventoryFull(NotEnoughLicenses):
+class HostInventoryFull(vmodl.fault.NotEnoughLicenses):
     @property
     def capacity(self) -> int: ...
     @capacity.setter
     def capacity(self, value: int):
         self._capacity = value
 
 
@@ -1683,15 +1683,15 @@
         @property
         def fault(self) -> vmodl.MethodFault: ...
         @fault.setter
         def fault(self, value: vmodl.MethodFault):
             self._fault = value
 
 
-class InUseFeatureManipulationDisallowed(NotEnoughLicenses): ...
+class InUseFeatureManipulationDisallowed(vmodl.fault.NotEnoughLicenses): ...
 
 
 class InaccessibleDatastore(InvalidDatastore):
     @property
     def detail(self) -> str: ...
     @detail.setter
     def detail(self, value: str):
@@ -1749,26 +1749,26 @@
 
 
     class IncompatibleReason(Enum):
         rpo = "rpo"
         netCompression = "netCompression"
 
 
-class IncompatibleSetting(InvalidArgument):
+class IncompatibleSetting(vmodl.fault.InvalidArgument):
     @property
     def conflictingProperty(self) -> PropertyPath: ...
     @conflictingProperty.setter
     def conflictingProperty(self, value: PropertyPath):
         self._conflictingProperty = value
 
 
 class IncorrectFileType(FileFault): ...
 
 
-class IncorrectHostInformation(NotEnoughLicenses): ...
+class IncorrectHostInformation(vmodl.fault.NotEnoughLicenses): ...
 
 
 class IndependentDiskVMotionNotSupported(MigrationFeatureNotSupported): ...
 
 
 class InsufficientAgentVmsDeployed(InsufficientResourcesFault):
     @property
@@ -1999,15 +1999,15 @@
     @property
     def controllerKey(self) -> int: ...
     @controllerKey.setter
     def controllerKey(self, value: int):
         self._controllerKey = value
 
 
-class InvalidDasConfigArgument(InvalidArgument):
+class InvalidDasConfigArgument(vmodl.fault.InvalidArgument):
     @property
     def entry(self) -> str: ...
     @entry.setter
     def entry(self, value: str):
         self._entry = value
     @property
     def clusterName(self) -> str: ...
@@ -2018,15 +2018,15 @@
 
     class EntryForInvalidArgument(Enum):
         admissionControl = "admissionControl"
         userHeartbeatDs = "userHeartbeatDs"
         vmConfig = "vmConfig"
 
 
-class InvalidDasRestartPriorityForFtVm(InvalidArgument):
+class InvalidDasRestartPriorityForFtVm(vmodl.fault.InvalidArgument):
     @property
     def vm(self) -> vim.VirtualMachine: ...
     @vm.setter
     def vm(self, value: vim.VirtualMachine):
         self._vm = value
     @property
     def vmName(self) -> str: ...
@@ -2087,28 +2087,28 @@
     def deviceIndex(self, value: int):
         self._deviceIndex = value
 
 
 class InvalidDiskFormat(InvalidFormat): ...
 
 
-class InvalidDrsBehaviorForFtVm(InvalidArgument):
+class InvalidDrsBehaviorForFtVm(vmodl.fault.InvalidArgument):
     @property
     def vm(self) -> vim.VirtualMachine: ...
     @vm.setter
     def vm(self, value: vim.VirtualMachine):
         self._vm = value
     @property
     def vmName(self) -> str: ...
     @vmName.setter
     def vmName(self, value: str):
         self._vmName = value
 
 
-class InvalidEditionLicense(NotEnoughLicenses):
+class InvalidEditionLicense(vmodl.fault.NotEnoughLicenses):
     @property
     def feature(self) -> str: ...
     @feature.setter
     def feature(self, value: str):
         self._feature = value
 
 
@@ -2139,15 +2139,15 @@
     @property
     def host(self) -> vim.HostSystem: ...
     @host.setter
     def host(self, value: vim.HostSystem):
         self._host = value
 
 
-class InvalidIndexArgument(InvalidArgument):
+class InvalidIndexArgument(vmodl.fault.InvalidArgument):
     @property
     def key(self) -> str: ...
     @key.setter
     def key(self, value: str):
         self._key = value
 
 
@@ -2305,15 +2305,15 @@
     @property
     def vm(self) -> vim.VirtualMachine: ...
     @vm.setter
     def vm(self, value: vim.VirtualMachine):
         self._vm = value
 
 
-class InventoryHasStandardAloneHosts(NotEnoughLicenses):
+class InventoryHasStandardAloneHosts(vmodl.fault.NotEnoughLicenses):
     @property
     def hosts(self) -> List[str]: ...
     @hosts.setter
     def hosts(self, value: List[str]):
         self._hosts = value
 
 
@@ -2452,15 +2452,15 @@
     @property
     def reason(self) -> str: ...
     @reason.setter
     def reason(self, value: str):
         self._reason = value
 
 
-class LicenseDowngradeDisallowed(NotEnoughLicenses):
+class LicenseDowngradeDisallowed(vmodl.fault.NotEnoughLicenses):
     @property
     def edition(self) -> str: ...
     @edition.setter
     def edition(self, value: str):
         self._edition = value
     @property
     def entityId(self) -> str: ...
@@ -2478,37 +2478,37 @@
     @property
     def entityId(self) -> str: ...
     @entityId.setter
     def entityId(self, value: str):
         self._entityId = value
 
 
-class LicenseExpired(NotEnoughLicenses):
+class LicenseExpired(vmodl.fault.NotEnoughLicenses):
     @property
     def licenseKey(self) -> str: ...
     @licenseKey.setter
     def licenseKey(self, value: str):
         self._licenseKey = value
 
 
-class LicenseKeyEntityMismatch(NotEnoughLicenses): ...
+class LicenseKeyEntityMismatch(vmodl.fault.NotEnoughLicenses): ...
 
 
-class LicenseRestricted(NotEnoughLicenses): ...
+class LicenseRestricted(vmodl.fault.NotEnoughLicenses): ...
 
 
 class LicenseServerUnavailable(VimFault):
     @property
     def licenseServer(self) -> str: ...
     @licenseServer.setter
     def licenseServer(self, value: str):
         self._licenseServer = value
 
 
-class LicenseSourceUnavailable(NotEnoughLicenses):
+class LicenseSourceUnavailable(vmodl.fault.NotEnoughLicenses):
     @property
     def licenseSource(self) -> vim.LicenseManager.LicenseSource: ...
     @licenseSource.setter
     def licenseSource(self, value: vim.LicenseManager.LicenseSource):
         self._licenseSource = value
 
 
@@ -2996,21 +2996,21 @@
     @property
     def vmName(self) -> str: ...
     @vmName.setter
     def vmName(self, value: str):
         self._vmName = value
 
 
-class NoLicenseServerConfigured(NotEnoughLicenses): ...
+class NoLicenseServerConfigured(vmodl.fault.NotEnoughLicenses): ...
 
 
 class NoPeerHostFound(HostPowerOpFailed): ...
 
 
-class NoPermission(SecurityError):
+class NoPermission(vmodl.fault.SecurityError):
     @property
     def object(self) -> ManagedObject: ...
     @object.setter
     def object(self, value: ManagedObject):
         self._object = value
     @property
     def privilegeId(self) -> str: ...
@@ -4399,15 +4399,15 @@
     @property
     def details(self) -> str: ...
     @details.setter
     def details(self, value: str):
         self._details = value
 
 
-class RestrictedVersion(SecurityError): ...
+class RestrictedVersion(vmodl.fault.SecurityError): ...
 
 
 class RollbackFailure(DvsFault):
     @property
     def entityName(self) -> str: ...
     @entityName.setter
     def entityName(self, value: str):
@@ -4564,15 +4564,15 @@
     @property
     def vmName(self) -> str: ...
     @vmName.setter
     def vmName(self, value: str):
         self._vmName = value
 
 
-class SolutionUserRequired(SecurityError): ...
+class SolutionUserRequired(vmodl.fault.SecurityError): ...
 
 
 class SsdDiskNotAvailable(VimFault):
     @property
     def devicePath(self) -> str: ...
     @devicePath.setter
     def devicePath(self, value: str):
@@ -5201,15 +5201,15 @@
     @property
     def hostName(self) -> str: ...
     @hostName.setter
     def hostName(self, value: str):
         self._hostName = value
 
 
-class VmLimitLicense(NotEnoughLicenses):
+class VmLimitLicense(vmodl.fault.NotEnoughLicenses):
     @property
     def limit(self) -> int: ...
     @limit.setter
     def limit(self, value: int):
         self._limit = value
 
 
@@ -5295,15 +5295,15 @@
 
 class VmotionInterfaceNotEnabled(HostPowerOpFailed): ...
 
 
 class VolumeEditorError(CustomizationFault): ...
 
 
-class VramLimitLicense(NotEnoughLicenses):
+class VramLimitLicense(vmodl.fault.NotEnoughLicenses):
     @property
     def limit(self) -> int: ...
     @limit.setter
     def limit(self, value: int):
         self._limit = value
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/host/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/host/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Literal
 from enum import Enum
-from pyVmomi import ClusterStatus, DecommissionMode, DiskMapping, DiskResult, VsanDiskInfo, VsanRuntimeInfo, vim, vmodl
+from pyVmomi import vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import Link, ManagedObject, NoneType, binary, byte, long, short
 
 
 class ActiveDirectoryAuthentication(DirectoryStore):
     def JoinDomain(self, domainName: str, userName: str, password: str) -> vim.Task: ...
     def JoinDomainWithCAM(self, domainName: str, camServer: str) -> vim.Task: ...
@@ -2607,23 +2607,23 @@
         @failureReason.setter
         def failureReason(self, value: str):
             self._failureReason = value
 
 
 class VsanSystem(ManagedObject):
     @property
-    def config(self) -> ConfigInfo: ...
-    def QueryDisksForVsan(self, canonicalName: List[str]) -> List[DiskResult]: ...
+    def config(self) -> vim.vsan.host.ConfigInfo: ...
+    def QueryDisksForVsan(self, canonicalName: List[str]) -> List[vim.vsan.host.DiskResult]: ...
     def AddDisks(self, disk: List[ScsiDisk]) -> vim.Task: ...
-    def InitializeDisks(self, mapping: List[DiskMapping]) -> vim.Task: ...
+    def InitializeDisks(self, mapping: List[vim.vsan.host.DiskMapping]) -> vim.Task: ...
     def RemoveDisk(self, disk: List[ScsiDisk], maintenanceSpec: MaintenanceSpec, timeout: int) -> vim.Task: ...
-    def RemoveDiskMapping(self, mapping: List[DiskMapping], maintenanceSpec: MaintenanceSpec, timeout: int) -> vim.Task: ...
-    def UnmountDiskMapping(self, mapping: List[DiskMapping]) -> vim.Task: ...
-    def Update(self, config: ConfigInfo) -> vim.Task: ...
-    def QueryHostStatus(self) -> ClusterStatus: ...
+    def RemoveDiskMapping(self, mapping: List[vim.vsan.host.DiskMapping], maintenanceSpec: MaintenanceSpec, timeout: int) -> vim.Task: ...
+    def UnmountDiskMapping(self, mapping: List[vim.vsan.host.DiskMapping]) -> vim.Task: ...
+    def Update(self, config: vim.vsan.host.ConfigInfo) -> vim.Task: ...
+    def QueryHostStatus(self) -> vim.vsan.host.ClusterStatus: ...
     def EvacuateNode(self, maintenanceSpec: MaintenanceSpec, timeout: int) -> vim.Task: ...
     def RecommissionNode(self) -> vim.Task: ...
 
 
 class ActiveDirectoryInfo(DirectoryStoreInfo):
     @property
     def joinedDomain(self) -> str: ...
@@ -3804,17 +3804,17 @@
         self._maskedFeatureCapability = value
     @property
     def vFlashConfigInfo(self) -> VFlashManager.VFlashConfigInfo: ...
     @vFlashConfigInfo.setter
     def vFlashConfigInfo(self, value: VFlashManager.VFlashConfigInfo):
         self._vFlashConfigInfo = value
     @property
-    def vsanHostConfig(self) -> ConfigInfo: ...
+    def vsanHostConfig(self) -> vim.vsan.host.ConfigInfo: ...
     @vsanHostConfig.setter
-    def vsanHostConfig(self, value: ConfigInfo):
+    def vsanHostConfig(self, value: vim.vsan.host.ConfigInfo):
         self._vsanHostConfig = value
     @property
     def domainList(self) -> List[str]: ...
     @domainList.setter
     def domainList(self, value: List[str]):
         self._domainList = value
     @property
@@ -7277,17 +7277,17 @@
     class ReloadTarget(Enum):
         currentConfig = "currentConfig"
         snapshotConfig = "snapshotConfig"
 
 
 class MaintenanceSpec(vmodl.DynamicData):
     @property
-    def vsanMode(self) -> DecommissionMode: ...
+    def vsanMode(self) -> vim.vsan.host.DecommissionMode: ...
     @vsanMode.setter
-    def vsanMode(self, value: DecommissionMode):
+    def vsanMode(self, value: vim.vsan.host.DecommissionMode):
         self._vsanMode = value
     @property
     def purpose(self) -> str: ...
     @purpose.setter
     def purpose(self, value: str):
         self._purpose = value
 
@@ -10130,17 +10130,17 @@
         self._dasHostState = value
     @property
     def tpmPcrValues(self) -> List[TpmDigestInfo]: ...
     @tpmPcrValues.setter
     def tpmPcrValues(self, value: List[TpmDigestInfo]):
         self._tpmPcrValues = value
     @property
-    def vsanRuntimeInfo(self) -> VsanRuntimeInfo: ...
+    def vsanRuntimeInfo(self) -> vim.vsan.host.VsanRuntimeInfo: ...
     @vsanRuntimeInfo.setter
-    def vsanRuntimeInfo(self, value: VsanRuntimeInfo):
+    def vsanRuntimeInfo(self, value: vim.vsan.host.VsanRuntimeInfo):
         self._vsanRuntimeInfo = value
     @property
     def networkRuntimeInfo(self) -> RuntimeInfo.NetworkRuntimeInfo: ...
     @networkRuntimeInfo.setter
     def networkRuntimeInfo(self, value: RuntimeInfo.NetworkRuntimeInfo):
         self._networkRuntimeInfo = value
     @property
@@ -10329,17 +10329,17 @@
         self._physicalLocation = value
     @property
     def emulatedDIXDIFEnabled(self) -> bool: ...
     @emulatedDIXDIFEnabled.setter
     def emulatedDIXDIFEnabled(self, value: bool):
         self._emulatedDIXDIFEnabled = value
     @property
-    def vsanDiskInfo(self) -> VsanDiskInfo: ...
+    def vsanDiskInfo(self) -> vim.vsan.host.VsanDiskInfo: ...
     @vsanDiskInfo.setter
-    def vsanDiskInfo(self, value: VsanDiskInfo):
+    def vsanDiskInfo(self, value: vim.vsan.host.VsanDiskInfo):
         self._vsanDiskInfo = value
     @property
     def scsiDiskType(self) -> str: ...
     @scsiDiskType.setter
     def scsiDiskType(self, value: str):
         self._scsiDiskType = value
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/net/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/net/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/option/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/option/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 from enum import Enum
 from pyVmomi import vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedObject, NoneType, PropertyPath
-from . import cluster, host
+from . import cluster as cluster
+from . import host as host
 
 
 class ComplianceManager(ManagedObject):
     def CheckCompliance(self, profile: List[Profile], entity: List[vim.ManagedEntity]) -> vim.Task: ...
     def QueryComplianceStatus(self, profile: List[Profile], entity: List[vim.ManagedEntity]) -> List[ComplianceResult]: ...
     def ClearComplianceStatus(self, profile: List[Profile], entity: List[vim.ManagedEntity]) -> NoneType: ...
     def QueryExpressionMetadata(self, expressionName: List[str], profile: Profile) -> List[ExpressionMetadata]: ...
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/cluster/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/profile/host/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 from enum import Enum
 from pyVmomi import vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedObject, NoneType, PropertyPath, binary, byte
-from . import profileEngine
+from . import profileEngine as profileEngine
 
 
 class HostProfile(vim.profile.Profile):
     @property
     def validationState(self) -> str: ...
     @property
     def validationStateUpdateTime(self) -> datetime: ...
@@ -180,17 +180,17 @@
     def RetrieveHostSpecification(self, host: vim.HostSystem, fromHost: bool) -> HostSpecification: ...
     def DeleteHostSubSpecification(self, host: vim.HostSystem, subSpecName: str) -> NoneType: ...
     def DeleteHostSpecification(self, host: vim.HostSystem) -> NoneType: ...
     def GetUpdatedHosts(self, startChangeID: str, endChangeID: str) -> List[vim.HostSystem]: ...
 
 
 class ProfileManager(vim.profile.ProfileManager):
-    def ApplyHostConfiguration(self, host: vim.HostSystem, configSpec: ConfigSpec, userInput: List[vim.profile.DeferredPolicyOptionParameter]) -> vim.Task: ...
-    def GenerateConfigTaskList(self, configSpec: ConfigSpec, host: vim.HostSystem) -> ProfileManager.ConfigTaskList: ...
-    def GenerateTaskList(self, configSpec: ConfigSpec, host: vim.HostSystem) -> vim.Task: ...
+    def ApplyHostConfiguration(self, host: vim.HostSystem, configSpec: vim.host.ConfigSpec, userInput: List[vim.profile.DeferredPolicyOptionParameter]) -> vim.Task: ...
+    def GenerateConfigTaskList(self, configSpec: vim.host.ConfigSpec, host: vim.HostSystem) -> ProfileManager.ConfigTaskList: ...
+    def GenerateTaskList(self, configSpec: vim.host.ConfigSpec, host: vim.HostSystem) -> vim.Task: ...
     def QueryProfileMetadata(self, profileName: List[type], profile: vim.profile.Profile) -> List[vim.profile.ProfileMetadata]: ...
     def QueryProfileStructure(self, profile: vim.profile.Profile) -> vim.profile.ProfileStructure: ...
     def CreateDefaultProfile(self, profileType: type, profileTypeName: str, profile: vim.profile.Profile) -> vim.profile.ApplyProfile: ...
     def UpdateAnswerFile(self, host: vim.HostSystem, configSpec: ProfileManager.AnswerFileCreateSpec) -> vim.Task: ...
     def RetrieveAnswerFile(self, host: vim.HostSystem) -> AnswerFile: ...
     def RetrieveAnswerFileForProfile(self, host: vim.HostSystem, applyProfile: HostApplyProfile) -> AnswerFile: ...
     def ExportAnswerFile(self, host: vim.HostSystem) -> vim.Task: ...
@@ -385,17 +385,17 @@
             @toBeReenableCC.setter
             def toBeReenableCC(self, value: HostApplyProfile):
                 self._toBeReenableCC = value
 
 
     class ConfigTaskList(vmodl.DynamicData):
         @property
-        def configSpec(self) -> ConfigSpec: ...
+        def configSpec(self) -> vim.host.ConfigSpec: ...
         @configSpec.setter
-        def configSpec(self, value: ConfigSpec):
+        def configSpec(self, value: vim.host.ConfigSpec):
             self._configSpec = value
         @property
         def taskDescription(self) -> List[vmodl.LocalizableMessage]: ...
         @taskDescription.setter
         def taskDescription(self, value: List[vmodl.LocalizableMessage]):
             self._taskDescription = value
         @property
@@ -553,17 +553,17 @@
 class ExecuteResult(vmodl.DynamicData):
     @property
     def status(self) -> str: ...
     @status.setter
     def status(self, value: str):
         self._status = value
     @property
-    def configSpec(self) -> ConfigSpec: ...
+    def configSpec(self) -> vim.host.ConfigSpec: ...
     @configSpec.setter
-    def configSpec(self, value: ConfigSpec):
+    def configSpec(self, value: vim.host.ConfigSpec):
         self._configSpec = value
     @property
     def inapplicablePath(self) -> List[PropertyPath]: ...
     @inapplicablePath.setter
     def inapplicablePath(self, value: List[PropertyPath]):
         self._inapplicablePath = value
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/scheduler/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/storageDrs/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/storageDrs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vcha/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vcha/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/view/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/view/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from typing import List, Literal
 from enum import Enum
 from pyVmomi import vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedObject, NoneType, PropertyPath, binary, long, short
-from . import check, customization, device, guest, replication
+from . import check as check
+from . import customization as customization
+from . import device as device
+from . import guest as guest
+from . import replication as replication
 
 
 class GuestCustomizationManager(ManagedObject):
-    def Customize(self, vm: vim.VirtualMachine, auth: guest.GuestAuthentication, spec: customization.Specification, configParams: List[vim.option.OptionValue]) -> vim.Task: ...
-    def StartNetwork(self, vm: vim.VirtualMachine, auth: guest.GuestAuthentication) -> vim.Task: ...
-    def AbortCustomization(self, vm: vim.VirtualMachine, auth: guest.GuestAuthentication) -> vim.Task: ...
+    def Customize(self, vm: vim.VirtualMachine, auth: vim.vm.guest.GuestAuthentication, spec: vim.vm.customization.Specification, configParams: List[vim.option.OptionValue]) -> vim.Task: ...
+    def StartNetwork(self, vm: vim.VirtualMachine, auth: vim.vm.guest.GuestAuthentication) -> vim.Task: ...
+    def AbortCustomization(self, vm: vim.VirtualMachine, auth: vim.vm.guest.GuestAuthentication) -> vim.Task: ...
 
 
 class Snapshot(vim.ExtensibleManagedObject):
     @property
     def config(self) -> ConfigInfo: ...
     @property
     def childSnapshot(self) -> List[Snapshot]: ...
@@ -390,17 +394,17 @@
         self._template = value
     @property
     def config(self) -> ConfigSpec: ...
     @config.setter
     def config(self, value: ConfigSpec):
         self._config = value
     @property
-    def customization(self) -> customization.Specification: ...
+    def customization(self) -> vim.vm.customization.Specification: ...
     @customization.setter
-    def customization(self, value: customization.Specification):
+    def customization(self, value: vim.vm.customization.Specification):
         self._customization = value
     @property
     def powerOn(self) -> bool: ...
     @powerOn.setter
     def powerOn(self, value: bool):
         self._powerOn = value
     @property
@@ -904,17 +908,17 @@
         self._capabilities = value
     @property
     def datastore(self) -> DatastoreOption: ...
     @datastore.setter
     def datastore(self, value: DatastoreOption):
         self._datastore = value
     @property
-    def defaultDevice(self) -> List[device.VirtualDevice]: ...
+    def defaultDevice(self) -> List[vim.vm.device.VirtualDevice]: ...
     @defaultDevice.setter
-    def defaultDevice(self, value: List[device.VirtualDevice]):
+    def defaultDevice(self, value: List[vim.vm.device.VirtualDevice]):
         self._defaultDevice = value
     @property
     def supportedMonitorType(self) -> List[str]: ...
     @supportedMonitorType.setter
     def supportedMonitorType(self, value: List[str]):
         self._supportedMonitorType = value
     @property
@@ -1135,17 +1139,17 @@
         self._virtualICH7MPresent = value
     @property
     def virtualSMCPresent(self) -> bool: ...
     @virtualSMCPresent.setter
     def virtualSMCPresent(self, value: bool):
         self._virtualSMCPresent = value
     @property
-    def deviceChange(self) -> List[device.VirtualDeviceSpec]: ...
+    def deviceChange(self) -> List[vim.vm.device.VirtualDeviceSpec]: ...
     @deviceChange.setter
-    def deviceChange(self, value: List[device.VirtualDeviceSpec]):
+    def deviceChange(self, value: List[vim.vm.device.VirtualDeviceSpec]):
         self._deviceChange = value
     @property
     def cpuAllocation(self) -> vim.ResourceAllocationInfo: ...
     @cpuAllocation.setter
     def cpuAllocation(self, value: vim.ResourceAllocationInfo):
         self._cpuAllocation = value
     @property
@@ -1730,17 +1734,17 @@
 class DefinedProfileSpec(ProfileSpec):
     @property
     def profileId(self) -> str: ...
     @profileId.setter
     def profileId(self, value: str):
         self._profileId = value
     @property
-    def replicationSpec(self) -> replication.ReplicationSpec: ...
+    def replicationSpec(self) -> vim.vm.replication.ReplicationSpec: ...
     @replicationSpec.setter
-    def replicationSpec(self, value: replication.ReplicationSpec):
+    def replicationSpec(self, value: vim.vm.replication.ReplicationSpec):
         self._replicationSpec = value
     @property
     def profileData(self) -> ProfileRawData: ...
     @profileData.setter
     def profileData(self, value: ProfileRawData):
         self._profileData = value
     @property
@@ -2000,17 +2004,17 @@
     @disks.setter
     def disks(self, value: List[FaultToleranceVMConfigSpec.FaultToleranceDiskSpec]):
         self._disks = value
 
 
     class FaultToleranceDiskSpec(vmodl.DynamicData):
         @property
-        def disk(self) -> device.VirtualDevice: ...
+        def disk(self) -> vim.vm.device.VirtualDevice: ...
         @disk.setter
-        def disk(self, value: device.VirtualDevice):
+        def disk(self, value: vim.vm.device.VirtualDevice):
             self._disk = value
         @property
         def datastore(self) -> vim.Datastore: ...
         @datastore.setter
         def datastore(self, value: vim.Datastore):
             self._datastore = value
 
@@ -3653,17 +3657,17 @@
         self._disk = value
     @property
     def transform(self) -> RelocateSpec.Transformation | Literal['flat', 'sparse']: ...
     @transform.setter
     def transform(self, value: RelocateSpec.Transformation | Literal['flat', 'sparse']):
         self._transform = value
     @property
-    def deviceChange(self) -> List[device.VirtualDeviceSpec]: ...
+    def deviceChange(self) -> List[vim.vm.device.VirtualDeviceSpec]: ...
     @deviceChange.setter
-    def deviceChange(self, value: List[device.VirtualDeviceSpec]):
+    def deviceChange(self, value: List[vim.vm.device.VirtualDeviceSpec]):
         self._deviceChange = value
     @property
     def profile(self) -> List[ProfileSpec]: ...
     @profile.setter
     def profile(self, value: List[ProfileSpec]):
         self._profile = value
     @property
@@ -3686,17 +3690,17 @@
             self._datastore = value
         @property
         def diskMoveType(self) -> str: ...
         @diskMoveType.setter
         def diskMoveType(self, value: str):
             self._diskMoveType = value
         @property
-        def diskBackingInfo(self) -> device.VirtualDevice.BackingInfo: ...
+        def diskBackingInfo(self) -> vim.vm.device.VirtualDevice.BackingInfo: ...
         @diskBackingInfo.setter
-        def diskBackingInfo(self, value: device.VirtualDevice.BackingInfo):
+        def diskBackingInfo(self, value: vim.vm.device.VirtualDevice.BackingInfo):
             self._diskBackingInfo = value
         @property
         def profile(self) -> List[ProfileSpec]: ...
         @profile.setter
         def profile(self, value: List[ProfileSpec]):
             self._profile = value
         @property
@@ -4947,17 +4951,17 @@
             self._deviceName = value
         @property
         def isConfigurable(self) -> bool: ...
         @isConfigurable.setter
         def isConfigurable(self, value: bool):
             self._isConfigurable = value
         @property
-        def device(self) -> device.VirtualDevice: ...
+        def device(self) -> vim.vm.device.VirtualDevice: ...
         @device.setter
-        def device(self, value: device.VirtualDevice):
+        def device(self, value: vim.vm.device.VirtualDevice):
             self._device = value
 
 
         class ComponentType(Enum):
             pciPassthru = "pciPassthru"
             nvidiaVgpu = "nvidiaVgpu"
             sriovNic = "sriovNic"
@@ -5131,17 +5135,17 @@
         self._virtualICH7MPresent = value
     @property
     def virtualSMCPresent(self) -> bool: ...
     @virtualSMCPresent.setter
     def virtualSMCPresent(self, value: bool):
         self._virtualSMCPresent = value
     @property
-    def device(self) -> List[device.VirtualDevice]: ...
+    def device(self) -> List[vim.vm.device.VirtualDevice]: ...
     @device.setter
-    def device(self, value: List[device.VirtualDevice]):
+    def device(self, value: List[vim.vm.device.VirtualDevice]):
         self._device = value
     @property
     def motherboardLayout(self) -> str: ...
     @motherboardLayout.setter
     def motherboardLayout(self, value: str):
         self._motherboardLayout = value
     @property
@@ -5159,17 +5163,17 @@
 class VirtualHardwareOption(vmodl.DynamicData):
     @property
     def hwVersion(self) -> int: ...
     @hwVersion.setter
     def hwVersion(self, value: int):
         self._hwVersion = value
     @property
-    def virtualDeviceOption(self) -> List[device.VirtualDeviceOption]: ...
+    def virtualDeviceOption(self) -> List[vim.vm.device.VirtualDeviceOption]: ...
     @virtualDeviceOption.setter
-    def virtualDeviceOption(self, value: List[device.VirtualDeviceOption]):
+    def virtualDeviceOption(self, value: List[vim.vm.device.VirtualDeviceOption]):
         self._virtualDeviceOption = value
     @property
     def deviceListReadonly(self) -> bool: ...
     @deviceListReadonly.setter
     def deviceListReadonly(self, value: bool):
         self._deviceListReadonly = value
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/check/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/check/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/customization/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/customization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/device/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/guest/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/guest/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/replication/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vm/replication/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/cluster/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/host/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vsan/host/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 from enum import Enum
-from pyVmomi import ScsiDisk, vim, vmodl
+from pyVmomi import vim, vmodl
 from datetime import datetime
 
 
 class ClusterStatus(vmodl.DynamicData):
     @property
     def uuid(self) -> str: ...
     @uuid.setter
@@ -204,30 +204,30 @@
     @error.setter
     def error(self, value: vmodl.MethodFault):
         self._error = value
 
 
 class DiskMapping(vmodl.DynamicData):
     @property
-    def ssd(self) -> ScsiDisk: ...
+    def ssd(self) -> vim.host.ScsiDisk: ...
     @ssd.setter
-    def ssd(self, value: ScsiDisk):
+    def ssd(self, value: vim.host.ScsiDisk):
         self._ssd = value
     @property
-    def nonSsd(self) -> List[ScsiDisk]: ...
+    def nonSsd(self) -> List[vim.host.ScsiDisk]: ...
     @nonSsd.setter
-    def nonSsd(self, value: List[ScsiDisk]):
+    def nonSsd(self, value: List[vim.host.ScsiDisk]):
         self._nonSsd = value
 
 
 class DiskResult(vmodl.DynamicData):
     @property
-    def disk(self) -> ScsiDisk: ...
+    def disk(self) -> vim.host.ScsiDisk: ...
     @disk.setter
-    def disk(self, value: ScsiDisk):
+    def disk(self, value: vim.host.ScsiDisk):
         self._disk = value
     @property
     def state(self) -> str: ...
     @state.setter
     def state(self, value: str):
         self._state = value
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 from enum import Enum
 from pyVmomi import vim, vmodl
 from datetime import datetime
 from pyVmomi.VmomiSupport import ManagedObject, long
-from . import host, vcenter
+from . import host as host
+from . import vcenter as vcenter
 
 
 class VStorageObjectManagerBase(ManagedObject): ...
 
 
 class BaseConfigInfo(vmodl.DynamicData):
     @property
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/host/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/vcenter/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vim/vslm/vcenter/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vmodl/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vmodl/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
 from pyVmomi import vmodl
 from pyVmomi.VmomiSupport import DataObject, PropertyPath
-from . import fault, query
+from . import fault as fault
+from . import query as query
 
 
 class DynamicArray(DataObject):
     @property
     def dynamicType(self) -> str: ...
     @property
     def val(self) -> List[object]: ...
```

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vmodl/fault/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vmodl/fault/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyVmomi/vmodl/query/__init__.pyi` & `pyvmomi-8.0.1.0.2/pyVmomi/vmodl/query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/pyvmomi.egg-info/PKG-INFO` & `pyvmomi-8.0.1.0.2/pyvmomi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvmomi
-Version: 8.0.1.0.1
+Version: 8.0.1.0.2
 Summary: VMware vSphere Python SDK
 Home-page: https://github.com/vmware/pyvmomi
 Author: VMware, Inc.
 Author-email: jhu@vmware.com
 License: License :: OSI Approved :: Apache Software License
 Keywords: pyvmomi,vsphere,vmware,esx
 Platform: Windows
@@ -36,18 +36,14 @@
 Requires-Python: >=2.7.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Provides-Extra: sso
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 pyvmomi
 ------------
-.. image:: https://travis-ci.org/vmware/pyvmomi.svg?branch=v6.0.0.2016.4
-    :target: https://travis-ci.org/vmware/pyvmomi
-    :alt: Build Status
-
 .. image:: https://img.shields.io/pypi/dm/pyvmomi.svg
     :target: https://pypi.python.org/pypi/pyvmomi/
     :alt: Downloads
 
 pyVmomi is the Python SDK for the VMware vSphere API that allows you to manage 
 ESX, ESXi, and vCenter.
```

### Comparing `pyvmomi-8.0.1.0.1/pyvmomi.egg-info/SOURCES.txt` & `pyvmomi-8.0.1.0.2/pyvmomi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 pyVmomi/__init__.py
 pyVmomi/_typeinfo_core.py
 pyVmomi/_typeinfo_eam.py
 pyVmomi/_typeinfo_pbm.py
 pyVmomi/_typeinfo_query.py
 pyVmomi/_typeinfo_sms.py
 pyVmomi/_typeinfo_vim.py
+pyVmomi/_typeinfo_vsan.py
+pyVmomi/_typeinfo_vslm.py
 pyVmomi/_typeinfos.py
 pyVmomi/py.typed
 pyVmomi/pyVmomiSettings.py
 pyVmomi/eam/__init__.pyi
 pyVmomi/eam/fault/__init__.pyi
 pyVmomi/eam/issue/__init__.pyi
 pyVmomi/eam/issue/cluster/__init__.pyi
@@ -93,32 +95,49 @@
 pyVmomi/vim/vsan/host/__init__.pyi
 pyVmomi/vim/vslm/__init__.pyi
 pyVmomi/vim/vslm/host/__init__.pyi
 pyVmomi/vim/vslm/vcenter/__init__.pyi
 pyVmomi/vmodl/__init__.pyi
 pyVmomi/vmodl/fault/__init__.pyi
 pyVmomi/vmodl/query/__init__.pyi
+pyVmomi/vslm/__init__.pyi
+pyVmomi/vslm/auth/__init__.pyi
+pyVmomi/vslm/event/__init__.pyi
+pyVmomi/vslm/fault/__init__.pyi
+pyVmomi/vslm/vso/__init__.pyi
 pyvmomi.egg-info/PKG-INFO
 pyvmomi.egg-info/SOURCES.txt
 pyvmomi.egg-info/dependency_links.txt
 pyvmomi.egg-info/requires.txt
 pyvmomi.egg-info/top_level.txt
 pyvmomi.egg-info/zip-safe
 tests/README.rst
 tests/__init__.py
+tests/__init__.pyc
 tests/test_connect.py
 tests/test_container_view.py
 tests/test_deserializer.py
 tests/test_iso8601.py
 tests/test_json.py
 tests/test_managed_object.py
 tests/test_pbm_check_compatibility.py
 tests/test_serializer.py
 tests/test_vim_session_oriented_stub.py
 tests/test_virtual_machine_object.py
+tests/__pycache__/__init__.cpython-310.pyc
+tests/__pycache__/test_connect.cpython-310.pyc
+tests/__pycache__/test_container_view.cpython-310.pyc
+tests/__pycache__/test_deserializer.cpython-310.pyc
+tests/__pycache__/test_iso8601.cpython-310.pyc
+tests/__pycache__/test_json.cpython-310.pyc
+tests/__pycache__/test_managed_object.cpython-310.pyc
+tests/__pycache__/test_pbm_check_compatibility.cpython-310.pyc
+tests/__pycache__/test_serializer.cpython-310.pyc
+tests/__pycache__/test_vim_session_oriented_stub.cpython-310.pyc
+tests/__pycache__/test_virtual_machine_object.cpython-310.pyc
 tests/files/test_json_datacenter_explode.expect
 tests/files/test_json_datastore_explode.expect
 tests/files/test_json_host_explode.expect
 tests/files/test_json_network_explode.expect
 tests/files/test_json_vm_explode_default.expect
 tests/files/test_json_vm_explode_objs_match.expect
 tests/files/test_json_vm_explode_strip_dynamic.expect
```

### Comparing `pyvmomi-8.0.1.0.1/setup.py` & `pyvmomi-8.0.1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     required = f.read().splitlines()
 
 with open('test-requirements.txt') as f:
     required_for_tests = f.read().splitlines()
 
 setup(
     name='pyvmomi',
-    version='8.0.1.0.1',
+    version='8.0.1.0.2',
     description='VMware vSphere Python SDK',
     # NOTE: pypi prefers the use of RST to render docs
     long_description=read('README.rst'),
     url='https://github.com/vmware/pyvmomi',
     author='VMware, Inc.',
     author_email='jhu@vmware.com',
     packages=['pyVmomi', 'pyVim'],
```

### Comparing `pyvmomi-8.0.1.0.1/tests/__init__.py` & `pyvmomi-8.0.1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_datacenter_explode.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_datacenter_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_datastore_explode.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_datastore_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_host_explode.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_host_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_network_explode.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_network_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_default.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_default.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_objs_match.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_objs_match.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_strip_dynamic.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_strip_dynamic.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_type_match.expect` & `pyvmomi-8.0.1.0.2/tests/files/test_json_vm_explode_type_match.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/files/unknown_method.xml` & `pyvmomi-8.0.1.0.2/tests/files/unknown_method.xml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/basic_connection.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection_bad_password.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/basic_connection_bad_password.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/basic_container_view.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/basic_container_view.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/http_proxy.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/http_proxy.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/iso8601_set_datetime.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/iso8601_set_datetime.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/pbm_check_compatibility.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/pbm_check_compatibility.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/root_folder_parent.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/root_folder_parent.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/smart_connection.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/smart_connection.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/ssl_tunnel_http_failure.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/ssl_tunnel_http_failure.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/sspi_connection.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/sspi_connection.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datacenter_explode.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_datacenter_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datastore_explode.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_datastore_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_host_explode.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_host_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_network_explode.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_network_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_default.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_default.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_objs.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_objs.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_type.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_json_vm_explode_type.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_simple_request_serializer.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_simple_request_serializer.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/test_vm_config_iso8601.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/test_vm_config_iso8601.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/fixtures/vm_nic_data.yaml` & `pyvmomi-8.0.1.0.2/tests/fixtures/vm_nic_data.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/test_connect.py` & `pyvmomi-8.0.1.0.2/tests/test_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     @patch('six.moves.http_client.HTTPSConnection')
     def test_http_proxy_with_cert_file(self, hs):
         conn = connect.SoapStubAdapter(
             'sdkTunnel', 8089, httpProxyHost='vcsa',
             certKeyFile='my_key_file', certFile='my_cert_file').GetConnection()
         conn.request('GET', '/')
         hs.assert_called_once_with('vcsa:80', cert_file='my_cert_file', key_file='my_key_file')
-        conn.set_tunnel.assert_called_once_with('sdkTunnel:8089')
+        conn.set_tunnel.assert_called_once_with('sdkTunnel:8089', headers={})
 
     @tests.VCRTestBase.my_vcr.use_cassette('http_proxy.yaml',
                       cassette_library_dir=tests.fixtures_path,
                       record_mode='once')
     def test_http_proxy(self):
         conn = connect.SoapStubAdapter(
             'vcenter.test', httpProxyHost='my-http-proxy',
```

### Comparing `pyvmomi-8.0.1.0.1/tests/test_container_view.py` & `pyvmomi-8.0.1.0.2/tests/test_container_view.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/test_deserializer.py` & `pyvmomi-8.0.1.0.2/tests/test_deserializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# VMware vSphere Python SDK
-# Copyright (c) 2016 VMware, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from pyVmomi import vim
-from pyVmomi.SoapAdapter import SoapStubAdapter, SoapResponseDeserializer
-import unittest
-
-#TODO: Fix the test Post 6.7 release
-# class DeserializerTests(unittest.TestCase):
-#
-#     def test_deserialize_unknown_managed_method(self):
-#         with open('tests/files/unknown_method.xml', 'rb') as f:
-#             data = f.read()
-#         stub = SoapStubAdapter(version="vim.version.version6")
-#         deserializer = SoapResponseDeserializer(stub)
-#         result = vim.TaskHistoryCollector._GetMethodInfo("ReadNext").result
-#         obj = deserializer.Deserialize(data, result)
-#         print(obj)
-#         with self.assertRaisesRegexp(Exception, "Managed method LeaseMapDiskRegion is not available"):
-#             obj[-1].name()
-
+# VMware vSphere Python SDK
+# Copyright (c) 2016 VMware, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from pyVmomi import vim
+from pyVmomi.SoapAdapter import SoapStubAdapter, SoapResponseDeserializer
+import unittest
+
+
+class DeserializerTests(unittest.TestCase):
+
+    def test_deserialize_unknown_managed_method(self):
+        with open('tests/files/unknown_method.xml', 'rb') as f:
+            data = f.read()
+        stub = SoapStubAdapter(version="vim.version.version6")
+        deserializer = SoapResponseDeserializer(stub)
+        result = vim.TaskHistoryCollector._GetMethodInfo("ReadNext").result
+        obj = deserializer.Deserialize(data, result)
+        with self.assertRaisesRegexp(Exception, "Managed method LeaseMapDiskRegion is not available"):
+            obj[-1].name()
+
```

### Comparing `pyvmomi-8.0.1.0.1/tests/test_iso8601.py` & `pyvmomi-8.0.1.0.2/tests/test_iso8601.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/test_json.py` & `pyvmomi-8.0.1.0.2/tests/test_json.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,182 +1,172 @@
-# -*- coding: utf-8 -*-
-
-# VMware vSphere Python SDK
-# Copyright (c) 2008-2018 VMware, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import tests
-
-from pyVim import connect
-from pyVmomi import vim
-from pyVmomi.VmomiSupport import VmomiJSONEncoder, templateOf
-from six import PY3
-
-import unittest
-import atexit
-import inspect
-import json
-import os
-
-
-class JSONTests(tests.VCRTestBase):
-    @property
-    def datacenter(self):
-        return getattr(vim, 'Datacenter')('datacenter-2', self.si._stub)
-        
-    @property
-    def datastore(self):
-        return getattr(vim, 'Datastore')('datastore-15', self.si._stub)
-        
-    @property
-    def host(self):
-        return getattr(vim, 'HostSystem')('host-14', self.si._stub)
-
-    @property
-    def network(self):
-        return getattr(vim, 'Network')('network-16', self.si._stub)
-        
-    @property
-    def si(self):
-        if not hasattr(self, '_si'):
-            self._si = connect.SmartConnectNoSSL(
-                host='vcenter', user='my_user', pwd='my_pass')
-            atexit.register(connect.Disconnect, self._si)
-        return self._si
-
-    @property
-    def vm(self):
-        return getattr(vim, 'VirtualMachine')('vm-22', self.si._stub)
-
-    @property
-    def vm2(self):
-        return getattr(vim, 'VirtualMachine')('vm-227', self.si._stub)
-
-    def expect(self, data):
-        """
-        Handle results expectation.  If the expect data file does not
-        exist we write one out.  Otherwise we read and compare.  This
-        means it is the responsibility of the individual creating the
-        .expect files to ensure they are correct.
-        """
-        testname = inspect.stack()[1][3]
-        expectfile = 'tests/files/{0}.expect'.format(testname)
-        if os.path.exists(expectfile):
-            with open(expectfile, 'r') as file:
-                expectdata = file.read()
-            self.assertEqual(data, expectdata)
-        else:
-            with open(expectfile, 'w') as file:
-                file.write(data)
-
-    # NOTE: sort_keys is needed for expect comparison to work;
-    #                 not required for consumption
-
-    # Explodes the VM
-    # By definition if the input is a ManagedObject then it explodes.
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_vm_explode_default.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_vm_explode_default(self):
-        raw = json.dumps(self.vm, cls=VmomiJSONEncoder, sort_keys=True)
-        self.expect(raw)
-        # Basic sanity check
-        data = json.loads(raw)
-        self.assertEqual(data['_vimid'], 'vm-22')
-        self.assertEqual(data['_vimref'], 'vim.VirtualMachine:vm-22')
-        self.assertEqual(data['_vimtype'], 'vim.VirtualMachine')
-        self.assertEqual(data['overallStatus'], 'green')
-        self.assertEqual(len(data['network']), 1)
-        self.assertEqual(len(data['capability']['dynamicProperty']), 0)
-        self.assertIsNone(data['capability']['dynamicType'])
-
-    # Explodes the VM disabling the dynamic field stripping
-    # By definition if the input is a ManagedObject then it explodes.
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_vm_explode_strip_dynamic.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_vm_explode_strip_dynamic(self):
-        raw = json.dumps(self.vm, cls=VmomiJSONEncoder, sort_keys=True,
-                         strip_dynamic=True)
-        self.expect(raw)
-        # Basic sanity check
-        data = json.loads(raw)
-        self.assertEqual(data['_vimid'], 'vm-22')
-        self.assertEqual(data['_vimref'], 'vim.VirtualMachine:vm-22')
-        self.assertEqual(data['_vimtype'], 'vim.VirtualMachine')
-        self.assertEqual(data['overallStatus'], 'green')
-        self.assertEqual(len(data['network']), 1)
-        self.assertTrue('dynamicProperty' not in data['capability'])
-        self.assertTrue('dynamicType' not in data['capability'])
-
-    # Explodes the VM and the VM's networks
-    # Here self.vm is redundant (see above) but not harmful.
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_vm_explode_objs.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_vm_explode_objs_match(self):
-        to_explode = [self.vm]
-        for item in self.vm.network:
-            to_explode.append(item)
-        self.expect(json.dumps(self.vm, cls=VmomiJSONEncoder, sort_keys=True,
-                               explode=to_explode))
-
-    # Explodes by type: all VirtualMachine and all of its snapshots
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_vm_explode_type.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_vm_explode_type_match(self):
-        self.expect(json.dumps([self.vm, self.vm2], cls=VmomiJSONEncoder,
-                               sort_keys=True,
-                               explode=[templateOf('VirtualMachine'),
-                                        templateOf('VirtualMachineSnapshot')]))
-
-    # Test Datacenter
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_datacenter_explode.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_datacenter_explode(self):
-          self.expect(json.dumps(self.datacenter, cls=VmomiJSONEncoder,
-                                 sort_keys=True))
-
-    # Test Datastore
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_datastore_explode.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_datastore_explode(self):
-          self.expect(json.dumps(self.datastore, cls=VmomiJSONEncoder,
-                                 sort_keys=True))
-
-    # Test HostSystem
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_host_explode.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_host_explode(self):
-          self.expect(json.dumps(self.host, cls=VmomiJSONEncoder,
-                                 sort_keys=True))
-
-    # Test Network
-    @unittest.skip("skipped for 7.0 release")
-    @tests.VCRTestBase.my_vcr.use_cassette(
-        'test_json_network_explode.yaml',
-        cassette_library_dir=tests.fixtures_path, record_mode='once')
-    def test_json_network_explode(self):
-          self.expect(json.dumps(self.network, cls=VmomiJSONEncoder,
-                                 sort_keys=True))
+# -*- coding: utf-8 -*-
+
+# VMware vSphere Python SDK
+# Copyright (c) 2008-2018 VMware, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import tests
+
+from pyVim import connect
+from pyVmomi import vim
+from pyVmomi.VmomiJSONEncoder import VmomiJSONEncoder, templateOf
+
+import atexit
+import inspect
+import json
+import os
+
+
+class JSONTests(tests.VCRTestBase):
+    @property
+    def datacenter(self):
+        return getattr(vim, 'Datacenter')('datacenter-2', self.si._stub)
+        
+    @property
+    def datastore(self):
+        return getattr(vim, 'Datastore')('datastore-15', self.si._stub)
+        
+    @property
+    def host(self):
+        return getattr(vim, 'HostSystem')('host-14', self.si._stub)
+
+    @property
+    def network(self):
+        return getattr(vim, 'Network')('network-16', self.si._stub)
+        
+    @property
+    def si(self):
+        if not hasattr(self, '_si'):
+            self._si = connect.SmartConnect(
+                host='vcenter', user='my_user', pwd='my_pass', disableSslCertValidation=True)
+            atexit.register(connect.Disconnect, self._si)
+        return self._si
+
+    @property
+    def vm(self):
+        return getattr(vim, 'VirtualMachine')('vm-22', self.si._stub)
+
+    @property
+    def vm2(self):
+        return getattr(vim, 'VirtualMachine')('vm-227', self.si._stub)
+
+    def expect(self, data):
+        """
+        Handle results expectation.  If the expect data file does not
+        exist we write one out.  Otherwise we read and compare.  This
+        means it is the responsibility of the individual creating the
+        .expect files to ensure they are correct.
+        """
+        testname = inspect.stack()[1][3]
+        expectfile = 'tests/files/{0}.expect'.format(testname)
+        if os.path.exists(expectfile):
+            with open(expectfile, 'r') as file:
+                expectdata = file.read()
+            self.assertEqual(data, expectdata)
+        else:
+            with open(expectfile, 'w') as file:
+                file.write(data)
+
+    # NOTE: sort_keys is needed for expect comparison to work;
+    #                 not required for consumption
+
+    # Explodes the VM
+    # By definition if the input is a ManagedObject then it explodes.
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_vm_explode_default.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_vm_explode_default(self):
+        raw = json.dumps(self.vm, cls=VmomiJSONEncoder, sort_keys=True)
+        self.expect(raw)
+        # Basic sanity check
+        data = json.loads(raw)
+        self.assertEqual(data['_vimid'], 'vm-22')
+        self.assertEqual(data['_vimref'], 'vim.VirtualMachine:vm-22')
+        self.assertEqual(data['_vimtype'], 'vim.VirtualMachine')
+        self.assertEqual(data['overallStatus'], 'green')
+        self.assertEqual(len(data['network']), 1)
+        self.assertEqual(len(data['capability']['dynamicProperty']), 0)
+        self.assertIsNone(data['capability']['dynamicType'])
+
+    # Explodes the VM disabling the dynamic field stripping
+    # By definition if the input is a ManagedObject then it explodes.
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_vm_explode_strip_dynamic.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_vm_explode_strip_dynamic(self):
+        raw = json.dumps(self.vm, cls=VmomiJSONEncoder, sort_keys=True,
+                         strip_dynamic=True)
+        self.expect(raw)
+        # Basic sanity check
+        data = json.loads(raw)
+        self.assertEqual(data['_vimid'], 'vm-22')
+        self.assertEqual(data['_vimref'], 'vim.VirtualMachine:vm-22')
+        self.assertEqual(data['_vimtype'], 'vim.VirtualMachine')
+        self.assertEqual(data['overallStatus'], 'green')
+        self.assertEqual(len(data['network']), 1)
+        self.assertTrue('dynamicProperty' not in data['capability'])
+        self.assertTrue('dynamicType' not in data['capability'])
+
+    # Explodes the VM and the VM's networks
+    # Here self.vm is redundant (see above) but not harmful.
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_vm_explode_objs.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_vm_explode_objs_match(self):
+        to_explode = [self.vm]
+        for item in self.vm.network:
+            to_explode.append(item)
+        self.expect(json.dumps(self.vm, cls=VmomiJSONEncoder, sort_keys=True,
+                               explode=to_explode))
+
+    # Explodes by type: all VirtualMachine and all of its snapshots
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_vm_explode_type.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_vm_explode_type_match(self):
+        self.expect(json.dumps([self.vm, self.vm2], cls=VmomiJSONEncoder,
+                               sort_keys=True,
+                               explode=[templateOf('VirtualMachine'),
+                                        templateOf('VirtualMachineSnapshot')]))
+
+    # Test Datacenter
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_datacenter_explode.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_datacenter_explode(self):
+          self.expect(json.dumps(self.datacenter, cls=VmomiJSONEncoder,
+                                 sort_keys=True))
+
+    # Test Datastore
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_datastore_explode.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_datastore_explode(self):
+          self.expect(json.dumps(self.datastore, cls=VmomiJSONEncoder,
+                                 sort_keys=True))
+
+    # Test HostSystem
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_host_explode.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_host_explode(self):
+          self.expect(json.dumps(self.host, cls=VmomiJSONEncoder,
+                                 sort_keys=True))
+
+    # Test Network
+    @tests.VCRTestBase.my_vcr.use_cassette(
+        'test_json_network_explode.yaml',
+        cassette_library_dir=tests.fixtures_path, record_mode='once')
+    def test_json_network_explode(self):
+          self.expect(json.dumps(self.network, cls=VmomiJSONEncoder,
+                                 sort_keys=True))
```

### Comparing `pyvmomi-8.0.1.0.1/tests/test_managed_object.py` & `pyvmomi-8.0.1.0.2/tests/test_managed_object.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0.1/tests/test_serializer.py` & `pyvmomi-8.0.1.0.2/tests/test_serializer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# -*- coding: utf-8 -*-
-
-# VMware vSphere Python SDK
-# Copyright (c) 2008-2015 VMware, Inc. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-import tests
-from vcr.stubs import VCRHTTPSConnection
-from vcr import config
-
-from pyVmomi import SoapAdapter
-from pyVmomi import SoapStubAdapter
-from pyVmomi import vim
-from pyVmomi.VmomiSupport import GetRequestContext
-
-
-
-class SerializerTests(tests.VCRTestBase):
-    def test_serialize_object(self):
-        val = vim.vm.device.VirtualDeviceSpec.FileOperation()
-        # This line should not raise an exception, especially on Python 3.
-        SoapAdapter.Serialize(val)
-
-    def test_serialize_integer(self):
-        lp = vim.LongPolicy()
-        lp.inherited = False
-        lp.value = 100
-        SoapAdapter.Serialize(lp, version='vim.version.version10')
-
-    def test_serialize_float(self):
-        pc = vim.host.VsanInternalSystem.PolicyCost()
-        pc.diskSpaceToAddressSpaceRatio = 1.0
-        SoapAdapter.Serialize(pc, version='vim.version.version10')
-
-    def test_serialize_unicode(self):
-        self.assertEqual(SoapAdapter.SerializeToUnicode('Ḃ'),
-                         u'<object xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="urn:vim25" xsi:type="xsd:string">\u1e02</object>')
-        self.assertEqual(SoapAdapter.SerializeToUnicode(u'Ḃ'),
-                         u'<object xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="urn:vim25" xsi:type="xsd:string">\u1e02</object>')
-        self.assertEqual(SoapAdapter.SerializeToUnicode(u'\u1e02'),
-                         u'<object xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="urn:vim25" xsi:type="xsd:string">\u1e02</object>')
-
-    def _base_serialize_test(self, soap_creator, request_matcher):
-        my_vcr = config.VCR(
-            custom_patches=(
-                (SoapAdapter, '_HTTPSConnection', VCRHTTPSConnection),))
-        my_vcr.register_matcher('request_matcher', request_matcher)
-
-        with my_vcr.use_cassette(
-                'test_simple_request_serializer.yaml',
-                cassette_library_dir=tests.fixtures_path,
-                record_mode='none',
-                match_on=['request_matcher']) as cass:
-            stub = soap_creator()
-            si = vim.ServiceInstance("ServiceInstance", stub)
-            content = si.RetrieveContent()
-            self.assertTrue(content is not None)
-            self.assertTrue(
-                '<_this type="ServiceInstance">ServiceInstance</_this>'
-                in cass.requests[0].body.decode("utf-8"))
-
-    def _body_request_matcher(self, r1, r2):
-        soap_msg = ('<soapenv:Body>'
-                    '<RetrieveServiceContent xmlns="urn:vim25">'
-                    '<_this type="ServiceInstance">'
-                    'ServiceInstance'
-                    '</_this>'
-                    '</RetrieveServiceContent>'
-                    '</soapenv:Body>')
-        if soap_msg in r1.body.decode("utf-8"):
-            return True
-        raise SystemError('serialization error occurred')
-
-    def _request_context_request_matcher(self, r1, r2):
-        request_context = ('<soapenv:Header><vcSessionCookie>123456789</vcSessionCookie></soapenv:Header>')
-        if request_context in r1.body.decode("utf-8"):
-            return True
-        raise SystemError('serialization error occurred')
-
-    def test_simple_request_serializer(self):
-        def soap_creator():
-            return SoapStubAdapter('vcsa', 443)
-        self._base_serialize_test(soap_creator, self._body_request_matcher)
-
-    def test_request_context_serializer_instance(self):
-        def request_matcher(r1, r2):
-            return self._request_context_request_matcher(r1, r2) and self._body_request_matcher(r1, r2)
-        def soap_creator():
-            return SoapStubAdapter('vcsa', 443, requestContext={'vcSessionCookie': '123456789'})
-        self._base_serialize_test(soap_creator, request_matcher)
-
-    def test_request_context_serializer_global(self):
-        def request_matcher(r1, r2):
-            return self._request_context_request_matcher(r1, r2) and self._body_request_matcher(r1, r2)
-        def soap_creator():
-            return SoapStubAdapter('vcsa', 443)
-        GetRequestContext()['vcSessionCookie'] = '123456789'
-        try:
-            self._base_serialize_test(soap_creator, request_matcher)
-        finally:
-            GetRequestContext().pop("vcSessionCookie")
-
+# -*- coding: utf-8 -*-
+
+# VMware vSphere Python SDK
+# Copyright (c) 2008-2015 VMware, Inc. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import tests
+from vcr.stubs import VCRHTTPSConnection
+from vcr import config
+
+from pyVmomi import SoapAdapter
+from pyVmomi import SoapStubAdapter
+from pyVmomi import vim
+from pyVmomi.VmomiSupport import GetRequestContext
+
+
+
+class SerializerTests(tests.VCRTestBase):
+    def test_serialize_object(self):
+        val = vim.vm.device.VirtualDeviceSpec.FileOperation()
+        # This line should not raise an exception, especially on Python 3.
+        SoapAdapter.Serialize(val)
+
+    def test_serialize_integer(self):
+        lp = vim.LongPolicy()
+        lp.inherited = False
+        lp.value = 100
+        SoapAdapter.Serialize(lp, version='vim.version.version10')
+
+    def test_serialize_float(self):
+        pc = vim.host.VsanInternalSystem.PolicyCost()
+        pc.diskSpaceToAddressSpaceRatio = 1.0
+        SoapAdapter.Serialize(pc, version='vim.version.version10')
+
+    def test_serialize_unicode(self):
+        self.assertEqual(SoapAdapter.SerializeToStr('Ḃ'),
+                         u'<obj versionId="" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="urn:vim25" xsi:type="xsd:string">\u1e02</obj>')
+        self.assertEqual(SoapAdapter.SerializeToStr(u'Ḃ'),
+                         u'<obj versionId="" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="urn:vim25" xsi:type="xsd:string">\u1e02</obj>')
+        self.assertEqual(SoapAdapter.SerializeToStr(u'\u1e02'),
+                         u'<obj versionId="" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="urn:vim25" xsi:type="xsd:string">\u1e02</obj>')
+
+    def _base_serialize_test(self, soap_creator, request_matcher):
+        my_vcr = config.VCR(
+            custom_patches=(
+                (SoapAdapter, '_HTTPSConnection', VCRHTTPSConnection),))
+        my_vcr.register_matcher('request_matcher', request_matcher)
+
+        with my_vcr.use_cassette(
+                'test_simple_request_serializer.yaml',
+                cassette_library_dir=tests.fixtures_path,
+                record_mode='none',
+                match_on=['request_matcher']) as cass:
+            stub = soap_creator()
+            si = vim.ServiceInstance("ServiceInstance", stub)
+            content = si.RetrieveContent()
+            self.assertTrue(content is not None)
+            self.assertTrue(
+                '<_this type="ServiceInstance">ServiceInstance</_this>'
+                in cass.requests[0].body.decode("utf-8"))
+
+    def _body_request_matcher(self, r1, r2):
+        soap_msg = ('<soapenv:Body>'
+                    '<RetrieveServiceContent xmlns="urn:vim25">'
+                    '<_this versionId="5.5" type="ServiceInstance">'
+                    'ServiceInstance'
+                    '</_this>'
+                    '</RetrieveServiceContent>'
+                    '</soapenv:Body>')
+        if soap_msg in r1.body.decode("utf-8"):
+            return True
+        raise SystemError('serialization error occurred')
+
+    def _request_context_request_matcher(self, r1, r2):
+        request_context = ('<soapenv:Header><vcSessionCookie versionId="5.5">123456789</vcSessionCookie></soapenv:Header>')
+        if request_context in r1.body.decode("utf-8"):
+            return True
+        raise SystemError('serialization error occurred')
+
+    def test_simple_request_serializer(self):
+        def soap_creator():
+            return SoapStubAdapter('vcsa', 443)
+        self._base_serialize_test(soap_creator, self._body_request_matcher)
+
+    def test_request_context_serializer_instance(self):
+        def request_matcher(r1, r2):
+            return self._request_context_request_matcher(r1, r2) and self._body_request_matcher(r1, r2)
+        def soap_creator():
+            return SoapStubAdapter('vcsa', 443, requestContext={'vcSessionCookie': '123456789'})
+        self._base_serialize_test(soap_creator, request_matcher)
+
+    def test_request_context_serializer_global(self):
+        def request_matcher(r1, r2):
+            return self._request_context_request_matcher(r1, r2) and self._body_request_matcher(r1, r2)
+        def soap_creator():
+            return SoapStubAdapter('vcsa', 443)
+        GetRequestContext()['vcSessionCookie'] = '123456789'
+        try:
+            self._base_serialize_test(soap_creator, request_matcher)
+        finally:
+            GetRequestContext().pop("vcSessionCookie")
+
```

### Comparing `pyvmomi-8.0.1.0.1/tests/test_virtual_machine_object.py` & `pyvmomi-8.0.1.0.2/tests/test_virtual_machine_object.py`

 * *Files identical despite different names*

