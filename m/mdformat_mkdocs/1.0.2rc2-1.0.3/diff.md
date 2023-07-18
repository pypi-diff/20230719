# Comparing `tmp/mdformat_mkdocs-1.0.2rc2.tar.gz` & `tmp/mdformat_mkdocs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-1.0.2rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-1.0.2rc2.tar` & `mdformat_mkdocs-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1819 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.gitignore
--rw-r--r--   0        0        0     1756 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      573 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.pre-commit-test.yaml
--rw-r--r--   0        0        0       33 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.tool-versions
--rw-r--r--   0        0        0      979 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/LICENSE
--rw-r--r--   0        0        0     3095 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/README.md
--rw-r--r--   0        0        0      175 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0     3613 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0      402 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/README.md
--rw-r--r--   0        0        0      672 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/docs/README.md
--rw-r--r--   0        0        0    78687 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdcs-demo-screenshot.png
--rw-r--r--   0        0        0       42 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdocs.yml
--rw-r--r--   0        0        0        0 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdocs_demo/__init__.py
--rw-r--r--   0        0        0    24503 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/poetry.lock
--rw-r--r--   0        0        0      372 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/pyproject.toml
--rw-r--r--   0        0        0     1639 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/pyproject.toml
--rw-r--r--   0        0        0      789 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/tox.ini
--rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.2rc2/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1756 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      571 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.pre-commit-test.yaml
+-rw-r--r--   0        0        0       33 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/.tool-versions
+-rw-r--r--   0        0        0      979 2023-07-18 22:29:37.293548 mdformat_mkdocs-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3265 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/README.md
+-rw-r--r--   0        0        0      172 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0     3728 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0      402 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/README.md
+-rw-r--r--   0        0        0     1063 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/docs/README.md
+-rw-r--r--   0        0        0    78687 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/mkdcs-demo-screenshot.png
+-rw-r--r--   0        0        0       42 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/mkdocs.yml
+-rw-r--r--   0        0        0        0 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/mkdocs_demo/__init__.py
+-rw-r--r--   0        0        0    24503 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/poetry.lock
+-rw-r--r--   0        0        0      372 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/mkdocs-demo/pyproject.toml
+-rw-r--r--   0        0        0     1630 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      789 2023-07-18 22:29:37.297548 mdformat_mkdocs-1.0.3/tox.ini
+-rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.3/PKG-INFO
```

### Comparing `mdformat_mkdocs-1.0.2rc2/.gitignore` & `mdformat_mkdocs-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/.pre-commit-config.yaml` & `mdformat_mkdocs-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/CONTRIBUTING.md` & `mdformat_mkdocs-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/LICENSE` & `mdformat_mkdocs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/README.md` & `mdformat_mkdocs-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 [cov-link]: https://codecov.io/gh/executablebooks/mdformat-mkdocs
  -->
 
 An [mdformat](https://github.com/executablebooks/mdformat) plugin for [mkdocs](https://github.com/mkdocs/mkdocs).
 
 ## Usage
 
-Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. See [additional information on `mdformat` plugins here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
+Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. For additional information on plugins, see [the official `mdformat` documentation here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
 
-Tip: this package specifies an "extra" (`recommended`) for plugins that work well with mkdocs:
+Tip: this package specifies an "extra" (`'recommended'`) for plugins that work well with mkdocs:
 
 - [mdformat-admon](https://pypi.org/project/mdformat-admon)
 - [mdformat-beautysh](https://pypi.org/project/mdformat-beautysh)
 - [mdformat-black](https://pypi.org/project/mdformat-black)
 - [mdformat-config](https://pypi.org/project/mdformat-config)
 - [mdformat-footnote](https://pypi.org/project/mdformat-footnote)
 - [mdformat-frontmatter](https://pypi.org/project/mdformat-frontmatter)
@@ -45,35 +45,37 @@
 ```sh
 pipx install mdformat
 pipx inject mdformat mdformat-mkdocs
 # Or
 # pipx inject mdformat "mdformat-mkdocs[recommended]"
 ```
 
-## Caveats
-
-- All indents are converted to 4-spaces
-- This plugin converts all bulleted items to dashes (`-`) and numerals to `1.`
+## CLI Options
 
-See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
-
-## Configuration
-
-`mdformat-mkdocs` adds the CLI argument `--align-semantic-breaks-in-numbered-lists` to optionally align line breaks in numbered lists to 3-spaces. If not specified, the default of 4-indents is followed universally.
+`mdformat-mkdocs` adds the CLI argument `--align-semantic-breaks-in-lists` to optionally align line breaks in numbered lists to 3-spaces. If not specified, the default of 4-indents is followed universally.
 
 ```txt
 # with: mdformat
 1. Semantic line feed where the following line is
     three spaces deep
 
-# vs. with: mdformat --align-semantic-breaks-in-numbered-lists
+# vs. with: mdformat --align-semantic-breaks-in-lists
 1. Semantic line feed where the following line is
    three spaces deep
 ```
 
+Note: the `align-semantic-breaks-in-lists` setting is not supported in the configuration file yet (https://github.com/executablebooks/mdformat/issues/378)
+
+## Caveats
+
+- All indents are converted to 4-spaces
+- This plugin converts all bulleted items to dashes (`-`) and numerals to `1.`
+
+See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
+
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-mkdocs/blob/main/CONTRIBUTING.md)
 
 [ci-badge]: https://github.com/kyleking/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
 [ci-link]: https://github.com/kyleking/mdformat-mkdocs/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
 [pypi-badge]: https://img.shields.io/pypi/v/mdformat-mkdocs.svg
```

### Comparing `mdformat_mkdocs-1.0.2rc2/mdformat_mkdocs/plugin.py` & `mdformat_mkdocs-1.0.3/mdformat_mkdocs/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 from markdown_it import MarkdownIt
 from mdformat.renderer import RenderContext, RenderTreeNode
 from mdformat.renderer.typing import Postprocess, Render
 
 _MKDOCS_INDENT_COUNT = 4
 """Use 4-spaces for mkdocs."""
 
-_ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS = False
-"""use 3-space on subsequent lines in semantic lists."""
+_ALIGN_SEMANTIC_BREAKS_IN_LISTS = False
+"""user-specified flag for toggling semantic breaks.
+
+- 3-spaces on subsequent lines in semantic numbered lists
+- and 2-spaces on subsequent bulleted items
+
+"""
 
 
 def add_cli_options(parser: argparse.ArgumentParser) -> None:
     """Add options to the mdformat CLI, to be stored in `mdit.options["mdformat"]`."""
     parser.add_argument(
-        "--align-semantic-breaks-in-numbered-lists",
+        "--align-semantic-breaks-in-lists",
         action="store_true",
-        help="If specified, align semantic indents in numbered lists to the text",
+        help="If specified, align semantic indents in numbered and bulleted lists to the text",
     )
 
 
 def update_mdit(mdit: MarkdownIt) -> None:
     """No changes to markdown parsing are necessary."""
-    global _ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS
-    _ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS = mdit.options["mdformat"].get(
-        "align_semantic_breaks_in_numbered_lists", False
+    global _ALIGN_SEMANTIC_BREAKS_IN_LISTS
+    _ALIGN_SEMANTIC_BREAKS_IN_LISTS = mdit.options["mdformat"].get(
+        "align_semantic_breaks_in_lists", False
     )
 
 
 _RE_INDENT = re.compile(r"(?P<indent>\s*)(?P<content>[^\s]?.*)")
 """Match `indent` and `content` against line`."""
 
 _RE_LIST_ITEM = re.compile(r"(?P<bullet>[\-\*\d\.]+)\s+(?P<item>.+)")
@@ -56,29 +61,30 @@
             is_numbered = list_match["bullet"] not in {"-", "*"}
             new_bullet = "1." if is_numbered else "-"
             new_line = f'{new_bullet} {list_match["item"]}'
 
         this_indent = match["indent"]
         if this_indent:
             indent_diff = len(this_indent) - len(last_indent)
-            if indent_diff == 0:
+            if not indent_diff:
                 ...
             elif indent_diff > 0:
                 indent_counter += 1
                 indent_lookup[this_indent] = indent_counter
             elif this_indent in indent_lookup:
                 indent_counter = indent_lookup[this_indent]
             else:
                 raise NotImplementedError(f"Error in indentation of: `{line}`")
         else:
             indent_counter = 0
         last_indent = this_indent
         new_indent = indent * indent_counter
-        if _ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS and not list_match and is_numbered:
-            new_indent = new_indent[:-1]
+        if _ALIGN_SEMANTIC_BREAKS_IN_LISTS and not list_match:
+            removed_indents = -1 if is_numbered else -2
+            new_indent = new_indent[:removed_indents]
         rendered += f"{new_indent}{new_line.strip()}{eol}"
     return rendered.rstrip()
 
 
 # A mapping from `RenderTreeNode.type` to a `Render` function that can
 # render the given `RenderTreeNode` type. These override the default
 # `Render` funcs defined in `mdformat.renderer.DEFAULT_RENDERERS`.
```

### Comparing `mdformat_mkdocs-1.0.2rc2/mkdocs-demo/docs/README.md` & `mdformat_mkdocs-1.0.3/mkdocs-demo/docs/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,43 @@
 1. Here indent width is
    three.
 
     1. Here indent width is
        three.
 
 1. Here indent width is
-   five (three). It needs to be so, because
+   five (three). The following indent needs to be four (but it is 3 with semantic change).
 
    Otherwise this next paragraph doesn't belong in the same list item.
 
 ---
 
 ### With current behavior
 
 1. Here indent width is
     three (four).
 
     1. Here indent width is
         three (four).
 
 1. Here indent width is
-    five (four). It needs to be so, because
+    five (four). The following indent needs to be four.
 
     Otherwise this next paragraph doesn't belong in the same list item.
+
+---
+
+### With proposed change for bullets
+
+1. Line
+   semantic line 1 (3 spaces deep)
+    - Bullet (4 spaces deep)
+      semantic line 2 (6 spaces deep)
+
+---
+
+### With proposed change for bullets nested in a numbered list
+
+- Line
+  semantic line 1 (2 spaces deep)
+    - Bullet (4 spaces deep)
+      semantic line 2 (6 spaces deep)
```

### Comparing `mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdcs-demo-screenshot.png` & `mdformat_mkdocs-1.0.3/mkdocs-demo/mkdcs-demo-screenshot.png`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/mkdocs-demo/poetry.lock` & `mdformat_mkdocs-1.0.3/mkdocs-demo/poetry.lock`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/pyproject.toml` & `mdformat_mkdocs-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["mdformat", "markdown", "markdown-it"]
 requires-python = ">=3.7.2"
 dependencies = [
     "mdformat >= 0.7.16",
     "mdformat-gfm >= 0.3.5",
-    "mdit-py-plugins[linkify] >= 0.3.3",
+    "mdit-py-plugins >= 0.3.3",
 ]
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 recommended = [
     # Keep in-sync with README
     "mdformat-admon",
```

### Comparing `mdformat_mkdocs-1.0.2rc2/tox.ini` & `mdformat_mkdocs-1.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.2rc2/PKG-INFO` & `mdformat_mkdocs-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 1.0.2rc2
+Version: 1.0.3
 Summary: An mdformat plugin for mkdocs.
 Keywords: mdformat,markdown,markdown-it
 Author-email: Kyle King <dev.act.kyle@gmail.com>
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: mdformat >= 0.7.16
 Requires-Dist: mdformat-gfm >= 0.3.5
-Requires-Dist: mdit-py-plugins[linkify] >= 0.3.3
+Requires-Dist: mdit-py-plugins >= 0.3.3
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mdformat-admon ; extra == "recommended"
 Requires-Dist: mdformat-beautysh ; extra == "recommended"
 Requires-Dist: mdformat-black ; extra == "recommended"
 Requires-Dist: mdformat-config ; extra == "recommended"
 Requires-Dist: mdformat-footnote ; extra == "recommended"
 Requires-Dist: mdformat-frontmatter ; extra == "recommended"
@@ -40,17 +40,17 @@
 [cov-link]: https://codecov.io/gh/executablebooks/mdformat-mkdocs
  -->
 
 An [mdformat](https://github.com/executablebooks/mdformat) plugin for [mkdocs](https://github.com/mkdocs/mkdocs).
 
 ## Usage
 
-Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. See [additional information on `mdformat` plugins here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
+Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. For additional information on plugins, see [the official `mdformat` documentation here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
 
-Tip: this package specifies an "extra" (`recommended`) for plugins that work well with mkdocs:
+Tip: this package specifies an "extra" (`'recommended'`) for plugins that work well with mkdocs:
 
 - [mdformat-admon](https://pypi.org/project/mdformat-admon)
 - [mdformat-beautysh](https://pypi.org/project/mdformat-beautysh)
 - [mdformat-black](https://pypi.org/project/mdformat-black)
 - [mdformat-config](https://pypi.org/project/mdformat-config)
 - [mdformat-footnote](https://pypi.org/project/mdformat-footnote)
 - [mdformat-frontmatter](https://pypi.org/project/mdformat-frontmatter)
@@ -78,35 +78,37 @@
 ```sh
 pipx install mdformat
 pipx inject mdformat mdformat-mkdocs
 # Or
 # pipx inject mdformat "mdformat-mkdocs[recommended]"
 ```
 
-## Caveats
-
-- All indents are converted to 4-spaces
-- This plugin converts all bulleted items to dashes (`-`) and numerals to `1.`
+## CLI Options
 
-See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
-
-## Configuration
-
-`mdformat-mkdocs` adds the CLI argument `--align-semantic-breaks-in-numbered-lists` to optionally align line breaks in numbered lists to 3-spaces. If not specified, the default of 4-indents is followed universally.
+`mdformat-mkdocs` adds the CLI argument `--align-semantic-breaks-in-lists` to optionally align line breaks in numbered lists to 3-spaces. If not specified, the default of 4-indents is followed universally.
 
 ```txt
 # with: mdformat
 1. Semantic line feed where the following line is
     three spaces deep
 
-# vs. with: mdformat --align-semantic-breaks-in-numbered-lists
+# vs. with: mdformat --align-semantic-breaks-in-lists
 1. Semantic line feed where the following line is
    three spaces deep
 ```
 
+Note: the `align-semantic-breaks-in-lists` setting is not supported in the configuration file yet (https://github.com/executablebooks/mdformat/issues/378)
+
+## Caveats
+
+- All indents are converted to 4-spaces
+- This plugin converts all bulleted items to dashes (`-`) and numerals to `1.`
+
+See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
+
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-mkdocs/blob/main/CONTRIBUTING.md)
 
 [ci-badge]: https://github.com/kyleking/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
 [ci-link]: https://github.com/kyleking/mdformat-mkdocs/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
 [pypi-badge]: https://img.shields.io/pypi/v/mdformat-mkdocs.svg
```

