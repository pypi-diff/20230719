# Comparing `tmp/mathbib-0.7.4.tar.gz` & `tmp/mathbib-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.7.4.tar", max compression
+gzip compressed data, was "mathbib-0.7.5.tar", max compression
```

## Comparing `mathbib-0.7.4.tar` & `mathbib-0.7.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.4/LICENSE
--rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.4/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.4/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.4/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.4/mathbib/bibtex.py
--rw-r--r--   0        0        0     3326 2023-07-13 10:48:13.319332 mathbib-0.7.4/mathbib/citegen.py
--rw-r--r--   0        0        0    10831 2023-07-13 10:33:28.789417 mathbib-0.7.4/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.4/mathbib/partition.py
--rw-r--r--   0        0        0     9500 2023-07-13 10:44:15.098639 mathbib-0.7.4/mathbib/record.py
--rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.4/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.4/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.4/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.4/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.4/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.4/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.4/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.4/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.4/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.4/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.4/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.4/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.4/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.4/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-07-13 10:48:54.865737 mathbib-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.5/LICENSE
+-rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.5/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.5/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.5/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.5/mathbib/bibtex.py
+-rw-r--r--   0        0        0     3326 2023-07-13 10:48:13.319332 mathbib-0.7.5/mathbib/citegen.py
+-rw-r--r--   0        0        0    11233 2023-07-19 13:51:55.915003 mathbib-0.7.5/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.5/mathbib/partition.py
+-rw-r--r--   0        0        0     9500 2023-07-13 10:44:15.098639 mathbib-0.7.5/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.5/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.5/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.5/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.5/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.5/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.5/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.5/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.5/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.5/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.5/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.5/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.5/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.5/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.5/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-07-19 13:52:25.170657 mathbib-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.5/PKG-INFO
```

### Comparing `mathbib-0.7.4/LICENSE` & `mathbib-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/README.md` & `mathbib-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/bibtex.py` & `mathbib-0.7.5/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/citegen.py` & `mathbib-0.7.5/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/command.py` & `mathbib-0.7.5/mathbib/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -297,38 +297,51 @@
 @click.pass_obj
 def get_alias(session: CLISession, alias_name: str):
     """Get record associated with alias."""
     click.echo(session.get_alias(alias_name))
 
 
 @alias.command(name="list", short_help="List all defined aliases.")
+@click.option(
+    "--keys-only",
+    "keys_only",
+    is_flag=True,
+    default=False,
+    help="Only print ALIASes.",
+)
 @click.argument(
     "key_sources",
     nargs=-1,
     type=click.Path(exists=True, file_okay=True, dir_okay=False, path_type=Path),
     metavar="KEYSOURCE",
 )
 @click.pass_obj
-def list_alias(session: CLISession, key_sources: Sequence[Path]):
+def list_alias(session: CLISession, keys_only: bool, key_sources: Sequence[Path]):
     """Print all defined aliases to the terminal. The aliases are printed
     as valid TOML as a list of ALIAS = KEY:ID entries.
 
     If any file paths are specified, only generate the alias entries corresponding
-    to citation keys in the corresponding files.
+    to citation keys in the corresponding files. This is useful for generating new
+    files to use with the top-level --alias option.
+
+    With the --keys-only, only print the ALIAS for each entry, separated by a newline.
     """
     if len(key_sources) > 0:
         alias_dict = {
             k: v
             for k, v in session.alias.items()
             if k in get_citekeys_from_paths(*key_sources)
         }
     else:
         alias_dict = session.alias
 
-    click.echo(dumps(alias_dict), nl=False)
+    if keys_only:
+        click.echo("\n".join(sorted(alias_dict.keys())))
+    else:
+        click.echo(dumps(alias_dict), nl=False)
 
 
 @cli.command(name="list", short_help="List all records.")
 @click.option(
     "--sep",
     "sep",
     type=str,
```

### Comparing `mathbib-0.7.4/mathbib/partition.py` & `mathbib-0.7.5/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/record.py` & `mathbib-0.7.5/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/__init__.py` & `mathbib-0.7.5/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/arxiv.py` & `mathbib-0.7.5/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/doi.py` & `mathbib-0.7.5/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/error.py` & `mathbib-0.7.5/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/isbn.py` & `mathbib-0.7.5/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/ol.py` & `mathbib-0.7.5/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/utils.py` & `mathbib-0.7.5/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/zbl.py` & `mathbib-0.7.5/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/remote/zbmath.py` & `mathbib-0.7.5/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/request.py` & `mathbib-0.7.5/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/resources/journal_abbrevs.json` & `mathbib-0.7.5/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/session.py` & `mathbib-0.7.5/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/mathbib/term.py` & `mathbib-0.7.5/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.4/pyproject.toml` & `mathbib-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.7.4"
+version = "0.7.5"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.7.4/PKG-INFO` & `mathbib-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.7.4
+Version: 0.7.5
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

