# Comparing `tmp/gitflow-pyproject-version-bumper-0.1.3.tar.gz` & `tmp/gitflow_pyproject_version_bumper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitflow-pyproject-version-bumper-0.1.3.tar", max compression
+gzip compressed data, was "gitflow_pyproject_version_bumper-0.1.4.tar", max compression
```

## Comparing `gitflow-pyproject-version-bumper-0.1.3.tar` & `gitflow_pyproject_version_bumper-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-11 19:43:24.234598 gitflow-pyproject-version-bumper-0.1.3/LICENSE
--rw-r--r--   0        0        0      953 2023-04-11 19:43:24.234598 gitflow-pyproject-version-bumper-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-30 21:36:49.551250 gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/__init__.py
--rw-r--r--   0        0        0     1614 2023-04-11 19:43:24.262598 gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/__main__.py
--rwxr-xr-x   0        0        0     1340 2023-04-11 19:43:57.506640 gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/post_checkout.py
--rw-r--r--   0        0        0      627 2023-04-11 19:44:04.234648 gitflow-pyproject-version-bumper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 gitflow-pyproject-version-bumper-0.1.3/setup.py
--rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 gitflow-pyproject-version-bumper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-11 19:43:24.234598 gitflow_pyproject_version_bumper-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1258 2023-07-19 08:48:20.141316 gitflow_pyproject_version_bumper-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-30 21:36:49.551250 gitflow_pyproject_version_bumper-0.1.4/gitflow_pyproject_version_bumper/__init__.py
+-rw-r--r--   0        0        0     2370 2023-07-19 08:48:20.141316 gitflow_pyproject_version_bumper-0.1.4/gitflow_pyproject_version_bumper/__main__.py
+-rwxr-xr-x   0        0        0     1493 2023-07-19 08:48:20.141316 gitflow_pyproject_version_bumper-0.1.4/gitflow_pyproject_version_bumper/post_checkout.py
+-rw-r--r--   0        0        0      627 2023-07-19 08:48:29.045394 gitflow_pyproject_version_bumper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 gitflow_pyproject_version_bumper-0.1.4/PKG-INFO
```

### Comparing `gitflow-pyproject-version-bumper-0.1.3/LICENSE` & `gitflow_pyproject_version_bumper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gitflow-pyproject-version-bumper-0.1.3/README.md` & `gitflow_pyproject_version_bumper-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -17,14 +17,23 @@
 
 ```
 python3 -m pip install poetry
 python3 -m pip install .
 python3 -m gitflow_pyproject_version_bumper install
 ```
 
+Install options:
+```
+  --force               overwrite hook if it exists
+  --commit-message-template COMMIT_MESSAGE_TEMPLATE
+                        commit message when updating the version. 
+                        Default: Version bumped to {version}
+```
+`{version}` - placeholder for the new version.
+
 # Usage
 Just start a release, as you usually do:
 `git flow release start 1.2.3`
 
 That's it.
 The app version in pyproject.toml has already been updated, 
 and the change has been committed.
```

### Comparing `gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/post_checkout.py` & `gitflow_pyproject_version_bumper-0.1.4/gitflow_pyproject_version_bumper/post_checkout.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 import git
 import tomlkit
 
 BRANCH_CHECKOUT_TYPE = "1"
 
-_, _, _, checkout_type = sys.argv
+checkout_type = sys.argv[-1]
 if checkout_type != BRANCH_CHECKOUT_TYPE:
     exit()
 
 repo = git.Repo()
 try:
     head = repo.active_branch
 except TypeError:
@@ -25,14 +25,19 @@
         fallback="release/",
     )
     gitflow_hotfix_prefix = git_config.get(
         section='gitflow "prefix"',
         option="hotfix",
         fallback="hotfix/",
     )
+    commit_message_template = git_config.get(
+        section="versionbumper",
+        option="commitmessagetemplate",
+        fallback="Version bumped to {version}",
+    )
 
 if head.name.startswith(gitflow_release_prefix):
     new_version = repo.active_branch.name[len(gitflow_release_prefix) :]
 elif head.name.startswith(gitflow_hotfix_prefix):
     new_version = repo.active_branch.name[len(gitflow_hotfix_prefix) :]
 else:
     exit()
@@ -44,9 +49,8 @@
     exit()
 
 pyproject["tool"]["poetry"]["version"] = new_version
 with open(pyproject_toml_path, "w") as f:
     tomlkit.dump(pyproject, f)
 
 repo.index.add(str(pyproject_toml_path))
-commit_message = f"Version bumped to {new_version}"
-repo.index.commit(commit_message)
+repo.index.commit(commit_message_template.format(version=new_version))
```

### Comparing `gitflow-pyproject-version-bumper-0.1.3/pyproject.toml` & `gitflow_pyproject_version_bumper-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitflow-pyproject-version-bumper"
-version = "0.1.3"
+version = "0.1.4"
 description = "Automatic pyproject.toml based app version bumper"
 authors = ["Grigory Bukovsky <booqoffsky@yandex.ru>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "gitflow_pyproject_version_bumper"}]
 repository = 'https://github.com/booqoffsky/gitflow-pyproject-version-bumper'
 keywords = ['gitflow', 'version', 'bumper', 'auto', 'pyproject', 'poetry', 'updater']
```

### Comparing `gitflow-pyproject-version-bumper-0.1.3/setup.py` & `gitflow_pyproject_version_bumper-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,61 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gitflow-pyproject-version-bumper
+Version: 0.1.4
+Summary: Automatic pyproject.toml based app version bumper
+Home-page: https://github.com/booqoffsky/gitflow-pyproject-version-bumper
+License: MIT
+Keywords: gitflow,version,bumper,auto,pyproject,poetry,updater
+Author: Grigory Bukovsky
+Author-email: booqoffsky@yandex.ru
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: GitPython (>=3.1.31,<4.0.0)
+Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
+Project-URL: Repository, https://github.com/booqoffsky/gitflow-pyproject-version-bumper
+Description-Content-Type: text/markdown
+
+![python version](https://img.shields.io/pypi/pyversions/gitflow-pyproject-version-bumper?style=for-the-badge) 
+[![version](https://img.shields.io/pypi/v/gitflow-pyproject-version-bumper?style=for-the-badge)](https://pypi.org/project/gitflow-pyproject-version-bumper/)
+
+# gitflow-pyproject-version-bumper
+> A git hook to automatically update the application version 
+> in pyproject.toml when a release is started using [gitflow](https://github.com/nvie/gitflow).
+
+# Installation
+From PyPi:
+
+```
+pip3 install gitflow-pyproject-version-bumper
+python3 -m gitflow_pyproject_version_bumper install
+```
+
+If you want to install it from sources, try this:
+
+```
+python3 -m pip install poetry
+python3 -m pip install .
+python3 -m gitflow_pyproject_version_bumper install
+```
+
+Install options:
+```
+  --force               overwrite hook if it exists
+  --commit-message-template COMMIT_MESSAGE_TEMPLATE
+                        commit message when updating the version. 
+                        Default: Version bumped to {version}
+```
+`{version}` - placeholder for the new version.
+
+# Usage
+Just start a release, as you usually do:
+`git flow release start 1.2.3`
+
+That's it.
+The app version in pyproject.toml has already been updated, 
+and the change has been committed.
 
-packages = \
-['gitflow_pyproject_version_bumper']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['GitPython>=3.1.31,<4.0.0', 'tomlkit>=0.11.7,<0.12.0']
-
-setup_kwargs = {
-    'name': 'gitflow-pyproject-version-bumper',
-    'version': '0.1.3',
-    'description': 'Automatic pyproject.toml based app version bumper',
-    'long_description': "![python version](https://img.shields.io/pypi/pyversions/gitflow-pyproject-version-bumper?style=for-the-badge) \n[![version](https://img.shields.io/pypi/v/gitflow-pyproject-version-bumper?style=for-the-badge)](https://pypi.org/project/gitflow-pyproject-version-bumper/)\n\n# gitflow-pyproject-version-bumper\n> A git hook to automatically update the application version \n> in pyproject.toml when a release is started using [gitflow](https://github.com/nvie/gitflow).\n\n# Installation\nFrom PyPi:\n\n```\npip3 install gitflow-pyproject-version-bumper\npython3 -m gitflow_pyproject_version_bumper install\n```\n\nIf you want to install it from sources, try this:\n\n```\npython3 -m pip install poetry\npython3 -m pip install .\npython3 -m gitflow_pyproject_version_bumper install\n```\n\n# Usage\nJust start a release, as you usually do:\n`git flow release start 1.2.3`\n\nThat's it.\nThe app version in pyproject.toml has already been updated, \nand the change has been committed.\n",
-    'author': 'Grigory Bukovsky',
-    'author_email': 'booqoffsky@yandex.ru',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/booqoffsky/gitflow-pyproject-version-bumper',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

