# Comparing `tmp/pynamicui-0.0.4.tar.gz` & `tmp/pynamicui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamicui-0.0.4.tar", last modified: Tue Jul 18 20:52:35 2023, max compression
+gzip compressed data, was "pynamicui-0.0.5.tar", last modified: Tue Jul 18 21:16:26 2023, max compression
```

## Comparing `pynamicui-0.0.4.tar` & `pynamicui-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.514414 pynamicui-0.0.4/
--rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      479 2023-07-18 20:52:35.515412 pynamicui-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4342 2023-07-18 08:45:35.000000 pynamicui-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.388892 pynamicui-0.0.4/pynamicui/
--rw-rw-rw-   0        0        0      386 2023-07-18 20:51:38.000000 pynamicui-0.0.4/pynamicui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.454410 pynamicui-0.0.4/pynamicui/createDom/
--rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.4/pynamicui/createDom/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-07-18 01:43:07.000000 pynamicui-0.0.4/pynamicui/createDom/createDom.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.478406 pynamicui-0.0.4/pynamicui/createElement/
--rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.4/pynamicui/createElement/__init__.py
--rw-rw-rw-   0        0        0     3302 2023-07-18 01:43:31.000000 pynamicui-0.0.4/pynamicui/createElement/createElement.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.511414 pynamicui-0.0.4/pynamicui/createStylesheet/
--rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.4/pynamicui/createStylesheet/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.4/pynamicui/createStylesheet/createStylesheet.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.429405 pynamicui-0.0.4/pynamicui.egg-info/
--rw-rw-rw-   0        0        0      479 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      779 2023-07-18 20:51:46.000000 pynamicui-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      904 2023-07-18 20:52:35.518413 pynamicui-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.998607 pynamicui-0.0.5/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4825 2023-07-18 21:16:25.996610 pynamicui-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4342 2023-07-18 08:45:35.000000 pynamicui-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.940065 pynamicui-0.0.5/pynamicui/
+-rw-rw-rw-   0        0        0      386 2023-07-18 21:13:29.000000 pynamicui-0.0.5/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.978606 pynamicui-0.0.5/pynamicui/createDom/
+-rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.5/pynamicui/createDom/__init__.py
+-rw-rw-rw-   0        0        0     1899 2023-07-18 01:43:07.000000 pynamicui-0.0.5/pynamicui/createDom/createDom.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.985607 pynamicui-0.0.5/pynamicui/createElement/
+-rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.5/pynamicui/createElement/__init__.py
+-rw-rw-rw-   0        0        0     3302 2023-07-18 01:43:31.000000 pynamicui-0.0.5/pynamicui/createElement/createElement.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.993607 pynamicui-0.0.5/pynamicui/createStylesheet/
+-rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.5/pynamicui/createStylesheet/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.5/pynamicui/createStylesheet/createStylesheet.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.970606 pynamicui-0.0.5/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0     4825 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-07-18 21:13:35.000000 pynamicui-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:16:25.998607 pynamicui-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-07-18 21:13:46.000000 pynamicui-0.0.5/setup.py
```

### Comparing `pynamicui-0.0.4/LICENSE` & `pynamicui-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.4/README.md` & `pynamicui-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.4/pynamicui/createDom/createDom.py` & `pynamicui-0.0.5/pynamicui/createDom/createDom.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.4/pynamicui/createElement/createElement.py` & `pynamicui-0.0.5/pynamicui/createElement/createElement.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.4/pynamicui/createStylesheet/createStylesheet.py` & `pynamicui-0.0.5/pynamicui/createStylesheet/createStylesheet.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.4/pyproject.toml` & `pynamicui-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
-requires = ["setuptools>=42", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/zacharie410/PynamicUI"
 
 [tool.tbump.version]
-current = "0.0.4"
+current = "0.0.5"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

