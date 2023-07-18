# Comparing `tmp/cz-gitmoji-0.0.1.tar.gz` & `tmp/cz-gitmoji-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz-gitmoji-0.0.1.tar", last modified: Tue Jul 18 21:47:15 2023, max compression
+gzip compressed data, was "cz-gitmoji-0.0.2.tar", last modified: Tue Jul 18 22:43:22 2023, max compression
```

## Comparing `cz-gitmoji-0.0.1.tar` & `cz-gitmoji-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:47:15.503129 cz-gitmoji-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 21:47:03.000000 cz-gitmoji-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 21:47:15.503129 cz-gitmoji-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 21:47:03.000000 cz-gitmoji-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 21:47:03.000000 cz-gitmoji-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:47:15.503129 cz-gitmoji-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:47:15.503129 cz-gitmoji-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:47:15.503129 cz-gitmoji-0.0.1/src/cz_gitmoji/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 21:47:03.000000 cz-gitmoji-0.0.1/src/cz_gitmoji/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:47:15.503129 cz-gitmoji-0.0.1/src/cz_gitmoji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 21:47:15.000000 cz-gitmoji-0.0.1/src/cz_gitmoji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 21:47:15.000000 cz-gitmoji-0.0.1/src/cz_gitmoji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:47:15.000000 cz-gitmoji-0.0.1/src/cz_gitmoji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 21:47:15.000000 cz-gitmoji-0.0.1/src/cz_gitmoji.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:43:22.747387 cz-gitmoji-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 22:43:11.000000 cz-gitmoji-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 22:43:22.747387 cz-gitmoji-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 22:43:11.000000 cz-gitmoji-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 22:43:11.000000 cz-gitmoji-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:43:22.747387 cz-gitmoji-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:43:22.743387 cz-gitmoji-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:43:22.743387 cz-gitmoji-0.0.2/src/cz_gitmoji/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 22:43:11.000000 cz-gitmoji-0.0.2/src/cz_gitmoji/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:43:22.747387 cz-gitmoji-0.0.2/src/cz_gitmoji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 22:43:22.000000 cz-gitmoji-0.0.2/src/cz_gitmoji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 22:43:22.000000 cz-gitmoji-0.0.2/src/cz_gitmoji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:43:22.000000 cz-gitmoji-0.0.2/src/cz_gitmoji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 22:43:22.000000 cz-gitmoji-0.0.2/src/cz_gitmoji.egg-info/top_level.txt
```

### Comparing `cz-gitmoji-0.0.1/LICENSE` & `cz-gitmoji-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cz-gitmoji-0.0.1/PKG-INFO` & `cz-gitmoji-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-gitmoji
-Version: 0.0.1
+Version: 0.0.2
 Summary: 🔖 Commitizen plugin for automatic version bumps and changelogs based on Gitmojis 😜
 Author-email: Kamil Paduszyński <paduszyk@gmail.com>
 Project-URL: Homepage, https://github.com/paduszyk/cz-gitmoji
 Project-URL: Repository, https://github.com/paduszyk/cz-gitmoji
 Project-URL: Documentation, https://github.com/paduszyk/cz-gitmoji#readme
 Keywords: commitizen,gitmoji
 Classifier: Development Status :: 1 - Planning
```

### Comparing `cz-gitmoji-0.0.1/README.md` & `cz-gitmoji-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cz-gitmoji-0.0.1/pyproject.toml` & `cz-gitmoji-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cz-gitmoji-0.0.1/src/cz_gitmoji.egg-info/PKG-INFO` & `cz-gitmoji-0.0.2/src/cz_gitmoji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-gitmoji
-Version: 0.0.1
+Version: 0.0.2
 Summary: 🔖 Commitizen plugin for automatic version bumps and changelogs based on Gitmojis 😜
 Author-email: Kamil Paduszyński <paduszyk@gmail.com>
 Project-URL: Homepage, https://github.com/paduszyk/cz-gitmoji
 Project-URL: Repository, https://github.com/paduszyk/cz-gitmoji
 Project-URL: Documentation, https://github.com/paduszyk/cz-gitmoji#readme
 Keywords: commitizen,gitmoji
 Classifier: Development Status :: 1 - Planning
```

