# Comparing `tmp/swh.objstorage-2.2.0.tar.gz` & `tmp/swh.objstorage-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.objstorage-2.2.0.tar", last modified: Fri Mar 24 15:00:56 2023, max compression
+gzip compressed data, was "swh.objstorage-2.3.0.tar", last modified: Wed Jul 19 15:19:17 2023, max compression
```

## Comparing `swh.objstorage-2.2.0.tar` & `swh.objstorage-2.3.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      145 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      126 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2514 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1470 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     3435 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/bin/swh-objstorage-azure
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     5513 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/docs/winery.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      554 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       16 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      234 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2642 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1915 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4975 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16660 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5150 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3152 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2163 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8664 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1115 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12594 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4060 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5368 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) docker     (999)       55 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4386 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4839 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2557 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2556 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5541 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2685 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6756 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3658 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)      547 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1184 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2970 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6679 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/interface.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/
--rw-r--r--   0 jenkins    (115) docker     (999)      121 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/
--rw-r--r--   0 jenkins    (115) docker     (999)     2617 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2721 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/filter.py
--rw-r--r--   0 jenkins    (115) docker     (999)      785 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/read_write_filter.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10697 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/multiplexer/multiplexer_objstorage.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4608 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/objstorage.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1436 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12998 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1473 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12045 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5298 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3934 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) docker     (999)      545 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1430 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2643 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5736 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1630 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10380 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11271 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2761 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3188 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4017 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5593 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2121 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) docker     (999)      541 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2514 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4066 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       54 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      392 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1689 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/tox.ini
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/winery-test-environment/
--rw-r--r--   0 jenkins    (115) docker     (999)     2649 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      209 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) docker     (999)      955 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) docker     (999)     4204 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     2038 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) docker     (999)     3932 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) docker     (999)      844 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     1836 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) docker     (999)      108 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) docker     (999)       91 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      822 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) docker     (999)       84 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) docker     (999)       75 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:56.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) docker     (999)       80 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2757 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2763 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2895 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2765 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) docker     (999)      824 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1333 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     1733 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) docker     (999)       40 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      198 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     2727 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      632 2023-03-24 15:00:54.000000 swh.objstorage-2.2.0/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      145 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      126 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2514 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1470 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.395903 swh.objstorage-2.3.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     3435 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/bin/swh-objstorage-azure
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.395903 swh.objstorage-2.3.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.395903 swh.objstorage-2.3.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.395903 swh.objstorage-2.3.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     5513 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      599 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       16 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      268 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2642 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.395903 swh.objstorage-2.3.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1915 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4975 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17589 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5150 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3638 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2163 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9287 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1115 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12594 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4060 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5731 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) docker     (999)       55 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4386 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4839 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2557 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2556 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5541 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2685 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6756 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3658 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      547 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1184 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2970 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7749 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/interface.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/multiplexer/
+-rw-r--r--   0 jenkins    (115) docker     (999)      121 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/multiplexer/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.399903 swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2617 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2721 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/filter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      785 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/read_write_filter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10697 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/multiplexer/multiplexer_objstorage.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4838 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/objstorage.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.403904 swh.objstorage-2.3.0/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1436 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13517 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1473 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12287 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7423 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4609 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      545 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1430 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2643 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5736 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1630 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10380 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11271 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2761 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3188 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4017 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5593 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2121 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      541 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.395903 swh.objstorage-2.3.0/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2514 2023-07-19 15:19:17.000000 swh.objstorage-2.3.0/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4066 2023-07-19 15:19:17.000000 swh.objstorage-2.3.0/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-19 15:19:17.000000 swh.objstorage-2.3.0/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       54 2023-07-19 15:19:17.000000 swh.objstorage-2.3.0/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      426 2023-07-19 15:19:17.000000 swh.objstorage-2.3.0/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-19 15:19:17.000000 swh.objstorage-2.3.0/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1689 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2649 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      209 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) docker     (999)      955 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     4204 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     2038 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)     3932 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      844 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     1836 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.391903 swh.objstorage-2.3.0/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) docker     (999)      108 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)       91 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      822 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)       84 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)       75 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:17.407904 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) docker     (999)       80 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2757 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2763 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2895 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2765 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      824 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1333 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     1733 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       40 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      198 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     2727 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      632 2023-07-19 15:19:11.000000 swh.objstorage-2.3.0/winery-test-environment/tests.yml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.objstorage-2.2.0/.pre-commit-config.yaml` & `swh.objstorage-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/CODE_OF_CONDUCT.md` & `swh.objstorage-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/LICENSE` & `swh.objstorage-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/PKG-INFO` & `swh.objstorage-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.2.0
+Version: 2.3.0
 Summary: Software Heritage Object Storage
 Home-page: https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh.objstorage-2.2.0/README.md` & `swh.objstorage-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/bin/swh-objstorage-azure` & `swh.objstorage-2.3.0/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/docs/winery.rst` & `swh.objstorage-2.3.0/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/mypy.ini` & `swh.objstorage-2.3.0/mypy.ini`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 [mypy-libcloud.*]
 ignore_missing_imports = True
 
 [mypy-msgpack.*]
 ignore_missing_imports = True
 
+[mypy-moto.*]
+ignore_missing_imports = True
+
 [mypy-pkg_resources.*]
 ignore_missing_imports = True
 
 [mypy-pytest.*]
 ignore_missing_imports = True
 
 [mypy-requests_toolbelt.*]
```

### Comparing `swh.objstorage-2.2.0/setup.py` & `swh.objstorage-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/api/client.py` & `swh.objstorage-2.3.0/swh/objstorage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/api/server.py` & `swh.objstorage-2.3.0/swh/objstorage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/azure.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/azure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# Copyright (C) 2016-2021  The Software Heritage developers
+# Copyright (C) 2016-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import asyncio
 import contextlib
-import datetime
+from datetime import datetime, timedelta
 from itertools import product
 import string
 from typing import Iterable, Iterator, Mapping, Optional, Union
 import warnings
 
 from azure.core.exceptions import ResourceExistsError, ResourceNotFoundError
 from azure.storage.blob import (
+    BlobSasPermissions,
     ContainerClient,
     ContainerSasPermissions,
+    generate_blob_sas,
     generate_container_sas,
 )
 from azure.storage.blob.aio import ContainerClient as AsyncContainerClient
 from typing_extensions import Literal
 
 from swh.model import hashutil
 from swh.objstorage.exc import Error, ObjNotFoundError
@@ -33,15 +35,15 @@
 
 
 def get_container_url(
     account_name: str,
     account_key: str,
     container_name: str,
     access_policy: str = "read_only",
-    expiry: datetime.timedelta = datetime.timedelta(days=365),
+    expiry: timedelta = timedelta(days=365),
     container_url_template: str = (
         "https://{account_name}.blob.core.windows.net/{container_name}?{signature}"
     ),
     **kwargs,
 ) -> str:
     """Get the full url, for the given container on the given account, with a
     Shared Access Signature granting the specified access policy.
@@ -64,22 +66,22 @@
         ),
         "append_only": ContainerSasPermissions(
             read=True, list=True, delete=False, write=True
         ),
         "full": ContainerSasPermissions(read=True, list=True, delete=True, write=True),
     }
 
-    current_time = datetime.datetime.utcnow()
+    current_time = datetime.utcnow()
 
     signature = generate_container_sas(
         account_name,
         container_name,
         account_key=account_key,
         permission=access_policies[access_policy],
-        start=current_time + datetime.timedelta(minutes=-1),
+        start=current_time + timedelta(minutes=-1),
         expiry=current_time + expiry,
     )
 
     return container_url_template.format(
         account_name=account_name,
         container_name=container_name,
         signature=signature,
@@ -336,14 +338,38 @@
         try:
             client.delete_blob()
         except ResourceNotFoundError:
             raise ObjNotFoundError(obj_id) from None
 
         return True
 
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        hex_obj_id = self._internal_id(obj_id)
+        client = self.get_blob_client(hex_obj_id)
+        try:
+            client.get_blob_properties()
+        except ResourceNotFoundError:
+            raise ObjNotFoundError(obj_id)
+        else:
+            signature = generate_blob_sas(
+                client.account_name,
+                client.container_name,
+                hex_obj_id,
+                account_key=client.credential.account_key,
+                permission=BlobSasPermissions(read=True),
+                expiry=datetime.now() + (expiry or timedelta(hours=24)),
+                content_disposition=content_disposition,
+            )
+            return f"{client.primary_endpoint}?{signature}"
+
 
 class PrefixedAzureCloudObjStorage(AzureCloudObjStorage):
     """ObjStorage with azure capabilities, striped by prefix.
 
     accounts is a dict containing entries of the form:
         <prefix>: <container_url_for_prefix>
     """
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/generator.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/generator.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/http.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from datetime import timedelta
 import logging
 from typing import Iterator, Optional
 from urllib.parse import urljoin
 
 import requests
 
 from swh.model import hashutil
 from swh.objstorage import exc
+from swh.objstorage.constants import ID_HASH_ALGO
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     DEFAULT_LIMIT,
     ObjStorage,
     compute_hash,
     decompressors,
     objid_to_default_hex,
@@ -84,16 +86,30 @@
             d = decompressors[self.compression]()
             ret = d.decompress(ret)
             if d.unused_data:
                 hex_obj_id = objid_to_default_hex(obj_id)
                 raise exc.Error("Corrupt object %s: trailing data found" % hex_obj_id)
         return ret
 
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        return self._path(obj_id)
+
     def check(self, obj_id: ObjId) -> None:
         # Check the content integrity
         obj_content = self.get(obj_id)
         content_obj_id = compute_hash(obj_content)
-        if content_obj_id != obj_id:
+        if content_obj_id != self._hash(obj_id):
             raise exc.Error(obj_id)
 
+    def _hash(self, obj_id: ObjId) -> bytes:
+        if isinstance(obj_id, dict):
+            return obj_id[ID_HASH_ALGO]
+        else:
+            return obj_id
+
     def _path(self, obj_id):
-        return urljoin(self.root_path, hashutil.hash_to_hex(obj_id))
+        return urljoin(self.root_path, hashutil.hash_to_hex(self._hash(obj_id)))
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/in_memory.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/libcloud.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/libcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright (C) 2016-2022  The Software Heritage developers
+# Copyright (C) 2016-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import abc
 from collections import OrderedDict
+from datetime import timedelta
 from typing import Iterator, Optional
 from urllib.parse import urlencode
 
 from libcloud.storage import providers
 import libcloud.storage.drivers.s3
 from libcloud.storage.types import ObjectDoesNotExistError, Provider
 from typing_extensions import Literal
@@ -174,14 +175,22 @@
         d = decompressors[self.compression]()
         ret = d.decompress(obj)
         if d.unused_data:
             hex_obj_id = objid_to_default_hex(obj_id)
             raise Error("Corrupt object %s: trailing data found" % hex_obj_id)
         return ret
 
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        return self._get_object(obj_id).get_cdn_url()
+
     def check(self, obj_id: ObjId) -> None:
         # Check that the file exists, as _get_object raises ObjNotFoundError
         self._get_object(obj_id)
         # Check the content integrity
         obj_content = self.get(obj_id)
         content_obj_id = compute_hash(obj_content)
         if isinstance(obj_id, dict):
@@ -247,13 +256,24 @@
 
 class AwsCloudObjStorage(CloudObjStorage):
     """Amazon's S3 Cloud-based object storage"""
 
     def _get_provider(self):
         return Provider.S3
 
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        return self.driver.get_object_cdn_url(
+            self._get_object(obj_id),
+            ex_expiry=(expiry.total_seconds() / 3600) if expiry is not None else 24,
+        )
+
 
 class OpenStackCloudObjStorage(CloudObjStorage):
     """OpenStack Swift Cloud based object storage"""
 
     def _get_provider(self):
         return Provider.OPENSTACK_SWIFT
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/noop.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/noop.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/pathslicing.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/seaweedfs/http.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2019-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from datetime import timedelta
 import io
 from itertools import islice
 import logging
 from typing import Iterator, Optional
 from urllib.parse import urlparse
 
 from typing_extensions import Literal
@@ -108,14 +109,25 @@
         d = decompressors[self.compression]()
         ret = d.decompress(obj)
         if d.unused_data:
             hex_obj_id = objid_to_default_hex(obj_id)
             raise Error("Corrupt object %s: trailing data found" % hex_obj_id)
         return ret
 
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        path = self._path(obj_id)
+        if not self.wf.exists(path):
+            raise ObjNotFoundError(obj_id)
+        return self.wf.build_url(path)
+
     def check(self, obj_id: ObjId) -> None:
         # Check the content integrity
         obj_content = self.get(obj_id)
         content_obj_id = compute_hash(obj_content)
         if isinstance(obj_id, dict):
             obj_id = obj_id[self.PRIMARY_HASH]
         if content_obj_id != obj_id:
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/database.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/database.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/objstorage.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/roshard.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/roshard.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/rwshard.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/rwshard.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/sharedbase.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/sharedbase.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/stats.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/backends/winery/throttler.py` & `swh.objstorage-2.3.0/swh/objstorage/backends/winery/throttler.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/cli.py` & `swh.objstorage-2.3.0/swh/objstorage/cli.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/constants.py` & `swh.objstorage-2.3.0/swh/objstorage/constants.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/exc.py` & `swh.objstorage-2.3.0/swh/objstorage/exc.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/factory.py` & `swh.objstorage-2.3.0/swh/objstorage/factory.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/interface.py` & `swh.objstorage-2.3.0/swh/objstorage/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2015-2023 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from datetime import timedelta
 from typing import Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
 
 from typing_extensions import Protocol, TypedDict, runtime_checkable
 
 from swh.core.api import remote_api_endpoint
 from swh.model.model import Sha1
 from swh.objstorage.constants import DEFAULT_LIMIT
@@ -154,14 +155,41 @@
             list of resulting contents, or None if the content could
             not be retrieved. Do not raise any exception as a fail for
             one content will not cancel the whole request.
 
         """
         ...
 
+    @remote_api_endpoint("content/download_url")
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        """Get a direct download link for the object if the obstorage backend supports
+        such feature.
+
+        Some objstorage backends, typically cloud based ones like azure or s3, can provide
+        a direct download link for a stored object.
+
+        Args:
+            obj_id: object identifier
+            content_disposition: set Content-Disposition header for the generated URL
+                response if the objstorage backend supports it
+            expiry: the duration after which the URL expires if the objstorage backend
+                supports it, if not provided the URL expires 24 hours after its creation
+
+        Returns:
+            Direct download URL for the object or :const:`None` if the objstorage backend does
+                not support such feature.
+        """
+
+        ...
+
     @remote_api_endpoint("content/check")
     def check(self, obj_id: ObjId) -> None:
         """Perform an integrity check for a given object.
 
         Verify that the file object is in place and that the content matches
         the object id.
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/__init__.py` & `swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/filter.py` & `swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/multiplexer/filter/read_write_filter.py` & `swh.objstorage-2.3.0/swh/objstorage/multiplexer/filter/read_write_filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/multiplexer/multiplexer_objstorage.py` & `swh.objstorage-2.3.0/swh/objstorage/multiplexer/multiplexer_objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/objstorage.py` & `swh.objstorage-2.3.0/swh/objstorage/objstorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import abc
 import bz2
 import collections
+from datetime import timedelta
 from itertools import dropwhile, islice
 import lzma
 from typing import Callable, Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
 import zlib
 
 from typing_extensions import Protocol
 
@@ -151,7 +152,15 @@
         limit: Optional[int] = DEFAULT_LIMIT,
     ) -> Iterator[CompositeObjId]:
         it = iter(self)
         if last_obj_id:
             last_obj_id_hex = objid_to_default_hex(last_obj_id)
             it = dropwhile(lambda x: objid_to_default_hex(x) <= last_obj_id_hex, it)
         return islice(it, limit)
+
+    def download_url(
+        self,
+        obj_id: ObjId,
+        content_disposition: Optional[str] = None,
+        expiry: Optional[timedelta] = None,
+    ) -> Optional[str]:
+        return None
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/conftest.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/objstorage_testing.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/objstorage_testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import inspect
 from typing import Tuple
 
+import pytest
+import requests
+
 from swh.objstorage import exc
 from swh.objstorage.interface import CompositeObjId, ObjStorageInterface
-from swh.objstorage.objstorage import compute_hash
+from swh.objstorage.objstorage import compute_hash, decompressors
 
 
 class ObjStorageTestFixture:
     num_objects = 1200
 
     def fill_objstorage(self, num_objects):
         all_ids = []
@@ -338,7 +341,19 @@
         ids = list(self.storage.list_content(last_obj_id=all_ids[-1], limit=100))
         assert not ids
 
         ids = list(
             self.storage.list_content(last_obj_id={"sha1": b"\xff" * 20}, limit=100)
         )
         assert not ids
+
+    def test_download_url(self):
+        content = b"foo"
+        obj_id = compute_hash(content)
+        self.storage.add(content, obj_id)
+        url = self.storage.download_url(obj_id)
+        if url is not None:
+            decompress = decompressors[self.storage.compression]().decompress
+            assert decompress(requests.get(url).content) == content
+
+            with pytest.raises(exc.ObjNotFoundError):
+                self.storage.download_url(b"\xff" * 20)
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_api.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_api.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_azure.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016-2022  The Software Heritage developers
+# Copyright (C) 2016-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import asyncio
 import base64
 import collections
@@ -256,14 +256,18 @@
             with self.assertRaises(Error) as e:
                 self.storage.check(obj_id)
         else:
             with self.assertRaises(Error) as e:
                 self.storage.get(obj_id)
             assert "trailing data" in e.exception.args[0]
 
+    @pytest.mark.skip("makes no sense to test this for the mocked azure")
+    def test_download_url(self):
+        pass
+
 
 class TestMockedAzureCloudObjStorageGzip(TestMockedAzureCloudObjStorage):
     compression = "gzip"
 
 
 class TestMockedAzureCloudObjStorageZlib(TestMockedAzureCloudObjStorage):
     compression = "zlib"
@@ -320,14 +324,18 @@
             prefix = hex_obj_id[0]
             self.assertTrue(
                 self.ContainerClient(self.storage.container_urls[prefix])
                 .get_blob_client(hex_obj_id)
                 .get_blob_properties()
             )
 
+    @pytest.mark.skip("makes no sense to test this for the mocked azure")
+    def test_download_url(self):
+        pass
+
 
 def test_get_container_url():
     # r=read, l=list, w=write, d=delete
     policy_map = {
         "read_only": "rl",
         "append_only": "rwl",
         "full": "rwdl",
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_cloud.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,30 @@
-# Copyright (C) 2016  The Software Heritage developers
+# Copyright (C) 2016-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from contextlib import closing
+import secrets
+import socket
 from typing import Optional
 import unittest
 
 from libcloud.common.types import InvalidCredsError
-from libcloud.storage.types import ContainerDoesNotExistError, ObjectDoesNotExistError
+from libcloud.storage.providers import get_driver
+from libcloud.storage.types import (
+    ContainerDoesNotExistError,
+    ObjectDoesNotExistError,
+    Provider,
+)
+import pytest
 
 from swh.objstorage.backends.libcloud import CloudObjStorage
 from swh.objstorage.exc import Error
+from swh.objstorage.factory import get_objstorage
 from swh.objstorage.objstorage import decompressors
 
 from .objstorage_testing import ObjStorageTestFixture
 
 API_KEY = "API_KEY"
 API_SECRET_KEY = "API SECRET KEY"
 CONTAINER_NAME = "test_container"
@@ -129,14 +139,18 @@
             with self.assertRaises(Error) as e:
                 self.storage.check(obj_id)
         else:
             with self.assertRaises(Error) as e:
                 self.storage.get(obj_id)
             assert "trailing data" in e.exception.args[0]
 
+    @pytest.mark.skip("makes no sense to test this for the mocked libcloud")
+    def test_download_url(self):
+        pass
+
 
 class TestCloudObjStorageBz2(TestCloudObjStorage):
     compression = "bz2"
 
 
 class TestCloudObjStorageGzip(TestCloudObjStorage):
     compression = "gzip"
@@ -158,7 +172,68 @@
         self.storage.add(content, obj_id=obj_id)
 
         container = self.storage.driver.containers[CONTAINER_NAME]
         object_path = self.storage._object_path(obj_id)
 
         assert object_path.startswith(self.path_prefix + "/")
         assert object_path in container
+
+
+def _find_free_port():
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
+        s.bind(("", 0))
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return s.getsockname()[1]
+
+
+try:
+    from moto.server import ThreadedMotoServer
+except ImportError:
+    moto_available = False
+else:
+    moto_available = True
+
+
+@pytest.mark.skipif(not moto_available, reason="moto package is not installed")
+class TestMotoS3CloudObjStorage(ObjStorageTestFixture, unittest.TestCase):
+    compression = "none"
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        cls.key = "testing"
+        cls.secret = "testing"
+        cls.host = "localhost"
+        cls.port = _find_free_port()
+        cls.server = ThreadedMotoServer(port=cls.port)
+        cls.server.start()
+        cls.container_name = secrets.token_hex(10)
+        driver_cls = get_driver(Provider.S3)
+        cls.driver = driver_cls(
+            key=cls.key, secret=cls.secret, secure=False, host=cls.host, port=cls.port
+        )
+        cls.container = cls.driver.create_container(container_name=cls.container_name)
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+        cls.driver.delete_container(cls.container)
+        cls.server.stop()
+
+    def setUp(self):
+        super().setUp()
+
+        self.storage = get_objstorage(
+            "s3",
+            container_name=self.container_name,
+            compression=self.compression,
+            key=self.key,
+            secret=self.secret,
+            secure=False,
+            host=self.host,
+            port=self.port,
+        )
+
+    def tearDown(self):
+        super().tearDown()
+        for obj in self.driver.list_container_objects(self.container):
+            self.driver.delete_object(obj)
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_http.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import pytest
+import requests
 import requests_mock
 from requests_mock.contrib import fixture
 
+from swh.model import hashutil
 from swh.objstorage import exc
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.objstorage import compute_hash
 
 
-def build_objstorage():
+def build_objstorage(multi_hash=False):
     """Build an HTTPReadOnlyObjStorage suitable for tests
 
     this instancaite 2 ObjStorage, one HTTPReadOnlyObjStorage (the "front" one
     being under test), and one InMemoryObjStorage (which actually stores the
     test content), and install a request mock fixture to route HTTP requests
     from the HTTPReadOnlyObjStorage to query the InMemoryStorage.
 
     Also fills the backend storage with a 100 objects.
     """
     sto_back = get_objstorage(cls="memory")
     objids = []
     for i in range(100):
         content = f"some content {i}".encode()
-        obj_id = compute_hash(content)
+        if multi_hash:
+            obj_id = hashutil.MultiHash.from_data(content).digest()
+        else:
+            obj_id = compute_hash(content)
         objids.append(obj_id)
         sto_back.add(content, obj_id=obj_id)
 
     url = "http://127.0.0.1/content/"
     sto_front = get_objstorage(cls="http", url=url)
     mock = fixture.Fixture()
     mock.setUp()
@@ -52,16 +57,17 @@
 
     mock.register_uri(requests_mock.GET, requests_mock.ANY, content=get_cb)
     mock.register_uri(requests_mock.HEAD, requests_mock.ANY, content=head_cb)
 
     return sto_front, sto_back, objids
 
 
-def test_http_objstorage():
-    sto_front, sto_back, objids = build_objstorage()
+@pytest.mark.parametrize("multi_hash", [False, True])
+def test_http_objstorage(multi_hash):
+    sto_front, sto_back, objids = build_objstorage(multi_hash)
 
     for objid in objids:
         assert objid in sto_front
         assert sto_front.get(objid) == sto_back.get(objid)
         assert sto_front.get(objid).decode().startswith("some content ")
 
 
@@ -74,16 +80,17 @@
 def test_http_objstorage_get_missing():
     sto_front, sto_back, objids = build_objstorage()
 
     with pytest.raises(exc.ObjNotFoundError):
         sto_front.get(b"\x00" * 20)
 
 
-def test_http_objstorage_check():
-    sto_front, sto_back, objids = build_objstorage()
+@pytest.mark.parametrize("multi_hash", [False, True])
+def test_http_objstorage_check(multi_hash):
+    sto_front, sto_back, objids = build_objstorage(multi_hash)
     for objid in objids:
         assert sto_front.check(objid) is None  # no Exception means OK
 
     # create an invalid object in the in-memory objstorage
     invalid_content = b"p0wn3d content"
     fake_objid = "\x01" * 20
     sto_back.add(invalid_content, fake_objid)
@@ -115,7 +122,17 @@
         iter(sto_front)
 
 
 def test_http_cannonical_url():
     url = "http://127.0.0.1/content"
     sto = get_objstorage(cls="http", url=url)
     assert sto.root_path == url + "/"
+
+
+@pytest.mark.parametrize("multi_hash", [False, True])
+def test_http_objstorage_download_url(multi_hash):
+    sto_front, sto_back, objids = build_objstorage(multi_hash)
+
+    for objid in objids:
+        assert objid in sto_front
+        response = requests.get(sto_front.download_url(objid))
+        assert response.text.startswith("some content ")
```

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_in_memory.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_multiplexer.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_multiplexer.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_noop.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_objstorage_winery.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_pathslicer.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_readonly_filter.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_readonly_filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/test_server.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/winery_benchmark.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/winery_benchmark.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/tests/winery_testing_helpers.py` & `swh.objstorage-2.3.0/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh/objstorage/utils.py` & `swh.objstorage-2.3.0/swh/objstorage/utils.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/swh.objstorage.egg-info/PKG-INFO` & `swh.objstorage-2.3.0/swh.objstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.2.0
+Version: 2.3.0
 Summary: Software Heritage Object Storage
 Home-page: https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh.objstorage-2.2.0/swh.objstorage.egg-info/SOURCES.txt` & `swh.objstorage-2.3.0/swh.objstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/tox.ini` & `swh.objstorage-2.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/README.md` & `swh.objstorage-2.3.0/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/bootstrap.yml` & `swh.objstorage-2.3.0/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/build-vms.sh` & `swh.objstorage-2.3.0/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/ceph.yml` & `swh.objstorage-2.3.0/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/fed4fire.rspec` & `swh.objstorage-2.3.0/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/fed4fire.sh` & `swh.objstorage-2.3.0/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/grid5000.yml` & `swh.objstorage-2.3.0/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/inventory/hosts.yml` & `swh.objstorage-2.3.0/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen.py` & `swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh.objstorage-2.3.0/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/osd.yml` & `swh.objstorage-2.3.0/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/remote-tox.sh` & `swh.objstorage-2.3.0/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/render-stats.py` & `swh.objstorage-2.3.0/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/rw.yml` & `swh.objstorage-2.3.0/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.2.0/winery-test-environment/tests.yml` & `swh.objstorage-2.3.0/winery-test-environment/tests.yml`

 * *Files identical despite different names*

