# Comparing `tmp/tokendito-2.1.1.tar.gz` & `tmp/tokendito-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokendito-2.1.1.tar", last modified: Sun May 21 00:35:26 2023, max compression
+gzip compressed data, was "tokendito-2.1.2.tar", last modified: Wed Jul 19 15:29:34 2023, max compression
```

## Comparing `tokendito-2.1.1.tar` & `tokendito-2.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:35:26.874058 tokendito-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-21 00:35:16.000000 tokendito-2.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-21 00:35:16.000000 tokendito-2.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 00:35:16.000000 tokendito-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-21 00:35:26.874058 tokendito-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-21 00:35:16.000000 tokendito-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-21 00:35:16.000000 tokendito-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 00:35:16.000000 tokendito-2.1.1/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-21 00:35:16.000000 tokendito-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:35:26.874058 tokendito-2.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-05-21 00:35:16.000000 tokendito-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:35:26.874058 tokendito-2.1.1/tokendito/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/duo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/tokendito.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:35:26.874058 tokendito-2.1.1/tokendito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:34.465836 tokendito-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-19 15:29:22.000000 tokendito-2.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-19 15:29:22.000000 tokendito-2.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-19 15:29:22.000000 tokendito-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-19 15:29:34.465836 tokendito-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-19 15:29:22.000000 tokendito-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-19 15:29:22.000000 tokendito-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 15:29:22.000000 tokendito-2.1.2/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-19 15:29:22.000000 tokendito-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:29:34.465836 tokendito-2.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-07-19 15:29:22.000000 tokendito-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:34.461836 tokendito-2.1.2/tokendito/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/tokendito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42153 2023-07-19 15:29:22.000000 tokendito-2.1.2/tokendito/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:34.465836 tokendito-2.1.2/tokendito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 15:29:34.000000 tokendito-2.1.2/tokendito.egg-info/top_level.txt
```

### Comparing `tokendito-2.1.1/LICENSE.txt` & `tokendito-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/PKG-INFO` & `tokendito-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokendito
-Version: 2.1.1
+Version: 2.1.2
 Summary: Get AWS STS tokens from Okta SSO
 Home-page: https://github.com/dowjones/tokendito
 Author: tokendito
 Author-email: tokendito@dowjones.com
 License: Apache 2.0
 Keywords: okta,aws,sts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tokendito-2.1.1/README.md` & `tokendito-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/setup.py` & `tokendito-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/__init__.py` & `tokendito-2.1.2/tokendito/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import os
 from os.path import expanduser
 import sys
 
 from platformdirs import user_config_dir
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 __title__ = "tokendito"
 __description__ = "Get AWS STS tokens from Okta SSO"
 __long_description_content_type__ = "text/markdown"
 __url__ = "https://github.com/dowjones/tokendito"
 __author__ = "tokendito"
 __author_email__ = "tokendito@dowjones.com"
 __license__ = "Apache 2.0"
```

### Comparing `tokendito-2.1.1/tokendito/__main__.py` & `tokendito-2.1.2/tokendito/__main__.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/aws.py` & `tokendito-2.1.2/tokendito/aws.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/duo.py` & `tokendito-2.1.2/tokendito/duo.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/okta.py` & `tokendito-2.1.2/tokendito/okta.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/tokendito.py` & `tokendito-2.1.2/tokendito/tokendito.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/tool.py` & `tokendito-2.1.2/tokendito/tool.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.1/tokendito/user.py` & `tokendito-2.1.2/tokendito/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,18 +127,23 @@
         dest="okta_org",
         help="Set the Okta Org base URL. This enables role auto-discovery",
     )
     okta_me_group.add_argument(
         "--okta-tile",
         help="Okta tile URL to use.",
     )
-    parser.add_argument("--okta-mfa", help="Sets the MFA method")
+    parser.add_argument(
+        "--okta-mfa",
+        help="Sets the MFA method. You "
+        "can also use the TOKENDITO_OKTA_MFA environment variable.",
+    )
     parser.add_argument(
         "--okta-mfa-response",
-        help="Sets the MFA response to a challenge",
+        help="Sets the MFA response to a challenge. You "
+        "can also use the TOKENDITO_OKTA_MFA_RESPONSE environment variable.",
     )
     parser.add_argument(
         "--quiet",
         dest="user_quiet",
         action="store_true",
         default=False,
         help="Suppress output",
@@ -578,15 +583,15 @@
     :param file: filename
     :param profile: profile to read
     :return: Config object with configuration values
     """
     res = dict()
     pattern = re.compile(r"^(.*?)_(.*)")
 
-    ini = configparser.ConfigParser(default_section=config.user["config_profile"])
+    ini = configparser.RawConfigParser(default_section=config.user["config_profile"])
     # Here, group(1) is the dictionary key, and group(2) the configuration element
     try:
         ini.read(file)
         for key, val in ini.items(profile):
             match = re.search(pattern, key.lower())
             if match:
                 if match.group(1) not in res:
```

### Comparing `tokendito-2.1.1/tokendito.egg-info/PKG-INFO` & `tokendito-2.1.2/tokendito.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokendito
-Version: 2.1.1
+Version: 2.1.2
 Summary: Get AWS STS tokens from Okta SSO
 Home-page: https://github.com/dowjones/tokendito
 Author: tokendito
 Author-email: tokendito@dowjones.com
 License: Apache 2.0
 Keywords: okta,aws,sts
 Classifier: License :: OSI Approved :: Apache Software License
```

