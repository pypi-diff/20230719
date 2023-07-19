# Comparing `tmp/mcred-1.0.1.tar.gz` & `tmp/mcred-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcred-1.0.1.tar", last modified: Mon Feb  6 22:25:49 2023, max compression
+gzip compressed data, was "mcred-1.0.2.tar", last modified: Wed Jul 19 07:56:09 2023, max compression
```

## Comparing `mcred-1.0.1.tar` & `mcred-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 22:25:49.823971 mcred-1.0.1/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-02-06 20:30:12.000000 mcred-1.0.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      465 2023-02-06 22:25:49.823801 mcred-1.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      283 2023-02-06 22:25:49.000000 mcred-1.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 22:25:49.822163 mcred-1.0.1/mcred/
--rwxrwxrwx   0 root         (0) root         (0)     1282 2023-02-06 22:25:22.000000 mcred-1.0.1/mcred/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 22:25:49.823449 mcred-1.0.1/mcred.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      465 2023-02-06 22:25:49.000000 mcred-1.0.1/mcred.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      188 2023-02-06 22:25:49.000000 mcred-1.0.1/mcred.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-02-06 22:25:49.000000 mcred-1.0.1/mcred.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-02-06 22:25:49.000000 mcred-1.0.1/mcred.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-02-06 22:25:49.000000 mcred-1.0.1/mcred.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-02-06 22:25:49.824038 mcred-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-02-06 22:25:36.000000 mcred-1.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 07:56:09.525420 mcred-1.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-07-19 07:54:44.000000 mcred-1.0.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      465 2023-07-19 07:56:09.525264 mcred-1.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      283 2023-07-19 07:56:09.000000 mcred-1.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 07:56:09.523821 mcred-1.0.2/mcred/
+-rwxrwxrwx   0 root         (0) root         (0)     1392 2023-07-19 07:55:38.000000 mcred-1.0.2/mcred/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-19 07:56:09.524963 mcred-1.0.2/mcred.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      465 2023-07-19 07:56:09.000000 mcred-1.0.2/mcred.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      188 2023-07-19 07:56:09.000000 mcred-1.0.2/mcred.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-19 07:56:09.000000 mcred-1.0.2/mcred.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-19 07:56:09.000000 mcred-1.0.2/mcred.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-07-19 07:56:09.000000 mcred-1.0.2/mcred.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-19 07:56:09.525468 mcred-1.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      467 2023-07-19 07:55:46.000000 mcred-1.0.2/setup.py
```

### Comparing `mcred-1.0.1/LICENSE` & `mcred-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcred-1.0.1/mcred/__init__.py` & `mcred-1.0.2/mcred/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from mclass import DictClass
 import json
 import pathlib
 import os
 import pysftp
-
+cnopts = pysftp.CnOpts()
+cnopts.hostkeys = None    # disable host key checking.
 
 
 class CredManager:
     def __init__(self, host=None, port=None, username=None, password=None, remote_credentials_file_path=None):
         self.host = host
         self.username = username
         self.password = password
@@ -19,14 +20,15 @@
     def pull(self, force=False):
         if not os.path.exists(self.local_file_path) or force:
             with pysftp.Connection(
                 host=self.host, 
                 username=self.username, 
                 password=self.password,
                 port=self.port,
+                cnopts=cnopts,
             ) as sftp:
                 print(f"Downloading credentials from {self.remote_file_path} to {self.local_file_path})")
                 sftp.get(remotepath=self.remote_file_path, localpath=self.local_file_path)
 
     def get(self):
         if os.path.exists(self.local_file_path):
             credentials_dict = json.load(open(self.local_file_path, "r"))
```

