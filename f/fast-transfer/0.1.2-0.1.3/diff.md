# Comparing `tmp/fast_transfer-0.1.2.tar.gz` & `tmp/fast_transfer-0.1.3.tar.gz`

## Comparing `fast_transfer-0.1.2.tar` & `fast_transfer-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0   207302 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/src/fast_transfer/static/bulma.min.css
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/src/fast_transfer/templates/index.html
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/LICENSE
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/README.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fast_transfer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0   207302 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/src/fast_transfer/static/bulma.min.css
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/src/fast_transfer/templates/index.html
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/LICENSE
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/README.md
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fast_transfer-0.1.3/PKG-INFO
```

### Comparing `fast_transfer-0.1.2/src/fast_transfer/static/bulma.min.css` & `fast_transfer-0.1.3/src/fast_transfer/static/bulma.min.css`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.2/src/fast_transfer/templates/index.html` & `fast_transfer-0.1.3/src/fast_transfer/templates/index.html`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.2/.gitignore` & `fast_transfer-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.2/LICENSE` & `fast_transfer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_transfer-0.1.2/pyproject.toml` & `fast_transfer-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ChanMo/fast-transfer"
 "Bug Tracker" = "https://github.com/ChanMo/fast-transfer/issues"
 
 [project.scripts]
-fast-transfer = "fast-transfer.app:cli"
+fast-transfer = "fast_transfer.app:cli"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 path = "src/fast_transfer/__about__.py"
```

### Comparing `fast_transfer-0.1.2/PKG-INFO` & `fast_transfer-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-transfer
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy and fast way to transfer files
 Project-URL: Homepage, https://github.com/ChanMo/fast-transfer
 Project-URL: Bug Tracker, https://github.com/ChanMo/fast-transfer/issues
 Author-email: ChanMo <chan.mo@outlook.com>
 License-File: LICENSE
 Keywords: fast-transfer,http.server,share,transfer
 Classifier: License :: OSI Approved :: MIT License
```

