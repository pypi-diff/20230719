# Comparing `tmp/hserv-0.0.2.tar.gz` & `tmp/hserv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hserv-0.0.2.tar", last modified: Wed Jul 19 06:39:00 2023, max compression
+gzip compressed data, was "hserv-0.0.3.tar", last modified: Wed Jul 19 10:15:45 2023, max compression
```

## Comparing `hserv-0.0.2.tar` & `hserv-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:39:00.333733 hserv-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-19 06:38:49.000000 hserv-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-19 06:38:49.000000 hserv-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 06:39:00.333733 hserv-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-19 06:38:49.000000 hserv-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:39:00.333733 hserv-0.0.2/hserv/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-19 06:38:49.000000 hserv-0.0.2/hserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-19 06:38:49.000000 hserv-0.0.2/hserv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-19 06:38:49.000000 hserv-0.0.2/hserv/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:39:00.333733 hserv-0.0.2/hserv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-19 06:38:49.000000 hserv-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 06:39:00.333733 hserv-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-19 06:38:49.000000 hserv-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 10:15:45.022321 hserv-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-19 10:15:27.000000 hserv-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-19 10:15:27.000000 hserv-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 10:15:45.022321 hserv-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-19 10:15:27.000000 hserv-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 10:15:45.018321 hserv-0.0.3/hserv/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-19 10:15:27.000000 hserv-0.0.3/hserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-19 10:15:27.000000 hserv-0.0.3/hserv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-07-19 10:15:27.000000 hserv-0.0.3/hserv/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-07-19 10:15:27.000000 hserv-0.0.3/hserv/supabase.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 10:15:45.022321 hserv-0.0.3/hserv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 10:15:45.000000 hserv-0.0.3/hserv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-19 10:15:45.000000 hserv-0.0.3/hserv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 10:15:45.000000 hserv-0.0.3/hserv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-19 10:15:45.000000 hserv-0.0.3/hserv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-19 10:15:45.000000 hserv-0.0.3/hserv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-19 10:15:27.000000 hserv-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 10:15:45.022321 hserv-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-19 10:15:27.000000 hserv-0.0.3/setup.py
```

### Comparing `hserv-0.0.2/LICENSE` & `hserv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hserv-0.0.2/hserv/server.py` & `hserv-0.0.3/hserv/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Optional, Union
 from dataclasses import dataclass
 import re
-import os
 
 from fabric import Connection
 
 
 @dataclass
 class HydrocodeServer(object):
     connection: Optional[Union[Connection, str]] = None
-    supabase_location: Optional[str] = os.path.expanduser('~')
 
     def __post_init__(self):
         # set connection to localhost if None
         if self.connection is None:
             self.connection = 'localhost'
         
         # create a connection
@@ -48,7 +46,10 @@
             docker_version=self._extract_semver('docker --version'),
             nginx_version=self._extract_semver('nginx -v'),
             certbot_version=self._extract_semver('certbot --version'),
         )
 
         # return
         return info
+
+    def supabase(self, project: str):
+        pass
```

### Comparing `hserv-0.0.2/setup.py` & `hserv-0.0.3/setup.py`

 * *Files identical despite different names*

