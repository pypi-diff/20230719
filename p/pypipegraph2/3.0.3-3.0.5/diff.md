# Comparing `tmp/pypipegraph2-3.0.3.tar.gz` & `tmp/pypipegraph2-3.0.5.tar.gz`

## Comparing `pypipegraph2-3.0.3.tar` & `pypipegraph2-3.0.5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.3/Cargo.toml
--rw-r--r--   0     1001      123      595 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.coveragerc
--rw-r--r--   0     1001      123     1231 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.github/workflows/pytest.yml
--rw-r--r--   0     1001      123     1876 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.github/workflows/release.yml
--rw-r--r--   0     1001      123      754 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.gitignore
--rw-r--r--   0     1001      123      754 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.gitignore.orig
--rw-r--r--   0     1001      123      106 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.hgignore
--rw-r--r--   0     1001      123       30 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.ppg/logs/runtimes.tsv
--rw-r--r--   0     1001      123       95 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/AUTHORS.rst
--rw-r--r--   0     1001      123      128 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/CHANGELOG.rst
--rw-r--r--   0     1001      123    13831 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/Cargo.lock
--rw-r--r--   0     1001      123     9569 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/README.md
--rw-r--r--   0     1001      123     1363 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/Session.vim
--rwxr-xr-x   0     1001      123       55 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/bacon.sh
--rw-r--r--   0     1001      123      700 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benches/bench1.rs
--rwxr-xr-x   0     1001      123      841 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_disjoint.py
--rwxr-xr-x   0     1001      123      802 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_kilo_jobs.py
--rwxr-xr-x   0     1001      123     1133 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_simple.py
--rwxr-xr-x   0     1001      123      985 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_tall.py
--rwxr-xr-x   0     1001      123      947 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_wide.py
--rw-r--r--   0     1001      123     6315 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/designgoals.md
--rw-r--r--   0     1001      123     7618 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/Makefile
--rw-r--r--   0     1001      123       18 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/_static/.gitignore
--rw-r--r--   0     1001      123       41 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/authors.rst
--rw-r--r--   0     1001      123       43 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/changelog.rst
--rw-r--r--   0     1001      123     9264 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/conf.py
--rw-r--r--   0     1001      123     2241 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/index.rst
--rw-r--r--   0     1001      123       67 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/license.rst
--rw-r--r--   0     1001      123    21307 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/Basic_notebook.ipynb
--rw-r--r--   0     1001      123     1409 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/abort_when_stalled.py
--rw-r--r--   0     1001      123     1120 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/call_externals.py
--rw-r--r--   0     1001      123     1126 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/long_for_interactive.py
--rw-r--r--   0     1001      123      260 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/massive_exception.py
--rw-r--r--   0     1001      123      501 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/nested_exception.py
--rw-r--r--   0     1001      123      563 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/pandas_exception.py
--rw-r--r--   0     1001      123      506 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/runtimes.py
--rw-r--r--   0     1001      123     5790 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/simplest/simplest.py
--rw-r--r--   0     1001      123     1148 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/slow_for_interactive.py
--rw-r--r--   0     1001      123     1241 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/stall.py
--rw-r--r--   0     1001      123     1458 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/stop_then_abort_when_stalled.py
--rw-r--r--   0     1001      123     1554 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/stop_when_stalled.py
--rw-r--r--   0     1001      123     2533 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/flake.lock
--rw-r--r--   0     1001      123     6109 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/flake.nix
--rw-r--r--   0     1001      123  1650094 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/flame.svg
--rwxr-xr-x   0     1001      123      121 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_cargo_test.sh
--rwxr-xr-x   0     1001      123      151 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_main.sh
--rwxr-xr-x   0     1001      123      162 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_ppg2_iterations_with_fail.sh
--rwxr-xr-x   0     1001      123      165 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_ppg2_iterations_without_fail.sh
--rwxr-xr-x   0     1001      123       64 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_pytest.sh
--rwxr-xr-x   0     1001      123      171 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/prep_for_tests.sh
--rw-r--r--   0     1001      123     1972 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/pyproject.toml
--rwxr-xr-x   0     1001      123     6124 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/__init__.py
--rw-r--r--   0     1001      123     3224 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/entry_points.py
--rw-r--r--   0     1001      123     1831 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/enums.py
--rw-r--r--   0     1001      123     1899 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/exceptions.py
--rwxr-xr-x   0     1001      123    28025 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/graph.py
--rw-r--r--   0     1001      123     1528 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/hashers.py
--rwxr-xr-x   0     1001      123     2063 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/history_comparisons.py
--rw-r--r--   0     1001      123    10730 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/interactive.py
--rwxr-xr-x   0     1001      123      843 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/job_status.py
--rwxr-xr-x   0     1001      123   112223 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/jobs.py
--rw-r--r--   0     1001      123     3408 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/parallel.py
--rw-r--r--   0     1001      123    18439 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/ppg1_compatibility.py
--rw-r--r--   0     1001      123     8513 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/ppg_traceback.py
--rwxr-xr-x   0     1001      123    40841 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/runner.py
--rw-r--r--   0     1001      123     2551 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/testing/__init__.py
--rw-r--r--   0     1001      123     9557 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/testing/fixtures.py
--rw-r--r--   0     1001      123     5217 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/util.py
--rwxr-xr-x   0     1001      123      167 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/run_pytest.sh
--rw-r--r--   0     1001      123     1645 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/setup.cfg
--rw-r--r--   0     1001      123      557 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/setup.py
--rwxr-xr-x   0     1001      123   106720 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/engine.rs
--rwxr-xr-x   0     1001      123    20032 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/lib.rs
--rw-r--r--   0     1001      123     1009 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/main.rs
--rw-r--r--   0     1001      123    15543 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/main_iterations_with_fail.rs
--rw-r--r--   0     1001      123    10553 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/main_iterations_without_fail.rs
--rwxr-xr-x   0     1001      123    91028 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/tests.rs
--rw-r--r--   0     1001      123      209 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/t.py
--rw-r--r--   0     1001      123        0 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/__init__.py
--rw-r--r--   0     1001      123      282 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/_import_does_not_hang.py
--rw-r--r--   0     1001      123     4975 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/conftest.py
--rw-r--r--   0     1001      123      677 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/old_history_for_conversion_test.gz
--rw-r--r--   0     1001      123        0 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/__init__.py
--rw-r--r--   0     1001      123      965 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/shared.py
--rw-r--r--   0     1001      123    27757 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cache_jobs.py
--rw-r--r--   0     1001      123     5840 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_compatibility_layer.py
--rw-r--r--   0     1001      123     3050 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cycles.py
--rw-r--r--   0     1001      123    75082 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
--rw-r--r--   0     1001      123    23004 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
--rw-r--r--   0     1001      123    17831 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_other.py
--rw-r--r--   0     1001      123    21651 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_plotjobs.py
--rw-r--r--   0     1001      123     4365 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_prune.py
--rw-r--r--   0     1001      123     3196 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_simple.py
--rw-r--r--   0     1001      123     4792 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_util.py
--rw-r--r--   0     1001      123      927 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/shared.py
--rw-r--r--   0     1001      123    69648 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_basics.py
--rw-r--r--   0     1001      123     7374 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_bootstrap.py
--rw-r--r--   0     1001      123    14235 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_cache_jobs.py
--rw-r--r--   0     1001      123     1636 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_cycles.py
--rw-r--r--   0     1001      123      558 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_flake8.py
--rw-r--r--   0     1001      123     3366 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_function_invariants.py
--rw-r--r--   0     1001      123     2499 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_interactive.py
--rw-r--r--   0     1001      123    47281 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_invariants_and_dependencies.py
--rw-r--r--   0     1001      123    11292 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_job_generating_jobs.py
--rwxr-xr-x   0     1001      123    67423 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_jobs.py
--rw-r--r--   0     1001      123    22839 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_other.py
--rw-r--r--   0     1001      123     2616 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parallel.py
--rw-r--r--   0     1001      123        2 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/A
--rw-r--r--   0     1001      123      759 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/manual.py
--rwxr-xr-x   0     1001      123       52 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/sleeper.sh
--rw-r--r--   0     1001      123      977 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/stage2.py
--rw-r--r--   0     1001      123    16239 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_plotjobs.py
--rw-r--r--   0     1001      123     2736 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_prune.py
--rw-r--r--   0     1001      123     1914 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_rust_conversion.py
--rw-r--r--   0     1001      123    23688 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_shared_jobs.py
--rw-r--r--   0     1001      123     1846 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_simple.py
--rw-r--r--   0     1001      123     3691 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_util.py
--rw-r--r--   0     1001      123      507 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_version.py
--rw-r--r--   0     1001      123    61338 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/tests_from_the_field.py
--rw-r--r--   0     1001      123     5453 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/todo.md
--rw-r--r--   0     1001      123      154 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tox.ini
--rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 pypipegraph2-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.5/Cargo.toml
+-rw-r--r--   0     1001      123      595 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.coveragerc
+-rw-r--r--   0     1001      123     1231 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.github/workflows/pytest.yml
+-rw-r--r--   0     1001      123     1876 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      754 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.gitignore
+-rw-r--r--   0     1001      123      754 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.gitignore.orig
+-rw-r--r--   0     1001      123      106 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.hgignore
+-rw-r--r--   0     1001      123       30 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/.ppg/logs/runtimes.tsv
+-rw-r--r--   0     1001      123       95 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/AUTHORS.rst
+-rw-r--r--   0     1001      123      128 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/CHANGELOG.rst
+-rw-r--r--   0     1001      123    13831 2023-07-19 13:30:27.000000 pypipegraph2-3.0.5/Cargo.lock
+-rw-r--r--   0     1001      123     9569 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/README.md
+-rw-r--r--   0     1001      123     1363 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/Session.vim
+-rwxr-xr-x   0     1001      123       55 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/bacon.sh
+-rw-r--r--   0     1001      123      700 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/benches/bench1.rs
+-rwxr-xr-x   0     1001      123      841 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/benchmarks/bench_disjoint.py
+-rwxr-xr-x   0     1001      123      802 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/benchmarks/bench_kilo_jobs.py
+-rwxr-xr-x   0     1001      123     1133 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/benchmarks/bench_simple.py
+-rwxr-xr-x   0     1001      123      985 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/benchmarks/bench_tall.py
+-rwxr-xr-x   0     1001      123      947 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/benchmarks/bench_wide.py
+-rw-r--r--   0     1001      123     6315 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/designgoals.md
+-rw-r--r--   0     1001      123     7618 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/Makefile
+-rw-r--r--   0     1001      123       18 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/_static/.gitignore
+-rw-r--r--   0     1001      123       41 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/authors.rst
+-rw-r--r--   0     1001      123       43 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/changelog.rst
+-rw-r--r--   0     1001      123     9264 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/conf.py
+-rw-r--r--   0     1001      123     2241 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/index.rst
+-rw-r--r--   0     1001      123       67 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/docs/license.rst
+-rwxr-xr-x   0     1001      123       93 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/edit_version.sh
+-rw-r--r--   0     1001      123    21307 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/Basic_notebook.ipynb
+-rw-r--r--   0     1001      123     1409 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/abort_when_stalled.py
+-rw-r--r--   0     1001      123     1120 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/call_externals.py
+-rw-r--r--   0     1001      123     1126 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/long_for_interactive.py
+-rw-r--r--   0     1001      123      260 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/massive_exception.py
+-rw-r--r--   0     1001      123      501 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/nested_exception.py
+-rw-r--r--   0     1001      123      563 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/pandas_exception.py
+-rw-r--r--   0     1001      123      506 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/runtimes.py
+-rw-r--r--   0     1001      123     5790 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/simplest/simplest.py
+-rw-r--r--   0     1001      123     1148 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/slow_for_interactive.py
+-rw-r--r--   0     1001      123     1241 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/stall.py
+-rw-r--r--   0     1001      123     1458 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/stop_then_abort_when_stalled.py
+-rw-r--r--   0     1001      123     1554 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/examples/stop_when_stalled.py
+-rw-r--r--   0     1001      123     2533 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/flake.lock
+-rw-r--r--   0     1001      123     6145 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/flake.nix
+-rwxr-xr-x   0     1001      123      121 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/loop_cargo_test.sh
+-rwxr-xr-x   0     1001      123      151 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/loop_main.sh
+-rwxr-xr-x   0     1001      123      162 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/loop_ppg2_iterations_with_fail.sh
+-rwxr-xr-x   0     1001      123      165 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/loop_ppg2_iterations_without_fail.sh
+-rwxr-xr-x   0     1001      123       64 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/loop_pytest.sh
+-rwxr-xr-x   0     1001      123      171 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/prep_for_tests.sh
+-rw-r--r--   0     1001      123     1985 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/pyproject.toml
+-rwxr-xr-x   0     1001      123     6124 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/__init__.py
+-rw-r--r--   0     1001      123     3224 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/entry_points.py
+-rw-r--r--   0     1001      123     1831 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/enums.py
+-rw-r--r--   0     1001      123     1899 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/exceptions.py
+-rwxr-xr-x   0     1001      123    28025 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/graph.py
+-rw-r--r--   0     1001      123     1528 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/hashers.py
+-rwxr-xr-x   0     1001      123     2063 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/history_comparisons.py
+-rw-r--r--   0     1001      123    10730 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/interactive.py
+-rwxr-xr-x   0     1001      123      843 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/job_status.py
+-rwxr-xr-x   0     1001      123   112812 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/jobs.py
+-rw-r--r--   0     1001      123     3408 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/parallel.py
+-rw-r--r--   0     1001      123    18439 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/ppg1_compatibility.py
+-rw-r--r--   0     1001      123     8513 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/ppg_traceback.py
+-rwxr-xr-x   0     1001      123    40841 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/runner.py
+-rw-r--r--   0     1001      123     2551 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/testing/__init__.py
+-rw-r--r--   0     1001      123     9557 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/testing/fixtures.py
+-rw-r--r--   0     1001      123     5217 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/python/pypipegraph2/util.py
+-rwxr-xr-x   0     1001      123      167 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/run_pytest.sh
+-rw-r--r--   0     1001      123     1655 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/setup.cfg
+-rw-r--r--   0     1001      123      557 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/setup.py
+-rwxr-xr-x   0     1001      123   106724 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/src/engine.rs
+-rwxr-xr-x   0     1001      123    20032 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/src/lib.rs
+-rw-r--r--   0     1001      123     1009 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/src/main.rs
+-rw-r--r--   0     1001      123    15543 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/src/main_iterations_with_fail.rs
+-rw-r--r--   0     1001      123    10553 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/src/main_iterations_without_fail.rs
+-rwxr-xr-x   0     1001      123    91028 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/src/tests.rs
+-rw-r--r--   0     1001      123      209 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/t.py
+-rw-r--r--   0     1001      123        0 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/__init__.py
+-rw-r--r--   0     1001      123      282 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/_import_does_not_hang.py
+-rw-r--r--   0     1001      123     4975 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/conftest.py
+-rw-r--r--   0     1001      123      677 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/old_history_for_conversion_test.gz
+-rw-r--r--   0     1001      123        0 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/__init__.py
+-rw-r--r--   0     1001      123      965 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/shared.py
+-rw-r--r--   0     1001      123    27757 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_cache_jobs.py
+-rw-r--r--   0     1001      123     5840 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_compatibility_layer.py
+-rw-r--r--   0     1001      123     3050 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_cycles.py
+-rw-r--r--   0     1001      123    75082 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
+-rw-r--r--   0     1001      123    23004 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
+-rw-r--r--   0     1001      123    17831 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_other.py
+-rw-r--r--   0     1001      123    21651 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_plotjobs.py
+-rw-r--r--   0     1001      123     4365 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_prune.py
+-rw-r--r--   0     1001      123     3196 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_simple.py
+-rw-r--r--   0     1001      123     4792 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_util.py
+-rw-r--r--   0     1001      123      927 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/shared.py
+-rw-r--r--   0     1001      123    69648 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_basics.py
+-rw-r--r--   0     1001      123     7374 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_bootstrap.py
+-rw-r--r--   0     1001      123    14235 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_cache_jobs.py
+-rw-r--r--   0     1001      123     1636 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_cycles.py
+-rw-r--r--   0     1001      123      558 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_flake8.py
+-rw-r--r--   0     1001      123     3366 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_function_invariants.py
+-rw-r--r--   0     1001      123     2499 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_interactive.py
+-rw-r--r--   0     1001      123    47281 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_invariants_and_dependencies.py
+-rw-r--r--   0     1001      123    11292 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_job_generating_jobs.py
+-rwxr-xr-x   0     1001      123    67423 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_jobs.py
+-rw-r--r--   0     1001      123    22839 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_other.py
+-rw-r--r--   0     1001      123     2616 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_parallel.py
+-rw-r--r--   0     1001      123        2 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_parent_termination_kills_children/A
+-rw-r--r--   0     1001      123      759 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_parent_termination_kills_children/manual.py
+-rwxr-xr-x   0     1001      123       52 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_parent_termination_kills_children/sleeper.sh
+-rw-r--r--   0     1001      123      977 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_parent_termination_kills_children/stage2.py
+-rw-r--r--   0     1001      123    16239 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_plotjobs.py
+-rw-r--r--   0     1001      123     2736 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_prune.py
+-rw-r--r--   0     1001      123     1914 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_rust_conversion.py
+-rw-r--r--   0     1001      123    23688 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_shared_jobs.py
+-rw-r--r--   0     1001      123     1846 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_simple.py
+-rw-r--r--   0     1001      123     3691 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_util.py
+-rw-r--r--   0     1001      123      507 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/test_version.py
+-rw-r--r--   0     1001      123    61338 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tests/tests_from_the_field.py
+-rw-r--r--   0     1001      123     5453 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/todo.md
+-rw-r--r--   0     1001      123      154 2023-07-19 13:29:35.000000 pypipegraph2-3.0.5/tox.ini
+-rw-r--r--   0        0        0    11422 1970-01-01 00:00:00.000000 pypipegraph2-3.0.5/PKG-INFO
```

### Comparing `pypipegraph2-3.0.3/Cargo.toml` & `pypipegraph2-3.0.5/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pypipegraph2"
-version = "3.0.3"
+version = "3.0.5"
 edition = "2018"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pypipegraph2"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `pypipegraph2-3.0.3/.coveragerc` & `pypipegraph2-3.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/.github/workflows/pytest.yml` & `pypipegraph2-3.0.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/.github/workflows/release.yml` & `pypipegraph2-3.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/.gitignore` & `pypipegraph2-3.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/.gitignore.orig` & `pypipegraph2-3.0.5/.gitignore.orig`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/Cargo.lock` & `pypipegraph2-3.0.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pypipegraph2"
-version = "3.0.3"
+version = "3.0.5"
 dependencies = [
  "backtrace",
  "colored",
  "env_logger",
  "itertools",
  "log",
  "num_cpus",
```

### Comparing `pypipegraph2-3.0.3/README.md` & `pypipegraph2-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/Session.vim` & `pypipegraph2-3.0.5/Session.vim`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/benches/bench1.rs` & `pypipegraph2-3.0.5/benches/bench1.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/benchmarks/bench_disjoint.py` & `pypipegraph2-3.0.5/benchmarks/bench_disjoint.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/benchmarks/bench_kilo_jobs.py` & `pypipegraph2-3.0.5/benchmarks/bench_kilo_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/benchmarks/bench_simple.py` & `pypipegraph2-3.0.5/benchmarks/bench_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/benchmarks/bench_tall.py` & `pypipegraph2-3.0.5/benchmarks/bench_tall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/benchmarks/bench_wide.py` & `pypipegraph2-3.0.5/benchmarks/bench_wide.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/designgoals.md` & `pypipegraph2-3.0.5/designgoals.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/docs/Makefile` & `pypipegraph2-3.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/docs/conf.py` & `pypipegraph2-3.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/docs/index.rst` & `pypipegraph2-3.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/Basic_notebook.ipynb` & `pypipegraph2-3.0.5/examples/Basic_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/abort_when_stalled.py` & `pypipegraph2-3.0.5/examples/abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/call_externals.py` & `pypipegraph2-3.0.5/examples/call_externals.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/long_for_interactive.py` & `pypipegraph2-3.0.5/examples/long_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/pandas_exception.py` & `pypipegraph2-3.0.5/examples/pandas_exception.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/simplest/simplest.py` & `pypipegraph2-3.0.5/examples/simplest/simplest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/slow_for_interactive.py` & `pypipegraph2-3.0.5/examples/slow_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/stall.py` & `pypipegraph2-3.0.5/examples/stall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/stop_then_abort_when_stalled.py` & `pypipegraph2-3.0.5/examples/stop_then_abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/examples/stop_when_stalled.py` & `pypipegraph2-3.0.5/examples/stop_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/flake.lock` & `pypipegraph2-3.0.5/flake.lock`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/flake.nix` & `pypipegraph2-3.0.5/flake.nix`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
            rich
            xxhash
            wrapt
            deepdiff
            psutil
            networkx
            cython
-
+           filelock
         '';
         format = "pyproject";
       };
     palettable = let
       p = pkgs.python39Packages;
     in
       p.buildPythonPackage rec {
@@ -201,14 +201,15 @@
       p.cython
       p.setproctitle
       dppd
       dppd_plotnine
       # for testing...
       ppg1
       plotnine
+      p.filelock
     ]);
   in {
     # pass in nixpkgs, mach-nix and what you want it to report back as a version
     mach-nix-build-python-package = build_mbf_bam;
     devShell.x86_64-linux = pkgs.mkShell {
       # supplx the specific rust version
       # be sure to set this back in your build scripts,
```

### Comparing `pypipegraph2-3.0.3/pyproject.toml` & `pypipegraph2-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.12,<0.13"]
 build-backend = "maturin"
 
 [project]
 name = "pypipegraph2"
-version = "3.0.3"
+version = "3.0.5"
 description = "Advanced python 'what changed and what do we need to do' tracking"
 long-description = "README.md"
 authors = [
  {"name" = "Florian Finkernagel", "email" = "finkernagel@imt.uni-marburg.de"}
 ]
 classifiers = [
 	"Development Status :: 4 - Beta",
@@ -22,14 +22,15 @@
 	"loguru",
 	"rich",
 	"xxhash",
 	"wrapt",
 	"deepdiff",
 	"psutil",
 	"networkx",
+	"filelock",
 ]
 
 
 [project.opetional-dependencies]
 dev = [
 	"flake8",
 	"pytest",
```

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/__init__.py` & `pypipegraph2-3.0.5/python/pypipegraph2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "3.0.3"
+__version__ = "3.0.5"
 
 from pathlib import Path
 import logging
 import contextlib
 from .graph import PyPipeGraph, ALL_CORES
 from .jobs import (
     FileGeneratingJob,
```

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/entry_points.py` & `pypipegraph2-3.0.5/python/pypipegraph2/entry_points.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/enums.py` & `pypipegraph2-3.0.5/python/pypipegraph2/enums.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/exceptions.py` & `pypipegraph2-3.0.5/python/pypipegraph2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/graph.py` & `pypipegraph2-3.0.5/python/pypipegraph2/graph.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/hashers.py` & `pypipegraph2-3.0.5/python/pypipegraph2/hashers.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/history_comparisons.py` & `pypipegraph2-3.0.5/python/pypipegraph2/history_comparisons.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/interactive.py` & `pypipegraph2-3.0.5/python/pypipegraph2/interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/job_status.py` & `pypipegraph2-3.0.5/python/pypipegraph2/job_status.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/jobs.py` & `pypipegraph2-3.0.5/python/pypipegraph2/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from functools import total_ordering
 
 from . import hashers, exceptions, ppg_traceback
 from .enums import Resources
 from .util import escape_logging
 import hashlib
 import shutil
+import random
+import filelock
 from .util import (
     log_info,
     log_error,
     log_warning,  # log_debug,
     log_trace,
     log_job_trace,
 )
@@ -2593,15 +2595,30 @@
             "mtime": int(time.time()),
         }  # so we can detect if the target changed
 
         # we clean up if we build,
         # or if we had no history
         if did_build or not self.job_id in runner.history:
             self._cleanup(runner)
-        self._log_local_usage(by_input_key)
+        lock_file = (
+            global_pipegraph.history_dir / SharedMultiFileGeneratingJob.log_filename
+        ).with_suffix(".lock")
+        lock = filelock.FileLock(lock_file, timeout=random.randint(8, 20))
+        try:
+            with lock:
+                self._log_local_usage(by_input_key)
+        except filelock.Timeout:
+            # guess we have as stale lock. This really shouldn't take this much time.
+            try:
+                lock_file.unlink()
+            except:  # noqa: E722
+                pass
+            with lock:
+                self._log_local_usage(by_input_key)
+
         return res
 
     def _log_local_usage(self, key):
         """Write the input key we used to a log file,
         so that non-ppg-interactive stuff may read it back
         and find the files"""
         from . import global_pipegraph
```

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/parallel.py` & `pypipegraph2-3.0.5/python/pypipegraph2/parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/ppg1_compatibility.py` & `pypipegraph2-3.0.5/python/pypipegraph2/ppg1_compatibility.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/ppg_traceback.py` & `pypipegraph2-3.0.5/python/pypipegraph2/ppg_traceback.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/runner.py` & `pypipegraph2-3.0.5/python/pypipegraph2/runner.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/testing/__init__.py` & `pypipegraph2-3.0.5/python/pypipegraph2/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/testing/fixtures.py` & `pypipegraph2-3.0.5/python/pypipegraph2/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/python/pypipegraph2/util.py` & `pypipegraph2-3.0.5/python/pypipegraph2/util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/setup.cfg` & `pypipegraph2-3.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [metadata]
 name = pypipegraph2
 description = Advanced python 'what changed and what do we need to do' tracking
-version = 3.0.3
+version = 3.0.5
 author = Florian Finkernagel
 author-email = finkernagel@imt.uni-marburg.de
 license = mit
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8
 url = https://github.com/pyscaffold/pyscaffold/
 project-urls = 
@@ -24,14 +24,15 @@
 	=src
 install_requires = networkx
 	loguru
 	rich
 	xxhash
 	wrapt
 	deepdiff
+	filelock
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `pypipegraph2-3.0.3/setup.py` & `pypipegraph2-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/src/engine.rs` & `pypipegraph2-3.0.5/src/engine.rs`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
     pub fn abort_remaining(&mut self) -> Result<(), PPGEvaluatorError> {
         let mut signal_failure = Vec::new();
 
         let mut new_signals: Vec<Signal> = Vec::new();
 
         for (job_idx, job) in self.jobs.iter_mut().enumerate() {
             if !job.state.is_finished() {
-                dbg!("Declaring upstream failure", job);
+                //dbg!("Declaring upstream failure", job);
                 signal_failure.push(job_idx);
             }
         }
 
         for job_idx in signal_failure {
             new_signals.push(NewSignal!(SignalKind::JobAborted, job_idx, self.jobs));
         }
@@ -780,15 +780,15 @@
                 // we need to *keep* the history.
                 //
                 //
                 // is this not a problem on abort?
                 // no abort fails the currently running jobs (external, python does that)
 
                 // paranoia...
-                dbg!(&job);
+                //dbg!(&job);
                 assert!(
                     job.state.is_failed()
                         || Self::_job_and_downstreams_are_ephemeral(&self.dag, &self.jobs, idx)
                 );
                 if !job.state.is_upstream_failure() {
                     out.remove(&job.job_id);
                     out.remove(&input_name_key);
```

### Comparing `pypipegraph2-3.0.3/src/lib.rs` & `pypipegraph2-3.0.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/src/main.rs` & `pypipegraph2-3.0.5/src/main.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/src/main_iterations_with_fail.rs` & `pypipegraph2-3.0.5/src/main_iterations_with_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/src/main_iterations_without_fail.rs` & `pypipegraph2-3.0.5/src/main_iterations_without_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/src/tests.rs` & `pypipegraph2-3.0.5/src/tests.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/conftest.py` & `pypipegraph2-3.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/old_history_for_conversion_test.gz` & `pypipegraph2-3.0.5/tests/old_history_for_conversion_test.gz`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/shared.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cache_jobs.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_compatibility_layer.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_compatibility_layer.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cycles.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_job_gen_jobs.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_job_gen_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_other.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_other.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_plotjobs.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_prune.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_simple.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_util.py` & `pypipegraph2-3.0.5/tests/ppg1_compatibility_layer/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/shared.py` & `pypipegraph2-3.0.5/tests/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_basics.py` & `pypipegraph2-3.0.5/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_bootstrap.py` & `pypipegraph2-3.0.5/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_cache_jobs.py` & `pypipegraph2-3.0.5/tests/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_cycles.py` & `pypipegraph2-3.0.5/tests/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_flake8.py` & `pypipegraph2-3.0.5/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_function_invariants.py` & `pypipegraph2-3.0.5/tests/test_function_invariants.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_interactive.py` & `pypipegraph2-3.0.5/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_invariants_and_dependencies.py` & `pypipegraph2-3.0.5/tests/test_invariants_and_dependencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_job_generating_jobs.py` & `pypipegraph2-3.0.5/tests/test_job_generating_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_jobs.py` & `pypipegraph2-3.0.5/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_other.py` & `pypipegraph2-3.0.5/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_parallel.py` & `pypipegraph2-3.0.5/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/manual.py` & `pypipegraph2-3.0.5/tests/test_parent_termination_kills_children/manual.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/stage2.py` & `pypipegraph2-3.0.5/tests/test_parent_termination_kills_children/stage2.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_plotjobs.py` & `pypipegraph2-3.0.5/tests/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_prune.py` & `pypipegraph2-3.0.5/tests/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_rust_conversion.py` & `pypipegraph2-3.0.5/tests/test_rust_conversion.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_shared_jobs.py` & `pypipegraph2-3.0.5/tests/test_shared_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_simple.py` & `pypipegraph2-3.0.5/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/test_util.py` & `pypipegraph2-3.0.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/tests/tests_from_the_field.py` & `pypipegraph2-3.0.5/tests/tests_from_the_field.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/todo.md` & `pypipegraph2-3.0.5/todo.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.3/PKG-INFO` & `pypipegraph2-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pypipegraph2
-Version: 3.0.3
+Version: 3.0.5
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: loguru
 Requires-Dist: rich
 Requires-Dist: xxhash
 Requires-Dist: wrapt
 Requires-Dist: deepdiff
 Requires-Dist: psutil
 Requires-Dist: networkx
+Requires-Dist: filelock
 License-File: AUTHORS.rst
 Summary: Advanced python 'what changed and what do we need to do' tracking
 Author-email: Florian Finkernagel <finkernagel@imt.uni-marburg.de>
 License: MIT License
 	
 	Copyright (c) 2023 Florian Finkernagel
```

