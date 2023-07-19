# Comparing `tmp/cmem_plugin_mattermost-1.0.0.tar.gz` & `tmp/cmem_plugin_mattermost-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_mattermost-1.0.0.tar", max compression
+gzip compressed data, was "cmem_plugin_mattermost-2.0.0.tar", max compression
```

## Comparing `cmem_plugin_mattermost-1.0.0.tar` & `cmem_plugin_mattermost-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11334 2023-03-13 10:06:08.313549 cmem_plugin_mattermost-1.0.0/LICENSE
--rw-r--r--   0        0        0      391 2023-03-13 10:06:08.313549 cmem_plugin_mattermost-1.0.0/README-public.md
--rw-r--r--   0        0        0        0 2023-03-13 10:06:08.313549 cmem_plugin_mattermost-1.0.0/cmem_plugin_mattermost/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:06:08.313549 cmem_plugin_mattermost-1.0.0/cmem_plugin_mattermost/workflow/__init__.py
--rw-r--r--   0        0        0    11554 2023-03-13 10:06:08.313549 cmem_plugin_mattermost-1.0.0/cmem_plugin_mattermost/workflow/mattermost_plugin.py
--rw-r--r--   0        0        0     1858 2023-03-13 10:06:37.682001 cmem_plugin_mattermost-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 cmem_plugin_mattermost-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-19 00:03:24.855655 cmem_plugin_mattermost-2.0.0/LICENSE
+-rw-r--r--   0        0        0      391 2023-07-19 00:03:24.855655 cmem_plugin_mattermost-2.0.0/README-public.md
+-rw-r--r--   0        0        0        0 2023-07-19 00:03:24.855655 cmem_plugin_mattermost-2.0.0/cmem_plugin_mattermost/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:03:24.855655 cmem_plugin_mattermost-2.0.0/cmem_plugin_mattermost/workflow/__init__.py
+-rw-r--r--   0        0        0    11554 2023-07-19 00:03:24.855655 cmem_plugin_mattermost-2.0.0/cmem_plugin_mattermost/workflow/mattermost_plugin.py
+-rw-r--r--   0        0        0     1988 2023-07-19 00:03:57.623858 cmem_plugin_mattermost-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 cmem_plugin_mattermost-2.0.0/PKG-INFO
```

### Comparing `cmem_plugin_mattermost-1.0.0/LICENSE` & `cmem_plugin_mattermost-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_mattermost-1.0.0/cmem_plugin_mattermost/workflow/mattermost_plugin.py` & `cmem_plugin_mattermost-2.0.0/cmem_plugin_mattermost/workflow/mattermost_plugin.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_mattermost-1.0.0/pyproject.toml` & `cmem_plugin_mattermost-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-mattermost"
-version = "1.0.0"
+version = "2.0.0"
 license = "Apache-2.0"
 description = "Send messages to Mattermost channels and users."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -14,35 +14,39 @@
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugin", "mattermost"
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-mattermost"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-responses = "^0.22.0"
-cmem-plugin-base = "^3"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
+responses = "^0.23.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.0"
-pytest-cov = "^4.0.0"
-pytest-memray = "^1.3.0"
-black = "^23.1.0"
-bandit = "^1.7.2"
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.3"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.4.0"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^1.0.0"
-coverage = "^7.1.0"
-defusedxml = "^0.7.1"
-wheel = "^0.38.3"
+typed-ast = "^1.5.4"
+wheel = "^0.38.4"
 types-requests = "^2.28.11.8"
 pytest-docker-compose = "^3.2.1"
+# Downgrade pyyaml to resolve reported in 
+# https://github.com/yaml/pyyaml/issues/724
+pyyaml= "==5.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `cmem_plugin_mattermost-1.0.0/PKG-INFO` & `cmem_plugin_mattermost-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-mattermost
-Version: 1.0.0
+Version: 2.0.0
 Summary: Send messages to Mattermost channels and users.
 Home-page: https://github.com/eccenca/cmem-plugin-mattermost
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,mattermost
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=3,<4)
-Requires-Dist: responses (>=0.22.0,<0.23.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
+Requires-Dist: responses (>=0.23.1,<0.24.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-mattermost
 
 Send messages to [Mattermost](https://mattermost.com/). channels and users.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```

