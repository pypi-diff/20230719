# Comparing `tmp/tiledbsoma-1.2.7.tar.gz` & `tmp/tiledbsoma-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.2.7.tar", last modified: Wed Jun 21 16:57:14 2023, max compression
+gzip compressed data, was "tiledbsoma-1.3.0.tar", last modified: Tue Jul 18 21:21:53 2023, max compression
```

## Comparing `tiledbsoma-1.2.7.tar` & `tiledbsoma-1.3.0.tar`

### file list

```diff
@@ -1,133 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5107 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.619202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.619202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10181 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15637 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.h
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_soma_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.627203 tiledbsoma-1.2.7/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    11110 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.623202 tiledbsoma-1.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7213 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33854 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11918 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    56332 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-06-21 16:57:11.000000 tiledbsoma-1.2.7/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 16:57:14.631203 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5107 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-21 16:57:14.000000 tiledbsoma-1.2.7/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-06-21 16:57:12.000000 tiledbsoma-1.2.7/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-18 21:21:50.000000 tiledbsoma-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5262 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-07-18 21:21:50.000000 tiledbsoma-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.810552 tiledbsoma-1.3.0/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-18 21:21:50.000000 tiledbsoma-1.3.0/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.810552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.810552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    11138 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.802552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.802552 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7897 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     8821 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7172 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    14575 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    16193 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    18139 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4413 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6905 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_object.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.814553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.818553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     7271 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.818553 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_soma_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    13593 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     4222 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.818553 tiledbsoma-1.3.0/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11110 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.806552 tiledbsoma-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33885 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11655 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62737 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7767 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 21:21:53.822553 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5262 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-18 21:21:53.000000 tiledbsoma-1.3.0/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-07-18 21:21:51.000000 tiledbsoma-1.3.0/version.py
```

### Comparing `tiledbsoma-1.2.7/PKG-INFO` & `tiledbsoma-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.7
+Version: 1.3.0
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
 Description: # Overview
         
         This is a Python implementation of the [SOMA API specification](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md) for interacting with the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
         
         # Installation
         
-        ## Using pip
+        TileDB-SOMA is available on [PyPI](https://pypi.org/project/tiledbsoma/) and [Conda](https://anaconda.org/tiledb/tiledbsoma-py), and can be installed via `pip` or `mamba` as indicated below.
         
-        This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can install using `pip`:
+        ```bash
+        python -m pip install tiledbsoma
+        ```
         
-        ```shell
-        $ python -m pip install tiledbsoma
+        ```bash
+        mamba install -c conda-forge -c tiledb tiledbsoma-py
         ```
         
         To install a specific version:
         
         ```shell
         $ python -m pip install git+https://github.com/single-cell-data/TileDB-SOMA.git@0.0.6#subdirectory=apis/python
         ```
```

### Comparing `tiledbsoma-1.2.7/README.md` & `tiledbsoma-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Overview
 
 This is a Python implementation of the [SOMA API specification](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md) for interacting with the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
 
 # Installation
 
-## Using pip
+TileDB-SOMA is available on [PyPI](https://pypi.org/project/tiledbsoma/) and [Conda](https://anaconda.org/tiledb/tiledbsoma-py), and can be installed via `pip` or `mamba` as indicated below.
 
-This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can install using `pip`:
+```bash
+python -m pip install tiledbsoma
+```
 
-```shell
-$ python -m pip install tiledbsoma
+```bash
+mamba install -c conda-forge -c tiledb tiledbsoma-py
 ```
 
 To install a specific version:
 
 ```shell
 $ python -m pip install git+https://github.com/single-cell-data/TileDB-SOMA.git@0.0.6#subdirectory=apis/python
 ```
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     # loaded by the Python and R tiledbsoma packages. Those packages -also- use TileDB-Py and
     # TileDB-R, each of which links their own 'copy' of TileDB Embedded, whose version we don't
     # control here. Ideally the TileDB Embedded versions should match! The show_package_versions()
     # helper function in each package can help to diagnose any mismatch.
     # NB When updating the pinned URLs here, please also update in file apis/r/tools/get_tarball.R
     if(DOWNLOAD_TILEDB_PREBUILT)
         if (WIN32) # Windows
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-windows-x86_64-2.15.2-90f30eb.zip")
-          SET(DOWNLOAD_SHA1 "1adc1ffa3c6c0f637bcb68d3cd278b0bee597b9c")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-windows-x86_64-2.16.0-d682dd0.zip")
+          SET(DOWNLOAD_SHA1 "82a79fda3daecc46ae24c86a328e52184460dabe")
         elseif(APPLE) # OSX
 
           # Status quo as of 2023-05-18:
           # * GitHub Actions does not have MacOS arm64 hardware available -- tracked at
           #   https://github.com/github/roadmap/issues/528
           # * The best we can do is cross-compile for arm64 while actually running on x86_64
           # * When we're invoked from python setup.py:
@@ -72,30 +72,30 @@
           #   o We must download the tiledb artifacts for the cross-compile architecture (x86_64 or arm64)
           #   o Therefore we must respect CMAKE_OSX_ARCHITECTURES not CMAKE_SYSTEM_PROCESSOR
           # * When we're invoked from R configure and src/Makevars.in:
           #   o CMAKE_OSX_ARCHITECTURES is unset
           #   o CMAKE_SYSTEM_PROCESSOR is x86_64
 
           if (CMAKE_OSX_ARCHITECTURES STREQUAL x86_64)
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-x86_64-2.15.2-90f30eb.tar.gz")
-            SET(DOWNLOAD_SHA1 "616b9ab508d1233d3bc3d6a2a7b1c42c8098f38a")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-x86_64-2.16.0-d682dd0.tar.gz")
+            SET(DOWNLOAD_SHA1 "d7b22fa3cb9cbe131734d9f18beb3362908aeccf")
           elseif (CMAKE_OSX_ARCHITECTURES STREQUAL arm64)
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-arm64-2.15.2-90f30eb.tar.gz")
-            SET(DOWNLOAD_SHA1 "882eadcc256f95a5c91094407770799a8bd4e759")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-arm64-2.16.0-d682dd0.tar.gz")
+            SET(DOWNLOAD_SHA1 "09c62e3211e5277263c1545d74d698d450ebcb77")
           elseif (CMAKE_SYSTEM_PROCESSOR MATCHES "(x86_64)|(AMD64|amd64)|(^i.86$)")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-x86_64-2.15.2-90f30eb.tar.gz")
-            SET(DOWNLOAD_SHA1 "616b9ab508d1233d3bc3d6a2a7b1c42c8098f38a")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-x86_64-2.16.0-d682dd0.tar.gz")
+            SET(DOWNLOAD_SHA1 "d7b22fa3cb9cbe131734d9f18beb3362908aeccf")
           elseif (CMAKE_SYSTEM_PROCESSOR MATCHES "^aarch64" OR CMAKE_SYSTEM_PROCESSOR MATCHES "^arm")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-arm64-2.15.2-90f30eb.tar.gz")
-            SET(DOWNLOAD_SHA1 "882eadcc256f95a5c91094407770799a8bd4e759")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-macos-arm64-2.16.0-d682dd0.tar.gz")
+            SET(DOWNLOAD_SHA1 "09c62e3211e5277263c1545d74d698d450ebcb77")
           endif()
 
         else() # Linux
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-linux-x86_64-2.15.2-90f30eb.tar.gz")
-          SET(DOWNLOAD_SHA1 "33ae11d507dc7bec82fbdfbd8e2b2e13cff16b89")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.16.0/tiledb-linux-x86_64-2.16.0-d682dd0.tar.gz")
+          SET(DOWNLOAD_SHA1 "be0bfd5512c159b960988a4bd41366e9f020115f")
         endif()
 
         ExternalProject_Add(ep_tiledb
                 PREFIX "externals"
                 URL ${DOWNLOAD_URL}
                 URL_HASH SHA1=${DOWNLOAD_SHA1}
                 CONFIGURE_COMMAND ""
@@ -109,16 +109,16 @@
                 LOG_CONFIGURE FALSE
                 LOG_BUILD FALSE
                 LOG_INSTALL FALSE
                 )
     else() # Build from source
         ExternalProject_Add(ep_tiledb
           PREFIX "externals"
-          URL "https://github.com/TileDB-Inc/TileDB/archive/2.15.2.zip"
-          URL_HASH SHA1=7443415b9f3081e87adaa638dea6e2d277fbb904
+          URL "https://github.com/TileDB-Inc/TileDB/archive/2.16.0.zip"
+          URL_HASH SHA1=c2779f931c84d931e5fca6dc3a858e66fc542276
           DOWNLOAD_NAME "tiledb.zip"
           CMAKE_ARGS
             -DCMAKE_INSTALL_PREFIX=${EP_INSTALL_PREFIX}
             -DCMAKE_PREFIX_PATH=${EP_INSTALL_PREFIX}
             -DTILEDB_S3=${TILEDB_S3}
             -DTILEDB_AZURE=${TILEDB_AZURE}
             -DTILEDB_GCS=${TILEDB_GCS}
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 # ###########################################################
 # Common object library
 # ###########################################################
 add_library(TILEDB_SOMA_OBJECTS OBJECT
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/utils/column_buffer.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_dataframe.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/column_buffer.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.cc
 
   # TODO: uncomment when thread_pool is enabled
   # ${CMAKE_CURRENT_SOURCE_DIR}/external/src/thread_pool/thread_pool.cc
@@ -167,40 +168,42 @@
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_sparse_ndarray.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/logger_public.h
 # )
 
 install(FILES 
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/logger_public.h
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.h
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/array_buffers.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/column_buffer.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.h 
-  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.h
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_object.h 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_dataframe.h 
   DESTINATION "include/tiledbsoma/soma"
 )
 
 install(FILES 
   ${CMAKE_CURRENT_SOURCE_DIR}/tiledbsoma/tiledbsoma
   DESTINATION "include/tiledbsoma"
 )
 
 install(FILES
-  ${CMAKE_CURRENT_SOURCE_DIR}/utils/array_buffers.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/arrow_adapter.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/carrow.h  
-  ${CMAKE_CURRENT_SOURCE_DIR}/utils/column_buffer.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/common.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.h
   DESTINATION "include/tiledbsoma/utils"
 )
 
 install(FILES 
   ${CMAKE_CURRENT_SOURCE_DIR}/external/include/span/span.hpp
-  DESTINATION "include/tiledbsoma/utils/span"
+  DESTINATION "include/tiledbsoma/soma/span"
 )
 
 
 # ###########################################################
 # API symbol exports
 # ###########################################################
 include(GenerateExportHeader)
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/logger_public.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 name));
         } else {
             columns_.push_back(name);
         }
     }
 }
 
-void ManagedQuery::submit() {
+void ManagedQuery::submit_read() {
     // Throw error if submit is called again before reading the results
     if (query_submitted_) {
         throw TileDBSOMAError(fmt::format(
             "[ManagedQuery][{}] read results before calling submit again",
             name_));
     }
 
@@ -154,14 +154,18 @@
     // Do not submit if the query contains only empty ranges
     if (!is_empty_query()) {
         query_->submit();
     }
     query_submitted_ = true;
 }
 
+void ManagedQuery::submit_write() {
+    query_->submit();
+}
+
 std::shared_ptr<ArrayBuffers> ManagedQuery::results() {
     if (is_empty_query()) {
         query_submitted_ = false;
         return buffers_;
     }
 
     if (!query_submitted_) {
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
  * @file   managed_query.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2022-2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -23,28 +23,28 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This declares the managed query API
+ *   This declares the managed query API.
  */
 
 #ifndef MANAGED_QUERY_H
 #define MANAGED_QUERY_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 #include <unordered_set>
 
 #include <tiledb/tiledb>
 
-#include "../utils/array_buffers.h"
-#include "../utils/column_buffer.h"
 #include "../utils/common.h"
+#include "array_buffers.h"
+#include "column_buffer.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 class ManagedQuery {
    public:
@@ -163,18 +163,124 @@
      * @param layout A tiledb_layout_t constant
      */
     void set_layout(tiledb_layout_t layout) {
         query_->set_layout(layout);
     }
 
     /**
-     * @brief Submit the query.
+     * @brief Set column data for write query.
+     *
+     * @param column_name Column name
+     * @param buff Buffer array pointer with elements of the column type.
+     * @param nelements Number of array elements in buffer
+     */
+    void set_column_data(
+        std::string column_name, std::shared_ptr<ColumnBuffer> column_buffer) {
+        if (array_->schema().array_type() == TILEDB_SPARSE ||
+            schema_->has_attribute(column_name)) {
+            auto data = column_buffer->data<std::byte>();
+            query_->set_data_buffer(
+                column_name, (void*)data.data(), data.size_bytes());
+        } else {
+            switch (column_buffer->type()) {
+                case TILEDB_STRING_ASCII:
+                case TILEDB_STRING_UTF8:
+                case TILEDB_CHAR:
+                case TILEDB_BLOB:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<std::string>()[0],
+                        column_buffer->data<std::string>()[1]);
+                    break;
+                case TILEDB_FLOAT32:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<float>()[0],
+                        column_buffer->data<float>()[1]);
+                    break;
+                case TILEDB_FLOAT64:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<double>()[0],
+                        column_buffer->data<double>()[1]);
+                    break;
+                case TILEDB_UINT8:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<uint8_t>()[0],
+                        column_buffer->data<uint8_t>()[1]);
+                    break;
+                case TILEDB_INT8:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<int8_t>()[0],
+                        column_buffer->data<int8_t>()[1]);
+                    break;
+                case TILEDB_UINT16:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<uint16_t>()[0],
+                        column_buffer->data<uint16_t>()[1]);
+                    break;
+                case TILEDB_INT16:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<int16_t>()[0],
+                        column_buffer->data<int16_t>()[1]);
+                    break;
+                case TILEDB_UINT32:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<uint32_t>()[0],
+                        column_buffer->data<uint32_t>()[1]);
+                    break;
+                case TILEDB_INT32:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<int32_t>()[0],
+                        column_buffer->data<int32_t>()[1]);
+                    break;
+                case TILEDB_UINT64:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<uint64_t>()[0],
+                        column_buffer->data<uint64_t>()[1]);
+                    break;
+                case TILEDB_INT64:
+                case TILEDB_TIME_SEC:
+                case TILEDB_TIME_MS:
+                case TILEDB_TIME_US:
+                case TILEDB_TIME_NS:
+                case TILEDB_DATETIME_SEC:
+                case TILEDB_DATETIME_MS:
+                case TILEDB_DATETIME_US:
+                case TILEDB_DATETIME_NS:
+                    subarray_->add_range(
+                        column_name,
+                        column_buffer->data<int64_t>()[0],
+                        column_buffer->data<int64_t>()[1]);
+                    break;
+                default:
+                    break;
+            }
+            query_->set_subarray(*subarray_);
+        }
+    }
+
+    /**
+     * @brief Submit the read query.
+     *
+     */
+    void submit_read();
+
+    /**
+     * @brief Submit the write query.
      *
      */
-    void submit();
+    void submit_write();
 
     /**
      * @brief Check if the query is complete.
      *
      * If `query_status_only` is true, return true if the query status is
      * complete.
      *
@@ -279,14 +385,23 @@
      *
      * @return true if the query contains only empty ranges.
      */
     bool is_empty_query() {
         return subarray_range_set_ && subarray_range_empty_;
     }
 
+    /**
+     * @brief Return the query type.
+     *
+     * @return TILEDB_READ or TILEDB_WRITE
+     */
+    tiledb_query_type_t query_type() const {
+        return query_->query_type();
+    }
+
    private:
     //===================================================================
     //= private non-static
     //===================================================================
 
     /**
      * @brief Check if column name is contained in the query results.
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
  * @file   soma_array.cc
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2022-2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -37,23 +37,37 @@
 namespace tiledbsoma {
 using namespace tiledb;
 
 //===================================================================
 //= public static
 //===================================================================
 
+void SOMAArray::create(
+    std::shared_ptr<Context> ctx,
+    std::string_view uri,
+    ArraySchema schema,
+    std::string soma_object_type) {
+    Array::create(std::string(uri), schema);
+    auto array = Array(*ctx, std::string(uri), TILEDB_WRITE);
+    array.put_metadata(
+        "soma_object_type", TILEDB_STRING_UTF8, 1, soma_object_type.c_str());
+    array.close();
+}
+
 std::unique_ptr<SOMAArray> SOMAArray::open(
     tiledb_query_type_t mode,
     std::string_view uri,
     std::string_view name,
     std::map<std::string, std::string> platform_config,
     std::vector<std::string> column_names,
     std::string_view batch_size,
     std::string_view result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
+    LOG_DEBUG(
+        fmt::format("[SOMAArray] static method 'cfg' opening array '{}'", uri));
     return std::make_unique<SOMAArray>(
         mode,
         uri,
         name,
         std::make_shared<Context>(Config(platform_config)),
         column_names,
         batch_size,
@@ -66,14 +80,16 @@
     std::shared_ptr<Context> ctx,
     std::string_view uri,
     std::string_view name,
     std::vector<std::string> column_names,
     std::string_view batch_size,
     std::string_view result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
+    LOG_DEBUG(
+        fmt::format("[SOMAArray] static method 'ctx' opening array '{}'", uri));
     return std::make_unique<SOMAArray>(
         mode,
         uri,
         name,
         ctx,
         column_names,
         batch_size,
@@ -105,28 +121,37 @@
             if (timestamp->first > timestamp->second) {
                 throw std::invalid_argument("timestamp start > end");
             }
             arr_->set_open_timestamp_start(timestamp->first);
             arr_->set_open_timestamp_end(timestamp->second);
             arr_->close();
             arr_->open(mode);
+            LOG_DEBUG(fmt::format(
+                "[SOMAArray] timestamp_start = {}",
+                arr_->open_timestamp_start()));
+            LOG_DEBUG(fmt::format(
+                "[SOMAArray] timestamp_end = {}", arr_->open_timestamp_end()));
         }
         mq_ = std::make_unique<ManagedQuery>(arr_, name);
-        LOG_DEBUG(
-            fmt::format("timestamp_start = {}", arr_->open_timestamp_start()));
-        LOG_DEBUG(
-            fmt::format("timestamp_end = {}", arr_->open_timestamp_end()));
     } catch (const std::exception& e) {
         throw TileDBSOMAError(
             fmt::format("Error opening array: '{}'\n  {}", uri_, e.what()));
     }
 
     reset(column_names, batch_size, result_order);
 }
 
+const std::string& SOMAArray::uri() const {
+    return uri_;
+};
+
+std::shared_ptr<Context> SOMAArray::ctx() {
+    return ctx_;
+};
+
 void SOMAArray::open(
     tiledb_query_type_t mode,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
     arr_->open(mode);
     if (timestamp) {
         if (timestamp->first > timestamp->second) {
             throw std::invalid_argument("timestamp start > end");
@@ -172,15 +197,19 @@
 
     first_read_next_ = true;
     submitted_ = false;
 }
 
 void SOMAArray::submit() {
     // Submit the query
-    mq_->submit();
+    if (mq_->query_type() == TILEDB_READ) {
+        mq_->submit_read();
+    } else {
+        mq_->reset();
+    }
     submitted_ = true;
 }
 
 std::optional<std::shared_ptr<ArrayBuffers>> SOMAArray::read_next() {
     if (!submitted_) {
         throw TileDBSOMAError(
             "[SOMAArray] submit must be called before read_next");
@@ -194,20 +223,32 @@
 
     // If the query is complete, return `std::nullopt`.
     if (mq_->is_complete()) {
         return std::nullopt;
     }
 
     // Submit the query
-    mq_->submit();
+    mq_->submit_read();
 
     // Return the results, possibly incomplete
     return mq_->results();
 }
 
+void SOMAArray::write(std::shared_ptr<ArrayBuffers> buffers) {
+    if (mq_->query_type() != TILEDB_WRITE) {
+        throw TileDBSOMAError("[SOMAArray] array must be opened in write mode");
+    }
+
+    for (auto col_name : buffers->names()) {
+        mq_->set_column_data(col_name, buffers->at(col_name));
+    }
+
+    mq_->submit_write();
+}
+
 uint64_t SOMAArray::nnz() {
     // Verify array is sparse
     if (mq_->schema()->array_type() != TILEDB_SPARSE) {
         throw TileDBSOMAError(
             "[SOMAArray] nnz is only supported for sparse arrays");
     }
 
@@ -329,15 +370,15 @@
     }
 
     return total_cell_num;
 }
 
 std::vector<int64_t> SOMAArray::shape() {
     std::vector<int64_t> result;
-    auto dimensions = this->schema().get()->domain().dimensions();
+    auto dimensions = mq_->schema()->domain().dimensions();
 
     for (const auto& dim : dimensions) {
         switch (dim.type()) {
             case TILEDB_UINT8:
                 result.push_back(
                     dim.domain<uint8_t>().second - dim.domain<uint8_t>().first +
                     1);
@@ -403,14 +444,27 @@
                 throw TileDBSOMAError("Dimension must be integer type.");
         }
     }
 
     return result;
 }
 
+uint64_t SOMAArray::ndim() const {
+    return this->schema().get()->domain().ndim();
+}
+
+std::vector<std::string> SOMAArray::dimension_names() const {
+    std::vector<std::string> result;
+    auto dimensions = this->schema().get()->domain().dimensions();
+    for (const auto& dim : dimensions) {
+        result.push_back(dim.name());
+    }
+    return result;
+}
+
 void SOMAArray::set_metadata(
     const std::string& key,
     tiledb_datatype_t value_type,
     uint32_t value_num,
     const void* value) {
     arr_->put_metadata(key, value_type, value_num, value);
 }
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
  * @file   soma_array.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2022-2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -23,15 +23,15 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This declares the SOMAArray
+ *   This declares the SOMAArray class.
  */
 
 #ifndef SOMA_ARRAY
 #define SOMA_ARRAY
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
@@ -47,14 +47,27 @@
 class SOMAArray {
    public:
     //===================================================================
     //= public static
     //===================================================================
 
     /**
+     * @brief Create a SOMAArray object at the given URI.
+     *
+     * @param ctx TileDB context
+     * @param uri URI to create the SOMAArray
+     * @param schema TileDB ArraySchema
+     */
+    static void create(
+        std::shared_ptr<Context> ctx,
+        std::string_view uri,
+        ArraySchema schema,
+        std::string soma_object_type);
+
+    /**
      * @brief Open an array at the specified URI and return SOMAArray
      * object.
      *
      * @param mode TILEDB_READ or TILEDB_WRITE
      * @param uri URI of the array
      * @param name Name of the array
      * @param platform_config Config parameter dictionary
@@ -123,14 +136,28 @@
 
     SOMAArray() = delete;
     SOMAArray(const SOMAArray&) = delete;
     SOMAArray(SOMAArray&&) = default;
     ~SOMAArray() = default;
 
     /**
+     * @brief Get URI of the SOMAArray.
+     *
+     * @return std::string URI
+     */
+    const std::string& uri() const;
+
+    /**
+     * @brief Get URI of the SOMAArray.
+     *
+     * @return std::string URI
+     */
+    std::shared_ptr<Context> ctx();
+
+    /**
      * Open the SOMAArray object.
      *
      * @param mode TILEDB_READ or TILEDB_WRITE
      * @param timestamp Timestamp
      */
     void open(
         tiledb_query_type_t mode,
@@ -284,25 +311,62 @@
 
     /**
      * @brief Read the next chunk of results from the query. If all results have
      * already been read, std::nullopt is returned.
      *
      * An example use model:
      *
-     *   auto reader = SOMAArray::open(uri);
+     *   auto reader = SOMAArray::open(TILEDB_READ, uri);
      *   reader->submit();
      *   while (auto batch = x_data->read_next()) {
      *       ...process batch ...
      *   }
      *
      * @return std::optional<std::shared_ptr<ArrayBuffers>>
      */
     std::optional<std::shared_ptr<ArrayBuffers>> read_next();
 
     /**
+     * @brief Set the write data for a column.
+     *
+     * @param column_name Column name
+     * @param buff Buffer array pointer with elements of the column type.
+     * @param nelements Number of array elements in buffer
+     */
+    void set_column_data(
+        std::string_view column_name,
+        std::shared_ptr<ColumnBuffer> column_buffer) {
+        mq_->set_column_data(std::string(column_name), column_buffer);
+    }
+
+    /**
+     * @brief Write ArrayBuffers data to the array.
+     *
+     * An example use model:
+     *
+     *   auto writer = SOMAArray::open(TILEDB_WRITE, uri);
+     *
+     *   std::vector<int> att{0, 1, 2, 3, 4, 5};
+     *   std::vector<int> dim{0, 1, 2, 3, 4, 5};
+     *
+     *   auto schema = *soma_array->schema();
+     *   auto array_buffer = std::make_shared<ArrayBuffers>();
+     *   array_buffer->emplace("att", ColumnBuffer::create(schema, "att", att));
+     *   array_buffer->emplace("dim", ColumnBuffer::create(schema, "dim", dim));
+     *
+     *   std::vector<int> x(10, 1);
+     *   writer->submit();
+     *   writer->write(array_buffer);
+     *   writer->close();
+     *
+     * @param buffers The ArrayBuffers to write to the array
+     */
+    void write(std::shared_ptr<ArrayBuffers> buffers);
+
+    /**
      * @brief Check if the query is complete.
      *
      * If `query_status_only` is true, return true if the query status is
      * complete.
      *
      * If `query_status_only` is false, return true if the query status
      * is complete or if the query is empty (no ranges have been added to the
@@ -333,38 +397,62 @@
      * @return size_t Total number of cells read
      */
     size_t total_num_cells() {
         return mq_->total_num_cells();
     }
 
     /**
+     * @brief Return whether next read is the initial read, or a subsequent
+     * read of a previous incomplete query.
+     *
+     * @return bool Logical value if initial read or not
+     */
+    bool is_initial_read() {
+        return first_read_next_;
+    }
+
+    /**
      * @brief Get the total number of unique cells in the array.
      *
      * @return uint64_t Total number of unique cells
      */
     uint64_t nnz();
 
     /**
      * @brief Get the schema of the array.
      *
      * @return std::shared_ptr<ArraySchema> Schema
      */
-    std::shared_ptr<ArraySchema> schema() {
+    std::shared_ptr<ArraySchema> schema() const {
         return mq_->schema();
     }
 
     /**
      * @brief Get the capacity of each dimension.
      *
      * @return A vector with length equal to the number of dimensions; each
      * value in the vector is the capcity of each dimension.
      */
     std::vector<int64_t> shape();
 
     /**
+     * @brief Get the number of dimensions.
+     *
+     * @return uint64_t Number of dimensions.
+     */
+    uint64_t ndim() const;
+
+    /**
+     * @brief Get the name of each dimensions.
+     *
+     * @return std::vector<std::string> Name of each dimensions.
+     */
+    std::vector<std::string> dimension_names() const;
+
+    /**
      * Set metadata key-value items to an open array. The array must
      * opened in WRITE mode, otherwise the function will error out.
      *
      * @param key The key of the metadata item to be added. UTF-8 encodings
      *     are acceptable.
      * @param value_type The datatype of the value.
      * @param value_num The value may consist of more than one items of the
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/soma/soma_group.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/soma_group.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files 6% similar despite different names*

```diff
@@ -39,18 +39,20 @@
 // #include "soma_dense_ndarray.h"
 // #include "soma_experiment.h"
 // #include "soma_measurement.h"
 // #include "soma_object.h"
 // #include "soma_sparse_ndarray.h"
 
 #include "utils/arrow_adapter.h"
-#include "utils/array_buffers.h"
-#include "utils/column_buffer.h"
 #include "utils/common.h"
 #include "utils/stats.h"
 #include "utils/version.h"
 #include "soma/logger_public.h"
 #include "soma/managed_query.h"
+#include "soma/array_buffers.h"
+#include "soma/column_buffer.h"
 #include "soma/soma_array.h"
 #include "soma/soma_group.h"
+#include "soma/soma_object.h"
+#include "soma/soma_dataframe.h"
 
 #endif
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/array_buffers.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/array_buffers.h`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,17 @@
 #ifndef ARRAY_BUFFERS_H
 #define ARRAY_BUFFERS_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <tiledb/tiledb>
 
+#include "../utils/common.h"
+#include "../utils/logger.h"
 #include "column_buffer.h"
-#include "common.h"
-#include "logger.h"
-#include "span/span.hpp"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 class ArrayBuffers {
    public:
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #ifndef ARROW_ADAPTER_H
 #define ARROW_ADAPTER_H
 
 #include <tiledb/tiledb>
-#include "../utils/column_buffer.h"
+#include "../soma/column_buffer.h"
 #include "../utils/logger.h"
 #ifndef ARROW_SCHEMA_AND_ARRAY_DEFINED
 #include "carrow.h"
 #endif
 
 // https://arrow.apache.org/docs/format/CDataInterface.html
 // https://arrow.apache.org/docs/format/Columnar.html#buffer-listing-for-each-layout
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/carrow.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.cc`

 * *Files 15% similar despite different names*

```diff
@@ -27,59 +27,60 @@
  *
  * @section DESCRIPTION
  *
  * This file defines the a ColumBuffer class.
  */
 
 #include "column_buffer.h"
-#include "array_buffers.h"
-#include "common.h"
-#include "logger.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 //===================================================================
 //= public static
 //===================================================================
 
 std::shared_ptr<ColumnBuffer> ColumnBuffer::create(
     std::shared_ptr<Array> array, std::string_view name) {
+    return ColumnBuffer::create(array->schema(), name);
+}
+
+std::shared_ptr<ColumnBuffer> ColumnBuffer::create(
+    ArraySchema schema, std::string_view name) {
     auto name_str = std::string(name);  // string for TileDB API
-    auto schema = array->schema();
 
     if (schema.has_attribute(name_str)) {
         auto attr = schema.attribute(name_str);
+        auto type = attr.type();
         bool is_var = attr.cell_val_num() == TILEDB_VAR_NUM;
         bool is_nullable = attr.nullable();
 
         if (!is_var && attr.cell_val_num() != 1) {
             throw TileDBSOMAError(
                 "[ColumnBuffer] Values per cell > 1 is not supported: " +
                 name_str);
         }
 
-        return ColumnBuffer::alloc(
-            array, attr.name(), attr.type(), is_var, is_nullable);
+        return ColumnBuffer::alloc(schema, name_str, type, is_var, is_nullable);
 
     } else if (schema.domain().has_dimension(name_str)) {
         auto dim = schema.domain().dimension(name_str);
+        auto type = dim.type();
         bool is_var = dim.cell_val_num() == TILEDB_VAR_NUM ||
                       dim.type() == TILEDB_STRING_ASCII ||
                       dim.type() == TILEDB_STRING_UTF8;
 
         if (!is_var && dim.cell_val_num() != 1) {
             throw TileDBSOMAError(
                 "[ColumnBuffer] Values per cell > 1 is not supported: " +
                 name_str);
         }
 
-        return ColumnBuffer::alloc(
-            array, dim.name(), dim.type(), is_var, false);
+        return ColumnBuffer::alloc(schema, name_str, type, is_var, false);
     }
 
     throw TileDBSOMAError("[ColumnBuffer] Column name not found: " + name_str);
 }
 
 void ColumnBuffer::to_bitmap(tcb::span<uint8_t> bytemap) {
     int i_dst = 0;
@@ -183,37 +184,37 @@
 }
 
 //===================================================================
 //= private static
 //===================================================================
 
 std::shared_ptr<ColumnBuffer> ColumnBuffer::alloc(
-    std::shared_ptr<Array> array,
+    ArraySchema schema,
     std::string_view name,
     tiledb_datatype_t type,
     bool is_var,
     bool is_nullable) {
     // Set number of bytes for the data buffer. Override with a value from
     // the config if present.
     auto num_bytes = DEFAULT_ALLOC_BYTES;
-    auto config = array->schema().context().config();
+    auto config = schema.context().config();
     if (config.contains(CONFIG_KEY_INIT_BYTES)) {
         auto value_str = config.get(CONFIG_KEY_INIT_BYTES);
         try {
             num_bytes = std::stoull(value_str);
         } catch (const std::exception& e) {
             throw TileDBSOMAError(fmt::format(
                 "[ColumnBuffer] Error parsing {}: '{}' ({})",
                 CONFIG_KEY_INIT_BYTES,
                 value_str,
                 e.what()));
         }
     }
 
-    bool is_dense = array->schema().array_type() == TILEDB_DENSE;
+    bool is_dense = schema.array_type() == TILEDB_DENSE;
     if (is_dense) {
         // TODO: Handle dense arrays similar to tiledb python module
     }
 
     // For variable length column types, allocate an extra num_bytes to hold
     //   offset values. The number of cells is the set by the size of the
     //   offset type.
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/column_buffer.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/soma/column_buffer.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
  * @file   column_buffer.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2022-2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -33,16 +33,16 @@
 #ifndef COLUMN_BUFFER_H
 #define COLUMN_BUFFER_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <tiledb/tiledb>
 
-#include "common.h"
-#include "logger.h"
+#include "../utils/common.h"
+#include "../utils/logger.h"
 #include "span/span.hpp"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 /**
@@ -66,14 +66,44 @@
      * @param name TileDB dimension or attribute name
      * @return ColumnBuffer
      */
     static std::shared_ptr<ColumnBuffer> create(
         std::shared_ptr<Array> array, std::string_view name);
 
     /**
+     * @brief Create a ColumnBuffer from a schema and column name.
+     *
+     * @param schema TileDB schema
+     * @param name TileDB dimension or attribute name
+     * @return ColumnBuffer
+     */
+    static std::shared_ptr<ColumnBuffer> create(
+        ArraySchema schema, std::string_view name);
+
+    /**
+     * @brief Create a ColumnBuffer from a schema, column name, and data.
+     *
+     * @param schema TileDB schema
+     * @param name TileDB dimension or attribute name
+     * @param data Data to set in buffer
+     * @return ColumnBuffer
+     */
+    template <typename T>
+    static std::shared_ptr<ColumnBuffer> create(
+        ArraySchema schema, std::string_view name, std::vector<T> data) {
+        auto column_buff = ColumnBuffer::create(schema, name);
+        column_buff->num_cells_ = data.size();
+        column_buff->data_.resize(data.size());
+        column_buff->data_.assign(
+            reinterpret_cast<std::byte*>(data.data()),
+            reinterpret_cast<std::byte*>(data.data() + data.size()));
+        return column_buff;
+    }
+
+    /**
      * @brief Convert a bytemap to a bitmap in place.
      *
      */
     static void to_bitmap(tcb::span<uint8_t> bytemap);
 
     //===================================================================
     //= public non-static
@@ -241,15 +271,15 @@
      * @param name Column name
      * @param type TileDB datatype
      * @param is_var True if variable length data
      * @param is_nullable True if nullable data
      * @return ColumnBuffer
      */
     static std::shared_ptr<ColumnBuffer> alloc(
-        std::shared_ptr<Array> array,
+        ArraySchema schema,
         std::string_view name,
         tiledb_datatype_t type,
         bool is_var,
         bool is_nullable);
 
     //===================================================================
     //= private non-static
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/src/utils/version.h` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 add_executable(unit_soma EXCLUDE_FROM_ALL
     $<TARGET_OBJECTS:TILEDB_SOMA_OBJECTS>
     unit_column_buffer.cc
     unit_managed_query.cc
     unit_soma_array.cc
     unit_soma_group.cc
+    unit_soma_dataframe.cc
 # TODO: uncomment when thread_pool is enabled
 #    unit_thread_pool.cc
 )
 
 target_link_libraries(unit_soma
   PRIVATE
     Catch2::Catch2WithMain
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/test_soma_array.py` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/test_soma_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,8 @@
 
     {
         auto buffers = ColumnBuffer::create(array, "a1");
         REQUIRE(buffers->name() == "a1");
         REQUIRE(buffers->is_var() == true);
         REQUIRE(buffers->is_nullable() == true);
     }
-}
+}
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     }
 
     std::string uri = "mem://unit-test-array";
     auto ctx = Context();
     auto [array, d0, a0, _] = create_array(uri, ctx);
 
     auto mq = ManagedQuery(array);
-    mq.submit();
+    mq.submit_read();
 
     auto results = mq.results();
     REQUIRE(mq.results_complete());
 
     auto num_cells = mq.total_num_cells();
     REQUIRE(num_cells == d0.size());
 
@@ -138,15 +138,15 @@
     std::string uri = "mem://unit-test-array";
     auto ctx = Context();
     auto [array, d0, a0, _] = create_array(uri, ctx);
 
     auto mq = ManagedQuery(array);
     mq.select_columns({"a0"});
     mq.select_points<std::string>("d0", {"a"});
-    mq.submit();
+    mq.submit_read();
 
     auto results = mq.results();
     REQUIRE(mq.results_complete());
 
     auto num_cells = mq.total_num_cells();
     REQUIRE(num_cells == 1);
 
@@ -160,15 +160,15 @@
 
 TEST_CASE("ManagedQuery: Validity test") {
     std::string uri = "mem://unit-test-array";
     auto ctx = Context();
     auto [array, d0, a0, a0_valids] = create_array(uri, ctx);
 
     auto mq = ManagedQuery(array);
-    mq.submit();
+    mq.submit_read();
 
     auto results = mq.results();
     REQUIRE(mq.results_complete());
 
     auto num_cells = mq.total_num_cells();
     REQUIRE(num_cells == d0.size());
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
  * @file   unit_soma_array.cc
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2022-2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -56,223 +56,286 @@
 
 const std::string src_path = TILEDBSOMA_SOURCE_ROOT;
 
 namespace {
 
 std::tuple<std::string, uint64_t> create_array(
     const std::string& uri_in,
-    Context& ctx,
+    std::shared_ptr<Context> ctx,
     int num_cells_per_fragment = 10,
     int num_fragments = 1,
     bool overlap = false,
-    bool allow_duplicates = false,
-    uint64_t timestamp = 1,
-    bool reuse_existing = false) {
+    bool allow_duplicates = false) {
     std::string uri = fmt::format(
         "{}-{}-{}-{}-{}",
         uri_in,
         num_cells_per_fragment,
         num_fragments,
         overlap,
         allow_duplicates);
-    // Create array, if not reusing the existing array
-    if (!reuse_existing) {
-        auto vfs = VFS(ctx);
-        if (vfs.is_dir(uri)) {
-            vfs.remove_dir(uri);
-        }
 
-        // Create schema
-        ArraySchema schema(ctx, TILEDB_SPARSE);
+    auto vfs = VFS(*ctx);
+    if (vfs.is_dir(uri)) {
+        vfs.remove_dir(uri);
+    }
+
+    // Create schema
+    ArraySchema schema(*ctx, TILEDB_SPARSE);
 
-        auto dim = Dimension::create<int64_t>(
-            ctx, "d0", {0, std::numeric_limits<int64_t>::max() - 1});
+    auto dim = Dimension::create<int64_t>(
+        *ctx, "d0", {0, std::numeric_limits<int64_t>::max() - 1});
 
-        Domain domain(ctx);
-        domain.add_dimension(dim);
-        schema.set_domain(domain);
-
-        auto attr = Attribute::create<int>(ctx, "a0");
-        schema.add_attribute(attr);
-        schema.set_allows_dups(allow_duplicates);
-        schema.check();
+    Domain domain(*ctx);
+    domain.add_dimension(dim);
+    schema.set_domain(domain);
+
+    auto attr = Attribute::create<int>(*ctx, "a0");
+    schema.add_attribute(attr);
+    schema.set_allows_dups(allow_duplicates);
+    schema.check();
 
-        // Create array
-        Array::create(uri, schema);
+    // Create array
+    SOMAArray::create(ctx, uri, schema, "NONE");
+
+    uint64_t nnz = num_fragments * num_cells_per_fragment;
+
+    if (allow_duplicates) {
+        return {uri, nnz};
     }
 
-    // Open array for writing
-    Array array(ctx, uri, TILEDB_WRITE, timestamp);
-    if (LOG_DEBUG_ENABLED()) {
-        array.schema().dump();
+    // Adjust nnz when overlap is enabled
+    if (overlap) {
+        nnz = (num_fragments + 1) / 2 * num_cells_per_fragment;
     }
 
+    return {uri, nnz};
+}
+
+std::tuple<std::vector<int64_t>, std::vector<int>> write_array(
+    const std::string& uri,
+    std::shared_ptr<Context> ctx,
+    int num_cells_per_fragment = 10,
+    int num_fragments = 1,
+    bool overlap = false,
+    uint64_t timestamp = 1) {
     // Generate fragments in random order
     std::vector<int> frags(num_fragments);
     std::iota(frags.begin(), frags.end(), 0);
     std::shuffle(frags.begin(), frags.end(), std::random_device{});
 
-    for (auto i : frags) {
+    // Write to SOMAArray
+    for (auto i = 0; i < num_fragments; ++i) {
+        auto frag_num = frags[i];
+        auto soma_array = SOMAArray::open(
+            TILEDB_WRITE,
+            ctx,
+            uri,
+            "",
+            {},
+            "auto",
+            "auto",
+            std::pair<uint64_t, uint64_t>(timestamp + i, timestamp + i));
+
+        if (LOG_DEBUG_ENABLED()) {
+            soma_array->schema()->dump();
+        }
+
         std::vector<int64_t> d0(num_cells_per_fragment);
         for (int j = 0; j < num_cells_per_fragment; j++) {
             // Overlap odd fragments when generating overlaps
-            if (overlap && i & 1) {
-                d0[j] = j + num_cells_per_fragment * (i - 1);
+            if (overlap && frag_num % 2 == 1) {
+                d0[j] = j + num_cells_per_fragment * (frag_num - 1);
             } else {
-                d0[j] = j + num_cells_per_fragment * i;
+                d0[j] = j + num_cells_per_fragment * frag_num;
             }
         }
-        std::vector<int> a0(num_cells_per_fragment, i);
+        std::vector<int> a0(num_cells_per_fragment, frag_num);
+
+        auto schema = *soma_array->schema();
+        auto array_buffer = std::make_shared<ArrayBuffers>();
+        array_buffer->emplace("a0", ColumnBuffer::create(schema, "a0", a0));
+        array_buffer->emplace("d0", ColumnBuffer::create(schema, "d0", d0));
 
         // Write data to array
-        Query query(ctx, array);
-        query.set_layout(TILEDB_UNORDERED)
-            .set_data_buffer("d0", d0)
-            .set_data_buffer("a0", a0);
-        query.submit();
+        soma_array->submit();
+        soma_array->write(array_buffer);
+        soma_array->close();
     }
 
-    array.close();
+    // Read from TileDB Array to get expected data
+    Array tiledb_array(*ctx, uri, TILEDB_READ, timestamp + num_fragments - 1);
+    tiledb_array.reopen();
 
-    uint64_t nnz = num_fragments * num_cells_per_fragment;
+    std::vector<int64_t> expected_d0(num_cells_per_fragment * num_fragments);
+    std::vector<int> expected_a0(num_cells_per_fragment * num_fragments);
 
-    if (allow_duplicates) {
-        return {uri, nnz};
-    }
+    Query query(*ctx, tiledb_array);
+    query.set_layout(TILEDB_UNORDERED)
+        .set_data_buffer("d0", expected_d0)
+        .set_data_buffer("a0", expected_a0);
+    query.submit();
 
-    // Adjust nnz when overlap is enabled
-    if (overlap) {
-        nnz = (num_fragments + 1) / 2 * num_cells_per_fragment;
-    }
+    tiledb_array.close();
 
-    return {uri, nnz};
+    expected_d0.resize(query.result_buffer_elements()["d0"].second);
+    expected_a0.resize(query.result_buffer_elements()["a0"].second);
+
+    return {expected_d0, expected_a0};
 }
 
 };  // namespace
 
 TEST_CASE("SOMAArray: nnz") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
-    auto allow_duplicates = GENERATE(false, true);
+    auto allow_duplicates = true;
     int num_cells_per_fragment = 128;
+    auto timestamp = 10;
 
     SECTION(fmt::format(
         " - fragments={}, overlap={}, allow_duplicates={}",
         num_fragments,
         overlap,
         allow_duplicates)) {
         auto ctx = std::make_shared<Context>();
 
-        // Create array at timestamp 10
+        // Create array
         std::string base_uri = "mem://unit-test-array";
         auto [uri, expected_nnz] = create_array(
             base_uri,
-            *ctx,
+            ctx,
+            num_cells_per_fragment,
+            num_fragments,
+            overlap,
+            allow_duplicates);
+
+        // Write at timestamp 10
+        auto [expected_d0, expected_a0] = write_array(
+            uri,
+            ctx,
             num_cells_per_fragment,
             num_fragments,
             overlap,
-            allow_duplicates,
-            10);
+            timestamp);
 
         // Get total cell num
-        auto soma_array = SOMAArray::open(TILEDB_READ, ctx, uri);
+        auto soma_array = SOMAArray::open(
+            TILEDB_READ,
+            ctx,
+            uri,
+            "",
+            {},
+            "auto",
+            "auto",
+            std::pair<uint64_t, uint64_t>(
+                timestamp, timestamp + num_fragments - 1));
 
         uint64_t nnz = soma_array->nnz();
         REQUIRE(nnz == expected_nnz);
 
         std::vector<int64_t> shape = soma_array->shape();
         REQUIRE(shape.size() == 1);
         REQUIRE(shape[0] == std::numeric_limits<int64_t>::max());
+
+        // Check that data from SOMAArray::read_next matches expected data
+        soma_array->submit();
+        while (auto batch = soma_array->read_next()) {
+            auto arrbuf = batch.value();
+            REQUIRE(arrbuf->names() == std::vector<std::string>({"d0", "a0"}));
+            REQUIRE(arrbuf->num_rows() == nnz);
+
+            auto d0span = arrbuf->at("d0")->data<int64_t>();
+            auto a0span = arrbuf->at("a0")->data<int>();
+
+            std::vector<int64_t> d0col(d0span.begin(), d0span.end());
+            std::vector<int> a0col(a0span.begin(), a0span.end());
+
+            REQUIRE(d0col == expected_d0);
+            REQUIRE(a0col == expected_a0);
+        }
+        soma_array->close();
     }
 }
 
 TEST_CASE("SOMAArray: nnz with timestamp") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
-    auto allow_duplicates = GENERATE(false, true);
+    auto allow_duplicates = true;
     int num_cells_per_fragment = 128;
 
     SECTION(fmt::format(
         " - fragments={}, overlap={}, allow_duplicates={}",
         num_fragments,
         overlap,
         allow_duplicates)) {
         auto ctx = std::make_shared<Context>();
 
-        // Create array at timestamp 10
+        // Create array
         std::string base_uri = "mem://unit-test-array";
         const auto& [uri, expected_nnz] = create_array(
             base_uri,
-            *ctx,
+            ctx,
             num_cells_per_fragment,
             num_fragments,
             overlap,
-            allow_duplicates,
-            10);
+            allow_duplicates);
 
-        // Write more data to the array at timestamp 20, which will be
+        // Write at timestamp 10
+        write_array(
+            uri, ctx, num_cells_per_fragment, num_fragments, overlap, 10);
+
+        // Write more data to the array at timestamp 40, which will be
         // not be included in the nnz call with a timestamp
-        create_array(
-            base_uri,
-            *ctx,
-            num_cells_per_fragment,
-            num_fragments,
-            overlap,
-            allow_duplicates,
-            20,
-            true);
+        write_array(
+            uri, ctx, num_cells_per_fragment, num_fragments, overlap, 40);
 
-        // Get total cell num at timestamp (0, 15)
-        std::pair<uint64_t, uint64_t> timestamp{0, 15};
+        // Get total cell num at timestamp (0, 20)
+        std::pair<uint64_t, uint64_t> timestamp{0, 20};
         auto soma_array = SOMAArray::open(
             TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto", timestamp);
 
         uint64_t nnz = soma_array->nnz();
         REQUIRE(nnz == expected_nnz);
     }
 }
 
 TEST_CASE("SOMAArray: nnz with consolidation") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
-    auto allow_duplicates = GENERATE(false, true);
+    auto allow_duplicates = true;
     auto vacuum = GENERATE(false, true);
     int num_cells_per_fragment = 128;
 
     SECTION(fmt::format(
         " - fragments={}, overlap={}, allow_duplicates={}, vacuum={}",
         num_fragments,
         overlap,
         allow_duplicates,
         vacuum)) {
         auto ctx = std::make_shared<Context>();
 
-        // Create array at timestamp 10
+        // Create array
         std::string base_uri = "mem://unit-test-array";
         const auto& [uri, expected_nnz] = create_array(
             base_uri,
-            *ctx,
+            ctx,
             num_cells_per_fragment,
             num_fragments,
             overlap,
-            allow_duplicates,
-            10);
+            allow_duplicates);
+
+        // Write at timestamp 10
+        write_array(
+            uri, ctx, num_cells_per_fragment, num_fragments, overlap, 10);
 
         // Write more data to the array at timestamp 20, which will be
         // duplicates of the data written at timestamp 10
         // The duplicates get merged into one fragment during consolidation.
-        create_array(
-            base_uri,
-            *ctx,
-            num_cells_per_fragment,
-            num_fragments,
-            overlap,
-            allow_duplicates,
-            20,
-            true);
+        write_array(
+            uri, ctx, num_cells_per_fragment, num_fragments, overlap, 20);
 
         // Consolidate and optionally vacuum
         Array::consolidate(*ctx, uri);
         if (vacuum) {
             Array::vacuum(*ctx, uri);
         }
 
@@ -290,15 +353,15 @@
     }
 }
 
 TEST_CASE("SOMAArray: metadata") {
     auto ctx = std::make_shared<Context>();
 
     std::string base_uri = "mem://unit-test-array";
-    const auto& [uri, expected_nnz] = create_array(base_uri, *ctx);
+    const auto& [uri, expected_nnz] = create_array(base_uri, ctx);
 
     auto soma_array = SOMAArray::open(
         TILEDB_WRITE,
         ctx,
         uri,
         "metadata_test",
         {},
@@ -330,8 +393,30 @@
     soma_array->delete_metadata("md");
     soma_array->close();
 
     soma_array->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(3, 3));
     REQUIRE(soma_array->has_metadata("md") == false);
     REQUIRE(soma_array->metadata_num() == 0);
     soma_array->close();
+}
+
+TEST_CASE("SOMAArray: Test buffer size") {
+    // Test soma.init_buffer_bytes by making buffer small
+    // enough to read one byte at a time so that read_next
+    // must be called 10 times instead of placing all data
+    // in buffer within a single read
+    Config cfg;
+    cfg["soma.init_buffer_bytes"] = 8;
+    auto ctx = std::make_shared<Context>(cfg);
+
+    std::string base_uri = "mem://unit-test-array";
+    auto [uri, expected_nnz] = create_array(base_uri, ctx);
+    auto [expected_d0, expected_a0] = write_array(uri, ctx);
+    auto soma_array = SOMAArray::open(TILEDB_READ, ctx, uri);
+
+    size_t loops = 0;
+    soma_array->submit();
+    while (auto batch = soma_array->read_next())
+        ++loops;
+    REQUIRE(loops == 10);
+    soma_array->close();
 }
```

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_soma_group.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.3.0/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/scripts/bld` & `tiledbsoma-1.3.0/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.3.0/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/scripts/show-versions.py` & `tiledbsoma-1.3.0/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.3.0/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/setup.py` & `tiledbsoma-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         "numpy>=1.18,<1.24; python_version<'3.11'",
         "numpy>=1.18,<1.25; python_version=='3.11'",
         "pandas",
         "pyarrow>=9.0.0",
         "scanpy>=1.9.2",
         "scipy",
         "somacore==1.0.3",
-        "tiledb~=0.21.3",
+        "tiledb~=0.22.0",
         "typing-extensions",  # Note "-" even though `import typing_extensions`
     ],
     extras_require={
         "dev": [
             "black",
             "ruff",
             "pytest",
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/__init__.py` & `tiledbsoma-1.3.0/src/tiledbsoma/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 SOMA --- stack of matrices, annotated --- is a flexible, extensible, and
 open-source API enabling access to data in a variety of formats, and is
 motivated by use cases from single-cell biology. The ``tiledbsoma``
 Python package is an implementation of SOMA using the
 `TileDB Embedded <https://github.com/TileDB-Inc/TileDB>`_ engine.
 
-Provides:
+Provides
 ----------
   1. The ability to store, query, and retrieve larger-than-core datasets,
      resident in both cloud (object-store) and local (file) systems.
   2. A data model supporting dataframes, and both sparse and dense
      multi-dimensional arrays.
   3. An extended data model with support for single-cell biology data.
 
 See the `SOMA GitHub repo <https://github.com/single-cell-data/SOMA>`_ for more
 information on the SOMA project.
 
-Using the documentation:
+Using the documentation
 -------------------------
 
 Documentation is also available via the Python builtin ``help`` function. We
 recommend exploring the package. For example:
 
 >>> import tiledbsoma
 >>> help(tiledbsoma.DataFrame)
 
-API maturity tags:
+API maturity tags
 ------------------
 
 Classes and functions are annotated with API maturity tags, for example:
 
     ``Lifecycle: experimental``
 
 These tags indicate the maturity of each interface, and are patterned after
@@ -45,26 +45,26 @@
   avoided where possible. Breaking changes that cannot be avoided will be
   accompanied by a major version bump.
 - ``deprecated``: The API is no longer recommended for use and may be removed
   in a future release.
 
 If no tag is present, the state is ``experimental``.
 
-Data types:
+Data types
 ------------
 
 The principal persistent types provided by SOMA are:
 
 - :class:`Collection` -- a string-keyed container of SOMA objects.
 - :class:`DataFrame` -- a multi-column table with a user-defined schema,
   defining the number of columns and their respective column name
   and value type.
 - :class:`SparseNDArray` -- a sparse multi-dimensional array, storing
   Arrow primitive data types, i.e., int, float, etc.
-- :class:`DenseNDArray` -- a dnese multi-dimensional array, storing
+- :class:`DenseNDArray` -- a dense multi-dimensional array, storing
   Arrow primitive data types, i.e., int, float, etc.
 - :class:`Experiment` -- a specialized :class:`Collection`, representing an
   annotated 2-D matrix of measurements.
 - :class:`Measurement` -- a specialized :class:`Collection`, for use within
   the :class:`Experiment` class, representing a set of measurements on
   a single set of variables (features, e.g., genes)
 
@@ -72,28 +72,25 @@
 single-cell biology.
 
 SOMA uses the `Arrow <https://arrow.apache.org/docs/python/index.html>`_ type
 system and memory model for its in-memory type system and schema. For
 example, the schema of a :class:`DataFrame` is expressed as an
 `Arrow Schema <https://arrow.apache.org/docs/python/generated/pyarrow.Schema.html>`_.
 
-Error handling:
+Error handling
 ---------------
 Most errors will be signaled with a raised Exception. Of note:
 
 - :class:`NotImplementedError` will be raised when the requested function or method
   is unsupported.
 - :class:`SOMAError` is a base class for all SOMA-specific errors.
 - ``TileDBError`` will be raised for many TileDB-specific errors.
 
 Most errors will raise an appropriate Python error, e.g., ::class:`TypeError` or
 :class:`ValueError`.
-
-Classes and functions:
-----------------------
 """
 
 # ^^ the rest is autogen whether viewed from Python on-line help, Sphinx/readthedocs, etc.  It's
 # crucial that we include a separator (e.g. "Classes and functions") to make an entry in the
 # readthedocs table of contents.
 
 from somacore import AxisColumnNames, AxisQuery, ExperimentAxisQuery
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_collection.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_collection.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_common_nd_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 for any intended future appends, as a sequence.  E.g. ``(100, 10)``.
                 All lengths must be in the postive int64 range, or ``None``.  It's
                 necessary to say ``shape=(None, None)`` or ``shape=(None, None,
                 None)``, as the sequence length determines the number of dimensions
                 N in the N-dimensional array.
 
                 For :class:`SparseNDArray` only, if a slot is None, then the maximum
-                possible int64 will be used.  This makes a :class:`SparseNDArray`
+                possible int32 will be used.  This makes a :class:`SparseNDArray`
                 growable.
             platform_config:
                 Platform-specific options used to create this array.
                 This may be provided as settings in a dictionary, with options
                 located in the ``{'tiledb': {'create': ...}}`` key,
                 or as a :class:`~tiledbsoma.TileDBCreateOptions` object.
             tiledb_timestamp:
@@ -78,21 +78,14 @@
                 If the ``shape`` is unsupported.
             TileDBError:
                 If unable to create the underlying object.
 
         Lifecycle:
             Experimental.
         """
-        # Implementor note: we carefully say "maximum possible int64 size" rather than 2**63-1. The
-        # reason that the latter, while temptingly simple, is actually untrue is that tiledb core
-        # requires that the capacity, when rounded up to an exact multiple of the extent, needs to
-        # be representable as a signed 64-bit integer.  So in particular when a unit test (or anyone
-        # else) sets extent to a not-power-of-two number like 999 or 1000 then the create fails if
-        # the upper limit is exactly 2**63-1.
-
         context = _validate_soma_tiledb_context(context)
         schema = cls._build_tiledb_schema(
             type,
             shape,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
             is_sparse=cls.is_sparse,
@@ -102,14 +95,16 @@
             handle,
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
 
     @property
     def shape(self) -> Tuple[int, ...]:
         """Returns capacity of each dimension, always a list of length ``ndim``.
+        This will not necessarily match the bounds of occupied cells within the array.
+        Rather, it is the bounds outside of which no data may be written.
 
         Lifecycle:
             Experimental.
         """
         return cast(Tuple[int, ...], tuple(self._soma_reader().shape))
 
     def reshape(self, shape: Tuple[int, ...]) -> None:
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -792,15 +792,15 @@
         slot_domain = None, None
     elif np.issubdtype(dtype, NPInteger):
         iinfo = np.iinfo(cast(NPInteger, dtype))
         slot_domain = iinfo.min, iinfo.max - 1
         # Here the slot_domain isn't specified by the user; we're setting it.
         # The SOMA spec disallows negative soma_joinid.
         if index_column_name == SOMA_JOINID:
-            slot_domain = (0, slot_domain[1])
+            slot_domain = (0, 2**31 - 2)  # R-friendly, which 2**63-1 is not
     elif np.issubdtype(dtype, NPFloating):
         finfo = np.finfo(cast(NPFloating, dtype))
         slot_domain = finfo.min, finfo.max
 
     # The `iinfo.min+1` is necessary as of tiledb core 2.15 / tiledb-py 0.21.1 since
     # `iinfo.min` maps to `NaT` (not a time), resulting in
     #   TypeError: invalid domain extent, domain cannot be safely cast to dtype dtype('<M8[s]')
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_exception.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_factory.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_sparse_nd_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -260,21 +260,16 @@
     ) -> Tuple[int, int]:
         """Given a user-specified shape (maybe ``None``) along a particular dimension,
         returns a tuple of the TileDB capacity and extent for that dimension, suitable
         for schema creation. If the user-specified shape is None, the largest possible
         int64 is returned for the capacity.
         """
         if dim_shape is None:
-            dim_capacity = 2**63
+            dim_capacity = 2**31 - 2  # Make this friendly for reads by tiledbsoma-r
             dim_extent = min(dim_capacity, create_options.dim_tile(dim_name, 2048))
-            # TileDB requires that each signed-64-bit-int domain slot, rounded up to
-            # a multiple of the tile extent in that slot, be representable as a
-            # signed 64-bit int. So if the tile extent is 999, say, that would
-            # exceed 2**63 - 1.
-            dim_capacity -= dim_extent
         else:
             if dim_shape <= 0:
                 raise ValueError(
                     "SOMASparseNDArray shape must be a non-zero-length tuple of positive ints or Nones"
                 )
             dim_capacity = dim_shape
             dim_extent = min(dim_shape, create_options.dim_tile(dim_name, 2048))
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_tiledb_object.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_types.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/_util.py` & `tiledbsoma-1.3.0/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/eta.py` & `tiledbsoma-1.3.0/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.3.0/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.3.0/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.3.0/src/tiledbsoma/io/ingest.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,14 +62,43 @@
 
 SparseMatrix = Union[sp.csr_matrix, sp.csc_matrix, SparseDataset]
 DenseMatrix = Union[NPNDArray, h5py.Dataset]
 Matrix = Union[DenseMatrix, SparseMatrix]
 _NDArr = TypeVar("_NDArr", bound=NDArray)
 _TDBO = TypeVar("_TDBO", bound=TileDBObject[RawHandle])
 
+# ----------------------------------------------------------------
+class IngestionParams:
+    """Maps from user-level ingest modes to a set of implementation-level boolean flags."""
+
+    write_schema_no_data: bool
+    error_if_already_exists: bool
+    skip_existing_nonempty_domain: bool
+
+    def __init__(self, ingest_mode: str) -> None:
+        if ingest_mode == "write":
+            self.write_schema_no_data = False
+            self.error_if_already_exists = True
+            self.skip_existing_nonempty_domain = False
+
+        elif ingest_mode == "schema_only":
+            self.write_schema_no_data = True
+            self.error_if_already_exists = True
+            self.skip_existing_nonempty_domain = False
+
+        elif ingest_mode == "resume":
+            self.write_schema_no_data = False
+            self.error_if_already_exists = False
+            self.skip_existing_nonempty_domain = True
+
+        else:
+            raise SOMAError(
+                f'expected ingest_mode to be one of {INGEST_MODES}; got "{ingest_mode}"'
+            )
+
 
 # ----------------------------------------------------------------
 def from_h5ad(
     experiment_uri: str,
     input_path: Path,
     measurement_name: str,
     *,
@@ -207,14 +236,17 @@
         Experimental.
     """
     if ingest_mode not in INGEST_MODES:
         raise SOMAError(
             f'expected ingest_mode to be one of {INGEST_MODES}; got "{ingest_mode}"'
         )
 
+    # Map the user-level ingest mode to a set of implementation-level boolean flags
+    ingestion_params = IngestionParams(ingest_mode)
+
     if not isinstance(anndata, ad.AnnData):
         raise TypeError(
             "Second argument is not an AnnData object -- did you want from_h5ad?"
         )
 
     context = _validate_soma_tiledb_context(context)
 
@@ -231,27 +263,27 @@
     logging.log_io(None, _util.format_elapsed(s, "FINISH DECATEGORICALIZING"))
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {experiment_uri}")
 
     # Must be done first, to create the parent directory.
     experiment = _create_or_open_coll(
-        Experiment, experiment_uri, ingest_mode, context=context
+        Experiment, experiment_uri, ingestion_params=ingestion_params, context=context
     )
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # OBS
     df_uri = _util.uri_joinpath(experiment_uri, "obs")
     with _write_dataframe(
         df_uri,
         conversions.decategoricalize_obs_or_var(anndata.obs),
         id_column_name="obs_id",
         platform_config=platform_config,
         context=context,
-        ingest_mode=ingest_mode,
+        ingestion_params=ingestion_params,
     ) as obs:
         _maybe_set(experiment, "obs", obs, use_relative_uri=use_relative_uri)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # MS
 
     # For local disk and S3, this is the same as experiment.ms.uri.
@@ -260,210 +292,210 @@
     # be of the form tiledb://namespace/uuid. Only for the former is it suitable
     # to append "/ms" so that is what we do here.
     experiment_ms_uri = f"{experiment_uri}/ms"
 
     with _create_or_open_coll(
         Collection[Measurement],
         experiment_ms_uri,
-        ingest_mode,
+        ingestion_params=ingestion_params,
         context=context,
     ) as ms:
         _maybe_set(experiment, "ms", ms, use_relative_uri=use_relative_uri)
 
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         # MS/meas
         measurement_uri = _util.uri_joinpath(experiment_ms_uri, measurement_name)
         with _create_or_open_coll(
             Measurement,
             measurement_uri,
-            ingest_mode,
+            ingestion_params=ingestion_params,
             context=context,
         ) as measurement:
             _maybe_set(
                 ms, measurement_name, measurement, use_relative_uri=use_relative_uri
             )
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # ms/meas/uns
             _maybe_ingest_uns(
                 measurement,
                 anndata.uns,
-                platform_config,
-                context,
-                ingest_mode,
+                platform_config=platform_config,
+                context=context,
+                ingestion_params=ingestion_params,
                 use_relative_uri=use_relative_uri,
             )
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # MS/meas/VAR
             with _write_dataframe(
                 _util.uri_joinpath(measurement_uri, "var"),
                 conversions.decategoricalize_obs_or_var(anndata.var),
                 id_column_name="var_id",
                 platform_config=platform_config,
                 context=context,
-                ingest_mode=ingest_mode,
+                ingestion_params=ingestion_params,
             ) as var:
                 _maybe_set(measurement, "var", var, use_relative_uri=use_relative_uri)
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # MS/meas/X/DATA
 
             measurement_X_uri = _util.uri_joinpath(measurement_uri, "X")
             with _create_or_open_coll(
                 Collection,
                 measurement_X_uri,
-                ingest_mode,
+                ingestion_params=ingestion_params,
                 context=context,
             ) as x:
                 _maybe_set(measurement, "X", x, use_relative_uri=use_relative_uri)
 
                 # Since we did ``anndata = ad.read_h5ad(path_to_h5ad, "r")`` with the "r":
                 # * If we do ``anndata.X[:]`` we're loading all of a CSR/CSC/etc into memory.
                 # * If we do ``anndata.X`` we're getting a pageable object which can be loaded
                 #   chunkwise into memory.
                 # Using the latter allows us to ingest larger .h5ad files without OOMing.
 
-                with create_from_matrix(
+                with _create_from_matrix(
                     X_kind,
                     _util.uri_joinpath(measurement_X_uri, "data"),
                     anndata.X,
-                    platform_config,
-                    ingest_mode,
-                    context,
+                    ingestion_params=ingestion_params,
+                    platform_config=platform_config,
+                    context=context,
                 ) as data:
                     _maybe_set(x, "data", data, use_relative_uri=use_relative_uri)
 
                 for layer_name, layer in anndata.layers.items():
-                    with create_from_matrix(
+                    with _create_from_matrix(
                         X_kind,
                         _util.uri_joinpath(measurement_X_uri, layer_name),
                         layer,
-                        platform_config,
-                        ingest_mode,
-                        context,
+                        ingestion_params=ingestion_params,
+                        platform_config=platform_config,
+                        context=context,
                     ) as layer_data:
                         _maybe_set(
                             x, layer_name, layer_data, use_relative_uri=use_relative_uri
                         )
 
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/meas/OBSM,VARM,OBSP,VARP
                 if len(anndata.obsm.keys()) > 0:  # do not create an empty collection
                     obsm_uri = _util.uri_joinpath(measurement_uri, "obsm")
                     with _create_or_open_coll(
                         Collection,
                         obsm_uri,
-                        ingest_mode,
+                        ingestion_params=ingestion_params,
                         context=context,
                     ) as obsm:
                         _maybe_set(
                             measurement, "obsm", obsm, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsm.keys():
-                            with create_from_matrix(
+                            with _create_from_matrix(
                                 # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
                                 # consider a use-dense flag at the tiledbsoma.io API
                                 # DenseNDArray,
                                 SparseNDArray,
                                 _util.uri_joinpath(obsm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.obsm[key]
                                 ),
-                                platform_config,
-                                ingest_mode,
+                                ingestion_params=ingestion_params,
+                                platform_config=platform_config,
                                 context=context,
                             ) as arr:
                                 _maybe_set(
                                     obsm, key, arr, use_relative_uri=use_relative_uri
                                 )
                             arr.close()
                     measurement.obsm.close()
 
                 if len(anndata.varm.keys()) > 0:  # do not create an empty collection
                     _util.uri_joinpath(measurement_uri, "varm")
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "varm"),
-                        ingest_mode,
+                        ingestion_params=ingestion_params,
                         context=context,
                     ) as varm:
                         _maybe_set(
                             measurement, "varm", varm, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.varm.keys():
-                            with create_from_matrix(
+                            with _create_from_matrix(
                                 # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
                                 # consider a use-dense flag at the tiledbsoma.io API
                                 # DenseNDArray,
                                 SparseNDArray,
                                 _util.uri_joinpath(varm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.varm[key]
                                 ),
-                                platform_config,
-                                ingest_mode,
+                                ingestion_params=ingestion_params,
+                                platform_config=platform_config,
                                 context=context,
                             ) as darr:
                                 _maybe_set(
                                     varm,
                                     key,
                                     darr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 if len(anndata.obsp.keys()) > 0:  # do not create an empty collection
                     _util.uri_joinpath(measurement_uri, "obsp")
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "obsp"),
-                        ingest_mode,
+                        ingestion_params=ingestion_params,
                         context=context,
                     ) as obsp:
                         _maybe_set(
                             measurement, "obsp", obsp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsp.keys():
-                            with create_from_matrix(
+                            with _create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(obsp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.obsp[key]
                                 ),
-                                platform_config,
-                                ingest_mode,
+                                ingestion_params=ingestion_params,
+                                platform_config=platform_config,
                                 context=context,
                             ) as sarr:
                                 _maybe_set(
                                     obsp,
                                     key,
                                     sarr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 if len(anndata.varp.keys()) > 0:  # do not create an empty collection
                     _util.uri_joinpath(measurement_uri, "obsp")
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "varp"),
-                        ingest_mode,
+                        ingestion_params=ingestion_params,
                         context=context,
                     ) as varp:
                         _maybe_set(
                             measurement, "varp", varp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.varp.keys():
-                            with create_from_matrix(
+                            with _create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(varp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.varp[key]
                                 ),
-                                platform_config,
-                                ingest_mode,
+                                ingestion_params=ingestion_params,
+                                platform_config=platform_config,
                                 context=context,
                             ) as sarr:
                                 _maybe_set(
                                     varp,
                                     key,
                                     sarr,
                                     use_relative_uri=use_relative_uri,
@@ -472,59 +504,59 @@
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/RAW
                 if anndata.raw is not None:
                     raw_uri = _util.uri_joinpath(experiment_ms_uri, "raw")
                     with _create_or_open_coll(
                         Measurement,
                         raw_uri,
-                        ingest_mode,
+                        ingestion_params=ingestion_params,
                         context=context,
                     ) as raw_measurement:
                         _maybe_set(
                             ms,
                             "raw",
                             raw_measurement,
                             use_relative_uri=use_relative_uri,
                         )
 
                         with _write_dataframe(
                             _util.uri_joinpath(raw_uri, "var"),
                             conversions.decategoricalize_obs_or_var(anndata.raw.var),
                             id_column_name="var_id",
+                            ingestion_params=ingestion_params,
                             platform_config=platform_config,
                             context=context,
-                            ingest_mode=ingest_mode,
                         ) as var:
                             _maybe_set(
                                 raw_measurement,
                                 "var",
                                 var,
                                 use_relative_uri=use_relative_uri,
                             )
 
                         raw_X_uri = _util.uri_joinpath(raw_uri, "X")
                         with _create_or_open_coll(
                             Collection,
                             raw_X_uri,
-                            ingest_mode,
+                            ingestion_params=ingestion_params,
                             context=context,
                         ) as rm_x:
                             _maybe_set(
                                 raw_measurement,
                                 "X",
                                 rm_x,
                                 use_relative_uri=use_relative_uri,
                             )
 
-                            with create_from_matrix(
+                            with _create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(raw_X_uri, "data"),
                                 anndata.raw.X,
-                                platform_config,
-                                ingest_mode,
+                                ingestion_params=ingestion_params,
+                                platform_config=platform_config,
                                 context=context,
                             ) as rm_x_data:
                                 _maybe_set(
                                     rm_x,
                                     "data",
                                     rm_x_data,
                                     use_relative_uri=use_relative_uri,
@@ -542,86 +574,82 @@
 def _maybe_set(
     coll: AnyTileDBCollection,
     key: str,
     value: AnyTileDBObject,
     *,
     use_relative_uri: Optional[bool],
 ) -> None:
+    if coll.closed or coll.mode != "w":
+        raise SOMAError(f"Collection must be open for write: {coll.uri}")
     try:
         coll.set(key, value, use_relative_uri=use_relative_uri)
     except SOMAError:
         # This is already a member of the collection.
         pass
 
 
 @overload
 def _create_or_open_coll(
     cls: Type[Experiment],
     uri: str,
-    ingest_mode: str,
+    *,
+    ingestion_params: IngestionParams,
     context: Optional[SOMATileDBContext],
 ) -> Experiment:
     ...
 
 
 @overload
 def _create_or_open_coll(
     cls: Type[Measurement],
     uri: str,
-    ingest_mode: str,
+    *,
+    ingestion_params: IngestionParams,
     context: Optional[SOMATileDBContext],
 ) -> Measurement:
     ...
 
 
 @overload
 def _create_or_open_coll(
     cls: Type[Collection[_TDBO]],
     uri: str,
-    ingest_mode: str,
+    *,
+    ingestion_params: IngestionParams,
     context: Optional[SOMATileDBContext],
 ) -> Collection[_TDBO]:
     ...
 
 
 @typeguard_ignore
 def _create_or_open_coll(
-    cls: Type[Any], uri: str, ingest_mode: str, context: Optional[SOMATileDBContext]
+    cls: Type[Any],
+    uri: str,
+    *,
+    ingestion_params: IngestionParams,
+    context: Optional[SOMATileDBContext],
 ) -> Any:
     try:
         thing = cls.open(uri, "w", context=context)
     except DoesNotExistError:
-        # This is always OK. Make a new one.
-        return cls.create(uri, context=context)
-    # It already exists. Are we resuming?
-    if ingest_mode == "resume":
+        pass  # This is always OK; make a new one.
+    else:
+        # It already exists. Are we resuming?
+        if ingestion_params.error_if_already_exists:
+            raise SOMAError(f"{uri} already exists")
         return thing
-    raise SOMAError(f"{uri} already exists")
 
+    return cls.create(uri, context=context)
 
-def _write_dataframe(
-    df_uri: str,
-    df: pd.DataFrame,
-    id_column_name: Optional[str],
-    platform_config: Optional[PlatformConfig] = None,
-    context: Optional[SOMATileDBContext] = None,
-    ingest_mode: IngestMode = "write",
-) -> DataFrame:
-    s = _util.get_start_stamp()
-    logging.log_io(None, f"START  WRITING {df_uri}")
-
-    df[SOMA_JOINID] = np.asarray(range(len(df)), dtype=np.int64)
-
-    df.reset_index(inplace=True)
-    if id_column_name is not None:
-        df.rename(columns={"index": id_column_name}, inplace=True)
-    df.set_index(SOMA_JOINID, inplace=True)
 
-    # Categoricals are not yet well supported, so we must flatten
-    # Also replace Numpy/Pandas-style nulls with Arrow-style nulls
+def _df_to_arrow(df: pd.DataFrame) -> pa.Table:
+    """
+    Categoricals are not yet well supported, so we must flatten.
+    Also replace Numpy/Pandas-style nulls with Arrow-style nulls.
+    """
     null_fields = set()
     for k in df:
         if df[k].dtype == "category":
             df[k] = df[k].astype(df[k].cat.categories.dtype)
         if df[k].isnull().any():
             if df[k].isnull().all():
                 df[k] = pa.nulls(df.shape[0], pa.infer_type(df[k]))
@@ -634,37 +662,78 @@
             null_fields.add(k)
     arrow_table = pa.Table.from_pandas(df)
     if null_fields:
         md = arrow_table.schema.metadata
         md.update(dict.fromkeys(null_fields, "nullable"))
         arrow_table = arrow_table.replace_schema_metadata(md)
 
+    return arrow_table
+
+
+def _write_dataframe(
+    df_uri: str,
+    df: pd.DataFrame,
+    id_column_name: Optional[str],
+    *,
+    ingestion_params: IngestionParams,
+    platform_config: Optional[PlatformConfig] = None,
+    context: Optional[SOMATileDBContext] = None,
+) -> DataFrame:
+    df[SOMA_JOINID] = np.arange(len(df), dtype=np.int64)
+
+    df.reset_index(inplace=True)
+    if id_column_name is not None:
+        df.rename(columns={"index": id_column_name}, inplace=True)
+    df.set_index(SOMA_JOINID, inplace=True)
+
+    return _write_dataframe_impl(
+        df,
+        df_uri,
+        ingestion_params=ingestion_params,
+        platform_config=platform_config,
+        context=context,
+    )
+
+
+def _write_dataframe_impl(
+    df: pd.DataFrame,
+    df_uri: str,
+    *,
+    ingestion_params: IngestionParams,
+    platform_config: Optional[PlatformConfig] = None,
+    context: Optional[SOMATileDBContext] = None,
+) -> DataFrame:
+    s = _util.get_start_stamp()
+    logging.log_io(None, f"START  WRITING {df_uri}")
+
+    arrow_table = _df_to_arrow(df)
+
     try:
         soma_df = _factory.open(df_uri, "w", soma_type=DataFrame, context=context)
     except DoesNotExistError:
         soma_df = DataFrame.create(
             df_uri,
             schema=arrow_table.schema,
             platform_config=platform_config,
             context=context,
         )
     else:
-        if ingest_mode == "resume":
+        if ingestion_params.skip_existing_nonempty_domain:
             storage_ned = _read_nonempty_domain(soma_df)
             dim_range = ((int(df.index.min()), int(df.index.max())),)
             if _chunk_is_contained_in(dim_range, storage_ned):
                 logging.log_io(
                     f"Skipped {soma_df.uri}",
                     _util.format_elapsed(s, f"SKIPPED {soma_df.uri}"),
                 )
                 return soma_df
         else:
             raise SOMAError(f"{soma_df.uri} already exists")
 
-    if ingest_mode == "schema_only":
+    if ingestion_params.write_schema_no_data:
         logging.log_io(
             f"Wrote schema {soma_df.uri}",
             _util.format_elapsed(s, f"FINISH WRITING SCHEMA {soma_df.uri}"),
         )
         return soma_df
 
     soma_df.write(arrow_table)
@@ -686,14 +755,37 @@
 ) -> _NDArr:
     """
     Create and populate the ``soma_matrix`` from the contents of ``matrix``.
 
     Lifecycle:
         Experimental.
     """
+    return _create_from_matrix(
+        cls,
+        uri,
+        matrix,
+        ingestion_params=IngestionParams(ingest_mode),
+        platform_config=platform_config,
+        context=context,
+    )
+
+
+@typeguard_ignore
+def _create_from_matrix(
+    cls: Type[_NDArr],
+    uri: str,
+    matrix: Union[Matrix, h5py.Dataset],
+    *,
+    ingestion_params: IngestionParams,
+    platform_config: Optional[PlatformConfig] = None,
+    context: Optional[SOMATileDBContext] = None,
+) -> _NDArr:
+    """
+    Internal helper for user-facing ``create_from_matrix``.
+    """
     # SparseDataset has no ndim but it has a shape
     if len(matrix.shape) != 2:
         raise ValueError(f"expected matrix.shape == 2; got {matrix.shape}")
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {uri}")
 
@@ -708,18 +800,18 @@
             uri,
             type=pa.from_numpy_dtype(matrix.dtype),
             shape=shape,
             platform_config=platform_config,
             context=context,
         )
     else:
-        if ingest_mode != "resume":
+        if ingestion_params.error_if_already_exists:
             raise SOMAError(f"{soma_ndarray.uri} already exists")
 
-    if ingest_mode == "schema_only":
+    if ingestion_params.write_schema_no_data:
         logging.log_io(
             f"Wrote schema {soma_ndarray.uri}",
             _util.format_elapsed(s, f"FINISH WRITING SCHEMA {soma_ndarray.uri}"),
         )
         return soma_ndarray
 
     logging.log_io(
@@ -731,25 +823,25 @@
         _write_matrix_to_denseNDArray(
             soma_ndarray,
             matrix,
             tiledb_create_options=TileDBCreateOptions.from_platform_config(
                 platform_config
             ),
             context=context,
-            ingest_mode=ingest_mode,
+            ingestion_params=ingestion_params,
         )
     elif isinstance(soma_ndarray, SparseNDArray):  # SOMASparseNDArray
         _write_matrix_to_sparseNDArray(
             soma_ndarray,
             matrix,
             tiledb_create_options=TileDBCreateOptions.from_platform_config(
                 platform_config
             ),
             context=context,
-            ingest_mode=ingest_mode,
+            ingestion_params=ingestion_params,
         )
     else:
         raise TypeError(f"unknown array type {type(soma_ndarray)}")
 
     logging.log_io(
         f"Wrote   {soma_ndarray.uri}",
         _util.format_elapsed(s, f"FINISH WRITING {soma_ndarray.uri}"),
@@ -771,14 +863,16 @@
     ``scanpy.pp.log1p``, etc.
 
     Use ``ingest_mode="resume"`` to not error out if the schema already exists.
 
     Lifecycle:
         Experimental.
     """
+    if exp.closed or exp.mode != "w":
+        raise SOMAError(f"Experiment must be open for write: {exp.uri}")
     add_matrix_to_collection(
         exp,
         measurement_name,
         "X",
         X_layer_name,
         X_layer_data,
         use_relative_uri=use_relative_uri,
@@ -801,32 +895,33 @@
     ``scanpy.pp.log1p``, etc.
 
     Use ``ingest_mode="resume"`` to not error out if the schema already exists.
 
     Lifecycle:
         Experimental.
     """
+    ingestion_params = IngestionParams(ingest_mode)
     with exp.ms[measurement_name] as meas:
         if collection_name in meas:
             coll = cast(Collection[RawHandle], meas[collection_name])
         else:
             coll = _create_or_open_coll(
                 Collection,
                 f"{meas.uri}/{collection_name}",
-                ingest_mode,
+                ingestion_params=ingestion_params,
                 context=context,
             )
             _maybe_set(meas, collection_name, coll, use_relative_uri=use_relative_uri)
         with coll:
             uri = f"{coll.uri}/{matrix_name}"
-            with create_from_matrix(
+            with _create_from_matrix(
                 SparseNDArray,
                 uri,
                 matrix_data,
-                ingest_mode=ingest_mode,
+                ingestion_params=ingestion_params,
                 context=context,
             ) as sparse_nd_array:
                 _maybe_set(
                     coll,
                     matrix_name,
                     sparse_nd_array,
                     use_relative_uri=use_relative_uri,
@@ -834,28 +929,28 @@
 
 
 def _write_matrix_to_denseNDArray(
     soma_ndarray: DenseNDArray,
     matrix: Union[Matrix, h5py.Dataset],
     tiledb_create_options: TileDBCreateOptions,
     context: Optional[SOMATileDBContext],
-    ingest_mode: IngestMode,
+    ingestion_params: IngestionParams,
 ) -> None:
     """Write a matrix to an empty DenseNDArray"""
 
     # There is a chunk-by-chunk already-done check for resume mode, below.
     # This full-matrix-level check here might seem redundant, but in fact it's important:
     # * By checking input bounds against storage NED here, we can see if the entire matrix
     #   was already ingested and avoid even loading chunks;
     # * By checking chunkwise we can catch the case where a matrix was already *partly*
     #   ingested.
     # * Of course, this also helps us catch already-completed writes in the non-chunked case.
     # TODO: make sure we're not using an old timestamp for this
     storage_ned = None
-    if ingest_mode == "resume":
+    if ingestion_params.skip_existing_nonempty_domain:
         # This lets us check for already-ingested chunks, when in resume-ingest mode.
         storage_ned = _read_nonempty_domain(soma_ndarray)
         matrix_bounds = [
             (0, int(n - 1)) for n in matrix.shape
         ]  # Cast for lint in case np.int64
         logging.log_io(
             None,
@@ -890,15 +985,15 @@
             None,
             "START  chunk rows %d..%d of %d (%.3f%%)"
             % (i, i2 - 1, nrow, chunk_percent),
         )
 
         chunk = matrix[i:i2, :]
 
-        if ingest_mode == "resume" and storage_ned is not None:
+        if ingestion_params.skip_existing_nonempty_domain and storage_ned is not None:
             chunk_bounds = matrix_bounds
             chunk_bounds[0] = (
                 int(i),
                 int(i2 - 1),
             )  # Cast for lint in case np.int64
             if _chunk_is_contained_in_axis(chunk_bounds, storage_ned, 0):
                 # Print doubly inclusive lo..hi like 0..17 and 18..31.
@@ -1004,15 +1099,15 @@
 
 
 def _write_matrix_to_sparseNDArray(
     soma_ndarray: SparseNDArray,
     matrix: Matrix,
     tiledb_create_options: TileDBCreateOptions,
     context: Optional[SOMATileDBContext],
-    ingest_mode: IngestMode,
+    ingestion_params: IngestionParams,
 ) -> None:
     """Write a matrix to an empty DenseNDArray"""
 
     def _coo_to_table(mat_coo: sp.coo_matrix, axis: int = 0, base: int = 0) -> pa.Table:
         pydict = {
             "soma_data": mat_coo.data,
             "soma_dim_0": mat_coo.row + base if base > 0 and axis == 0 else mat_coo.row,
@@ -1025,15 +1120,15 @@
     # * By checking input bounds against storage NED here, we can see if the entire matrix
     #   was already ingested and avoid even loading chunks;
     # * By checking chunkwise we can catch the case where a matrix was already *partly*
     #   ingested.
     # * Of course, this also helps us catch already-completed writes in the non-chunked case.
     # TODO: make sure we're not using an old timestamp for this
     storage_ned = None
-    if ingest_mode == "resume":
+    if ingestion_params.skip_existing_nonempty_domain:
         # This lets us check for already-ingested chunks, when in resume-ingest mode.
         # THIS IS A HACK AND ONLY WORKS BECAUSE WE ARE DOING THIS BEFORE ALL WRITES.
         storage_ned = _read_nonempty_domain(soma_ndarray)
         matrix_bounds = [
             (0, int(n - 1)) for n in matrix.shape
         ]  # Cast for lint in case np.int64
         logging.log_io(
@@ -1092,15 +1187,15 @@
         i2 = i + chunk_size
 
         coords[stride_axis] = slice(i, i2)
         chunk_coo = sp.coo_matrix(matrix[tuple(coords)])
 
         chunk_percent = min(100, 100 * (i2 - 1) / dim_max_size)
 
-        if ingest_mode == "resume" and storage_ned is not None:
+        if ingestion_params.skip_existing_nonempty_domain and storage_ned is not None:
             chunk_bounds = matrix_bounds
             chunk_bounds[stride_axis] = (
                 int(i),
                 int(i2 - 1),
             )  # Cast for lint in case np.int64
             if _chunk_is_contained_in_axis(chunk_bounds, storage_ned, stride_axis):
                 # Print doubly inclusive lo..hi like 0..17 and 18..31.
@@ -1187,122 +1282,208 @@
 
     return True
 
 
 def _maybe_ingest_uns(
     m: Measurement,
     uns: Mapping[str, object],
+    *,
     platform_config: Optional[PlatformConfig],
     context: Optional[SOMATileDBContext],
-    ingest_mode: IngestMode,
-    *,
+    ingestion_params: IngestionParams,
     use_relative_uri: Optional[bool],
 ) -> None:
     # Don't try to ingest an empty uns.
     if not uns:
         return
     _ingest_uns_dict(
         m,
         "uns",
         uns,
-        platform_config,
-        context,
-        ingest_mode,
+        platform_config=platform_config,
+        context=context,
+        ingestion_params=ingestion_params,
         use_relative_uri=use_relative_uri,
     )
 
 
 def _ingest_uns_dict(
     parent: AnyTileDBCollection,
     parent_key: str,
     dct: Mapping[str, object],
+    *,
     platform_config: Optional[PlatformConfig],
     context: Optional[SOMATileDBContext],
-    ingest_mode: IngestMode,
-    *,
+    ingestion_params: IngestionParams,
     use_relative_uri: Optional[bool],
 ) -> None:
+
     with _create_or_open_coll(
         Collection,
         _util.uri_joinpath(parent.uri, parent_key),
-        ingest_mode,
+        ingestion_params=ingestion_params,
         context=context,
     ) as coll:
         _maybe_set(parent, parent_key, coll, use_relative_uri=use_relative_uri)
         coll.metadata["soma_tiledbsoma_type"] = "uns"
         for key, value in dct.items():
-            if isinstance(value, np.generic):
-                # This is some kind of numpy scalar value. Metadata entries
-                # only accept native Python types, so unwrap it.
-                value = value.item()
-            if isinstance(value, (int, float, str)):
-                # Primitives get set on the metadata.
-                coll.metadata[key] = value
-                continue
-            if isinstance(value, Mapping):
-                # Mappings are represented as sub-dictionaries.
-                _ingest_uns_dict(
-                    coll,
-                    key,
-                    value,
-                    platform_config,
-                    context,
-                    ingest_mode,
-                    use_relative_uri=use_relative_uri,
-                )
-                continue
-            if isinstance(value, pd.DataFrame):
-                with _write_dataframe(
-                    _util.uri_joinpath(coll.uri, key),
-                    value,
-                    None,
-                    platform_config,
-                    context=context,
-                    ingest_mode=ingest_mode,
-                ) as df:
-                    _maybe_set(coll, key, df, use_relative_uri=use_relative_uri)
-                continue
-            if isinstance(value, list) or "numpy" in str(type(value)):
-                value = np.asarray(value)
-            if isinstance(value, np.ndarray):
-                if value.dtype.names is not None:
-                    msg = (
-                        f"Skipped {coll.uri}[{key!r}]"
-                        " (uns): unsupported structured array"
-                    )
-                    # This is a structured array, which we do not support.
-                    logging.log_io(msg, msg)
-                    continue
+            _ingest_uns_node(
+                coll,
+                key,
+                value,
+                platform_config=platform_config,
+                context=context,
+                ingestion_params=ingestion_params,
+                use_relative_uri=use_relative_uri,
+            )
 
-                _ingest_uns_ndarray(
-                    coll,
-                    key,
-                    value,
-                    platform_config,
-                    context=context,
-                    use_relative_uri=use_relative_uri,
-                )
-            else:
-                msg = (
-                    f"Skipped {coll.uri}[{key!r}]"
-                    f" (uns object): unrecognized type {type(value)}"
-                )
-                logging.log_io(msg, msg)
     msg = f"Wrote   {coll.uri} (uns collection)"
     logging.log_io(msg, msg)
 
 
+def _ingest_uns_node(
+    coll: Any,
+    key: Any,
+    value: Any,
+    *,
+    platform_config: Optional[PlatformConfig],
+    context: Optional[SOMATileDBContext],
+    ingestion_params: IngestionParams,
+    use_relative_uri: Optional[bool],
+) -> None:
+
+    if isinstance(value, np.generic):
+        # This is some kind of numpy scalar value. Metadata entries
+        # only accept native Python types, so unwrap it.
+        value = value.item()
+
+    if isinstance(value, (int, float, str)):
+        # Primitives get set on the metadata.
+        coll.metadata[key] = value
+        return
+
+    if isinstance(value, Mapping):
+        # Mappings are represented as sub-dictionaries.
+        _ingest_uns_dict(
+            coll,
+            key,
+            value,
+            platform_config=platform_config,
+            context=context,
+            ingestion_params=ingestion_params,
+            use_relative_uri=use_relative_uri,
+        )
+        return
+
+    if isinstance(value, pd.DataFrame):
+        with _write_dataframe(
+            _util.uri_joinpath(coll.uri, key),
+            value,
+            None,
+            platform_config=platform_config,
+            context=context,
+            ingestion_params=ingestion_params,
+        ) as df:
+            _maybe_set(coll, key, df, use_relative_uri=use_relative_uri)
+        return
+
+    if isinstance(value, list) or "numpy" in str(type(value)):
+        value = np.asarray(value)
+    if isinstance(value, np.ndarray):
+        if value.dtype.names is not None:
+            msg = f"Skipped {coll.uri}[{key!r}]" " (uns): unsupported structured array"
+            # This is a structured array, which we do not support.
+            logging.log_io(msg, msg)
+            return
+
+        if value.dtype.char in ("U", "O"):
+            # In the wild it's quite common to see arrays of strings in uns data.
+            # Frequent example: uns["louvain_colors"].
+            _ingest_uns_string_array(
+                coll,
+                key,
+                value,
+                platform_config,
+                context=context,
+                use_relative_uri=use_relative_uri,
+                ingestion_params=ingestion_params,
+            )
+        else:
+            _ingest_uns_ndarray(
+                coll,
+                key,
+                value,
+                platform_config,
+                context=context,
+                use_relative_uri=use_relative_uri,
+                ingestion_params=ingestion_params,
+            )
+        return
+
+    msg = (
+        f"Skipped {coll.uri}[{key!r}]" f" (uns object): unrecognized type {type(value)}"
+    )
+    logging.log_io(msg, msg)
+
+
+def _ingest_uns_string_array(
+    coll: AnyTileDBCollection,
+    key: str,
+    value: NPNDArray,
+    platform_config: Optional[PlatformConfig],
+    context: Optional[SOMATileDBContext],
+    *,
+    use_relative_uri: Optional[bool],
+    ingestion_params: IngestionParams,
+) -> None:
+    """
+    Ingest an uns string array. In the SOMA data model, we have NDArrays _of number only_ ...
+    so we need to make this a SOMADataFrame.
+
+    Ideally we don't want to an index column "soma_joinid" -- "index", maybe.
+    However, ``SOMADataFrame`` _requires_ that soma_joinid be present, either
+    as an index column, or as a data column. The former is less confusing.
+    """
+    if len(value.shape) != 1:
+        msg = (
+            f"Skipped {coll.uri}[{key!r}]"
+            f" (uns object): string-array is not one-dimensional"
+        )
+        logging.log_io(msg, msg)
+        return
+
+    n = len(value)
+    df_uri = _util.uri_joinpath(coll.uri, key)
+    df = pd.DataFrame(
+        data={
+            "soma_joinid": np.arange(n, dtype=np.int64),
+            "values": [str(e) if e else "" for e in value],
+        }
+    )
+    df.set_index("soma_joinid", inplace=True)
+
+    with _write_dataframe_impl(
+        df,
+        df_uri,
+        ingestion_params=ingestion_params,
+        platform_config=platform_config,
+        context=context,
+    ) as soma_df:
+        _maybe_set(coll, key, soma_df, use_relative_uri=use_relative_uri)
+
+
 def _ingest_uns_ndarray(
     coll: AnyTileDBCollection,
     key: str,
     value: NPNDArray,
     platform_config: Optional[PlatformConfig],
     context: Optional[SOMATileDBContext],
     *,
     use_relative_uri: Optional[bool],
+    ingestion_params: IngestionParams,
 ) -> None:
     arr_uri = _util.uri_joinpath(coll.uri, key)
 
     if any(e <= 0 for e in value.shape):
         msg = f"Skipped {arr_uri} (uns ndarray): zero in shape {value.shape}"
         logging.log_io(msg, msg)
         return
@@ -1322,14 +1503,27 @@
         soma_arr = DenseNDArray.create(
             arr_uri,
             type=pa_dtype,
             shape=value.shape,
             platform_config=platform_config,
             context=context,
         )
+
+    # If resume mode: don't re-write existing data. This is the user's explicit request
+    # that we not re-write things that have already been written.
+    if ingestion_params.skip_existing_nonempty_domain:
+        storage_ned = _read_nonempty_domain(soma_arr)
+        dim_range = ((0, value.shape[0] - 1),)
+        if _chunk_is_contained_in(dim_range, storage_ned):
+            logging.log_io(
+                f"Skipped {soma_arr.uri}",
+                f"Skipped {soma_arr.uri}",
+            )
+            return
+
     with soma_arr:
         _maybe_set(coll, key, soma_arr, use_relative_uri=use_relative_uri)
         soma_arr.write(
             (),
             pa.Tensor.from_numpy(value),
             platform_config=platform_config,
         )
@@ -1337,27 +1531,34 @@
 
 
 # ----------------------------------------------------------------
 def to_h5ad(
     experiment: Experiment,
     h5ad_path: Path,
     measurement_name: str,
+    *,
     X_layer_name: str = "data",
+    obs_id_name: str = "obs_id",
+    var_id_name: str = "var_id",
 ) -> None:
     """Converts the experiment group to `AnnData <https://anndata.readthedocs.io/>`_
     format and writes it to the specified ``.h5ad`` file.
 
     Lifecycle:
         Experimental.
     """
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  Experiment.to_h5ad -> {h5ad_path}")
 
     anndata = to_anndata(
-        experiment, measurement_name=measurement_name, X_layer_name=X_layer_name
+        experiment,
+        measurement_name=measurement_name,
+        obs_id_name=obs_id_name,
+        var_id_name=var_id_name,
+        X_layer_name=X_layer_name,
     )
 
     s2 = _util.get_start_stamp()
     logging.log_io(None, f"START  write {h5ad_path}")
 
     anndata.write_h5ad(h5ad_path)
 
@@ -1369,17 +1570,17 @@
 
 
 # ----------------------------------------------------------------
 def to_anndata(
     experiment: Experiment,
     measurement_name: str,
     *,
+    X_layer_name: str = "data",
     obs_id_name: str = "obs_id",
     var_id_name: str = "var_id",
-    X_layer_name: str = "data",
 ) -> ad.AnnData:
     """Converts the experiment group to `AnnData <https://anndata.readthedocs.io/>`_
     format. Choice of matrix formats is following what we often see in input
     ``.h5ad`` files:
 
     * ``X`` as ``scipy.sparse.csr_matrix``
     * ``obs``,``var`` as ``pandas.dataframe``
@@ -1399,23 +1600,23 @@
         )
     measurement = experiment.ms[measurement_name]
 
     obs_df = experiment.obs.read().concat().to_pandas()
     obs_df.drop([SOMA_JOINID], axis=1, inplace=True)
     if obs_id_name not in obs_df.keys():
         raise ValueError(
-            f"requested obs IDs column name {obs_id_name} not found in inputinput: {obs_df.keys()}"
+            f"requested obs IDs column name {obs_id_name} not found in input: {obs_df.keys()}"
         )
     obs_df.set_index(obs_id_name, inplace=True)
 
     var_df = measurement.var.read().concat().to_pandas()
     var_df.drop([SOMA_JOINID], axis=1, inplace=True)
     if var_id_name not in var_df.keys():
         raise ValueError(
-            f"requested var IDs column name {var_id_name} not found in inputinput: {var_df.keys()}"
+            f"requested var IDs column name {var_id_name} not found in input: {var_df.keys()}"
         )
     var_df.set_index(var_id_name, inplace=True)
 
     nobs = len(obs_df.index)
     nvar = len(var_df.index)
 
     if X_layer_name not in measurement.X:
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/logging.py` & `tiledbsoma-1.3.0/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.3.0/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.3.0/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.3.0/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.3.0/src/tiledbsoma/query_condition.cc`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     } catch (TileDBError &e) {
       TPY_ERROR_LOC(e.what());
     }
   }
 
   shared_ptr<QueryCondition> ptr() { return qc_; }
 
-  py::capsule __capsule__() { return py::capsule(&qc_, "qc", nullptr); }
+  py::capsule __capsule__() { return py::capsule(&qc_, "qc"); }
 
   PyQueryCondition
   combine(PyQueryCondition rhs,
           tiledb_query_condition_combination_op_t combination_op) const {
 
     auto pyqc = PyQueryCondition(nullptr, ctx_.ptr().get());
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.3.0/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.7
+Version: 1.3.0
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
 Description: # Overview
         
         This is a Python implementation of the [SOMA API specification](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md) for interacting with the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
         
         # Installation
         
-        ## Using pip
+        TileDB-SOMA is available on [PyPI](https://pypi.org/project/tiledbsoma/) and [Conda](https://anaconda.org/tiledb/tiledbsoma-py), and can be installed via `pip` or `mamba` as indicated below.
         
-        This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can install using `pip`:
+        ```bash
+        python -m pip install tiledbsoma
+        ```
         
-        ```shell
-        $ python -m pip install tiledbsoma
+        ```bash
+        mamba install -c conda-forge -c tiledb tiledbsoma-py
         ```
         
         To install a specific version:
         
         ```shell
         $ python -m pip install git+https://github.com/single-cell-data/TileDB-SOMA.git@0.0.6#subdirectory=apis/python
         ```
```

### Comparing `tiledbsoma-1.2.7/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.3.0/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,30 @@
 dist_links/libtiledbsoma/src/external/.clang-format
 dist_links/libtiledbsoma/src/external/include/span/span.hpp
 dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
 dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
 dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
 dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
 dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+dist_links/libtiledbsoma/src/soma/array_buffers.h
+dist_links/libtiledbsoma/src/soma/column_buffer.cc
+dist_links/libtiledbsoma/src/soma/column_buffer.h
 dist_links/libtiledbsoma/src/soma/logger_public.h
 dist_links/libtiledbsoma/src/soma/managed_query.cc
 dist_links/libtiledbsoma/src/soma/managed_query.h
 dist_links/libtiledbsoma/src/soma/soma_array.cc
 dist_links/libtiledbsoma/src/soma/soma_array.h
+dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
+dist_links/libtiledbsoma/src/soma/soma_dataframe.h
 dist_links/libtiledbsoma/src/soma/soma_group.cc
 dist_links/libtiledbsoma/src/soma/soma_group.h
+dist_links/libtiledbsoma/src/soma/soma_object.h
 dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-dist_links/libtiledbsoma/src/utils/array_buffers.h
 dist_links/libtiledbsoma/src/utils/arrow_adapter.h
 dist_links/libtiledbsoma/src/utils/carrow.h
-dist_links/libtiledbsoma/src/utils/column_buffer.cc
-dist_links/libtiledbsoma/src/utils/column_buffer.h
 dist_links/libtiledbsoma/src/utils/common.h
 dist_links/libtiledbsoma/src/utils/logger.cc
 dist_links/libtiledbsoma/src/utils/logger.h
 dist_links/libtiledbsoma/src/utils/stats.cc
 dist_links/libtiledbsoma/src/utils/stats.h
 dist_links/libtiledbsoma/src/utils/util.cc
 dist_links/libtiledbsoma/src/utils/util.h
@@ -54,14 +57,15 @@
 dist_links/libtiledbsoma/test/CMakeLists.txt
 dist_links/libtiledbsoma/test/test_query_condition.py
 dist_links/libtiledbsoma/test/test_simple.py
 dist_links/libtiledbsoma/test/test_soma_array.py
 dist_links/libtiledbsoma/test/unit_column_buffer.cc
 dist_links/libtiledbsoma/test/unit_managed_query.cc
 dist_links/libtiledbsoma/test/unit_soma_array.cc
+dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
 dist_links/libtiledbsoma/test/unit_soma_group.cc
 dist_links/libtiledbsoma/test/unit_thread_pool.cc
 dist_links/scripts/README.md
 dist_links/scripts/bld
 dist_links/scripts/run-clang-format.sh
 dist_links/scripts/show-versions.py
 dist_links/scripts/update-tiledb-version.py
```

### Comparing `tiledbsoma-1.2.7/version.py` & `tiledbsoma-1.3.0/version.py`

 * *Files identical despite different names*

