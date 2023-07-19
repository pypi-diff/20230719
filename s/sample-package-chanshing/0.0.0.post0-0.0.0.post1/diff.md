# Comparing `tmp/sample-package-chanshing-0.0.0.post0.tar.gz` & `tmp/sample-package-chanshing-0.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-package-chanshing-0.0.0.post0.tar", last modified: Wed Apr 19 20:47:03 2023, max compression
+gzip compressed data, was "sample-package-chanshing-0.0.0.post1.tar", last modified: Wed Jul 19 14:46:55 2023, max compression
```

## Comparing `sample-package-chanshing-0.0.0.post0.tar` & `sample-package-chanshing-0.0.0.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/sample_package/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/src/sample_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/sample_package/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/src/sample_package/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/src/sample_package/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/src/sample_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/src/sample_package/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/src/sample_package/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:46:55.191328 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-19 14:46:55.000000 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-19 14:46:55.000000 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:46:55.000000 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 14:46:55.000000 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-19 14:46:55.000000 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 14:46:55.000000 sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-19 14:46:45.000000 sample-package-chanshing-0.0.0.post1/versioneer.py
```

### Comparing `sample-package-chanshing-0.0.0.post0/PKG-INFO` & `sample-package-chanshing-0.0.0.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-package-chanshing
-Version: 0.0.0.post0
+Version: 0.0.0.post1
 Summary: An example Python project
 Home-page: https://github.com/chanshing/sample-package
 Download-URL: https://github.com/chanshing/sample-package
 Author: Shing Chan
 Maintainer: Shing Chan
 Maintainer-email: cshing.m@gmail.com
 License: See LICENSE file.
@@ -43,12 +43,14 @@
     $ versioneer install
     ```
     Then *commit* the changes produced by `versioneer`. See [here](https://github.com/python-versioneer/python-versioneer/blob/master/INSTALL.md) to learn more.
 1. Setup your PyPI credentials. See the section *Saving credentials on Github* of [this guide](https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/). You should use the variable names `TEST_PYPI_API_TOKEN` and `PYPI_API_TOKEN` for the TestPyPI and PyPI tokens, respectively. See *.github/workflows/release.yaml*.
 
 You are all set! It should now be possible to run `git tag vX.Y.Z && git push --tags` to automatically version, build and publish a new release to PyPI.
 
+Finally, it is a good idea to [configure tag protection rules](https://docs.github.com/en/enterprise-server@3.8/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-tag-protection-rules) in your repository.
+
 ## References
 - Python packaging guide: https://packaging.python.org/en/latest/tutorials/packaging-projects/
     - ...and how things are changing: https://snarky.ca/what-the-heck-is-pyproject-toml/ &mdash; in particular, note that while *pyproject.toml* seems to be the future, currently Versioneer still depends on *setup.py*.
 - Versioneer: https://github.com/python-versioneer/python-versioneer
 - GitHub Actions: https://docs.github.com/en/actions
```

### Comparing `sample-package-chanshing-0.0.0.post0/README.md` & `sample-package-chanshing-0.0.0.post1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,14 @@
     $ versioneer install
     ```
     Then *commit* the changes produced by `versioneer`. See [here](https://github.com/python-versioneer/python-versioneer/blob/master/INSTALL.md) to learn more.
 1. Setup your PyPI credentials. See the section *Saving credentials on Github* of [this guide](https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/). You should use the variable names `TEST_PYPI_API_TOKEN` and `PYPI_API_TOKEN` for the TestPyPI and PyPI tokens, respectively. See *.github/workflows/release.yaml*.
 
 You are all set! It should now be possible to run `git tag vX.Y.Z && git push --tags` to automatically version, build and publish a new release to PyPI.
 
+Finally, it is a good idea to [configure tag protection rules](https://docs.github.com/en/enterprise-server@3.8/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-tag-protection-rules) in your repository.
+
 ## References
 - Python packaging guide: https://packaging.python.org/en/latest/tutorials/packaging-projects/
     - ...and how things are changing: https://snarky.ca/what-the-heck-is-pyproject-toml/ &mdash; in particular, note that while *pyproject.toml* seems to be the future, currently Versioneer still depends on *setup.py*.
 - Versioneer: https://github.com/python-versioneer/python-versioneer
 - GitHub Actions: https://docs.github.com/en/actions
```

### Comparing `sample-package-chanshing-0.0.0.post0/pyproject.toml` & `sample-package-chanshing-0.0.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sample-package-chanshing-0.0.0.post0/setup.py` & `sample-package-chanshing-0.0.0.post1/setup.py`

 * *Files identical despite different names*

### Comparing `sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/PKG-INFO` & `sample-package-chanshing-0.0.0.post1/src/sample_package_chanshing.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-package-chanshing
-Version: 0.0.0.post0
+Version: 0.0.0.post1
 Summary: An example Python project
 Home-page: https://github.com/chanshing/sample-package
 Download-URL: https://github.com/chanshing/sample-package
 Author: Shing Chan
 Maintainer: Shing Chan
 Maintainer-email: cshing.m@gmail.com
 License: See LICENSE file.
@@ -43,12 +43,14 @@
     $ versioneer install
     ```
     Then *commit* the changes produced by `versioneer`. See [here](https://github.com/python-versioneer/python-versioneer/blob/master/INSTALL.md) to learn more.
 1. Setup your PyPI credentials. See the section *Saving credentials on Github* of [this guide](https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/). You should use the variable names `TEST_PYPI_API_TOKEN` and `PYPI_API_TOKEN` for the TestPyPI and PyPI tokens, respectively. See *.github/workflows/release.yaml*.
 
 You are all set! It should now be possible to run `git tag vX.Y.Z && git push --tags` to automatically version, build and publish a new release to PyPI.
 
+Finally, it is a good idea to [configure tag protection rules](https://docs.github.com/en/enterprise-server@3.8/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-tag-protection-rules) in your repository.
+
 ## References
 - Python packaging guide: https://packaging.python.org/en/latest/tutorials/packaging-projects/
     - ...and how things are changing: https://snarky.ca/what-the-heck-is-pyproject-toml/ &mdash; in particular, note that while *pyproject.toml* seems to be the future, currently Versioneer still depends on *setup.py*.
 - Versioneer: https://github.com/python-versioneer/python-versioneer
 - GitHub Actions: https://docs.github.com/en/actions
```

### Comparing `sample-package-chanshing-0.0.0.post0/versioneer.py` & `sample-package-chanshing-0.0.0.post1/versioneer.py`

 * *Files identical despite different names*

