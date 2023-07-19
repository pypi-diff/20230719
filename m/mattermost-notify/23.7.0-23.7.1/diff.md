# Comparing `tmp/mattermost_notify-23.7.0.tar.gz` & `tmp/mattermost_notify-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattermost_notify-23.7.0.tar", max compression
+gzip compressed data, was "mattermost_notify-23.7.1.tar", max compression
```

## Comparing `mattermost_notify-23.7.0.tar` & `mattermost_notify-23.7.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/LICENSE
--rw-r--r--   0        0        0     1754 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/README.md
--rw-r--r--   0        0        0       53 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/mattermost_notify/__init__.py
--rw-r--r--   0        0        0      103 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/mattermost_notify/__version__.py
--rw-r--r--   0        0        0     4717 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/mattermost_notify/git.py
--rw-r--r--   0        0        0     1628 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/mattermost_notify/parser.py
--rw-r--r--   0        0        0      343 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/mattermost_notify/status.py
--rw-r--r--   0        0        0    51650 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/poetry.lock
--rw-r--r--   0        0        0     2097 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/pyproject.toml
--rw-r--r--   0        0        0       53 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/tests/__init__.py
--rw-r--r--   0        0        0     4041 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/tests/test_git.py
--rw-r--r--   0        0        0     3830 2023-07-18 08:42:21.636245 mattermost_notify-23.7.0/tests/test_parser.py
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 mattermost_notify-23.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/LICENSE
+-rw-r--r--   0        0        0     1754 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/README.md
+-rw-r--r--   0        0        0       53 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/__version__.py
+-rw-r--r--   0        0        0      203 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/errors.py
+-rw-r--r--   0        0        0     4946 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/git.py
+-rw-r--r--   0        0        0     1628 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/parser.py
+-rw-r--r--   0        0        0      519 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/post.py
+-rw-r--r--   0        0        0      343 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/mattermost_notify/status.py
+-rw-r--r--   0        0        0    51646 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/poetry.lock
+-rw-r--r--   0        0        0     2097 2023-07-19 15:13:09.329993 mattermost_notify-23.7.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-07-19 15:13:09.333993 mattermost_notify-23.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     3862 2023-07-19 15:13:09.333993 mattermost_notify-23.7.1/tests/test_git.py
+-rw-r--r--   0        0        0     3830 2023-07-19 15:13:09.333993 mattermost_notify-23.7.1/tests/test_parser.py
+-rw-r--r--   0        0        0     1353 2023-07-19 15:13:09.333993 mattermost_notify-23.7.1/tests/test_post.py
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 mattermost_notify-23.7.1/PKG-INFO
```

### Comparing `mattermost_notify-23.7.0/LICENSE` & `mattermost_notify-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mattermost_notify-23.7.0/README.md` & `mattermost_notify-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mattermost_notify-23.7.0/mattermost_notify/git.py` & `mattermost_notify-23.7.1/mattermost_notify/git.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 # pylint: disable=invalid-name
 
 import json
 import os
 from pathlib import Path
 from typing import Any, Optional
 
-import httpx
-from pontos.terminal.terminal import ConsoleTerminal
+from pontos.git import Git
+from pontos.terminal import RichTerminal
 
+from mattermost_notify.errors import MattermostNotifyError
 from mattermost_notify.parser import parse_args
+from mattermost_notify.post import post
 from mattermost_notify.status import Status
 
 LONG_TEMPLATE = (
     "#### Status: {status}\n\n"
     "| Workflow | {workflow} |\n"
     "| --- | --- |\n"
     "| Repository (branch) | {repository} ({branch}) |\n"
@@ -30,50 +32,47 @@
 
 
 def linker(name: str, url: Optional[str] = None) -> str:
     # create a markdown link
     return f"[{name}]({url})" if url else name
 
 
-def get_github_event_json(term: ConsoleTerminal) -> dict[str, Any]:
+def get_github_event_json() -> dict[str, Any]:
     github_event_path = os.environ.get("GITHUB_EVENT_PATH")
 
     if not github_event_path:
         return {}
 
     json_path = Path(github_event_path)
 
     try:
         with json_path.open("r", encoding="utf-8") as f:
             return json.load(f)
     except FileNotFoundError:
-        term.error("Could not find GitHub Event JSON file.")
+        raise MattermostNotifyError("Could not find GitHub Event JSON file.")
     except json.JSONDecodeError:
-        term.error("Could not decode the JSON object.")
-
-    return {}
+        raise MattermostNotifyError("Could not decode the JSON object.")
 
 
 def fill_template(
     *,
     short: bool = False,
     highlight: Optional[list[str]] = None,
     commit: Optional[str] = None,
     commit_message: Optional[str] = None,
     branch: Optional[str] = None,
     repository: Optional[str] = None,
     status: Optional[str] = None,
     workflow_id: Optional[str] = None,
     workflow_name: Optional[str] = None,
-    terminal: ConsoleTerminal,
 ) -> str:
     template = SHORT_TEMPLATE if short else LONG_TEMPLATE
 
     # try to get information from the GiTHUB_EVENT json
-    event = get_github_event_json(terminal)
+    event = get_github_event_json()
     workflow_info: dict[str, Any] = event.get("workflow_run", {})
 
     status = status if status else workflow_info.get("conclusion")
     workflow_status = Status[status.upper()] if status else Status.UNKNOWN
 
     used_workflow_name: str = (
         workflow_name if workflow_name else workflow_info.get("name", "")
@@ -101,19 +100,24 @@
         else workflow_info.get("html_url", "")
     )
 
     head_commit = workflow_info.get("head_commit", {})
 
     if commit:
         commit_url = f"{repository_url}/commit/{commit}"
+
+        if not commit_message:
+            commit_message = Git().show(
+                format="format:%s", patch=False, objects=commit  # type: ignore[assignment] # noqa: E501
+            )
     else:
         commit_url = f'{repository_url}/commit/{head_commit.get("id", "")}'
 
-    if not commit_message:
-        commit_message = head_commit.get("message", "").split("\n", 1)[0]
+        if not commit_message:
+            commit_message = head_commit.get("message", "").split("\n", 1)[0]
 
     highlight_str = ""
     if highlight and workflow_status is not Status.SUCCESS:
         highlight_str = "".join([f"@{h}\n" for h in highlight])
 
     return template.format(
         status=workflow_status.value,
@@ -124,37 +128,35 @@
         highlight=highlight_str,
     )
 
 
 def main() -> None:
     parsed_args = parse_args()
 
-    term = ConsoleTerminal()
-
-    if not parsed_args.free:
-        body = fill_template(
-            highlight=parsed_args.highlight,
-            short=parsed_args.short,
-            branch=parsed_args.branch,
-            commit=parsed_args.commit,
-            repository=parsed_args.repository,
-            status=parsed_args.status,
-            workflow_id=parsed_args.workflow,
-            workflow_name=parsed_args.workflow_name,
-            terminal=term,
-        )
+    term = RichTerminal()
 
-        data = {"channel": parsed_args.channel, "text": body}
-    else:
-        data = {"channel": parsed_args.channel, "text": parsed_args.free}
+    try:
+        if not parsed_args.free:
+            body = fill_template(
+                highlight=parsed_args.highlight,
+                short=parsed_args.short,
+                branch=parsed_args.branch,
+                commit=parsed_args.commit,
+                repository=parsed_args.repository,
+                status=parsed_args.status,
+                workflow_id=parsed_args.workflow,
+                workflow_name=parsed_args.workflow_name,
+            )
+            post(parsed_args.url, parsed_args.channel, body)
+        else:
+            post(parsed_args.url, parsed_args.channel, parsed_args.free)
 
-    response = httpx.post(url=parsed_args.url, json=data)
-    if response.is_success:
         term.ok(
-            f"Successfully posted on Mattermost channel {parsed_args.channel}"
+            "Successfully posted on Mattermost channel "
+            f"{parsed_args.channel}"
         )
-    else:
-        term.error("Failed to post on Mattermost")
+    except MattermostNotifyError as e:
+        term.error(f"❌ Error: {e}")
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mattermost_notify-23.7.0/mattermost_notify/parser.py` & `mattermost_notify-23.7.1/mattermost_notify/parser.py`

 * *Files identical despite different names*

### Comparing `mattermost_notify-23.7.0/poetry.lock` & `mattermost_notify-23.7.1/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 [package.extras]
 doc = ["Sphinx", "packaging", "sphinx-autodoc-typehints (>=1.2.0)", "sphinx-rtd-theme (>=1.2.2)", "sphinxcontrib-jquery"]
 test = ["anyio[trio]", "coverage[toml] (>=4.5)", "hypothesis (>=4.0)", "mock (>=4)", "psutil (>=5.9)", "pytest (>=7.0)", "pytest-mock (>=3.6.1)", "trustme", "uvloop (>=0.17)"]
 trio = ["trio (<0.22)"]
 
 [[package]]
 name = "autohooks"
-version = "23.4.0"
+version = "23.7.0"
 description = "Library for managing git hooks"
 optional = false
-python-versions = ">=3.7.2,<4.0.0"
+python-versions = ">=3.8,<4.0"
 files = [
-    {file = "autohooks-23.4.0-py3-none-any.whl", hash = "sha256:2c3b8506890565ad8c9b690db9b70a9b65068ff9f1c2a2d601d2914ad576cfff"},
-    {file = "autohooks-23.4.0.tar.gz", hash = "sha256:6880ad263f0aaab607bbfc1d42afc407de6234320fcff10d75d4e89f4e711ccd"},
+    {file = "autohooks-23.7.0-py3-none-any.whl", hash = "sha256:1fa417891efc3681bdf109cb2e99688948d1f3587d91dab17f1ed9b4428590a4"},
+    {file = "autohooks-23.7.0.tar.gz", hash = "sha256:cf486581fc111122fc3ea394b60a26bc4da0844cf916b6e4fadf90ff97633fe5"},
 ]
 
 [package.dependencies]
 pontos = ">=22.8.0"
 rich = ">=12.5.1"
 tomlkit = ">=0.5.11"
 
@@ -152,21 +152,21 @@
 files = [
     {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
     {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
 ]
 
 [[package]]
 name = "click"
-version = "8.1.5"
+version = "8.1.6"
 description = "Composable command line interface toolkit"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "click-8.1.5-py3-none-any.whl", hash = "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"},
-    {file = "click-8.1.5.tar.gz", hash = "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367"},
+    {file = "click-8.1.6-py3-none-any.whl", hash = "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"},
+    {file = "click-8.1.6.tar.gz", hash = "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "colorama"
@@ -623,21 +623,21 @@
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pontos"
-version = "23.7.6"
+version = "23.7.7"
 description = "Common utilities and tools maintained by Greenbone Networks"
 optional = false
 python-versions = ">=3.9"
 files = [
-    {file = "pontos-23.7.6-py3-none-any.whl", hash = "sha256:c85c802acd7640a2333a523e4ecd9317bb5915620498bdc792a1b073287a5d63"},
-    {file = "pontos-23.7.6.tar.gz", hash = "sha256:c6b9ce4812b5db48686bf418a0bd1edd64da8059a311f6aaa47cf9da1354e56f"},
+    {file = "pontos-23.7.7-py3-none-any.whl", hash = "sha256:00eec64a17873d9730be165688d7fe4e5e63a92f8ed2052e26cd171b4d8a45f2"},
+    {file = "pontos-23.7.7.tar.gz", hash = "sha256:b5be54727b1f8d759278f65fd33c9fe17266d4d42664d7e22803d8f8eb4fcfb6"},
 ]
 
 [package.dependencies]
 colorful = ">=0.5.4"
 httpx = {version = ">=0.23,<0.25", extras = ["http2"]}
 lxml = ">=4.9.0"
 packaging = ">=20.3"
@@ -783,8 +783,8 @@
     {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
     {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [metadata]
 lock-version = "2.0"
 python-versions = ">=3.9"
-content-hash = "5d6f53fe3c49ae7d0835717f9325c4d824c806954ce5fc50874c609ee21e760f"
+content-hash = "005d964206b2a56e7b9a2722bba14e98b60a9b036e420aee2372c13498aa4822"
```

### Comparing `mattermost_notify-23.7.0/pyproject.toml` & `mattermost_notify-23.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mattermost-notify"
-version = "23.7.0"
+version = "23.7.1"
 description = "Python tool to post GitHub Action runs to mattermost"
 authors = ["Jaspar Stach <jasp.stac@gmx.de>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 classifiers=[
   # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
@@ -25,15 +25,15 @@
   { include = "poetry.lock", format = "sdist" },
 ]
 include = [
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-pontos = ">=22.7.0"
+pontos = ">=22.7.7"
 httpx = ">=0.23.1"
 
 [tool.poetry.dev-dependencies]
 autohooks-plugin-black = { version = ">=22.11.0", python = "^3.9" }
 autohooks-plugin-isort = { version = ">=22.8.0", python = "^3.9" }
 autohooks-plugin-ruff = { version = ">=23.6.0", python = "^3.9" }
 autohooks-plugin-mypy = { version = ">=23.3.0", python = "^3.9" }
```

### Comparing `mattermost_notify-23.7.0/tests/test_git.py` & `mattermost_notify-23.7.1/tests/test_git.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 
 class FillTemplateTestCase(unittest.TestCase):
     def test_success_no_highlight(self):
         actual = fill_template(
             highlight=["user1", "user2"],
             status=Status.SUCCESS.name,
-            terminal=MagicMock(),
         )
         expected = """#### Status: :white_check_mark: success
 
 | Workflow |  |
 | --- | --- |
 | Repository (branch) |  ([](/tree/)) |
 | Related commit | [](/commit/) |
@@ -38,15 +37,14 @@
 """
         self.assertEqual(expected, actual)
 
     def test_failure_highlight(self):
         actual = fill_template(
             highlight=["user1", "user2"],
             status=Status.FAILURE.name,
-            terminal=MagicMock(),
         )
         expected = """#### Status: :x: failure
 
 | Workflow |  |
 | --- | --- |
 | Repository (branch) |  ([](/tree/)) |
 | Related commit | [](/commit/) |
@@ -62,15 +60,14 @@
             status=Status.SUCCESS.name,
             workflow_name="SomeWorkflow",
             workflow_id="w1",
             commit="12345",
             commit_message="Add foo",
             repository="foo/bar",
             branch="main",
-            terminal=MagicMock(),
         )
         expected = (
             ":white_check_mark: success: [SomeWorkflow](https://github.com/foo/bar/actions/runs/w1) "
             "([Add foo](https://github.com/foo/bar/commit/12345)) in "
             "[foo/bar](https://github.com/foo/bar) ([main](https://github.com/foo/bar/tree/main))"
         )
         self.assertEqual(expected, actual)
@@ -81,15 +78,14 @@
             status=Status.SUCCESS.name,
             workflow_name="SomeWorkflow",
             workflow_id="w1",
             commit="12345",
             commit_message="Add foo",
             repository="foo/bar",
             branch="main",
-            terminal=MagicMock(),
         )
         expected = """#### Status: :white_check_mark: success
 
 | Workflow | [SomeWorkflow](https://github.com/foo/bar/actions/runs/w1) |
 | --- | --- |
 | Repository (branch) | [foo/bar](https://github.com/foo/bar) ([main](https://github.com/foo/bar/tree/main)) |
 | Related commit | [Add foo](https://github.com/foo/bar/commit/12345) |
@@ -110,17 +106,15 @@
                 "head_branch": "main",
                 "head_commit": {"id": "12345", "message": "Add foo"},
                 "workflow_id": "w1",
             }
         }
         mock.return_value = event
 
-        actual = fill_template(
-            terminal=MagicMock(),
-        )
+        actual = fill_template()
         expected = """#### Status: :white_check_mark: success
 
 | Workflow | [SomeWorkflow](https://github.com/foo/bar/actions/runs/w1) |
 | --- | --- |
 | Repository (branch) | [foo/bar](https://github.com/foo/bar) ([main](https://github.com/foo/bar/tree/main)) |
 | Related commit | [Add foo](https://github.com/foo/bar/commit/12345) |
```

### Comparing `mattermost_notify-23.7.0/tests/test_parser.py` & `mattermost_notify-23.7.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `mattermost_notify-23.7.0/PKG-INFO` & `mattermost_notify-23.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattermost-notify
-Version: 23.7.0
+Version: 23.7.1
 Summary: Python tool to post GitHub Action runs to mattermost
 License: GPL-3.0-or-later
 Author: Jaspar Stach
 Author-email: jasp.stac@gmx.de
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx (>=0.23.1)
-Requires-Dist: pontos (>=22.7.0)
+Requires-Dist: pontos (>=22.7.7)
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # mattermost-notify <!-- omit in toc -->
 
 [![GitHub releases](https://img.shields.io/github/release/greenbone/mattermost-notify.svg)](https://github.com/greenbone/mattermost-notify/releases)
```

