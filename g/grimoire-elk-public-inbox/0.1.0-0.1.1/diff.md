# Comparing `tmp/grimoire_elk_public_inbox-0.1.0.tar.gz` & `tmp/grimoire_elk_public_inbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoire_elk_public_inbox-0.1.0.tar", max compression
+gzip compressed data, was "grimoire_elk_public_inbox-0.1.1.tar", max compression
```

## Comparing `grimoire_elk_public_inbox-0.1.0.tar` & `grimoire_elk_public_inbox-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       50 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/AUTHORS
--rw-r--r--   0        0        0    35149 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/LICENSE
--rw-r--r--   0        0        0      187 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/NEWS
--rw-r--r--   0        0        0     1620 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/__init__.py
--rw-r--r--   0        0        0       86 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/_version.py
--rw-r--r--   0        0        0        0 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/enriched/__init__.py
--rw-r--r--   0        0        0      925 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/enriched/public_inbox.py
--rw-r--r--   0        0        0        0 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/raw/__init__.py
--rw-r--r--   0        0        0     2200 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/raw/public_inbox.py
--rw-r--r--   0        0        0     1071 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/utils.py
--rw-r--r--   0        0        0     1459 2023-06-29 07:45:46.252784 grimoire_elk_public_inbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 grimoire_elk_public_inbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/AUTHORS
+-rw-r--r--   0        0        0    35149 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/LICENSE
+-rw-r--r--   0        0        0      513 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/NEWS
+-rw-r--r--   0        0        0     1620 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/__init__.py
+-rw-r--r--   0        0        0       86 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/_version.py
+-rw-r--r--   0        0        0        0 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/enriched/__init__.py
+-rw-r--r--   0        0        0      925 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/enriched/public_inbox.py
+-rw-r--r--   0        0        0        0 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/raw/__init__.py
+-rw-r--r--   0        0        0     2200 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/raw/public_inbox.py
+-rw-r--r--   0        0        0     1071 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/utils.py
+-rw-r--r--   0        0        0     1459 2023-07-19 08:56:32.854222 grimoire_elk_public_inbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 grimoire_elk_public_inbox-0.1.1/PKG-INFO
```

### Comparing `grimoire_elk_public_inbox-0.1.0/LICENSE` & `grimoire_elk_public_inbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.0/README.md` & `grimoire_elk_public_inbox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/enriched/public_inbox.py` & `grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/enriched/public_inbox.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/raw/public_inbox.py` & `grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/raw/public_inbox.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.0/grimoire_elk_public_inbox/utils.py` & `grimoire_elk_public_inbox-0.1.1/grimoire_elk_public_inbox/utils.py`

 * *Files identical despite different names*

### Comparing `grimoire_elk_public_inbox-0.1.0/pyproject.toml` & `grimoire_elk_public_inbox-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoire-elk-public-inbox"
-version = "0.1.0"
+version = "0.1.1"
 description = "GrimoireELK plugic for public-inbox."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `grimoire_elk_public_inbox-0.1.0/PKG-INFO` & `grimoire_elk_public_inbox-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoire-elk-public-inbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: GrimoireELK plugic for public-inbox.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

