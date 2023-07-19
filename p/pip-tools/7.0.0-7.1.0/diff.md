# Comparing `tmp/pip-tools-7.0.0.tar.gz` & `tmp/pip-tools-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-tools-7.0.0.tar", last modified: Fri Jul 14 19:40:40 2023, max compression
+gzip compressed data, was "pip-tools-7.1.0.tar", last modified: Wed Jul 19 05:17:55 2023, max compression
```

## Comparing `pip-tools-7.0.0.tar` & `pip-tools-7.1.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.586777 pip-tools-7.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.586777 pip-tools-7.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.586777 pip-tools-7.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/reusable-qa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42979 2023-07-14 19:40:12.000000 pip-tools-7.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-14 19:40:12.000000 pip-tools-7.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-14 19:40:12.000000 pip-tools-7.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-14 19:40:12.000000 pip-tools-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-14 19:40:40.610777 pip-tools-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-14 19:40:12.000000 pip-tools-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 19:40:12.000000 pip-tools-7.0.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/django.in
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/flask.in
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/hypothesis.in
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/protection.in
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/sentry.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-14 19:40:12.000000 pip-tools-7.0.0/img/pip-tools-overview.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/_compat/pip_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22000 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/scripts/compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9713 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/scripts/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 19:40:12.000000 pip-tools-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:40:40.610777 pip-tools-7.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.602777 pip-tools-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    92853 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_cli_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_cli_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.602777 pip-tools-7.0.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/fake-editables.json
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/fake-index.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.606778 pip-tools-7.0.0/tests/test_data/minimal_wheels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.582777 pip-tools-7.0.0/tests/test_data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.606778 pip-tools-7.0.0/tests/test_data/packages/fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.606778 pip-tools-7.0.0/tests/test_data/packages/small_fake_a/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_a/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.582777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_subdir/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_unpinned_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_fake_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_minimal_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_repository_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_repository_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_top_level_editable.py
--rw-r--r--   0 runner    (1001) docker     (123)    24294 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.702570 pip-tools-7.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.702570 pip-tools-7.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.702570 pip-tools-7.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.github/workflows/reusable-qa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-19 05:17:37.000000 pip-tools-7.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    43302 2023-07-19 05:17:37.000000 pip-tools-7.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-19 05:17:37.000000 pip-tools-7.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-19 05:17:37.000000 pip-tools-7.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-19 05:17:37.000000 pip-tools-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-19 05:17:55.726570 pip-tools-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-19 05:17:37.000000 pip-tools-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 05:17:37.000000 pip-tools-7.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.706570 pip-tools-7.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-19 05:17:37.000000 pip-tools-7.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.706570 pip-tools-7.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/django.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/flask.in
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/hypothesis.in
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/protection.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 05:17:37.000000 pip-tools-7.1.0/examples/sentry.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.706570 pip-tools-7.1.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-19 05:17:37.000000 pip-tools-7.1.0/img/pip-tools-overview.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.710570 pip-tools-7.1.0/pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 05:17:55.000000 pip-tools-7.1.0/pip_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.710570 pip-tools-7.1.0/piptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.714570 pip-tools-7.1.0/piptools/_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/_compat/pip_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.714570 pip-tools-7.1.0/piptools/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/repositories/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.714570 pip-tools-7.1.0/piptools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22000 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/scripts/compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9713 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/scripts/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23984 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-19 05:17:37.000000 pip-tools-7.1.0/piptools/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-19 05:17:37.000000 pip-tools-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:17:55.726570 pip-tools-7.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.718571 pip-tools-7.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13145 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93693 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_cli_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_cli_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.722571 pip-tools-7.1.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/fake-editables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/fake-index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/minimal_wheels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.694570 pip-tools-7.1.0/tests/test_data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_a/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.694570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_subdir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:55.726570 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_unpinned_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_fake_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_minimal_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_repository_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_repository_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_top_level_editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-19 05:17:37.000000 pip-tools-7.1.0/tox.ini
```

### Comparing `pip-tools-7.0.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pip-tools-7.1.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.github/PULL_REQUEST_TEMPLATE.md` & `pip-tools-7.1.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.github/release-drafter.yml` & `pip-tools-7.1.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.github/workflows/ci.yml` & `pip-tools-7.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.github/workflows/release-drafter.yml` & `pip-tools-7.1.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.github/workflows/release.yml` & `pip-tools-7.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.github/workflows/reusable-qa.yml` & `pip-tools-7.1.0/.github/workflows/reusable-qa.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/.pre-commit-config.yaml` & `pip-tools-7.1.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
       - id: black
         args: [--target-version=py38]
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-pytest-style
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         # Avoid error: Duplicate module named 'setup'
         # https://github.com/python/mypy/issues/4008
         # Keep exclude in sync with mypy own excludes
         exclude: ^tests/test_data/
         additional_dependencies:
@@ -36,13 +36,13 @@
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args: [--ini, .bandit]
         exclude: ^tests/
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v3.0.0
     hooks:
       - id: prettier
         additional_dependencies:
           - "prettier"
           - "prettier-plugin-toml"
```

### Comparing `pip-tools-7.0.0/CHANGELOG.md` & `pip-tools-7.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 7.1.0 (2023-07-18)
+
+Features:
+
+- Validate parsed config against CLI options
+  ([#1910](https://github.com/jazzband/pip-tools/pull/1910)). Thanks @atugushev
+
+Bug Fixes:
+
+- Fix a bug where pip-sync would unexpectedly uninstall some packages
+  ([#1919](https://github.com/jazzband/pip-tools/pull/1919)). Thanks @atugushev
+
 ## 7.0.0 (2023-07-14)
 
 Backwards Incompatible Changes:
 
 - Default to `--resolver=backtracking`
   ([#1897](https://github.com/jazzband/pip-tools/pull/1897)). Thanks @atugushev
 - Drop support for Python 3.7
```

### Comparing `pip-tools-7.0.0/CODE_OF_CONDUCT.md` & `pip-tools-7.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/CONTRIBUTING.md` & `pip-tools-7.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/LICENSE` & `pip-tools-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/PKG-INFO` & `pip-tools-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 7.0.0
+Version: 7.1.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Author-email: Vincent Driessen <me@nvie.com>
 License: BSD
 Project-URL: homepage, https://github.com/jazzband/pip-tools/
 Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jazzband/pip-tools
 Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
@@ -448,37 +448,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
```

### Comparing `pip-tools-7.0.0/README.md` & `pip-tools-7.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -411,37 +411,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
```

### Comparing `pip-tools-7.0.0/img/pip-tools-overview.svg` & `pip-tools-7.1.0/img/pip-tools-overview.svg`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/pip_tools.egg-info/PKG-INFO` & `pip-tools-7.1.0/pip_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 7.0.0
+Version: 7.1.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Author-email: Vincent Driessen <me@nvie.com>
 License: BSD
 Project-URL: homepage, https://github.com/jazzband/pip-tools/
 Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jazzband/pip-tools
 Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
@@ -448,37 +448,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.0.0
+    rev: 7.1.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
```

### Comparing `pip-tools-7.0.0/pip_tools.egg-info/SOURCES.txt` & `pip-tools-7.1.0/pip_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/_compat/pip_compat.py` & `pip-tools-7.1.0/piptools/_compat/pip_compat.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/cache.py` & `pip-tools-7.1.0/piptools/cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/exceptions.py` & `pip-tools-7.1.0/piptools/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/logging.py` & `pip-tools-7.1.0/piptools/logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/repositories/base.py` & `pip-tools-7.1.0/piptools/repositories/base.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/repositories/local.py` & `pip-tools-7.1.0/piptools/repositories/local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/repositories/pypi.py` & `pip-tools-7.1.0/piptools/repositories/pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/resolver.py` & `pip-tools-7.1.0/piptools/resolver.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/scripts/compile.py` & `pip-tools-7.1.0/piptools/scripts/compile.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/scripts/sync.py` & `pip-tools-7.1.0/piptools/scripts/sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/subprocess_utils.py` & `pip-tools-7.1.0/piptools/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/piptools/sync.py` & `pip-tools-7.1.0/piptools/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pip._internal.models.direct_url import ArchiveInfo
 from pip._internal.req import InstallRequirement
 from pip._internal.utils.compat import stdlib_pkgs
 from pip._internal.utils.direct_url_helpers import (
     direct_url_as_pep440_direct_reference,
     direct_url_from_link,
 )
+from pip._vendor.packaging.utils import canonicalize_name
 
 from ._compat import Distribution, get_dev_pkgs
 from .exceptions import IncompatibleRequirements
 from .logging import log
 from .utils import (
     flat_map,
     format_requirement,
@@ -55,15 +56,15 @@
 
     if root_key in installed_keys:
         dep = installed_keys[root_key]
         queue.append(dep)
 
     while queue:
         v = queue.popleft()
-        key = v.key
+        key = str(canonicalize_name(v.key))
         if key in dependencies:
             continue
 
         dependencies.add(key)
 
         for dep_specifier in v.requires:
             dep_name = key_from_req(dep_specifier)
@@ -81,15 +82,15 @@
     Returns a collection of package names to ignore when performing pip-sync,
     based on the currently installed environment.  For example, when pip-tools
     is installed in the local environment, it should be ignored, including all
     of its dependencies (e.g. click).  When pip-tools is not installed
     locally, click should also be installed/uninstalled depending on the given
     requirements.
     """
-    installed_keys = {r.key: r for r in installed}
+    installed_keys = {str(canonicalize_name(r.key)): r for r in installed}
     return list(
         flat_map(lambda req: dependency_tree(installed_keys, req), PACKAGES_TO_IGNORE)
     )
 
 
 def merge(
     requirements: Iterable[InstallRequirement], ignore_conflicts: bool
@@ -139,15 +140,15 @@
         # TODO: Also support VCS and editable installs.
         return str(ireq.link)
     return key_from_ireq(ireq)
 
 
 def diff_key_from_req(req: Distribution) -> str:
     """Get a unique key for the requirement."""
-    key = req.key
+    key = str(canonicalize_name(req.key))
     if (
         req.direct_url
         and isinstance(req.direct_url.info, ArchiveInfo)
         and req.direct_url.info.hash
     ):
         key = direct_url_as_pep440_direct_reference(req.direct_url, key)
     # TODO: Also support VCS and editable installs.
```

### Comparing `pip-tools-7.0.0/piptools/utils.py` & `pip-tools-7.1.0/piptools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import collections
 import copy
+import difflib
 import itertools
 import json
 import os
 import re
 import shlex
 import sys
 from pathlib import Path
@@ -173,15 +174,15 @@
     Generic formatter for pretty printing the specifier part of
     InstallRequirements to the terminal.
     """
     # TODO: Ideally, this is carried over to the pip library itself
     specs = ireq.specifier if ireq.req is not None else SpecifierSet()
     # FIXME: remove ignore type marker once the following issue get fixed
     #        https://github.com/python/mypy/issues/9656
-    specs = sorted(specs, key=lambda x: x.version)  # type: ignore
+    specs = sorted(specs, key=lambda x: x.version)
     return ",".join(str(s) for s in specs) or "<any>"
 
 
 def is_pinned_requirement(ireq: InstallRequirement) -> bool:
     """
     Returns whether an InstallRequirement is a "pinned" requirement.
 
@@ -557,14 +558,15 @@
         if config_file is None:
             return None
     else:
         config_file = Path(value)
 
     config = parse_config_file(config_file)
     if config:
+        _validate_config(ctx, config)
         _assign_config_to_cli_context(ctx, config)
 
     return config_file
 
 
 def _assign_config_to_cli_context(
     click_context: click.Context,
@@ -572,14 +574,53 @@
 ) -> None:
     if click_context.default_map is None:
         click_context.default_map = {}
 
     click_context.default_map.update(cli_config_mapping)
 
 
+def _validate_config(
+    click_context: click.Context,
+    config: dict[str, Any],
+) -> None:
+    """
+    Validate parsed config against click command params.
+
+    :raises click.NoSuchOption: if config contains unknown keys.
+    :raises click.BadOptionUsage: if config contains invalid values.
+    """
+    cli_params = {
+        param.name: param
+        for param in click_context.command.params
+        if param.name is not None
+    }
+
+    for key, value in config.items():
+        # Validate unknown keys
+        if key not in cli_params:
+            possibilities = difflib.get_close_matches(key, cli_params.keys())
+            raise click.NoSuchOption(
+                option_name=key,
+                message=f"No such config key {key!r}.",
+                possibilities=possibilities,
+                ctx=click_context,
+            )
+
+        # Validate invalid values
+        param = cli_params[key]
+        try:
+            param.type.convert(value=value, param=param, ctx=click_context)
+        except Exception as e:
+            raise click.BadOptionUsage(
+                option_name=key,
+                message=f"Invalid value for config key {key!r}: {value!r}.",
+                ctx=click_context,
+            ) from e
+
+
 def select_config_file(src_files: tuple[str, ...]) -> Path | None:
     """
     Returns the config file to use for defaults given ``src_files`` provided.
     """
     # NOTE: If no src_files were specified, consider the current directory the
     # NOTE: only config file lookup candidate. This usually happens when a
     # NOTE: pip-tools invocation gets its incoming requirements from standard
@@ -610,14 +651,15 @@
 
 # Some of the defined click options have different `dest` values than the defaults
 NON_STANDARD_OPTION_DEST_MAP: dict[str, str] = {
     "extra": "extras",
     "upgrade_package": "upgrade_packages",
     "resolver": "resolver_name",
     "user": "user_only",
+    "pip_args": "pip_args_str",
 }
 
 
 def get_click_dest_for_option(option_name: str) -> str:
     """
     Returns the click ``dest`` value for the given option name.
     """
```

### Comparing `pip-tools-7.0.0/piptools/writer.py` & `pip-tools-7.1.0/piptools/writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/pyproject.toml` & `pip-tools-7.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -106,7 +106,8 @@
 markers = ["network: mark tests that require internet access"]
 
 [tool.setuptools.packages.find]
 # needed only because we did not adopt src layout yet
 include = ["piptools*"]
 
 [tool.setuptools_scm]
+local_scheme = "dirty-tag"
```

### Comparing `pip-tools-7.0.0/tests/conftest.py` & `pip-tools-7.1.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
 @pytest.fixture
 def fake_dist():
     def _fake_dist(line, deps=None):
         if deps is None:
             deps = []
         req = Requirement.parse(line)
-        key = req.key
+        key = req.name
         if "==" in line:
             version = line.split("==")[1]
         else:
             version = "0+unknown"
         requires = [Requirement.parse(d) for d in deps]
         direct_url = None
         if req.url:
```

### Comparing `pip-tools-7.0.0/tests/test_cache.py` & `pip-tools-7.1.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_cli_compile.py` & `pip-tools-7.1.0/tests/test_cli_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -2985,7 +2985,35 @@
 
     out = runner.invoke(
         cli, [req_in.as_posix(), "--no-config", "--config", config_file.as_posix()]
     )
 
     assert out.exit_code == 0
     assert "Dry-run, so nothing updated" not in out.stderr
+
+
+def test_raise_error_on_unknown_config_option(
+    pip_conf, runner, tmp_path, make_config_file
+):
+    config_file = make_config_file("unknown-option", True)
+
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
+
+    assert out.exit_code == 2
+    assert "No such config key 'unknown_option'" in out.stderr
+
+
+def test_raise_error_on_invalid_config_option(
+    pip_conf, runner, tmp_path, make_config_file
+):
+    config_file = make_config_file("dry-run", ["invalid", "value"])
+
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
+
+    assert out.exit_code == 2
+    assert "Invalid value for config key 'dry_run': ['invalid', 'value']" in out.stderr
```

### Comparing `pip-tools-7.0.0/tests/test_cli_sync.py` & `pip-tools-7.1.0/tests/test_cli_sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -394,7 +394,33 @@
     with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
         reqs_txt.write("six==1.10.0")
 
     out = runner.invoke(cli, ["--no-config", "--config", config_file.as_posix()])
 
     assert out.exit_code == 0
     assert "Would install:" not in out.stdout
+
+
+@mock.patch("piptools.sync.run")
+def test_raise_error_on_unknown_config_option(run, runner, tmp_path, make_config_file):
+    config_file = make_config_file("unknown-option", True)
+
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
+        reqs_txt.write("six==1.10.0")
+
+    out = runner.invoke(cli, ["--config", config_file.as_posix()])
+
+    assert out.exit_code == 2
+    assert "No such config key 'unknown_option'" in out.stderr
+
+
+@mock.patch("piptools.sync.run")
+def test_raise_error_on_invalid_config_option(run, runner, tmp_path, make_config_file):
+    config_file = make_config_file("dry-run", ["invalid", "value"])
+
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
+        reqs_txt.write("six==1.10.0")
+
+    out = runner.invoke(cli, ["--config", config_file.as_posix()])
+
+    assert out.exit_code == 2
+    assert "Invalid value for config key 'dry_run': ['invalid', 'value']" in out.stderr
```

### Comparing `pip-tools-7.0.0/tests/test_data/fake-index.json` & `pip-tools-7.1.0/tests/test_data/fake-index.json`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.1.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_data/packages/fake_with_deps/setup.py` & `pip-tools-7.1.0/tests/test_data/packages/fake_with_deps/setup.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_fake_index.py` & `pip-tools-7.1.0/tests/test_fake_index.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_logging.py` & `pip-tools-7.1.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_minimal_upgrade.py` & `pip-tools-7.1.0/tests/test_minimal_upgrade.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_repository_local.py` & `pip-tools-7.1.0/tests/test_repository_local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_repository_pypi.py` & `pip-tools-7.1.0/tests/test_repository_pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_resolver.py` & `pip-tools-7.1.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tests/test_sync.py` & `pip-tools-7.1.0/tests/test_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -222,24 +222,26 @@
     reqs = [from_line("django==1.7")]
 
     to_install, to_uninstall = diff(reqs, installed)
     assert to_install == set()
     assert to_uninstall == {"first"}
 
 
-def test_diff_leave_piptools_alone(fake_dist, from_line):
+def test_diff_leave_piptools_and_its_dependencies_alone(fake_dist, from_line):
     # Suppose an env contains Django, and pip-tools itself (including all of
     # its dependencies)
     installed = [
         fake_dist("django==1.7"),
         fake_dist("first==2.0.1"),
-        fake_dist("pip-tools==1.1.1", ["click>=4", "first", "six"]),
+        fake_dist("pip-tools==1.1.1", ["click>=4", "first", "six", "build"]),
         fake_dist("six==1.9.0"),
         fake_dist("click==4.1"),
         fake_dist("foobar==0.3.6"),
+        fake_dist("build==0.10.0", ["pyproject_hooks"]),
+        fake_dist("pyproject_hooks==1.0.0"),
     ]
 
     # Then this Django-only requirement should keep pip around (i.e. NOT
     # uninstall it), but uninstall first
     reqs = [from_line("django==1.7")]
 
     to_install, to_uninstall = diff(reqs, installed)
@@ -270,14 +272,35 @@
     reqs = [from_line(line)]
 
     to_install, to_uninstall = diff(reqs, installed)
     assert to_install == set()
     assert to_uninstall == set()
 
 
+@pytest.mark.parametrize(
+    ("installed_dist", "compiled_req"),
+    (
+        pytest.param("Django==1.7", "django==1.7", id="case insensitive"),
+        pytest.param(
+            "jaraco.classes==3.2",
+            "jaraco-classes==3.2",
+            id="different namespace notation",
+        ),
+    ),
+)
+def test_diff_respects_canonical_package_names(
+    fake_dist, from_line, installed_dist, compiled_req
+):
+    installed = [fake_dist(installed_dist)]
+    reqs = [from_line(compiled_req)]
+    to_install, to_uninstall = diff(reqs, installed)
+    assert to_install == set()
+    assert to_uninstall == set()
+
+
 def test_diff_with_no_url_hash(fake_dist, from_line):
     # if URL hash is not provided, assume the contents have
     # changed and reinstall
     line = "example@file:///example.zip"
     installed = [fake_dist(line)]
     reqs = [from_line(line)]
```

### Comparing `pip-tools-7.0.0/tests/test_utils.py` & `pip-tools-7.1.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,29 +569,24 @@
     for path in result:
         assert path in sys.path
 
 
 @pytest.mark.parametrize(
     ("pyproject_param", "new_default"),
     (
-        # From sync
-        ("ask", True),
         ("dry-run", True),
         ("find-links", ["changed"]),
         ("extra-index-url", ["changed"]),
         ("trusted-host", ["changed"]),
         ("no-index", True),
-        ("python-executable", "changed"),
         ("verbose", True),
         ("quiet", True),
-        ("user", True),
         ("cert", "changed"),
         ("client-cert", "changed"),
         ("pip-args", "changed"),
-        # From compile, unless also in sync
         ("pre", True),
         ("rebuild", True),
         ("extras", ["changed"]),
         ("all-extras", True),
         ("index-url", "changed"),
         ("header", False),
         ("emit-trusted-host", False),
```

### Comparing `pip-tools-7.0.0/tests/test_writer.py` & `pip-tools-7.1.0/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.0.0/tox.ini` & `pip-tools-7.1.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
   \t$ python3 -m http.server --directory \
   \N\{QUOTATION MARK\}\{docs_dir\}\N\{QUOTATION MARK\} 0\n\n" +\
   "=" * 120)'
 changedir = {toxinidir}/docs
 isolated_build = true
 passenv =
   SSH_AUTH_SOCK
-skip_install = true
+skip_install = false
 allowlist_externals =
   git
 
 
 [testenv:preview-docs]
 description = preview the docs
 deps =
@@ -147,10 +147,10 @@
     -d "{temp_dir}/.doctrees" \
     . \
     "{envdir}/docs_out"
 changedir = {toxinidir}/docs
 isolated_build = true
 passenv =
   SSH_AUTH_SOCK
-skip_install = true
+skip_install = false
 allowlist_externals =
   git
```

