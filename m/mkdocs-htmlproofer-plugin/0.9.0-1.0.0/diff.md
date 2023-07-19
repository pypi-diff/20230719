# Comparing `tmp/mkdocs-htmlproofer-plugin-0.9.0.tar.gz` & `tmp/mkdocs-htmlproofer-plugin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-htmlproofer-plugin-0.9.0.tar", last modified: Fri Oct  7 12:31:39 2022, max compression
+gzip compressed data, was "mkdocs-htmlproofer-plugin-1.0.0.tar", last modified: Wed Jul 19 14:05:25 2023, max compression
```

## Comparing `mkdocs-htmlproofer-plugin-0.9.0.tar` & `mkdocs-htmlproofer-plugin-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/
--rw-r--r--   0 tianlzhang (110523479) 110523479     4998 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/PKG-INFO
--rw-r--r--   0 tianlzhang (110523479) 110523479     3148 2021-09-18 01:12:34.000000 mkdocs-htmlproofer-plugin-0.9.0/README.md
-drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/
--rw-r--r--   0 tianlzhang (110523479) 110523479        0 2021-09-18 01:12:34.000000 mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/__init__.py
--rw-r--r--   0 tianlzhang (110523479) 110523479     7480 2022-10-07 12:29:09.000000 mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/plugin.py
-drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/
--rw-r--r--   0 tianlzhang (110523479) 110523479     4998 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO
--rw-r--r--   0 tianlzhang (110523479) 110523479      360 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479        1 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       69 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/entry_points.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       51 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/requires.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       12 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/top_level.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       38 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/setup.cfg
--rw-r--r--   0 tianlzhang (110523479) 110523479     1444 2022-10-07 12:30:55.000000 mkdocs-htmlproofer-plugin-0.9.0/setup.py
+drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2023-07-19 14:05:25.889182 mkdocs-htmlproofer-plugin-1.0.0/
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     1070 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.0.0/LICENSE.md
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     4950 2023-07-19 14:05:25.888896 mkdocs-htmlproofer-plugin-1.0.0/PKG-INFO
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     4048 2023-07-19 14:03:09.000000 mkdocs-htmlproofer-plugin-1.0.0/README.md
+drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2023-07-19 14:05:25.883519 mkdocs-htmlproofer-plugin-1.0.0/htmlproofer/
+-rw-r--r--   0 tianlzhang   (503) staff       (20)        0 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.0.0/htmlproofer/__init__.py
+-rw-r--r--   0 tianlzhang   (503) staff       (20)    11782 2023-07-19 14:03:09.000000 mkdocs-htmlproofer-plugin-1.0.0/htmlproofer/plugin.py
+drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2023-07-19 14:05:25.888090 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     4950 2023-07-19 14:05:25.000000 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 tianlzhang   (503) staff       (20)      386 2023-07-19 14:05:25.000000 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)        1 2023-07-19 14:05:25.000000 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       68 2023-07-19 14:05:25.000000 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       47 2023-07-19 14:05:25.000000 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/requires.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       12 2023-07-19 14:05:25.000000 mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/top_level.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)      175 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.0.0/pyproject.toml
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       38 2023-07-19 14:05:25.889233 mkdocs-htmlproofer-plugin-1.0.0/setup.cfg
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     1431 2023-07-19 14:03:45.000000 mkdocs-htmlproofer-plugin-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mkdocs-htmlproofer-plugin-0.9.0/PKG-INFO` & `mkdocs-htmlproofer-plugin-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 Metadata-Version: 2.1
 Name: mkdocs-htmlproofer-plugin
-Version: 0.9.0
+Version: 1.0.0
 Summary: A MkDocs plugin that validates URL in rendered HTML files
 Home-page: https://github.com/manuzhang/mkdocs-htmlproofer-plugin
 Author: Manu Zhang
 Author-email: owenzhang1990@gmail.com
 License: MIT
-Description: # mkdocs-htmlproofer-plugin [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-htmlproofer-plugin.svg)](https://pypi.org/project/mkdocs-htmlproofer-plugin)
-        
-        [![GitHub Actions](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml)
-        
-        *A [MkDocs](https://www.mkdocs.org/) plugin that validates URLs, including anchors, in rendered html files*.
-        
-        ## Installation
-        
-        0. Prerequisites
-        
-        * Python >= 3.6
-        * MkDocs >= 0.17
-        
-        1. Install the package with pip:
-        
-        ```bash
-        pip install mkdocs-htmlproofer-plugin
-        ```
-        
-        2. Enable the plugin in your `mkdocs.yml`:
-        
-        ```yaml
-        plugins:
-            - search
-            - htmlproofer
-        ```
-        
-        > **Note:** If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin.
-        MkDocs enables it by default if there is no `plugins` entry set, but now you have to enable it explicitly.
-        
-        ```yaml
-        plugins:
-            - search
-            - htmlproofer
-        ```
-        
-        To enable cross-page anchor validation, you must set `use_directory_urls = False` in `mkdocs.yml`:
-        
-        ```yaml
-        use_directory_urls: False
-        ```
-        
-        ## Configuring
-        
-        ### `enabled`
-        
-        True by default, allows toggling whether the plugin is enabled.
-        Useful for local development where you may want faster build times.
-        
-        ```yaml
-        plugins:
-          - htmlproofer:
-              enabled: !ENV [ENABLED_HTMLPROOFER, True]
-        ```
-        
-        Which enables you do disable the plugin locally using:
-        
-        ```bash
-        export ENABLED_HTMLPROOFER=false
-        mkdocs serve
-        ```
-        
-        
-        ### `raise_error`
-        
-        Optionally, you may raise an error and fail the build on bad url status.
-        
-        ```yaml
-        plugins:
-          - htmlproofer:
-              raise_error: True
-        ```
-        
-        ### `raise_error_excludes`
-        
-        When specifying `raise_error: True`, it is possible to ignore errors
-        for combinations of urls (`'*'` means all urls) and status codes with `raise_error_excludes`.
-        
-        ```yaml
-        plugins:
-          - search
-          - htmlproofer:
-              raise_error: True
-              raise_error_excludes:
-                504: ['https://www.mkdocs.org/']
-                404: ['https://github.com/manuzhang/mkdocs-htmlproofer-plugin']
-                400: ['*']
-        ```
-        
-        ### `validate_external_urls`
-        
-        Avoids validating any external URLs (i.e those starting with http:// or https://).
-        This will be faster if you just want to validate local anchors, as it does not make any network requests.
-        
-        ```
-        plugins:
-          - htmlproofer:
-              validate_external_urls: False
-        ```
-        
-        ### `validate_rendered_template`
-        
-        Validates the entire rendered template for each page - including the navigation, header, footer, etc.
-        This defaults to off because it is much slower and often redundant to repeat for every single page.
-        
-        ```
-        plugins:
-          - htmlproofer:
-              validate_rendered_template: True
-        ```
-        
-        ## Improving
-        
-        More information about plugins in the [MkDocs documentation](http://www.mkdocs.org/user-guide/plugins/)
-        
-        ## Acknowledgement
-        
-        This work is based on the [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) project and the [Finding and Fixing Website Link Rot with Python, BeautifulSoup and Requests](https://www.twilio.com/blog/2018/07/find-fix-website-link-rot-python-beautifulsoup-requests.html) article. 
-        
 Keywords: mkdocs python markdown
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# mkdocs-htmlproofer-plugin [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-htmlproofer-plugin.svg)](https://pypi.org/project/mkdocs-htmlproofer-plugin)
+
+[![GitHub Actions](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml)
+
+*A [MkDocs](https://www.mkdocs.org/) plugin that validates URLs, including anchors, in rendered html files*.
+
+## Installation
+
+0. Prerequisites
+
+* Python >= 3.8
+* MkDocs >= 1.4.0
+
+1. Install the package with pip:
+
+```bash
+pip install mkdocs-htmlproofer-plugin
+```
+
+2. Enable the plugin in your `mkdocs.yml`:
+
+> **Note:** If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin.
+MkDocs enables it by default if there is no `plugins` entry set, but now you have to enable it explicitly.
+
+```yaml
+plugins:
+    - search
+    - htmlproofer
+```
+
+To enable cross-page anchor validation, you must set `use_directory_urls = False` in `mkdocs.yml`:
+
+```yaml
+use_directory_urls: False
+```
+
+## Configuring
+
+### `enabled`
+
+True by default, allows toggling whether the plugin is enabled.
+Useful for local development where you may want faster build times.
+
+```yaml
+plugins:
+  - htmlproofer:
+      enabled: !ENV [ENABLED_HTMLPROOFER, True]
+```
+
+Which enables you do disable the plugin locally using:
+
+```bash
+export ENABLED_HTMLPROOFER=false
+mkdocs serve
+```
+
+
+### `raise_error`
+
+Optionally, you may raise an error and fail the build on first bad url status. Takes precedense over `raise_error_after_finish`.
+
+```yaml
+plugins:
+  - htmlproofer:
+      raise_error: True
+```
+
+### `raise_error_after_finish`
+
+Optionally, you may want to raise an error and fail the build on at least one bad url status after all links have been checked.
+
+```yaml
+plugins:
+  - htmlproofer:
+      raise_error_after_finish: True
+```
+
+### `raise_error_excludes`
+
+When specifying `raise_error: True` or `raise_error_after_finish: True`, it is possible to ignore errors
+for combinations of urls (`'*'` means all urls) and status codes with `raise_error_excludes`.
+
+```yaml
+plugins:
+  - search
+  - htmlproofer:
+      raise_error: True
+      raise_error_excludes:
+        504: ['https://www.mkdocs.org/']
+        404: ['https://github.com/manuzhang/mkdocs-htmlproofer-plugin']
+        400: ['*']
+```
+
+### `validate_external_urls`
+
+Avoids validating any external URLs (i.e those starting with http:// or https://).
+This will be faster if you just want to validate local anchors, as it does not make any network requests.
+
+```yaml
+plugins:
+  - htmlproofer:
+      validate_external_urls: False
+```
+
+### `validate_rendered_template`
+
+Validates the entire rendered template for each page - including the navigation, header, footer, etc.
+This defaults to off because it is much slower and often redundant to repeat for every single page.
+
+```yaml
+plugins:
+  - htmlproofer:
+      validate_rendered_template: True
+```
+
+## Compatibility with `attr_list` extension
+
+If you need to manually specify anchors make use of the `attr_list` [extension](https://python-markdown.github.io/extensions/attr_list) in the markdown. 
+This can be useful for multilingual documentation to keep anchors as language neutral permalinks in all languages.
+
+* A sample for a heading `# Grüße {#greetings}` (the slugified generated anchor `Gre` is overwritten with `greetings`).
+* This also works for images `this is a nice image [](foo-bar.png){#nice-image}` 
+* And generall for paragraphs:
+```markdown
+Listing: This is noteworthy.
+{#paragraphanchor}
+```
+
+## Improving
+
+More information about plugins in the [MkDocs documentation](http://www.mkdocs.org/user-guide/plugins/)
+
+## Acknowledgement
+
+This work is based on the [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) project and the [Finding and Fixing Website Link Rot with Python, BeautifulSoup and Requests](https://www.twilio.com/blog/2018/07/find-fix-website-link-rot-python-beautifulsoup-requests.html) article.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs-htmlproofer-plugin-0.9.0/README.md` & `mkdocs-htmlproofer-plugin-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,31 +4,25 @@
 
 *A [MkDocs](https://www.mkdocs.org/) plugin that validates URLs, including anchors, in rendered html files*.
 
 ## Installation
 
 0. Prerequisites
 
-* Python >= 3.6
-* MkDocs >= 0.17
+* Python >= 3.8
+* MkDocs >= 1.4.0
 
 1. Install the package with pip:
 
 ```bash
 pip install mkdocs-htmlproofer-plugin
 ```
 
 2. Enable the plugin in your `mkdocs.yml`:
 
-```yaml
-plugins:
-    - search
-    - htmlproofer
-```
-
 > **Note:** If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin.
 MkDocs enables it by default if there is no `plugins` entry set, but now you have to enable it explicitly.
 
 ```yaml
 plugins:
     - search
     - htmlproofer
@@ -59,25 +53,35 @@
 export ENABLED_HTMLPROOFER=false
 mkdocs serve
 ```
 
 
 ### `raise_error`
 
-Optionally, you may raise an error and fail the build on bad url status.
+Optionally, you may raise an error and fail the build on first bad url status. Takes precedense over `raise_error_after_finish`.
 
 ```yaml
 plugins:
   - htmlproofer:
       raise_error: True
 ```
 
+### `raise_error_after_finish`
+
+Optionally, you may want to raise an error and fail the build on at least one bad url status after all links have been checked.
+
+```yaml
+plugins:
+  - htmlproofer:
+      raise_error_after_finish: True
+```
+
 ### `raise_error_excludes`
 
-When specifying `raise_error: True`, it is possible to ignore errors
+When specifying `raise_error: True` or `raise_error_after_finish: True`, it is possible to ignore errors
 for combinations of urls (`'*'` means all urls) and status codes with `raise_error_excludes`.
 
 ```yaml
 plugins:
   - search
   - htmlproofer:
       raise_error: True
@@ -88,31 +92,44 @@
 ```
 
 ### `validate_external_urls`
 
 Avoids validating any external URLs (i.e those starting with http:// or https://).
 This will be faster if you just want to validate local anchors, as it does not make any network requests.
 
-```
+```yaml
 plugins:
   - htmlproofer:
       validate_external_urls: False
 ```
 
 ### `validate_rendered_template`
 
 Validates the entire rendered template for each page - including the navigation, header, footer, etc.
 This defaults to off because it is much slower and often redundant to repeat for every single page.
 
-```
+```yaml
 plugins:
   - htmlproofer:
       validate_rendered_template: True
 ```
 
+## Compatibility with `attr_list` extension
+
+If you need to manually specify anchors make use of the `attr_list` [extension](https://python-markdown.github.io/extensions/attr_list) in the markdown. 
+This can be useful for multilingual documentation to keep anchors as language neutral permalinks in all languages.
+
+* A sample for a heading `# Grüße {#greetings}` (the slugified generated anchor `Gre` is overwritten with `greetings`).
+* This also works for images `this is a nice image [](foo-bar.png){#nice-image}` 
+* And generall for paragraphs:
+```markdown
+Listing: This is noteworthy.
+{#paragraphanchor}
+```
+
 ## Improving
 
 More information about plugins in the [MkDocs documentation](http://www.mkdocs.org/user-guide/plugins/)
 
 ## Acknowledgement
 
 This work is based on the [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) project and the [Finding and Fixing Website Link Rot with Python, BeautifulSoup and Requests](https://www.twilio.com/blog/2018/07/find-fix-website-link-rot-python-beautifulsoup-requests.html) article.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/plugin.py` & `mkdocs-htmlproofer-plugin-1.0.0/htmlproofer/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,168 +1,273 @@
-from functools import lru_cache
+from functools import lru_cache, partial
 import os.path
 import pathlib
 import re
-import sys
-from typing import Optional, Set
+from typing import Dict, Optional, Set
+import urllib.parse
 import uuid
 
 from bs4 import BeautifulSoup, SoupStrainer
 from markdown.extensions.toc import slugify
+from mkdocs import utils
 from mkdocs.config import Config, config_options
 from mkdocs.exceptions import PluginError
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import File, Files
 from mkdocs.structure.pages import Page
 import requests
 import urllib3
 
 URL_TIMEOUT = 10.0
 _URL_BOT_ID = f'Bot {uuid.uuid4()}'
-URL_HEADERS = {'User-Agent': _URL_BOT_ID}
+URL_HEADERS = {'User-Agent': _URL_BOT_ID, 'Accept-Language': '*'}
+NAME = "htmlproofer"
 
-EXTERNAL_URL_PATTERN = re.compile(r'https?://')
-MARKDOWN_ANCHOR_PATTERN = re.compile(r'(.+)#(.+)')
+MARKDOWN_ANCHOR_PATTERN = re.compile(r'([^#]+)(#(.+))?')
 HEADING_PATTERN = re.compile(r'\s*#+\s*(.*)')
 HTML_LINK_PATTERN = re.compile(r'.*<a id=\"(.*)\">.*')
 IMAGE_PATTERN = re.compile(r'\[\!\[.*\]\(.*\)\].*|\!\[.*\]\[.*\].*')
 LOCAL_PATTERNS = [
     re.compile(rf'https?://{local}')
     for local in ('localhost', '127.0.0.1', 'app_server')
 ]
+ATTRLIST_ANCHOR_PATTERN = re.compile(r'\{.*?\#([^\s\}]*).*?\}')
+ATTRLIST_PATTERN = re.compile(r'\{.*?\}')
+
+# Example emojis:
+#   :banana:
+#   :smiley_cat:
+#   :octicons-apps-16:
+#   :material-star:
+EMOJI_PATTERN = re.compile(r'\:[a-z0-9_-]+\:')
 
 urllib3.disable_warnings()
 
 
+def log_info(msg, *args, **kwargs):
+    utils.log.info(f"{NAME}: {msg}", *args, **kwargs)
+
+
+def log_warning(msg, *args, **kwargs):
+    utils.log.warning(f"{NAME}: {msg}", *args, **kwargs)
+
+
+def log_error(msg, *args, **kwargs):
+    utils.log.error(f"{NAME}: {msg}", *args, **kwargs)
+
+
 class HtmlProoferPlugin(BasePlugin):
-    files: Files
+    files: Dict[str, File]
+    invalid_links = False
 
     config_scheme = (
         ("enabled", config_options.Type(bool, default=True)),
         ('raise_error', config_options.Type(bool, default=False)),
+        ('raise_error_after_finish', config_options.Type(bool, default=False)),
         ('raise_error_excludes', config_options.Type(dict, default={})),
         ('validate_external_urls', config_options.Type(bool, default=True)),
         ('validate_rendered_template', config_options.Type(bool, default=False)),
     )
 
     def __init__(self):
         self._session = requests.Session()
         self._session.verify = False
         self._session.headers.update(URL_HEADERS)
         self._session.max_redirects = 5
+        self.files = {}
+        self.scheme_handlers = {
+            "http": partial(HtmlProoferPlugin.resolve_web_scheme, self),
+            "https": partial(HtmlProoferPlugin.resolve_web_scheme, self),
+        }
         super().__init__()
 
+    def on_post_build(self, config: Config) -> None:
+        if self.config['raise_error_after_finish'] and self.invalid_links:
+            raise PluginError("Invalid links present.")
+
     def on_page_markdown(self, markdown: str, page: Page, config: Config, files: Files) -> None:
         # Store files to allow inspecting Markdown files in later stages.
-        self.files = files
+        self.files.update({os.path.normpath(file.url): file for file in files})
 
     def on_post_page(self, output_content: str, page: Page, config: Config) -> None:
         if not self.config['enabled']:
             return
 
         use_directory_urls = config.data["use_directory_urls"]
 
         # Optimization: only parse links and headings
         # li, sup are used for footnotes
         strainer = SoupStrainer(('a', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li', 'sup', 'img'))
 
         content = output_content if self.config['validate_rendered_template'] else page.content
-        soup = BeautifulSoup(content, 'lxml', parse_only=strainer)
+        soup = BeautifulSoup(content, 'html.parser', parse_only=strainer)
 
         all_element_ids = set(tag['id'] for tag in soup.select('[id]'))
         all_element_ids.add('')  # Empty anchor is commonly used, but not real
         for a in soup.find_all('a', href=True):
             url = a['href']
 
             url_status = self.get_url_status(url, page.file.src_path, all_element_ids, self.files, use_directory_urls)
 
-            if self.bad_url(url_status) is True:
-                error = f'invalid url - {url} [{url_status}] [{page.file.src_path}]'
+            if self.bad_url(url_status) and self.is_error(self.config, url, url_status):
+                self.report_invalid_url(url, url_status, page.file.src_path)
 
-                is_error = self.is_error(self.config, url, url_status)
-                if self.config['raise_error'] and is_error:
-                    raise PluginError(error)
-                elif is_error:
-                    print(error)
+    def report_invalid_url(self, url, url_status, src_path):
+        error = f'invalid url - {url} [{url_status}] [{src_path}]'
+        if self.config['raise_error']:
+            raise PluginError(error)
+        elif self.config['raise_error_after_finish']:
+            log_error(error)
+            self.invalid_links = True
+        else:
+            log_warning(error)
+
+    def get_external_url(self, url, scheme, src_path):
+        try:
+            return self.scheme_handlers[scheme](url)
+        except KeyError:
+            log_info(f'Unknown url-scheme "{scheme}:" detected. "{url}" from "{src_path}" will not be checked.')
+        return 0
 
     @lru_cache(maxsize=1000)
-    def get_external_url(self, url: str) -> int:
+    def resolve_web_scheme(self, url: str) -> int:
         try:
-            response = self._session.head(url, timeout=URL_TIMEOUT)
+            response = self._session.get(url, timeout=URL_TIMEOUT)
             return response.status_code
         except requests.exceptions.Timeout:
             return 504
         except requests.exceptions.TooManyRedirects:
             return -1
         except requests.exceptions.ConnectionError:
             return -1
 
-    def get_url_status(self, url: str, src_path: str, all_element_ids: Set[str], files: Files,
-                       use_directory_urls: bool) -> int:
+    def get_url_status(
+            self,
+            url: str,
+            src_path: str,
+            all_element_ids: Set[str],
+            files: Dict[str, File],
+            use_directory_urls: bool
+    ) -> int:
         if any(pat.match(url) for pat in LOCAL_PATTERNS):
             return 0
 
-        if url.startswith('#'):
+        scheme, _, path, _, fragment = urllib.parse.urlsplit(url)
+        if scheme:
+            if self.config['validate_external_urls']:
+                return self.get_external_url(url, scheme, src_path)
+            return 0
+        if fragment and not path:
             return 0 if url[1:] in all_element_ids else 404
-        elif EXTERNAL_URL_PATTERN.match(url):
-            if not self.config['validate_external_urls']:
-                return 0
-            return self.get_external_url(url)
         elif not use_directory_urls:
             # use_directory_urls = True injects too many challenges for locating the correct target
             # Markdown file, so disable target anchor validation in this case. Examples include:
             # ../..#BAD_ANCHOR style links to index.html and extra ../ inserted into relative
             # links.
-
-            match = MARKDOWN_ANCHOR_PATTERN.match(url)
-            if match is not None:
-                # URL is a link to another local Markdown file that includes an anchor.
-                url_target, anchor = match.groups()
-                target_markdown = self.find_target_markdown(url_target, src_path, files)
-                if (target_markdown is None
-                        or not self.contains_anchor(target_markdown, anchor)):
-                    # The corresponding Markdown header for this anchor was not found.
-                    return 404
+            is_valid = self.is_url_target_valid(url, src_path, files)
+            url_status = 404
+            if not is_valid and self.is_error(self.config, url, url_status):
+                log_warning(f"Unable to locate source file for: {url}")
+                return url_status
+            return 0
         return 0
 
     @staticmethod
-    def find_target_markdown(url: str, src_path: str, files: Files) -> Optional[str]:
-        """From a built URL, find the original Markdown source from the project that built it."""
+    def is_url_target_valid(url: str, src_path: str, files: Dict[str, File]) -> bool:
+        match = MARKDOWN_ANCHOR_PATTERN.match(url)
+        if match is None:
+            return True
+
+        url_target, _, optional_anchor = match.groups()
+        _, extension = os.path.splitext(url_target)
+        if extension == ".html":
+            # URL is a link to another local Markdown file that may include an anchor.
+            target_markdown = HtmlProoferPlugin.find_target_markdown(url_target, src_path, files)
+            if target_markdown is None:
+                # The corresponding Markdown page was not found.
+                return False
+            if optional_anchor and not HtmlProoferPlugin.contains_anchor(target_markdown, optional_anchor):
+                # The corresponding Markdown header for this anchor was not found.
+                return False
+        elif HtmlProoferPlugin.find_source_file(url_target, src_path, files) is None:
+            return False
+        return True
 
-        # Handle relative links by concatenating the source dir with the destination path
-        search = os.path.normpath(str(pathlib.Path(src_path).parent / pathlib.Path(url)))
-        for file in files.src_paths.values():  # type: File
-            if file.url == search and file.page:
-                return file.page.markdown
+    @staticmethod
+    def find_target_markdown(url: str, src_path: str, files: Dict[str, File]) -> Optional[str]:
+        """From a built URL, find the original Markdown source from the project that built it."""
 
-        print(f"Warning: Unable to locate Markdown source file for: {url}", file=sys.stderr)
+        file = HtmlProoferPlugin.find_source_file(url, src_path, files)
+        if file and file.page:
+            return file.page.markdown
         return None
 
     @staticmethod
+    def find_source_file(url: str, src_path: str, files: Dict[str, File]) -> Optional[File]:
+        """From a built URL, find the original file from the project that built it."""
+
+        if len(url) > 1 and url[0] == '/':
+            # Convert root/site paths
+            search_path = os.path.normpath(url[1:])
+        else:
+            # Handle relative links by concatenating the source dir with the destination path
+            search_path = os.path.normpath(str(pathlib.Path(src_path).parent / pathlib.Path(url)))
+
+        try:
+            return files[search_path]
+        except KeyError:
+            return None
+
+    @staticmethod
     def contains_anchor(markdown: str, anchor: str) -> bool:
         """Check if a set of Markdown source text contains a heading that corresponds to a
         given anchor."""
         for line in markdown.splitlines():
             # Markdown allows whitespace before headers and an arbitrary number of #'s.
             heading_match = HEADING_PATTERN.match(line)
             if heading_match is not None:
                 heading = heading_match.groups()[0]
 
+                # Headings are allowed to have attr_list after them, of the form:
+                # # Heading { #testanchor .testclass }
+                # # Heading {: #testanchor .testclass }
+                # # Heading {.testclass #testanchor}
+                # # Heading {.testclass}
+                # these can override the headings anchor id, or alternatively just provide additional class etc.
+                attr_list_anchor_match = ATTRLIST_ANCHOR_PATTERN.match(heading)
+                if attr_list_anchor_match is not None:
+                    attr_list_anchor = heading_match.groups()[1]
+                    if anchor == attr_list_anchor:
+                        return True
+
+                heading = re.sub(ATTRLIST_PATTERN, '', heading)  # remove any attribute list from heading, before slugify
+
                 # Headings are allowed to have images after them, of the form:
                 # # Heading [![Image](image-link)] or ![Image][image-reference]
                 # But these images are not included in the generated anchor, so remove them.
                 heading = re.sub(IMAGE_PATTERN, '', heading)
+
+                # Headings are allowed to have emojis in them under certain Mkdocs themes.
+                # https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#emoji
+                heading = re.sub(EMOJI_PATTERN, '', heading)
+
                 anchor_slug = slugify(heading, '-')
                 if anchor == anchor_slug:
                     return True
 
             link_match = HTML_LINK_PATTERN.match(line)
             if link_match is not None and link_match.group(1) == anchor:
                 return True
 
+            # Any attribute list at end of paragraphs or after images can also generate an anchor (in addition to
+            # the heading ones) so gather those and check as well (multiple could be a line so gather all)
+            for attr_list_anchor in re.findall(ATTRLIST_ANCHOR_PATTERN, line):
+                if anchor == attr_list_anchor:
+                    return True
+
         return False
 
     @staticmethod
     def bad_url(url_status: int) -> bool:
         if url_status == -1:
             return True
         elif url_status == 401 or url_status == 403:
```

### Comparing `mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO` & `mkdocs-htmlproofer-plugin-1.0.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 Metadata-Version: 2.1
 Name: mkdocs-htmlproofer-plugin
-Version: 0.9.0
+Version: 1.0.0
 Summary: A MkDocs plugin that validates URL in rendered HTML files
 Home-page: https://github.com/manuzhang/mkdocs-htmlproofer-plugin
 Author: Manu Zhang
 Author-email: owenzhang1990@gmail.com
 License: MIT
-Description: # mkdocs-htmlproofer-plugin [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-htmlproofer-plugin.svg)](https://pypi.org/project/mkdocs-htmlproofer-plugin)
-        
-        [![GitHub Actions](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml)
-        
-        *A [MkDocs](https://www.mkdocs.org/) plugin that validates URLs, including anchors, in rendered html files*.
-        
-        ## Installation
-        
-        0. Prerequisites
-        
-        * Python >= 3.6
-        * MkDocs >= 0.17
-        
-        1. Install the package with pip:
-        
-        ```bash
-        pip install mkdocs-htmlproofer-plugin
-        ```
-        
-        2. Enable the plugin in your `mkdocs.yml`:
-        
-        ```yaml
-        plugins:
-            - search
-            - htmlproofer
-        ```
-        
-        > **Note:** If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin.
-        MkDocs enables it by default if there is no `plugins` entry set, but now you have to enable it explicitly.
-        
-        ```yaml
-        plugins:
-            - search
-            - htmlproofer
-        ```
-        
-        To enable cross-page anchor validation, you must set `use_directory_urls = False` in `mkdocs.yml`:
-        
-        ```yaml
-        use_directory_urls: False
-        ```
-        
-        ## Configuring
-        
-        ### `enabled`
-        
-        True by default, allows toggling whether the plugin is enabled.
-        Useful for local development where you may want faster build times.
-        
-        ```yaml
-        plugins:
-          - htmlproofer:
-              enabled: !ENV [ENABLED_HTMLPROOFER, True]
-        ```
-        
-        Which enables you do disable the plugin locally using:
-        
-        ```bash
-        export ENABLED_HTMLPROOFER=false
-        mkdocs serve
-        ```
-        
-        
-        ### `raise_error`
-        
-        Optionally, you may raise an error and fail the build on bad url status.
-        
-        ```yaml
-        plugins:
-          - htmlproofer:
-              raise_error: True
-        ```
-        
-        ### `raise_error_excludes`
-        
-        When specifying `raise_error: True`, it is possible to ignore errors
-        for combinations of urls (`'*'` means all urls) and status codes with `raise_error_excludes`.
-        
-        ```yaml
-        plugins:
-          - search
-          - htmlproofer:
-              raise_error: True
-              raise_error_excludes:
-                504: ['https://www.mkdocs.org/']
-                404: ['https://github.com/manuzhang/mkdocs-htmlproofer-plugin']
-                400: ['*']
-        ```
-        
-        ### `validate_external_urls`
-        
-        Avoids validating any external URLs (i.e those starting with http:// or https://).
-        This will be faster if you just want to validate local anchors, as it does not make any network requests.
-        
-        ```
-        plugins:
-          - htmlproofer:
-              validate_external_urls: False
-        ```
-        
-        ### `validate_rendered_template`
-        
-        Validates the entire rendered template for each page - including the navigation, header, footer, etc.
-        This defaults to off because it is much slower and often redundant to repeat for every single page.
-        
-        ```
-        plugins:
-          - htmlproofer:
-              validate_rendered_template: True
-        ```
-        
-        ## Improving
-        
-        More information about plugins in the [MkDocs documentation](http://www.mkdocs.org/user-guide/plugins/)
-        
-        ## Acknowledgement
-        
-        This work is based on the [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) project and the [Finding and Fixing Website Link Rot with Python, BeautifulSoup and Requests](https://www.twilio.com/blog/2018/07/find-fix-website-link-rot-python-beautifulsoup-requests.html) article. 
-        
 Keywords: mkdocs python markdown
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# mkdocs-htmlproofer-plugin [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-htmlproofer-plugin.svg)](https://pypi.org/project/mkdocs-htmlproofer-plugin)
+
+[![GitHub Actions](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml/badge.svg)](https://github.com/manuzhang/mkdocs-htmlproofer-plugin/actions/workflows/ci.yml)
+
+*A [MkDocs](https://www.mkdocs.org/) plugin that validates URLs, including anchors, in rendered html files*.
+
+## Installation
+
+0. Prerequisites
+
+* Python >= 3.8
+* MkDocs >= 1.4.0
+
+1. Install the package with pip:
+
+```bash
+pip install mkdocs-htmlproofer-plugin
+```
+
+2. Enable the plugin in your `mkdocs.yml`:
+
+> **Note:** If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin.
+MkDocs enables it by default if there is no `plugins` entry set, but now you have to enable it explicitly.
+
+```yaml
+plugins:
+    - search
+    - htmlproofer
+```
+
+To enable cross-page anchor validation, you must set `use_directory_urls = False` in `mkdocs.yml`:
+
+```yaml
+use_directory_urls: False
+```
+
+## Configuring
+
+### `enabled`
+
+True by default, allows toggling whether the plugin is enabled.
+Useful for local development where you may want faster build times.
+
+```yaml
+plugins:
+  - htmlproofer:
+      enabled: !ENV [ENABLED_HTMLPROOFER, True]
+```
+
+Which enables you do disable the plugin locally using:
+
+```bash
+export ENABLED_HTMLPROOFER=false
+mkdocs serve
+```
+
+
+### `raise_error`
+
+Optionally, you may raise an error and fail the build on first bad url status. Takes precedense over `raise_error_after_finish`.
+
+```yaml
+plugins:
+  - htmlproofer:
+      raise_error: True
+```
+
+### `raise_error_after_finish`
+
+Optionally, you may want to raise an error and fail the build on at least one bad url status after all links have been checked.
+
+```yaml
+plugins:
+  - htmlproofer:
+      raise_error_after_finish: True
+```
+
+### `raise_error_excludes`
+
+When specifying `raise_error: True` or `raise_error_after_finish: True`, it is possible to ignore errors
+for combinations of urls (`'*'` means all urls) and status codes with `raise_error_excludes`.
+
+```yaml
+plugins:
+  - search
+  - htmlproofer:
+      raise_error: True
+      raise_error_excludes:
+        504: ['https://www.mkdocs.org/']
+        404: ['https://github.com/manuzhang/mkdocs-htmlproofer-plugin']
+        400: ['*']
+```
+
+### `validate_external_urls`
+
+Avoids validating any external URLs (i.e those starting with http:// or https://).
+This will be faster if you just want to validate local anchors, as it does not make any network requests.
+
+```yaml
+plugins:
+  - htmlproofer:
+      validate_external_urls: False
+```
+
+### `validate_rendered_template`
+
+Validates the entire rendered template for each page - including the navigation, header, footer, etc.
+This defaults to off because it is much slower and often redundant to repeat for every single page.
+
+```yaml
+plugins:
+  - htmlproofer:
+      validate_rendered_template: True
+```
+
+## Compatibility with `attr_list` extension
+
+If you need to manually specify anchors make use of the `attr_list` [extension](https://python-markdown.github.io/extensions/attr_list) in the markdown. 
+This can be useful for multilingual documentation to keep anchors as language neutral permalinks in all languages.
+
+* A sample for a heading `# Grüße {#greetings}` (the slugified generated anchor `Gre` is overwritten with `greetings`).
+* This also works for images `this is a nice image [](foo-bar.png){#nice-image}` 
+* And generall for paragraphs:
+```markdown
+Listing: This is noteworthy.
+{#paragraphanchor}
+```
+
+## Improving
+
+More information about plugins in the [MkDocs documentation](http://www.mkdocs.org/user-guide/plugins/)
+
+## Acknowledgement
+
+This work is based on the [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) project and the [Finding and Fixing Website Link Rot with Python, BeautifulSoup and Requests](https://www.twilio.com/blog/2018/07/find-fix-website-link-rot-python-beautifulsoup-requests.html) article.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs-htmlproofer-plugin-0.9.0/setup.py` & `mkdocs-htmlproofer-plugin-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,42 +5,41 @@
 
 def read(fname: str):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='mkdocs-htmlproofer-plugin',
-    version='0.9.0',
+    version='1.0.0',
     description='A MkDocs plugin that validates URL in rendered HTML files',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown',
     url='https://github.com/manuzhang/mkdocs-htmlproofer-plugin',
     author='Manu Zhang',
     author_email='owenzhang1990@gmail.com',
     license='MIT',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=[
-        'mkdocs>=0.17',
+        'mkdocs>=1.4.0',
         'Markdown',
         'requests',
         'beautifulsoup4',
-        'lxml',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     packages=find_packages(exclude=['*.tests']),
     entry_points={
         'mkdocs.plugins': [
             'htmlproofer = htmlproofer.plugin:HtmlProoferPlugin'
         ]
     }
```

