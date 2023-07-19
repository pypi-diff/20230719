# Comparing `tmp/lxd-sphinx-extensions-0.0.8.tar.gz` & `tmp/lxd-sphinx-extensions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxd-sphinx-extensions-0.0.8.tar", last modified: Fri Jul 14 11:28:21 2023, max compression
+gzip compressed data, was "lxd-sphinx-extensions-0.0.9.tar", last modified: Wed Jul 19 09:18:01 2023, max compression
```

## Comparing `lxd-sphinx-extensions-0.0.8.tar` & `lxd-sphinx-extensions-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/config-options/
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/config-options/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.css
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/custom-rst-roles/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/custom-rst-roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/related-links/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/related-links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/related-links/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/related-links/_static/related-links.css
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/related-links/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/terminal-output/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/terminal-output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/terminal-output/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/terminal-output/_static/terminal-output.css
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/terminal-output/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/youtube-links/
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/youtube-links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/youtube-links/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/youtube-links/_static/youtube.css
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/youtube-links/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.201318 lxd-sphinx-extensions-0.0.9/config-options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/config-options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.201318 lxd-sphinx-extensions-0.0.9/config-options/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/config-options/_static/config-options.css
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/config-options/_static/config-options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/config-options/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.201318 lxd-sphinx-extensions-0.0.9/custom-rst-roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/custom-rst-roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.201318 lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-19 09:18:01.000000 lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-19 09:18:01.000000 lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:18:01.000000 lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 09:18:01.000000 lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 09:18:01.000000 lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.201318 lxd-sphinx-extensions-0.0.9/related-links/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/related-links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.201318 lxd-sphinx-extensions-0.0.9/related-links/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/related-links/_static/related-links.css
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/related-links/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/terminal-output/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/terminal-output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/terminal-output/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/terminal-output/_static/terminal-output.css
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/terminal-output/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/youtube-links/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/youtube-links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:18:01.205318 lxd-sphinx-extensions-0.0.9/youtube-links/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/youtube-links/_static/youtube.css
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 09:17:53.000000 lxd-sphinx-extensions-0.0.9/youtube-links/common.py
```

### Comparing `lxd-sphinx-extensions-0.0.8/LICENSE` & `lxd-sphinx-extensions-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/PKG-INFO` & `lxd-sphinx-extensions-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxd-sphinx-extensions
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of Sphinx extensions used in LXD
 Home-page: https://github.com/canonical/lxd-sphinx-extensions
 Author: Ruth Fuchss
 Author-email: ruth.fuchss@canonical.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lxd-sphinx-extensions-0.0.8/README.md` & `lxd-sphinx-extensions-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/config-options/__init__.py` & `lxd-sphinx-extensions-0.0.9/config-options/__init__.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.css` & `lxd-sphinx-extensions-0.0.9/config-options/_static/config-options.css`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.js` & `lxd-sphinx-extensions-0.0.9/config-options/_static/config-options.js`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/config-options/common.py` & `lxd-sphinx-extensions-0.0.9/config-options/common.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/PKG-INFO` & `lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxd-sphinx-extensions
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of Sphinx extensions used in LXD
 Home-page: https://github.com/canonical/lxd-sphinx-extensions
 Author: Ruth Fuchss
 Author-email: ruth.fuchss@canonical.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/SOURCES.txt` & `lxd-sphinx-extensions-0.0.9/lxd_sphinx_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/related-links/__init__.py` & `lxd-sphinx-extensions-0.0.9/related-links/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                     title = split[0][1:]
                     link = split[2][:-1]
                 else:
                     try:
                         r = requests.get(link)
                         r.raise_for_status()
                         soup = BeautifulSoup(r.text, "html.parser")
-                        if soup is None:
+                        if soup.title is None:
                             logger.warning(
                                 pagename
                                 + ": "
                                 + link
                                 + " doesn't have a title."
                             )
                         else:
```

### Comparing `lxd-sphinx-extensions-0.0.8/related-links/_static/related-links.css` & `lxd-sphinx-extensions-0.0.9/related-links/_static/related-links.css`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/related-links/common.py` & `lxd-sphinx-extensions-0.0.9/related-links/common.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/setup.cfg` & `lxd-sphinx-extensions-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lxd-sphinx-extensions
-version = 0.0.8
+version = 0.0.9
 author = Ruth Fuchss
 author_email = ruth.fuchss@canonical.com
 description = A collection of Sphinx extensions used in LXD
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/canonical/lxd-sphinx-extensions
```

### Comparing `lxd-sphinx-extensions-0.0.8/terminal-output/__init__.py` & `lxd-sphinx-extensions-0.0.9/terminal-output/__init__.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/terminal-output/common.py` & `lxd-sphinx-extensions-0.0.9/terminal-output/common.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/youtube-links/__init__.py` & `lxd-sphinx-extensions-0.0.9/youtube-links/__init__.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/youtube-links/_static/youtube.css` & `lxd-sphinx-extensions-0.0.9/youtube-links/_static/youtube.css`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.8/youtube-links/common.py` & `lxd-sphinx-extensions-0.0.9/youtube-links/common.py`

 * *Files identical despite different names*

