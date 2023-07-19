# Comparing `tmp/timedctl-3.0.0.tar.gz` & `tmp/timedctl-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-3.0.0.tar", max compression
+gzip compressed data, was "timedctl-3.0.1.tar", max compression
```

## Comparing `timedctl-3.0.0.tar` & `timedctl-3.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-19 10:03:17.733500 timedctl-3.0.0/LICENSE
--rw-r--r--   0        0        0      810 2023-07-19 10:03:17.733500 timedctl-3.0.0/README.md
--rw-r--r--   0        0        0      823 2023-07-19 10:03:18.757514 timedctl-3.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-19 10:03:17.733500 timedctl-3.0.0/timedctl/__init__.py
--rwxr-xr-x   0        0        0    11501 2023-07-19 10:03:17.733500 timedctl-3.0.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 timedctl-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-19 12:07:18.079848 timedctl-3.0.1/LICENSE
+-rw-r--r--   0        0        0      810 2023-07-19 12:07:18.079848 timedctl-3.0.1/README.md
+-rw-r--r--   0        0        0      824 2023-07-19 12:07:19.087905 timedctl-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-19 12:07:18.079848 timedctl-3.0.1/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    11501 2023-07-19 12:07:18.083849 timedctl-3.0.1/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1519 1970-01-01 00:00:00.000000 timedctl-3.0.1/PKG-INFO
```

### Comparing `timedctl-3.0.0/LICENSE` & `timedctl-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-3.0.0/README.md` & `timedctl-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-3.0.0/pyproject.toml` & `timedctl-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "timedctl"
-version = "3.0.0"
+version = "3.0.1"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "0.2.0"
+libtimed = "^0.2.1"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
```

### Comparing `timedctl-3.0.0/timedctl/timedctl.py` & `timedctl-3.0.1/timedctl/timedctl.py`

 * *Files identical despite different names*

### Comparing `timedctl-3.0.0/PKG-INFO` & `timedctl-3.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 3.0.0
+Version: 3.0.1
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: libtimed (==0.2.0)
+Requires-Dist: libtimed (>=0.2.1,<0.3.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

