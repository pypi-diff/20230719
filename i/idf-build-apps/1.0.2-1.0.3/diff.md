# Comparing `tmp/idf_build_apps-1.0.2.tar.gz` & `tmp/idf_build_apps-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.2.tar` & `idf_build_apps-1.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      351 2023-07-05 01:10:03.945090 idf_build_apps-1.0.2/.editorconfig
--rw-r--r--   0        0        0      123 2023-07-05 01:10:03.945090 idf_build_apps-1.0.2/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-07-05 01:10:03.945090 idf_build_apps-1.0.2/.gitattributes
--rw-r--r--   0        0        0      513 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      253 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3870 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.gitignore
--rw-r--r--   0        0        0     1077 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.readthedocs.yml
--rw-r--r--   0        0        0     5408 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1882 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/LICENSE
--rw-r--r--   0        0        0     3843 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/README.md
--rw-r--r--   0        0        0       33 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/config_file.md
--rw-r--r--   0        0        0    10473 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/index.rst
--rw-r--r--   0        0        0     5894 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    27051 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/config.py
--rw-r--r--   0        0        0     2182 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6328 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/log.py
--rw-r--r--   0        0        0    30607 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6368 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5956 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     7081 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/license_header.txt
--rw-r--r--   0        0        0     2060 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/conftest.py
--rw-r--r--   0        0        0     3347 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_build.py
--rw-r--r--   0        0        0    16908 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_finder.py
--rw-r--r--   0        0        0     1568 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_manifest.py
--rw-r--r--   0        0        0     3710 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_utils.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.2/setup.py
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.editorconfig
+-rw-r--r--   0        0        0      123 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.gitattributes
+-rw-r--r--   0        0        0      513 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      253 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3870 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1077 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.readthedocs.yml
+-rw-r--r--   0        0        0     5583 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1882 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3843 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/README.md
+-rw-r--r--   0        0        0       33 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/config_file.md
+-rw-r--r--   0        0        0    10473 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0     5894 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/manifest.md
+-rw-r--r--   0        0        0      481 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    27235 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2182 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6328 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30514 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6368 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5956 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7081 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/license_header.txt
+-rw-r--r--   0        0        0     2060 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_build.py
+-rw-r--r--   0        0        0    17534 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_finder.py
+-rw-r--r--   0        0        0     1568 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_manifest.py
+-rw-r--r--   0        0        0     3710 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.3/setup.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.3/PKG-INFO
```

### Comparing `idf_build_apps-1.0.2/.github/dependabot.yml` & `idf_build_apps-1.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.3/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.3/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.3/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.3/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.3/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.gitignore` & `idf_build_apps-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/.pre-commit-config.yaml` & `idf_build_apps-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/CHANGELOG.md` & `idf_build_apps-1.0.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## v1.0.3 (2023-07-19)
+
+### Fix
+
+- correct final reports with skipped apps and failed built apps
+- skip while collecting only when both depend components and files unmatched
+
 ## v1.0.2 (2023-07-05)
 
 ### Feat
 
 - support placeholder "@v"
 - Support keyword `IDF_VERSION` in the if statement
```

### Comparing `idf_build_apps-1.0.2/CONTRIBUTING.md` & `idf_build_apps-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/LICENSE` & `idf_build_apps-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/README.md` & `idf_build_apps-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/Makefile` & `idf_build_apps-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.3/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.3/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/conf.py` & `idf_build_apps-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/config_file.md` & `idf_build_apps-1.0.3/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/find_build.md` & `idf_build_apps-1.0.3/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/docs/manifest.md` & `idf_build_apps-1.0.3/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/app.py` & `idf_build_apps-1.0.3/idf_build_apps/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,16 +541,18 @@
                 _modified_files = BuildOrNot.YES
             # if not defined dependency, we left it unknown and decide with idf.py reconfigure
             elif self.depends_filepatterns:
                 _modified_files = BuildOrNot.NO
 
         if _modified_components == BuildOrNot.YES or _modified_files == BuildOrNot.YES:
             self.should_build = BuildOrNot.YES
-        elif _modified_components == BuildOrNot.NO or _modified_files == BuildOrNot.NO:
+        elif _modified_components == BuildOrNot.NO:  # _modified_files == BuildOrNot.NO or UNKNOWN
             self.should_build = BuildOrNot.NO
+        # elif modified_components == BuildOrNot.UNKNOWN and modified_files == BuildOrNot.No or UNKNOWN:
+        #     we left it unknown and decide with idf.py reconfigure
 
         self._checked_should_build = True
 
 
 class CMakeApp(App):
     BUILD_SYSTEM = 'cmake'
```

### Comparing `idf_build_apps-1.0.2/idf_build_apps/config.py` & `idf_build_apps-1.0.3/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/constants.py` & `idf_build_apps-1.0.3/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/finder.py` & `idf_build_apps-1.0.3/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/log.py` & `idf_build_apps-1.0.3/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/main.py` & `idf_build_apps-1.0.3/idf_build_apps/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,14 @@
 
     for f in collect_files:
         if os.path.isfile(f):
             os.remove(f)
             LOGGER.info('=> Remove existing collect file %s', f)
         Path(f).touch()
 
-    actual_built_apps = []
     built_apps = []  # type: list[App]
     skipped_apps = []  # type: list[App]
     for i, app in enumerate(apps):
         index = i + 1  # we use 1-based
         if index < start or index > stop:
             continue
 
@@ -335,33 +334,30 @@
                 manifest_rootpath=manifest_rootpath,
                 modified_components=modified_components,
                 modified_files=modified_files,
                 check_app_dependencies=_check_app_dependency(
                     manifest_rootpath, modified_components, modified_files, ignore_app_dependencies_filepatterns
                 ),
             )
+            if is_built:
+                built_apps.append(app)
+            else:
+                skipped_apps.append(app)
         except BuildError as e:
             LOGGER.error(str(e))
+            failed_apps.append(app)
             if keep_going:
-                failed_apps.append(app)
                 exit_code = 1
             else:
                 if modified_components is not None:
-                    return 1, actual_built_apps
+                    return 1, built_apps
                 else:
                     return 1
         finally:
             if is_built:
-                built_apps.append(app)
-            else:
-                skipped_apps.append(app)
-
-            if is_built:
-                actual_built_apps.append(app)
-
                 if app.collect_app_info:
                     with open(app.collect_app_info, 'a') as fw:
                         fw.write(app.to_json() + '\n')
                     LOGGER.info('=> Recorded app info in %s', app.collect_app_info)
 
                 if app.collect_size_info and app.size_json_path:
                     try:
@@ -412,15 +408,15 @@
 
     if failed_apps:
         LOGGER.error('Build failed for the following apps:')
         for app in failed_apps:
             LOGGER.error('  %s', app)
 
     if modified_components is not None:
-        return exit_code, actual_built_apps
+        return exit_code, built_apps
     else:
         return exit_code
 
 
 class IdfBuildAppsCliFormatter(argparse.HelpFormatter):
     LINE_SEP = '$LINE_SEP$'
```

### Comparing `idf_build_apps-1.0.2/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.3/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.3/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.3/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/idf_build_apps/utils.py` & `idf_build_apps-1.0.3/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/pyproject.toml` & `idf_build_apps-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 changelog = "https://github.com/espressif/idf-build-apps/blob/master/CHANGELOG.md"
 
 [project.scripts]
 idf-build-apps = "idf_build_apps:main.main"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.2"
+version = "1.0.3"
 tag_format = "v$version"
 version_files = [
     "idf_build_apps/__init__.py",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-s --log-cli-level DEBUG"
```

### Comparing `idf_build_apps-1.0.2/tests/conftest.py` & `idf_build_apps-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/tests/test_build.py` & `idf_build_apps-1.0.3/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/tests/test_finder.py` & `idf_build_apps-1.0.3/tests/test_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,27 +182,29 @@
             assert filtered_apps == apps
         else:
             assert not filtered_apps
 
     @pytest.mark.parametrize(
         'modified_components, modified_files, could_find_apps',
         [
-            ([], str(IDF_PATH / 'examples' / 'README.md'), False),
-            (None, [str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], False),
+            ([], str(IDF_PATH / 'examples' / 'README.md'), (True, False)),
+            (None, [str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], (True, True)),
             (
                 [],
                 [
                     str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
                     str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
                 ],
-                True,
+                (True, True),
             ),
         ],
     )
-    def test_with_depends_filepatterns(self, tmp_path, modified_components, modified_files, could_find_apps):
+    def test_with_depends_components_and_filepatterns(
+        self, tmp_path, modified_components, modified_files, could_find_apps
+    ):
         test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
         apps = find_apps(test_dir, 'esp32', recursive=True)
         assert apps
 
         yaml_file = tmp_path / 'test.yml'
         yaml_file.write_text(
             f'''
@@ -214,20 +216,44 @@
             encoding='utf8',
         )
 
         filtered_apps = find_apps(
             test_dir,
             'esp32',
             recursive=True,
+            manifest_files=yaml_file,
+            modified_components=modified_components,
+        )
+        if could_find_apps[0]:
+            assert filtered_apps == apps
+        else:
+            assert not filtered_apps
+
+        yaml_file.write_text(
+            f'''
+{test_dir}:
+    depends_components:
+        - foo
+    depends_filepatterns:
+        - examples/get-started/hello_world/**
+        - examples/foo/**
+''',
+            encoding='utf8',
+        )
+
+        filtered_apps = find_apps(
+            test_dir,
+            'esp32',
+            recursive=True,
             manifest_rootpath=str(IDF_PATH),
             manifest_files=yaml_file,
             modified_components=modified_components,
             modified_files=modified_files,
         )
-        if could_find_apps:
+        if could_find_apps[1]:
             assert filtered_apps == apps
         else:
             assert not filtered_apps
 
     @pytest.mark.parametrize(
         'modified_files, could_find_apps',
         [
```

### Comparing `idf_build_apps-1.0.2/tests/test_manifest.py` & `idf_build_apps-1.0.3/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/tests/test_utils.py` & `idf_build_apps-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.2/setup.py` & `idf_build_apps-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.2',
+      version='1.0.3',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.2/PKG-INFO` & `idf_build_apps-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

