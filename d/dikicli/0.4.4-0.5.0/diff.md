# Comparing `tmp/dikicli-0.4.4.tar.gz` & `tmp/dikicli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dikicli-0.4.4.tar", last modified: Wed May  4 10:09:11 2022, max compression
+gzip compressed data, was "dikicli-0.5.0.tar", max compression
```

## Comparing `dikicli-0.4.4.tar` & `dikicli-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,10 @@
-drwxr-xr-x   0 dawid     (1000) dawid     (1000)        0 2022-05-04 10:09:11.369742 dikicli-0.4.4/
--rw-rw-r--   0 dawid     (1000) dawid     (1000)       36 2018-12-14 14:05:45.000000 dikicli-0.4.4/.isort.cfg
--rw-rw-r--   0 dawid     (1000) dawid     (1000)       25 2018-12-03 18:22:37.000000 dikicli-0.4.4/.lvimrc
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     1067 2018-05-21 10:37:44.000000 dikicli-0.4.4/LICENSE
--rw-r--r--   0 dawid     (1000) dawid     (1000)      275 2022-05-04 09:19:00.000000 dikicli-0.4.4/Makefile
--rw-r--r--   0 dawid     (1000) dawid     (1000)     1639 2022-05-04 10:09:11.369742 dikicli-0.4.4/PKG-INFO
--rw-r--r--   0 dawid     (1000) dawid     (1000)      277 2021-02-03 19:28:15.000000 dikicli-0.4.4/Pipfile
--rw-r--r--   0 dawid     (1000) dawid     (1000)    49325 2022-05-04 09:13:16.000000 dikicli-0.4.4/Pipfile.lock
--rw-rw-r--   0 dawid     (1000) dawid     (1000)      363 2018-04-01 09:06:03.000000 dikicli-0.4.4/README.md
--rw-r--r--   0 dawid     (1000) dawid     (1000)       53 2020-02-21 13:41:59.000000 dikicli-0.4.4/TODO.txt
-drwxr-xr-x   0 dawid     (1000) dawid     (1000)        0 2022-05-04 10:09:11.363742 dikicli-0.4.4/dikicli/
--rw-rw-r--   0 dawid     (1000) dawid     (1000)        0 2017-12-05 19:47:04.000000 dikicli-0.4.4/dikicli/__init__.py
--rw-r--r--   0 dawid     (1000) dawid     (1000)       37 2020-02-18 11:24:58.000000 dikicli-0.4.4/dikicli/__main__.py
--rw-r--r--   0 dawid     (1000) dawid     (1000)     4065 2021-09-21 10:40:02.000000 dikicli-0.4.4/dikicli/cli.py
--rw-r--r--   0 dawid     (1000) dawid     (1000)    18908 2021-09-21 10:40:00.000000 dikicli-0.4.4/dikicli/core.py
--rw-rw-r--   0 dawid     (1000) dawid     (1000)      838 2018-12-03 21:05:56.000000 dikicli-0.4.4/dikicli/templates.py
-drwxr-xr-x   0 dawid     (1000) dawid     (1000)        0 2022-05-04 10:09:11.365742 dikicli-0.4.4/dikicli.egg-info/
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     1639 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/PKG-INFO
--rw-rw-r--   0 dawid     (1000) dawid     (1000)      706 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/SOURCES.txt
--rw-rw-r--   0 dawid     (1000) dawid     (1000)        1 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/dependency_links.txt
--rw-rw-r--   0 dawid     (1000) dawid     (1000)       94 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/entry_points.txt
--rw-r--r--   0 dawid     (1000) dawid     (1000)        1 2020-02-21 12:26:00.000000 dikicli-0.4.4/dikicli.egg-info/not-zip-safe
--rw-r--r--   0 dawid     (1000) dawid     (1000)       47 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/pbr.json
--rw-r--r--   0 dawid     (1000) dawid     (1000)       31 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/requires.txt
--rw-rw-r--   0 dawid     (1000) dawid     (1000)        8 2022-05-04 10:09:11.000000 dikicli-0.4.4/dikicli.egg-info/top_level.txt
--rw-r--r--   0 dawid     (1000) dawid     (1000)      100 2022-05-04 09:11:42.000000 dikicli-0.4.4/pyproject.toml
--rw-r--r--   0 dawid     (1000) dawid     (1000)     2476 2022-05-04 09:18:00.000000 dikicli-0.4.4/requirements-dev.txt
--rw-r--r--   0 dawid     (1000) dawid     (1000)       31 2022-05-04 09:17:29.000000 dikicli-0.4.4/requirements.txt
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     1210 2022-05-04 10:09:11.370742 dikicli-0.4.4/setup.cfg
--rw-rw-r--   0 dawid     (1000) dawid     (1000)      117 2020-02-21 12:25:35.000000 dikicli-0.4.4/setup.py
-drwxr-xr-x   0 dawid     (1000) dawid     (1000)        0 2022-05-04 10:09:11.366742 dikicli-0.4.4/tests/
--rw-rw-r--   0 dawid     (1000) dawid     (1000)        0 2018-12-06 15:36:18.000000 dikicli-0.4.4/tests/__init__.py
--rw-rw-r--   0 dawid     (1000) dawid     (1000)      768 2017-12-06 23:47:12.000000 dikicli-0.4.4/tests/context.py
-drwxr-xr-x   0 dawid     (1000) dawid     (1000)        0 2022-05-04 10:09:11.369742 dikicli-0.4.4/tests/html_cache/
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     1410 2017-12-05 10:41:55.000000 dikicli-0.4.4/tests/html_cache/cork.html
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     6297 2017-12-05 11:02:27.000000 dikicli-0.4.4/tests/html_cache/dog.html
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     1107 2017-12-05 15:59:00.000000 dikicli-0.4.4/tests/html_cache/elusive.html
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     3168 2017-12-05 12:41:59.000000 dikicli-0.4.4/tests/html_cache/guest.html
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     1267 2017-12-05 12:10:53.000000 dikicli-0.4.4/tests/html_cache/snitch.html
--rw-rw-r--   0 dawid     (1000) dawid     (1000)     4680 2017-12-05 12:10:48.000000 dikicli-0.4.4/tests/html_cache/switch.html
--rw-r--r--   0 dawid     (1000) dawid     (1000)    11715 2020-02-18 12:45:44.000000 dikicli-0.4.4/tests/test_core.py
+-rw-r--r--   0        0        0     1067 2018-05-21 10:37:44.713780 dikicli-0.5.0/LICENSE
+-rw-r--r--   0        0        0      405 2022-09-21 21:19:04.521934 dikicli-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2017-12-05 19:47:04.220751 dikicli-0.5.0/dikicli/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-18 11:24:58.892450 dikicli-0.5.0/dikicli/__main__.py
+-rw-r--r--   0        0        0     4500 2022-09-21 20:56:58.012666 dikicli-0.5.0/dikicli/cli.py
+-rw-r--r--   0        0        0    17981 2023-04-11 10:14:01.972309 dikicli-0.5.0/dikicli/core.py
+-rw-r--r--   0        0        0      838 2018-12-03 21:05:56.436116 dikicli-0.5.0/dikicli/templates.py
+-rw-r--r--   0        0        0      963 2022-09-21 21:13:37.227658 dikicli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1218 1970-01-01 00:00:00.000000 dikicli-0.5.0/setup.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dikicli-0.5.0/PKG-INFO
```

### Comparing `dikicli-0.4.4/LICENSE` & `dikicli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dikicli-0.4.4/PKG-INFO` & `dikicli-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 Metadata-Version: 2.1
 Name: dikicli
-Version: 0.4.4
-Summary: Commandline interface to diki.pl polish-english dictionary
+Version: 0.5.0
+Summary: Commandline interface for diki.pl polish-english dictionary
 Home-page: https://github.com/silenc3r/dikicli
-Author: Dawid Zych
-Author-email: dawid.zych@yandex.com
 License: MIT
-Description: # dikicli
-        
-        Commandline interface to diki.pl polish-english dictionary.
-        
-        Dikicli allows you to use diki.pl from comfort of your terminal.
-        All results are cached for faster retrieval in the future.
-        
-        ## Usage:
-        
-        Translate english to polish:
-        
-            diki word
-        
-        Translate polish to engish:
-        
-            diki -p word
-        
-        Display html file of all words translated so far:
-        
-            diki -i
-        
-        
-Platform: UNKNOWN
+Keywords: diki,dictionary
+Author: Dawid Zych
+Author-email: dwd@mailo.com
+Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Polish
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: beautifulsoup4 (>=4.0)
+Requires-Dist: requests (>=2.25.1)
+Project-URL: Repository, https://github.com/silenc3r/dikicli
+Description-Content-Type: text/markdown
+
+# dikicli
+
+Commandline interface to diki.pl polish-english dictionary.
+
+Dikicli allows you to use diki.pl from comfort of your terminal.
+All results are cached for faster retrieval in the future.
+
+## Usage:
+
+Translate english to polish:
+
+    diki word
+
+Translate polish to engish:
+
+    diki -p word
+
+Display html file of all words translated so far:
+
+    diki -i
+
+Show usage statistics:
+
+    diki --stats
+
```

### Comparing `dikicli-0.4.4/dikicli/cli.py` & `dikicli-0.5.0/dikicli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 
 import argparse
 import logging
 import logging.config
+import pathlib
 import sys
 
 import requests
 
 from .core import CACHE_DIR
 from .core import DEBUG
 from .core import Config
 from .core import WordNotFound
 from .core import display_index
+from .core import get_stats
 from .core import translate
 from .core import wrap_text
 
 LOG_FILE = CACHE_DIR.joinpath("diki.log")
 if not CACHE_DIR.exists():
     CACHE_DIR.mkdir(parents=True)
 
@@ -70,14 +72,15 @@
         action="version",
         version="dikicli {version}".format(version=get_version()),
     )
     parser.add_argument(
         "--create-config", action="store_true", help="create default configuration file"
     )
     parser.add_argument("-r", "--refresh", action="store_true", help="ignore cache")
+    parser.add_argument("-s", "--stats", action="store_true", help="show statistics")
     translation = parser.add_argument_group("translation")
     translation.add_argument("word", nargs="?", help="word to translate")
     translation.add_argument(
         "-p", "--pol-eng", action="store_true", help="translate polish word to english"
     )
     translation.add_argument(
         "-w",
@@ -130,20 +133,28 @@
         except (WordNotFound, requests.exceptions.ConnectionError) as e:
             logger.error(e)
             sys.exit(1)
 
     # open index file in browser
     if args.display_index:
         try:
-            display_index(config)
+            browser = config["web browser"]
+            data_dir = pathlib.Path(config["data dir"])
+            display_index(data_dir, browser)
             sys.exit(0)
         except FileNotFoundError as e:
             logger.error(e)
             sys.exit(1)
 
+    if args.stats:
+        en, pl = get_stats(pathlib.Path(config["data dir"]))
+        print("english words:  {}".format(en))
+        print(" polish words:  {}".format(pl))
+        sys.exit(0)
+
 
 def main():
     try:
         _main()
     except KeyboardInterrupt:
         logger.warning("aborting...")
         sys.exit(1)
```

### Comparing `dikicli-0.4.4/dikicli/core.py` & `dikicli-0.5.0/dikicli/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,56 +261,17 @@
             translation = _parse_cached(f.read())
             return translation
     logger.debug("Cache miss: %s", word)
     return None
 
 
 def _get_words(data_dir):
-    """Get list of words from history file.
-
-    Parameters
-    ----------
-    data_dir : pathlib.Path
-        Directory where data is saved.
-
-    Returns
-    -------
-    word_list : list of str
-        List of words.
-    """
-    words_file = data_dir.joinpath("words.txt")
-    word_list = []
-    if not words_file.is_file():
-        return word_list
-    with open(words_file, mode="r") as f:
-        for l in f:
-            line = l.rstrip()
-            word_list.append(line)
-    return word_list
-
-
-def _save_to_history(word, data_dir):
-    """Write word to history file.
-
-    Parameters
-    ----------
-    word : str
-        Word to save to history.
-    data_dir : pathlib.Path
-        Directory where history file should be saved.
-
-    data_dir and it's parent directories will be created if needed.
-    """
-    if not data_dir.exists():
-        logger.debug("Creating DATA DIR: %s", data_dir.as_posix())
-        data_dir.mkdir(parents=True)
-    if word not in _get_words(data_dir):
-        with open(data_dir.joinpath("words.txt"), mode="a+") as f:
-            logger.debug("Adding to history: %s", word)
-            f.write(word + "\n")
+    """Return list of translated words."""
+    trans_dir = data_dir / "translations"
+    return [file.stem for file in trans_dir.iterdir()]
 
 
 def _create_html_file_content(translations):
     """Create html string out of translation dict.
 
     Parameters
     ----------
@@ -409,26 +370,17 @@
     if not words:
         content.append("<i>Nothing to see here ...yet!</i>")
 
     return "\n".join(content)
 
 
 def _write_index_file(data_dir):
-    """Create index file of cached translations.
+    """Create index file of cached translations."""
 
-    Parameters
-    ----------
-    data_dir : pathlib.Path
-        Cache directory location.
-    """
-    cached_words = [
-        w
-        for w in _get_words(data_dir)
-        if data_dir.joinpath("translations/{}.html".format(w)).is_file()
-    ]
+    cached_words = _get_words(data_dir)
 
     content_str = _create_index_content(cached_words)
     html_string = HTML_TEMPLATE.replace("{% word %}", "Index")
     html_string = html_string.replace("{% content %}", content_str)
 
     filename = data_dir.joinpath("index.html")
     save_file(filename, html_string, mk_parents=True)
@@ -516,53 +468,55 @@
         return translation
 
     html_dump = _lookup_online(word)
     translation = _parse_html(html_dump, native=to_eng)
     _write_html_file(word, translation, data_dir, native=to_eng)
 
     if not to_eng:
-        _save_to_history(word, data_dir)
         _write_index_file(data_dir)
 
     return translation
 
 
-def display_index(config):
+def display_index(data_dir: Path, browser: str):
     """Open index in web browser.
-
-    Parameters
-    ----------
-    config : Config
-        Configuration settings.
-
-    Raises
-    ------
-    FileNotFoundError
-        If index file doesn't exist.
+    Raises FileNotFoundError if index file doesn't exist.
     """
-    browser = config["web browser"].lower()
-    data_dir = Path(config["data dir"])
-    if browser in webbrowser._browsers:
-        b = webbrowser.get(browser)
-    else:
-        if browser != "default":
-            logger.warning(
-                "Couldn't find '%s' browser. Falling back to default.", browser
-            )
-        b = webbrowser.get()
+    get_browser = lambda b: webbrowser.get() if b == "default" else webbrowser.get(b)
+    try:
+        b = get_browser(browser)
+    except webbrowser.Error:
+        logger.warning("Couldn't find '%s' browser. Falling back to default.", browser)
+        b = get_browser("default")
 
+    _write_index_file(data_dir)
     index_file = data_dir.joinpath("index.html")
     if not index_file.exists():
         raise FileNotFoundError(
             "Index file doesn't exist: {index}".format(index=index_file.as_posix())
         )
     logger.info("Opening %s in '%s'", index_file.as_posix(), b.name)
     b.open(index_file.as_uri())
 
 
+def get_stats(data_dir: Path):
+    """Get usage statistics.
+    Returns (num_of_en_words, num_of_pl_words) tuple.
+    """
+    en_dir = data_dir.joinpath("translations")
+    pl_dir = data_dir.joinpath("translations_native")
+
+    def count_words(dir):
+        return len(list(dir.glob("*.html"))) if dir.is_dir() else 0
+
+    num_of_en_words = count_words(en_dir)
+    num_of_pl_words = count_words(pl_dir)
+    return num_of_en_words, num_of_pl_words
+
+
 def wrap_text(translations, linewrap=0):
     """Pretty print translations.
 
     If linewrap is set to 0 disble line wrapping.
 
     Parameters
     ----------
```

### Comparing `dikicli-0.4.4/dikicli/templates.py` & `dikicli-0.5.0/dikicli/templates.py`

 * *Files identical despite different names*

