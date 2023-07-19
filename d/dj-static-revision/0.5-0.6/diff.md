# Comparing `tmp/dj-static-revision-0.5.tar.gz` & `tmp/dj_static_revision-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-static-revision-0.5.tar", max compression
+gzip compressed data, was "dj_static_revision-0.6.tar", max compression
```

## Comparing `dj-static-revision-0.5.tar` & `dj_static_revision-0.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1886 2020-04-18 17:56:35.799170 dj-static-revision-0.5/README.rst
--rw-r--r--   0        0        0      145 2020-04-01 16:23:10.110946 dj-static-revision-0.5/dj_static_revision/__init__.py
--rw-r--r--   0        0        0      240 2020-04-18 17:45:36.456484 dj-static-revision-0.5/dj_static_revision/context_processors.py
--rw-r--r--   0        0        0        0 2022-05-08 03:42:36.702829 dj-static-revision-0.5/dj_static_revision/py.typed
--rw-r--r--   0        0        0     1685 2020-04-18 17:43:17.811748 dj-static-revision-0.5/dj_static_revision/utils.py
--rw-r--r--   0        0        0      968 2022-05-08 03:51:23.711488 dj-static-revision-0.5/pyproject.toml
--rw-r--r--   0        0        0     2704 2022-05-08 03:55:58.919236 dj-static-revision-0.5/setup.py
--rw-r--r--   0        0        0     3069 2022-05-08 03:55:58.919474 dj-static-revision-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1886 2023-07-19 10:51:15.578757 dj_static_revision-0.6/README.rst
+-rw-r--r--   0        0        0      145 2020-04-01 16:23:10.000000 dj_static_revision-0.6/dj_static_revision/__init__.py
+-rw-r--r--   0        0        0      240 2020-04-18 17:45:36.000000 dj_static_revision-0.6/dj_static_revision/context_processors.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:23:07.163312 dj_static_revision-0.6/dj_static_revision/py.typed
+-rw-r--r--   0        0        0     1685 2020-04-18 17:43:17.000000 dj_static_revision-0.6/dj_static_revision/utils.py
+-rw-r--r--   0        0        0     1482 2023-07-19 10:58:10.489489 dj_static_revision-0.6/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 dj_static_revision-0.6/PKG-INFO
```

### Comparing `dj-static-revision-0.5/README.rst` & `dj_static_revision-0.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Install
 -------
 
 .. code-block:: shell
 
     pip3 install dj-static-revision
 
-`Django Static Revision` only supports Python 3.6+.
+`Django Static Revision` only supports Python 3.8+.
 
 
 Usage
 -----
 
 Add ``dj_static_revision.context_processors.static_revision`` to your ``context_processors`` list.
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ====================== Django Static Revision ====================== .. image::
 https://madewithlove.now.sh/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d ..
 image:: https://badgen.net/pypi/v/dj-static-revision :target: https://pypi.org/
 project/dj-static-revision Django plugin to provide a context variable for
 retrieving the version of running application. This variable is meant to change
 the URL of a static file, to invalidate browser cache. Install ------- .. code-
 block:: shell pip3 install dj-static-revision `Django Static Revision` only
-supports Python 3.6+. Usage ----- Add
+supports Python 3.8+. Usage ----- Add
 ``dj_static_revision.context_processors.static_revision`` to your
 ``context_processors`` list. .. code-block:: python TEMPLATES = ( { 'NAME':
 'jinja2', 'BACKEND': 'django_jinja.backend.Jinja2', 'OPTIONS':
 { 'context_processors': ( # Other context processors
 'dj_static_revision.context_processors.static_revision', ), A variable
 ``REVISION`` will then exists in your template, you can use it to append to
 static file URL. .. code-block:: jinja
```

### Comparing `dj-static-revision-0.5/dj_static_revision/utils.py` & `dj_static_revision-0.6/dj_static_revision/utils.py`

 * *Files identical despite different names*

### Comparing `dj-static-revision-0.5/pyproject.toml` & `dj_static_revision-0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,69 @@
 [tool.poetry]
 name = "dj-static-revision"
-version = "0.5"
+version = "0.6"
 description = "Revision info for Django static file"
 authors = ["Nguyễn Hồng Quân <ng.hong.quan@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/AgriConnect/dj-static-revision.git"
 homepage = "https://github.com/AgriConnect/dj-static-revision"
 readme = "README.rst"
 keywords = ["django", "static", "version", "cache"]
 classifiers = [
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
-    "Framework :: Django :: 3.0",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Environment :: Web Environment",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-dulwich = "^0.19.15"
+python = "^3.8"
+dulwich = "^0.21.5"
 single-version = "^1.5.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-flake8 = "^1.1.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+pytest-env = "^0.8.2"
+
+
+[tool.poetry.group.lint.dependencies]
+ruff = "^0.0.278"
+
+[tool.ruff]
+line-length = 120
+
+target-version = "py310"
+
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "*/migrations/*",
+    "*/static/CACHE/*",
+]
+
+[tool.ruff.per-file-ignores]
+"tests/test_dj_static_revision.py" = ["E402"]
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `dj-static-revision-0.5/setup.py` & `dj_static_revision-0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dj-static-revision
+Version: 0.6
+Summary: Revision info for Django static file
+Home-page: https://github.com/AgriConnect/dj-static-revision
+License: Apache-2.0
+Keywords: django,static,version,cache
+Author: Nguyễn Hồng Quân
+Author-email: ng.hong.quan@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: dulwich (>=0.21.5,<0.22.0)
+Requires-Dist: single-version (>=1.5.1,<2.0.0)
+Project-URL: Repository, https://github.com/AgriConnect/dj-static-revision.git
+Description-Content-Type: text/x-rst
 
-packages = \
-['dj_static_revision']
+======================
+Django Static Revision
+======================
 
-package_data = \
-{'': ['*']}
+.. image:: https://madewithlove.now.sh/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d
+.. image:: https://badgen.net/pypi/v/dj-static-revision
+   :target: https://pypi.org/project/dj-static-revision
 
-install_requires = \
-['dulwich>=0.19.15,<0.20.0', 'single-version>=1.5.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'dj-static-revision',
-    'version': '0.5',
-    'description': 'Revision info for Django static file',
-    'long_description': '======================\nDjango Static Revision\n======================\n\n.. image:: https://madewithlove.now.sh/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d\n.. image:: https://badgen.net/pypi/v/dj-static-revision\n   :target: https://pypi.org/project/dj-static-revision\n\n\nDjango plugin to provide a context variable for retrieving the version of running application.\n\nThis variable is meant to change the URL of a static file, to invalidate browser cache.\n\n\nInstall\n-------\n\n.. code-block:: shell\n\n    pip3 install dj-static-revision\n\n`Django Static Revision` only supports Python 3.6+.\n\n\nUsage\n-----\n\nAdd ``dj_static_revision.context_processors.static_revision`` to your ``context_processors`` list.\n\n.. code-block:: python\n\n    TEMPLATES = (\n        {\n            \'NAME\': \'jinja2\',\n            \'BACKEND\': \'django_jinja.backend.Jinja2\',\n            \'OPTIONS\': {\n                \'context_processors\': (\n                    # Other context processors\n                    \'dj_static_revision.context_processors.static_revision\',\n                ),\n\nA variable ``REVISION`` will then exists in your template, you can use it to append to static file URL.\n\n.. code-block:: jinja\n\n    <script src="{{ static(\'js/app.js\') }}?v={{ REVISION }}"></script>\n\n\n`Django Static Revision` retrieves revision string from Git history.\nIf your source code is not managed by Git, the revision info will be read from a file named `.version` placed next to `manage.py` file.\n\n\nSettings\n--------\n\nThe revision string will be truncated to 10 characters. You can change that by add to Django settings:\n\n.. code-block:: python\n\n    STATIC_REVISION_STRING_LENGTH = 10\n\nYou can also change the file for `Django Static Revision` to read revision string from, by add this setting:\n\n.. code-block:: python\n\n    STATIC_REVISION_VERSION_FILE = \'.version\'\n\nwhere *.version* is a text file containing any string you want.\n',
-    'author': 'Nguyễn Hồng Quân',
-    'author_email': 'ng.hong.quan@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/AgriConnect/dj-static-revision',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
 
+Django plugin to provide a context variable for retrieving the version of running application.
+
+This variable is meant to change the URL of a static file, to invalidate browser cache.
+
+
+Install
+-------
+
+.. code-block:: shell
+
+    pip3 install dj-static-revision
+
+`Django Static Revision` only supports Python 3.8+.
+
+
+Usage
+-----
+
+Add ``dj_static_revision.context_processors.static_revision`` to your ``context_processors`` list.
+
+.. code-block:: python
+
+    TEMPLATES = (
+        {
+            'NAME': 'jinja2',
+            'BACKEND': 'django_jinja.backend.Jinja2',
+            'OPTIONS': {
+                'context_processors': (
+                    # Other context processors
+                    'dj_static_revision.context_processors.static_revision',
+                ),
+
+A variable ``REVISION`` will then exists in your template, you can use it to append to static file URL.
+
+.. code-block:: jinja
+
+    <script src="{{ static('js/app.js') }}?v={{ REVISION }}"></script>
+
+
+`Django Static Revision` retrieves revision string from Git history.
+If your source code is not managed by Git, the revision info will be read from a file named `.version` placed next to `manage.py` file.
+
+
+Settings
+--------
+
+The revision string will be truncated to 10 characters. You can change that by add to Django settings:
+
+.. code-block:: python
+
+    STATIC_REVISION_STRING_LENGTH = 10
+
+You can also change the file for `Django Static Revision` to read revision string from, by add this setting:
+
+.. code-block:: python
+
+    STATIC_REVISION_VERSION_FILE = '.version'
+
+where *.version* is a text file containing any string you want.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,34 +1,39 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['dj_static_revision'] package_data = \ {'': ['*']} install_requires = \
-['dulwich>=0.19.15,<0.20.0', 'single-version>=1.5.1,<2.0.0'] setup_kwargs =
-{ 'name': 'dj-static-revision', 'version': '0.5', 'description': 'Revision info
-for Django static file', 'long_description': '======================\nDjango
-Static Revision\n======================\n\n.. image:: https://
-madewithlove.now.sh/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d\n.. image::
-https://badgen.net/pypi/v/dj-static-revision\n :target: https://pypi.org/
-project/dj-static-revision\n\n\nDjango plugin to provide a context variable for
-retrieving the version of running application.\n\nThis variable is meant to
-change the URL of a static file, to invalidate browser cache.\n\n\nInstall\n---
-----\n\n.. code-block:: shell\n\n pip3 install dj-static-revision\n\n`Django
-Static Revision` only supports Python 3.6+.\n\n\nUsage\n-----\n\nAdd
-``dj_static_revision.context_processors.static_revision`` to your
-``context_processors`` list.\n\n.. code-block:: python\n\n TEMPLATES = (\n {\n
-\'NAME\': \'jinja2\',\n \'BACKEND\': \'django_jinja.backend.Jinja2\',\n
-\'OPTIONS\': {\n \'context_processors\': (\n # Other context processors\n
-\'dj_static_revision.context_processors.static_revision\',\n ),\n\nA variable
+Metadata-Version: 2.1 Name: dj-static-revision Version: 0.6 Summary: Revision
+info for Django static file Home-page: https://github.com/AgriConnect/dj-
+static-revision License: Apache-2.0 Keywords: django,static,version,cache
+Author: Nguyá»n Há»ng QuÃ¢n Author-email: ng.hong.quan@gmail.com Requires-
+Python: >=3.8,<4.0 Classifier: Environment :: Web Environment Classifier:
+Framework :: Django Classifier: Framework :: Django :: 3.2 Classifier:
+Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier:
+Framework :: Django :: 4.2 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Dist: dulwich
+(>=0.21.5,<0.22.0) Requires-Dist: single-version (>=1.5.1,<2.0.0) Project-URL:
+Repository, https://github.com/AgriConnect/dj-static-revision.git Description-
+Content-Type: text/x-rst ====================== Django Static Revision
+====================== .. image:: https://madewithlove.now.sh/
+vn?heart=true&colorA=%23ffcd00&colorB=%23da251d .. image:: https://badgen.net/
+pypi/v/dj-static-revision :target: https://pypi.org/project/dj-static-revision
+Django plugin to provide a context variable for retrieving the version of
+running application. This variable is meant to change the URL of a static file,
+to invalidate browser cache. Install ------- .. code-block:: shell pip3 install
+dj-static-revision `Django Static Revision` only supports Python 3.8+. Usage --
+--- Add ``dj_static_revision.context_processors.static_revision`` to your
+``context_processors`` list. .. code-block:: python TEMPLATES = ( { 'NAME':
+'jinja2', 'BACKEND': 'django_jinja.backend.Jinja2', 'OPTIONS':
+{ 'context_processors': ( # Other context processors
+'dj_static_revision.context_processors.static_revision', ), A variable
 ``REVISION`` will then exists in your template, you can use it to append to
-static file URL.\n\n.. code-block:: jinja\n\n
-\n\n\n`Django Static Revision` retrieves revision string from Git history.\nIf
-your source code is not managed by Git, the revision info will be read from a
-file named `.version` placed next to `manage.py` file.\n\n\nSettings\n--------
-\n\nThe revision string will be truncated to 10 characters. You can change that
-by add to Django settings:\n\n.. code-block:: python\n\n
-STATIC_REVISION_STRING_LENGTH = 10\n\nYou can also change the file for `Django
-Static Revision` to read revision string from, by add this setting:\n\n.. code-
-block:: python\n\n STATIC_REVISION_VERSION_FILE = \'.version\'\n\nwhere
-*.version* is a text file containing any string you want.\n', 'author':
-'Nguyá»n Há»ng QuÃ¢n', 'author_email': 'ng.hong.quan@gmail.com',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/
-AgriConnect/dj-static-revision', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.7,<4.0', } setup(**setup_kwargs)
+static file URL. .. code-block:: jinja
+ `Django Static Revision` retrieves revision string from Git history. If your
+source code is not managed by Git, the revision info will be read from a file
+named `.version` placed next to `manage.py` file. Settings -------- The
+revision string will be truncated to 10 characters. You can change that by add
+to Django settings: .. code-block:: python STATIC_REVISION_STRING_LENGTH = 10
+You can also change the file for `Django Static Revision` to read revision
+string from, by add this setting: .. code-block:: python
+STATIC_REVISION_VERSION_FILE = '.version' where *.version* is a text file
+containing any string you want.
```

