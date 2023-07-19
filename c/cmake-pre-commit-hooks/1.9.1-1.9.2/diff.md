# Comparing `tmp/cmake_pre_commit_hooks-1.9.1.tar.gz` & `tmp/cmake_pre_commit_hooks-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_pre_commit_hooks-1.9.1.tar", last modified: Sun Jun 18 10:20:02 2023, max compression
+gzip compressed data, was "cmake_pre_commit_hooks-1.9.2.tar", last modified: Wed Jul 19 05:44:08 2023, max compression
```

## Comparing `cmake_pre_commit_hooks-1.9.1.tar` & `cmake_pre_commit_hooks-1.9.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.codespell.allow
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.809317 cmake_pre_commit_hooks-1.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.809317 cmake_pre_commit_hooks-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/draft_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.809317 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_call_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_cmake.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_tidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/include_what_you_use.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1738 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/lizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/misc/license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/bad.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/good.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/tests/python/
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_argparse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_call_process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18568 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_cmake_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/clang_format_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/clang_tidy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/cppcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/cpplint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/iwyu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/lizard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/run_tests.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.798348 cmake_pre_commit_hooks-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.codespell.allow
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.786348 cmake_pre_commit_hooks-1.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.790348 cmake_pre_commit_hooks-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/workflows/draft_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-19 05:44:08.798348 cmake_pre_commit_hooks-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.794348 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_call_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_cmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/clang_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/clang_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/include_what_you_use.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1917 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/lizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.794348 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-19 05:44:08.000000 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-19 05:44:08.000000 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:44:08.000000 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-19 05:44:08.000000 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-19 05:44:08.000000 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 05:44:08.000000 cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.794348 cmake_pre_commit_hooks-1.9.2/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/misc/license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-19 05:44:08.798348 cmake_pre_commit_hooks-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.794348 cmake_pre_commit_hooks-1.9.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.798348 cmake_pre_commit_hooks-1.9.2/tests/cmake_bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_bad/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_bad/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_bad/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_bad/bad.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.798348 cmake_pre_commit_hooks-1.9.2/tests/cmake_good/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_good/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_good/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_good/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/cmake_good/good.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:44:08.798348 cmake_pre_commit_hooks-1.9.2/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/_argparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/_call_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/_cmake_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/clang_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/clang_tidy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/cppcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/cpplint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/iwyu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/python/lizard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/run_tests.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-07-19 05:43:58.000000 cmake_pre_commit_hooks-1.9.2/tests/run_tests.sh
```

### Comparing `cmake_pre_commit_hooks-1.9.1/.github/workflows/ci.yml` & `cmake_pre_commit_hooks-1.9.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/.github/workflows/codeql-analysis.yml` & `cmake_pre_commit_hooks-1.9.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/.github/workflows/draft_release.yml` & `cmake_pre_commit_hooks-1.9.2/.github/workflows/draft_release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
           create_branch: true
           file_pattern: 'CHANGELOG.md'
           commit_message: Preparing release ${{ github.event.inputs.tag }}
           commit_author: github-actions[bot] <noreply@github.com>
 
       # yamllint disable rule:line-length
       - name: Create pull request
-        uses: thomaseizinger/create-pull-request@1.3.0
+        uses: thomaseizinger/create-pull-request@1.3.1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           head: release/${{ github.event.inputs.tag }}
           base: main
           title: Release version ${{ github.event.inputs.tag }}
           reviewers: ${{ github.actor }}
```

### Comparing `cmake_pre_commit_hooks-1.9.1/.github/workflows/format.yml` & `cmake_pre_commit_hooks-1.9.2/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/.github/workflows/publish_release.yml` & `cmake_pre_commit_hooks-1.9.2/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/.github/workflows/pull_request.yml` & `cmake_pre_commit_hooks-1.9.2/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/.gitignore` & `cmake_pre_commit_hooks-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.2/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     rev: v1.1.1
     hooks:
       - id: doc8
         require_serial: false
         additional_dependencies: [tomli]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         files: .*\.(py|txt|cmake|md|rst|sh|ps1|hpp|tpp|cpp|cc)$
         args: [-I, .codespell.allow]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.5
@@ -47,24 +47,24 @@
 
   - repo: https://github.com/adrienverge/yamllint.git
     rev: v1.32.0
     hooks:
       - id: yamllint
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         language_version: python3
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.15.0
     hooks:
       - id: blacken-docs
         args: [-S, -l, '120']
         additional_dependencies: [black==22.12.0]
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.278
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-source, --show-fixes]
```

### Comparing `cmake_pre_commit_hooks-1.9.1/.pre-commit-hooks.yaml` & `cmake_pre_commit_hooks-1.9.2/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/CHANGELOG.md` & `cmake_pre_commit_hooks-1.9.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v1.9.2] - 2023-07-19
+
+### Added
+
+- Added `--no-cmake-configure` option to avoid calling CMake configure but still use a compilation database if one can
+  be found
+
+### Repository
+
+- Update `asottile/blacken-docs` hook to v1.15.0
+- Update `astral-sh/ruff-pre-commit` to v0.0.278
+- Update `charliermarsh/ruff-pre-commit` hook to v0.0.275
+- Update `codespell-project/codespell` hook to v2.2.5
+- Update `psf/black` hook to v23.7.0
+- Upgrade GitHub Action `thomaseizinger/create-pull-request` to v1.3.1
+
 ## [v1.9.1] - 2023-06-18
 
 ### Changed
 
 - Add proper support for clang-format "linter" mode (ie. `--dry-run`)
 
 ### Fixed
@@ -305,15 +321,15 @@
 
 Initial release with support for:
 
 - clang-format
 - clang-tidy
 - cppcheck
 
-[unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.1...HEAD
+[unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.2...HEAD
 [v1.0.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/20b1113bf223273cda31a14a82c9d573a342de4a...v1.0.0
 [v1.0.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.0...v1.0.1
 [v1.1.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.1...v1.1.0
 [v1.1.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.0...v1.1.1
 [v1.1.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.1...v1.1.2
 [v1.2.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.2...v1.2.0
 [v1.3.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.2.0...v1.3.0
@@ -324,7 +340,8 @@
 [v1.5.3]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.2...v1.5.3
 [v1.6.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.3...v1.6.0
 [v1.7.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.6.0...v1.7.0
 [v1.8.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.7.0...v1.8.0
 [v1.8.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...v1.8.1
 [v1.9.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...v1.9.0
 [v1.9.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.0...v1.9.1
+[v1.9.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.1...v1.9.2
```

### Comparing `cmake_pre_commit_hooks-1.9.1/LICENSE` & `cmake_pre_commit_hooks-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/PKG-INFO` & `cmake_pre_commit_hooks-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake_pre_commit_hooks
-Version: 1.9.1
+Version: 1.9.2
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -212,14 +212,15 @@
 |------------------------------|--------------------------------------------------------|--------------|
 | `--all-at-once`              | Pass all filenames to the command at once              | Since v1.4.0 |
 | `--clean`                    | Perform a clean CMake build                            | Since v1.4.0 |
 | `--cmake`                    | Specify path to CMake executable                       | Since v1.4.0 |
 | `--detect-configured-files`  | Enable cmake tracing and detection of configured files | Since v1.9.0 |
 | `--dump-toml`                | Dump the current configuration as TOML on stdout       | Since v1.9.0 |
 | `--no-automatic-discovery`   | Disable automatic build directory discovery            | Since v1.9.0 |
+| `--no-cmake-configure`       | Do not call CMake configure                            | Since v1.9.2 |
 | `--read-json-db`             | Append file list from compile database                 | Since v1.7.0 |
 | `--linux`                    | Linux-only CMake options                               | Since v1.3.0 |
 | `--mac`                      | MacOS-only CMake options                               | Since v1.3.0 |
 | `--win`                      | Windows-only CMake options                             | Since v1.3.0 |
 
 NB: by specifying `--all-at-once` the linter/formatter command will only be called once for all the files instead of
 calling the command once per file.
@@ -228,14 +229,17 @@
 to control the level of verbosity of each of the commands. To show all debug messages, set `LOGLEVEL=DEBUG` in your
 environment variables when running the hooks.
 
 NB: by specifying `--read-json-db` the hook will read the list of files from the `compile_commands.json` generated by
 CMake and will append those files to the list of files to process regardless of the list of files otherwise passed on
 the command line.
 
+NB: by specifying `--no-cmake-configure` the hook will not attempt to create a compilation database by using
+CMake. However, if one is present, then it will be used by the relevant hooks.
+
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
   rev: v1.8.0
   hooks:
```

### Comparing `cmake_pre_commit_hooks-1.9.1/README.md` & `cmake_pre_commit_hooks-1.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 |------------------------------|--------------------------------------------------------|--------------|
 | `--all-at-once`              | Pass all filenames to the command at once              | Since v1.4.0 |
 | `--clean`                    | Perform a clean CMake build                            | Since v1.4.0 |
 | `--cmake`                    | Specify path to CMake executable                       | Since v1.4.0 |
 | `--detect-configured-files`  | Enable cmake tracing and detection of configured files | Since v1.9.0 |
 | `--dump-toml`                | Dump the current configuration as TOML on stdout       | Since v1.9.0 |
 | `--no-automatic-discovery`   | Disable automatic build directory discovery            | Since v1.9.0 |
+| `--no-cmake-configure`       | Do not call CMake configure                            | Since v1.9.2 |
 | `--read-json-db`             | Append file list from compile database                 | Since v1.7.0 |
 | `--linux`                    | Linux-only CMake options                               | Since v1.3.0 |
 | `--mac`                      | MacOS-only CMake options                               | Since v1.3.0 |
 | `--win`                      | Windows-only CMake options                             | Since v1.3.0 |
 
 NB: by specifying `--all-at-once` the linter/formatter command will only be called once for all the files instead of
 calling the command once per file.
@@ -206,14 +207,17 @@
 to control the level of verbosity of each of the commands. To show all debug messages, set `LOGLEVEL=DEBUG` in your
 environment variables when running the hooks.
 
 NB: by specifying `--read-json-db` the hook will read the list of files from the `compile_commands.json` generated by
 CMake and will append those files to the list of files to process regardless of the list of files otherwise passed on
 the command line.
 
+NB: by specifying `--no-cmake-configure` the hook will not attempt to create a compilation database by using
+CMake. However, if one is present, then it will be used by the relevant hooks.
+
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
   rev: v1.8.0
   hooks:
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/__init__.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_argparse.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,17 +127,17 @@
         3. Arguments from a default TOML config file location
         4. Arguments from an existing pyproject.toml file location
     """
 
     def __init__(
         self,
         *args: Any,
-        default_config_name: str = None,
-        pyproject_section_name: str = None,
-        args_groups: list[dict] = None,
+        default_config_name: str | None = None,
+        pyproject_section_name: str | None = None,
+        args_groups: list[dict] | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Initialize an instance of ArgumentParser.
 
         Keyword Args:
             default_config_name (str): Default name for a TOML configuration file
@@ -167,15 +167,17 @@
         group.add_argument(
             '--dump-toml',
             action='store_true',
             help='Dump the current set of CLI arguments as TOML-formatted output',
         )
         self._default_args = {}
 
-    def parse_known_args(self, args: list = None, namespace: argparse.Namespace = None) -> argparse.Namespace:
+    def parse_known_args(
+        self, args: list | None = None, namespace: argparse.Namespace | None = None
+    ) -> argparse.Namespace:
         """
         Convert argument strings to objects and assign them as attributes of the namespace.
 
         Args:
             args: List of strings to parse. The default is taken from sys.argv.
             namespace: An object to take the attributes. The default is a new empty Namespace object.
 
@@ -239,15 +241,15 @@
     def _load_from_toml(  # noqa: PLR0913
         self,
         namespace: argparse.Namespace,
         path: Path,
         section: str = '',
         path_must_exist: bool = True,
         section_must_exist: bool = True,
-        overridable_keys: set = None,
+        overridable_keys: set | None = None,
     ) -> None:
         """
         Load a TOML file and set the attributes within the argparse namespace object.
 
         Args:
             namespace: Namespace to store results into
             path: Path to TOML file
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_call_process.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_call_process.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_cmake.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         """
         self.command = get_cmake_command(cmake_names)
         self.source_dir = None
         self.build_dir = None
         self.cmake_args = ['-DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=ON']
         self.cmake_trace_log = None
         self.cmake_configured_files = []
+        self.no_cmake_configure = False
 
     def add_cmake_arguments_to_parser(self, parser):
         """Add CMake options to an argparse.ArgumentParser."""
         # Create option group here to control the order
         cmake_options = parser.add_argument_group(
             title='CMake options',
             description='Options mirroring those of CMake and that will be passed onto CMake as-is.',
@@ -135,14 +136,23 @@
         )
         options.add_argument(
             '--no-automatic-discovery',
             action='store_false',
             dest='automatic_discovery',
             help='Do not attempt to automatically look for a build directory',
         )
+        options.add_argument(
+            '--no-cmake-configure',
+            action='store_true',
+            dest='no_cmake_configure',
+            help=(
+                'Do not call CMake configure to generate a compilation database '
+                '(ie. do not call CMake but still try to locate a compilation database if possible)'
+            ),
+        )
 
         # Platform-specific CMake options
         platform_specific_cmake.add_argument(
             '--unix',
             action=_argparse.OSSpecificAction,
             type=str,
             help='Unix-only (ie. Linux and MacOS) options for CMake',
@@ -207,14 +217,19 @@
         if automatic_discovery:
             for path in sorted(self.source_dir.glob('*')):
                 if path.is_dir() and (path / 'CMakeCache.txt').exists():
                     logging.info('Automatic build dir discovery resulted in: %s', str(path))
                     self.build_dir = path
                     return
 
+        if self.no_cmake_configure:
+            logging.info('Unable to locate a valid build directory. Will not be creating one')
+            self.build_dir = None
+            return
+
         if not build_dir_list:
             self.build_dir = self.source_dir / self.DEFAULT_BUILD_DIR
         else:
             self.build_dir = Path(build_dir_list[0]).resolve()
         logging.info('Unable to locate a valid build directory. Will be creating one at %s', str(self.build_dir))
 
     def setup_cmake_args(self, cmake_args):
@@ -237,20 +252,21 @@
                 - 'linux': list[str]
                 - 'mac': list[str]
                 - 'win': list[str]
         """
         self.source_dir = Path(cmake_args.source_dir).resolve()
         if cmake_args.cmake:
             self.command = [Path(cmake_args.cmake).resolve()]
+        self.no_cmake_configure = cmake_args.no_cmake_configure
 
         self.resolve_build_directory(
             build_dir_list=cmake_args.build_dir, automatic_discovery=cmake_args.automatic_discovery
         )
 
-        if cmake_args.detect_configured_files:
+        if cmake_args.detect_configured_files and self.build_dir:
             self.cmake_trace_log = self.build_dir / self.DEFAULT_TRACE_LOG
 
         keyword_args = {
             'defines': ([], '-D{}'),
             'undefines': ([], '-U{}'),
             'errors': ([], '-Werror={}'),
             'no_errors': ([], '-Wno-error={}'),
@@ -293,14 +309,18 @@
         """
         Run a CMake configure step (multi-process safe).
 
         Args:
             command (str): Name of calling command
             clean_build (bool): Clean build directory before calling CMake configure
         """
+        if self.no_cmake_configure:
+            logging.debug('Not calling CMake configure')
+            return
+
         if self.source_dir is None:
             logging.error('No source dir was for CMake! Did you call `setup_cmake_args()`?')
             sys.exit(1)
 
         cmake_configure_lock_file = Path(self.build_dir, '_cmake_configure_lock')
         cmake_configure_try_lock_file = Path(self.build_dir, '_cmake_configure_try_lock')
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_utils.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,16 @@
 from ._cmake import CMakeCommand
 
 _LOGLEVEL = os.environ.get('LOGLEVEL', 'INFO').upper()
 logging.basicConfig(level=_LOGLEVEL, format='%(levelname)-5s:cmake-pc-hooks:%(message)s')
 logging.getLogger('filelock').setLevel(logging.WARNING)
 
 
-def _read_compile_commands_json(build_dir: Path) -> list[str]:
+def _read_compile_commands_json(compile_db: Path) -> list[str]:
     """Read a JSON compile database and return the list of files contained within."""
-    compile_db = build_dir / 'compile_commands.json'
     if compile_db.exists():
         with compile_db.open(encoding='utf-8') as fd:
             data = json.load(fd)
         return [entry['file'] for entry in data]
     return []
 
 
@@ -51,14 +50,15 @@
         """Initialize a Command object."""
         super().__init__(command, look_behind, args)
         self.ddash_args = []
         self.cmake = CMakeCommand()
         self.clean_build = False
         self.all_at_once = False
         self.read_json_db = False
+        self.build_dir_list = ['.', CMakeCommand.DEFAULT_BUILD_DIR]
 
         self.history = []
 
     def parse_args(self, args):
         """
         Parse some arguments into some usable variables.
 
@@ -91,14 +91,15 @@
         hook_options.add_argument('positionals', metavar='filenames', nargs='*', help='Filenames to check')
 
         known_args, self.args = parser.parse_known_args(args[1:])
 
         self.all_at_once = known_args.all_at_once
         self.read_json_db = known_args.read_json_db
         self.clean_build = known_args.clean
+        self.build_dir_list.extend(known_args.build_dir if known_args.build_dir else [])
 
         if not known_args.build_dir and known_args.preset:
             raise RuntimeError('You *must* specify -B|--build-dir if you pass --preset as a CMake argument!')
 
         if self.setup_cmake:
             self.cmake.setup_cmake_args(known_args)
 
@@ -113,18 +114,20 @@
         # NB: if '--' may be present on the command line, the command class for that particular command needs to call
         #     handle_ddash_args() in order to properly handle the filenames in those cases.
         self.files = known_args.positionals
 
     def run(self):
         """Run the command."""
         self.cmake.configure(self.command)
-        if self.read_json_db:
-            self.files.extend(set(_read_compile_commands_json(self.cmake.build_dir)) - set(self.files))
         self.files.extend(self.cmake.cmake_configured_files)
 
+        compile_db = self._resolve_compilation_database(self.cmake.build_dir, self.build_dir_list)
+        if self.read_json_db and compile_db:
+            self.files.extend(set(_read_compile_commands_json(compile_db)) - set(self.files))
+
         if self.all_at_once:
             self.run_command(self.files)
         elif self.files:
             for filename in self.files:
                 self.run_command([filename])
         else:
             logging.error('No files to process!')
@@ -148,14 +151,28 @@
         self.stdout = self.history[-1].stdout.encode()
         self.stderr = self.history[-1].stderr.encode()
         self.returncode = self.history[-1].returncode
 
     def _parse_output(self, result):  # noqa: ARG002
         return NotImplemented
 
+    def _resolve_compilation_database(self, cmake_build_dir, build_dir_list):
+        """Locate a compilation database based on internal list of directories."""
+        if cmake_build_dir and cmake_build_dir / 'compile_commands.json':
+            return cmake_build_dir / 'compile_commands.json'
+
+        build_dir_list = [] if build_dir_list is None else [Path(path) for path in build_dir_list]
+        for build_dir in build_dir_list:
+            path = Path(build_dir, 'compile_commands.json')
+            if build_dir.exists() and path.exists():
+                logging.debug('Located valid compilation database at: %s', str(path))
+                return path
+        logging.debug('No valid compilation database located')
+        return None
+
 
 class ClangAnalyzerCmd(Command):
     """Commands that statically analyze code: clang-tidy, oclint."""
 
     def handle_ddash_args(self):
         """
         Handle arguments after a '--'.
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_format.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/clang_format.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_tidy.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/clang_tidy.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Wrapper script for clang-tidy."""
 
 import logging
 import sys
-from pathlib import Path
 
 from ._utils import ClangAnalyzerCmd
 
 
 class ClangTidyCmd(ClangAnalyzerCmd):
     """Class for the clang-tidy command."""
 
@@ -30,16 +29,17 @@
     def __init__(self, args):
         """Initialize a ClangTidyCmd object."""
         super().__init__(self.command, self.lookbehind, args)
         self.parse_args(args)
         self.edit_in_place = '-fix' in self.args or '--fix-errors' in self.args
         self.handle_ddash_args()
 
-        # Force location of compile database
-        self.add_if_missing([f'-p={Path(self.cmake.build_dir, "compile_commands.json")}'])
+        compile_db = self._resolve_compilation_database(self.cmake.build_dir, self.build_dir_list)
+        if not self.cmake.no_cmake_configure or compile_db:
+            self.add_if_missing([f'-p={compile_db}'])
 
     def _parse_output(self, result):
         """
         Parse output and check whether some errors occurred.
 
         Args:
             result (namedtuple): Result from calling a command
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cppcheck.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/cppcheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,18 @@
         self.parse_args(args)
         # quiet for stdout purposes
         self.add_if_missing(['-q'])
         # make cppcheck behave as expected for pre-commit
         self.add_if_missing(['--error-exitcode=1'])
         # Enable all of the checks
         self.add_if_missing(['--enable=all'])
-        # Force location of compile database
-        self.add_if_missing([f'--project={Path(self.cmake.build_dir, "compile_commands.json")}'])
+
+        compile_db = self._resolve_compilation_database(self.cmake.build_dir, self.build_dir_list)
+        if not self.cmake.no_cmake_configure or compile_db:
+            self.add_if_missing([f'--project={compile_db}'])
 
     def run_command(self, filenames):
         """Run the command and check for errors."""
         filter_args = [f'--file-filter=*{Path(filename).parent.name}/{Path(filename).name}' for filename in filenames]
         self.history.append(_call_process.call_process([self.command, *filter_args, *self.args, *self.ddash_args]))
         self._clinters_compat()
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cpplint.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/cpplint.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/include_what_you_use.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/include_what_you_use.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 """Wrapper script for cppcheck."""
 
 import logging
 import shutil
 import sys
-from pathlib import Path
 
 from ._utils import ClangAnalyzerCmd
 
 
 def get_iwyu_tool_command(iwyu_tool_names=None):
     """
     Get the path to the iwyu-tool.py executable on the PATH or in the virtual environment.
@@ -83,15 +82,17 @@
 
         super().__init__(self.command, self.lookbehind, args)
         self.check_installed()
         self.parse_args(args)
         self.handle_ddash_args()
 
         # Force location of compile database
-        self.add_if_missing([f'-p={Path(self.cmake.build_dir, "compile_commands.json")}'])
+        compile_db = self._resolve_compilation_database(self.cmake.build_dir, self.build_dir_list)
+        if compile_db:
+            self.add_if_missing([f'-p={compile_db}'])
 
     def _parse_output(self, result):
         """
         Parse output and check whether some errors occurred.
 
         Args:
             result (namedtuple): Result from calling a command
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/lizard.py` & `cmake_pre_commit_hooks-1.9.2/cmake_pc_hooks/lizard.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,20 @@
         """Initialize a LizardCmd object."""
         super().__init__(self.command, self.lookbehind, args)
         self.parse_args(args)
 
     def run(self):
         """Run lizard."""
         if self.read_json_db:
-            self.cmake.configure(self.command)
-            self.files.extend(set(_read_compile_commands_json(self.cmake.build_dir)) - set(self.files))
+            if not self.cmake.no_cmake_configure:
+                self.cmake.configure(self.command)
+
+            compile_db = self._resolve_compilation_database(self.cmake.build_dir, self.build_dir_list)
+            if compile_db:
+                self.files.extend(set(_read_compile_commands_json(compile_db)) - set(self.files))
 
         if self.all_at_once:
             self.run_command(self.files)
             self.exit_on_error()
         else:
             for filename in self.files:
                 self.run_command([filename])
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/PKG-INFO` & `cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-pre-commit-hooks
-Version: 1.9.1
+Version: 1.9.2
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -212,14 +212,15 @@
 |------------------------------|--------------------------------------------------------|--------------|
 | `--all-at-once`              | Pass all filenames to the command at once              | Since v1.4.0 |
 | `--clean`                    | Perform a clean CMake build                            | Since v1.4.0 |
 | `--cmake`                    | Specify path to CMake executable                       | Since v1.4.0 |
 | `--detect-configured-files`  | Enable cmake tracing and detection of configured files | Since v1.9.0 |
 | `--dump-toml`                | Dump the current configuration as TOML on stdout       | Since v1.9.0 |
 | `--no-automatic-discovery`   | Disable automatic build directory discovery            | Since v1.9.0 |
+| `--no-cmake-configure`       | Do not call CMake configure                            | Since v1.9.2 |
 | `--read-json-db`             | Append file list from compile database                 | Since v1.7.0 |
 | `--linux`                    | Linux-only CMake options                               | Since v1.3.0 |
 | `--mac`                      | MacOS-only CMake options                               | Since v1.3.0 |
 | `--win`                      | Windows-only CMake options                             | Since v1.3.0 |
 
 NB: by specifying `--all-at-once` the linter/formatter command will only be called once for all the files instead of
 calling the command once per file.
@@ -228,14 +229,17 @@
 to control the level of verbosity of each of the commands. To show all debug messages, set `LOGLEVEL=DEBUG` in your
 environment variables when running the hooks.
 
 NB: by specifying `--read-json-db` the hook will read the list of files from the `compile_commands.json` generated by
 CMake and will append those files to the list of files to process regardless of the list of files otherwise passed on
 the command line.
 
+NB: by specifying `--no-cmake-configure` the hook will not attempt to create a compilation database by using
+CMake. However, if one is present, then it will be used by the relevant hooks.
+
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
   rev: v1.8.0
   hooks:
```

### Comparing `cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt` & `cmake_pre_commit_hooks-1.9.2/cmake_pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/misc/license_header.txt` & `cmake_pre_commit_hooks-1.9.2/misc/license_header.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/pyproject.toml` & `cmake_pre_commit_hooks-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/setup.cfg` & `cmake_pre_commit_hooks-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/setup.py` & `cmake_pre_commit_hooks-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.2/tests/cmake_bad/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/cmake_good/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.2/tests/cmake_good/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/_argparse_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/_argparse_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/_call_process_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/_call_process_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/_cmake_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/_cmake_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,26 +134,28 @@
     cmake.resolve_build_directory(
         None if dir_list is None else [tmp_path / path for path in dir_list], automatic_discovery=False
     )
     assert cmake.build_dir == tmp_path / cmake.DEFAULT_BUILD_DIR if dir_list is None else dir_list[0]
 
 
 @pytest.mark.parametrize('system', ['Linux', 'Darwin', 'Windows'])
-def test_setup_cmake_args(mocker, system):  # noqa: PLR0915
+@pytest.mark.parametrize('no_cmake_configure', [False, True])
+def test_setup_cmake_args(mocker, system, no_cmake_configure):  # noqa: PLR0915, PLR0912
     original_system = platform.system()
 
     def system_stub():
         return system
 
     mocker.patch('platform.system', system_stub)
 
     cmake = CMakeCommand()
 
     args = argparse.Namespace()
     args.detect_configured_files = True
+    args.no_cmake_configure = no_cmake_configure
     if original_system == 'Windows':
         args.source_dir = 'C:/path/to/source'
         args.build_dir = ['C:/path/to/build', 'C:/path/to/other_build']
         args.cmake = Path('C:/path/to/cmake')
     else:
         args.source_dir = '/path/to/source'
         args.build_dir = ['/path/to/build', '/path/to/other_build']
@@ -175,16 +177,20 @@
     assert cmake.source_dir is None
     assert cmake.build_dir is None
     assert not cmake.cmake_trace_log
     cmake.setup_cmake_args(args)
 
     assert cmake.source_dir == Path(args.source_dir)
     assert cmake.command == [args.cmake]
-    assert cmake.build_dir is not None
-    assert cmake.cmake_trace_log == cmake.build_dir / cmake.DEFAULT_TRACE_LOG
+    if no_cmake_configure:
+        assert cmake.build_dir is None
+        assert cmake.cmake_trace_log is None
+    else:
+        assert cmake.build_dir is not None
+        assert cmake.cmake_trace_log == cmake.build_dir / cmake.DEFAULT_TRACE_LOG
 
     assert '-GNinja' in cmake.cmake_args
     assert '-A64' in cmake.cmake_args
     assert '-Tclang-toolset' in cmake.cmake_args
 
     assert '-Wdev' in cmake.cmake_args
     assert '-Wno_dev' in cmake.cmake_args
@@ -212,15 +218,16 @@
         for win in args.win:
             assert any(win in arg for arg in cmake.cmake_args)
 
 
 @pytest.mark.parametrize('detect_configured_files', [False, True], ids=['no_trace', 'w_trace'])
 @pytest.mark.parametrize('returncode', [0, 1])
 @pytest.mark.parametrize('clean_build', [False, True])
-def test_configure_cmake(mocker, tmp_path, clean_build, returncode, detect_configured_files):
+@pytest.mark.parametrize('no_cmake_configure', [False, True])
+def test_configure_cmake(mocker, tmp_path, clean_build, returncode, no_cmake_configure, detect_configured_files):
     sys_exit = mocker.patch('sys.exit')
     FileLock = mocker.MagicMock(filelock.FileLock)  # noqa: N806
     mocker.patch(filelock_module_name, FileLock)
     InterProcessReaderWriterLock = mocker.MagicMock(fasteners.InterProcessReaderWriterLock)  # noqa: N806
     mocker.patch(interprocess_rw_lock_module_name, InterProcessReaderWriterLock)
     _configure = mocker.Mock(return_value=returncode)
     mocker.patch(internal_cmake_configure_name, _configure)
@@ -230,22 +237,29 @@
 
     build_dir = tmp_path / 'build'
     build_dir.mkdir(parents=True, exist_ok=True)
 
     cmake = CMakeCommand()
     cmake.source_dir = tmp_path
     cmake.build_dir = build_dir
+    cmake.no_cmake_configure = no_cmake_configure
     cmake.cmake_args.append('-DCMAKE_CXX_COMPILER=g++')
     if detect_configured_files:
         cmake.cmake_trace_log = tmp_path / 'log.json'
 
     cmake.configure(command='test', clean_build=clean_build)
 
     # ----------------------------------
 
+    if no_cmake_configure:
+        FileLock.assert_not_called()
+        InterProcessReaderWriterLock.assert_not_called()
+        _configure.assert_not_called()
+        return
+
     FileLock.assert_called_once_with(build_dir / '_cmake_configure_try_lock')
     InterProcessReaderWriterLock.assert_called_once_with(build_dir / '_cmake_configure_lock')
     _configure.assert_called_once_with(
         lock_files=(InterProcessReaderWriterLock.call_args[0][0], FileLock.call_args[0][0]), clean_build=clean_build
     )
 
     if detect_configured_files:
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/_test_utils.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/_test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,47 +26,49 @@
 
 def run_command_default_assertions(
     read_json_db,
     json_db_file_list,
     file_list,
     command,
     all_at_once,
+    no_cmake_configure,
+    create_compilation_db,
     configure,
     call_process,
     returncode,
     sys_exit,
     exit_success=None,
     do_configure_test=True,
     detect_configured_files=False,
     **kwargs,  # noqa: ARG001
 ):
     assert set(command.files) == {str(fname) for fname in file_list}
 
     with contextlib.suppress(ExitError):
         command.run()
 
-    if do_configure_test:
+    if do_configure_test and not no_cmake_configure:
         configure.assert_called_once_with(command.command)
 
     if exit_success is None:
         exit_success = returncode == 0
 
     n_files = len(file_list)
 
-    if read_json_db:
+    if read_json_db and create_compilation_db:
         n_files += len(json_db_file_list)
-    if detect_configured_files:
+    if detect_configured_files and not no_cmake_configure:
         n_files += len(command.cmake.cmake_configured_files)
 
     assert len(command.files) == n_files
 
     for fname in file_list:
         assert str(fname) in command.files
 
-    if read_json_db:
+    if read_json_db and create_compilation_db:
         for fname in json_db_file_list:
             assert str(fname) in command.files
 
     for fname in command.cmake.cmake_configured_files:
         assert str(fname) in command.files
 
     if all_at_once:
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/_utils_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from cmake_pc_hooks import _utils
 from cmake_pc_hooks._cmake import CMakeCommand
 
 # ==============================================================================
 
 
 def test_read_compile_commands_no_file(tmp_path):
-    assert not _utils._read_compile_commands_json(tmp_path)
+    assert not _utils._read_compile_commands_json(tmp_path / 'compile_commands.json')
 
 
 def test_read_compile_commands(compile_commands):
     path, file_list = compile_commands
-    files = _utils._read_compile_commands_json(path.parent)
+    files = _utils._read_compile_commands_json(path)
     assert files == [str(fname) for fname in file_list]
 
 
 # ==============================================================================
 
 
 @pytest.mark.parametrize('look_behind', [False, True])
@@ -115,15 +115,15 @@
 
     command_name = 'test-exec'
     args = [f'{command_name}', f'-B{path.parent}', *setup_command.cmd_args]
 
     command = _utils.Command(command_name, look_behind=False, args=args)
     command.parse_args(args)
 
-    if detect_configured_files:
+    if detect_configured_files and not setup_command.no_cmake_configure:
         command.cmake.cmake_configured_files = ['configured.cpp']
 
     run_command_default_assertions(
         command=command,
         detect_configured_files=detect_configured_files,
         exit_success=not parsing_failed,
         **setup_command._asdict(),
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/clang_format_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/clang_format_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/clang_tidy_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/clang_tidy_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 
     # ----------------------------------
 
     command_name = 'clang-tidy'
     args = [f'{command_name}', f'-B{path.parent}', *setup_command.cmd_args]
     command = clang_tidy.ClangTidyCmd(args=args)
 
-    assert f'-p={path}' in command.args
+    if not setup_command.no_cmake_configure:
+        assert f'-p={path}' in command.args
 
     run_command_default_assertions(
         command=command,
         exit_success=returncode == 0 and (error_msg is None or not stdout),
         **setup_command._asdict(),
     )
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/conftest.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,28 +39,38 @@
 
 # ==============================================================================
 
 
 _setup_commands_args = itertools.product(
     (False, True),  # all_at_once
     (False, True),  # read_json_db
+    (False, True),  # no_cmake_configure
+    (False, True),  # create_compilation_db
     (0, 1),  # returncode
 )
 
 
 def _setup_command_ids(param):
-    all_at_once, read_json_db, returncode = param
-    return f'{"all_files" if all_at_once else "single_file"}-{"w_db" if read_json_db else "no_db"}-ret_{returncode}'
+    all_at_once, read_json_db, no_cmake_configure, create_compilation_db, returncode = param
+    return (
+        f'{"all_files" if all_at_once else "single_file"}'
+        f'-{"w_read_db" if read_json_db else "no_read_db"}'
+        f'-{"no_conf" if no_cmake_configure else "cmake_conf"}'
+        f'-{"create_db" if create_compilation_db else "no_create_db"}'
+        f'-ret_{returncode}'
+    )
 
 
 SetupCommandData = namedtuple(
     'SetupCommandData',
     [
         'all_at_once',
         'read_json_db',
+        'no_cmake_configure',
+        'create_compilation_db',
         'compile_db_path',
         'json_db_file_list',
         'returncode',
         'file_list',
         'cmd_args',
         'configure',
         'sys_exit',
@@ -68,37 +78,45 @@
     ],
 )
 
 
 @pytest.fixture(params=_setup_commands_args, ids=_setup_command_ids)
 def setup_command(mocker, tmp_path, compile_commands, request):
     mocker.patch('hooks.utils.Command.check_installed', return_value=True)
-    all_at_once, read_json_db, returncode = request.param
+    all_at_once, read_json_db, no_cmake_configure, create_compilation_db, returncode = request.param
 
     configure = mocker.patch('cmake_pc_hooks._cmake.CMakeCommand.configure', return_value=0)
     sys_exit = mocker.patch('sys.exit', side_effect=ExitError)
     call_process = mocker.patch(
         'cmake_pc_hooks._call_process.call_process',
         return_value=mocker.Mock(stdout='', stderr='', returncode=returncode),
     )
 
+    if not create_compilation_db:
+        compile_commands[0].unlink()
+
     file_list = [tmp_path / 'file1.cpp', tmp_path / 'file2.cpp']
     for file in file_list:
         file.write_text('')
 
     args = []
     if read_json_db:
         args.append('--read-json-db')
 
     if all_at_once:
         args.append('--all-at-once')
 
+    if no_cmake_configure:
+        args.append('--no-cmake-configure')
+
     return SetupCommandData(
         all_at_once=all_at_once,
         read_json_db=read_json_db,
+        no_cmake_configure=no_cmake_configure,
+        create_compilation_db=create_compilation_db,
         compile_db_path=compile_commands[0],
         json_db_file_list=compile_commands[1],
         returncode=returncode,
         file_list=file_list,
         cmd_args=[*args, *[str(fname) for fname in file_list]],
         configure=configure,
         sys_exit=sys_exit,
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/cppcheck_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/cppcheck_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     command_name = 'cppcheck'
     args = [f'{command_name}', f'-B{path.parent}', *setup_command.cmd_args]
 
     command = cppcheck.CppcheckCmd(args=args)
     assert '-q' in command.args
     assert '--error-exitcode=1' in command.args
     assert '--enable=all' in command.args
-    assert f'--project={path}' in command.args
+    if not setup_command.no_cmake_configure:
+        assert f'--project={path}' in command.args
 
     run_command_default_assertions(
         command=command,
         **setup_command._asdict(),
     )
 
     assert not any(
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/cpplint_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/cpplint_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/iwyu_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/iwyu_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         ),
     )
 
     command_name = 'iwyu-tool'
     args = [f'{command_name}', f'-B{path.parent}', *setup_command.cmd_args]
 
     command = include_what_you_use.IWYUToolCmd(args=args)
-    assert f'-p={path}' in command.args
+    if not setup_command.no_cmake_configure:
+        assert f'-p={path}' in command.args
 
     run_command_default_assertions(
         command=command,
         **setup_command._asdict(),
     )
```

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/python/lizard_test.py` & `cmake_pre_commit_hooks-1.9.2/tests/python/lizard_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/run_tests.ps1` & `cmake_pre_commit_hooks-1.9.2/tests/run_tests.ps1`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.1/tests/run_tests.sh` & `cmake_pre_commit_hooks-1.9.2/tests/run_tests.sh`

 * *Files identical despite different names*

