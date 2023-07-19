# Comparing `tmp/stardist-0.8.2.tar.gz` & `tmp/stardist-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stardist-0.8.2.tar", last modified: Sun Apr 10 16:23:20 2022, max compression
+gzip compressed data, was "stardist-0.8.3.tar", last modified: Fri Jun  3 12:57:56 2022, max compression
```

## Comparing `stardist-0.8.2.tar` & `stardist-0.8.3.tar`

### file list

```diff
@@ -1,142 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.678112 stardist-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-04-10 16:23:06.000000 stardist-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-10 16:23:06.000000 stardist-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    19584 2022-04-10 16:23:20.678112 stardist-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18639 2022-04-10 16:23:06.000000 stardist-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-10 16:23:06.000000 stardist-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-10 16:23:20.678112 stardist-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5297 2022-04-10 16:23:06.000000 stardist-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.666112 stardist-0.8.2/stardist/
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24004 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/big.py
--rw-r--r--   0 runner    (1001) docker     (121)    19488 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/bioimageio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.666112 stardist-0.8.2/stardist/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.666112 stardist-0.8.2/stardist/data/images/
--rw-r--r--   0 runner    (1001) docker     (121)    35505 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/data/images/histo.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   524544 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/data/images/img2d.tif
--rw-r--r--   0 runner    (1001) docker     (121)   138925 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/data/images/img3d.tif
--rw-r--r--   0 runner    (1001) docker     (121)   524544 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/data/images/mask2d.tif
--rw-r--r--   0 runner    (1001) docker     (121)    15419 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/data/images/mask3d.tif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.666112 stardist-0.8.2/stardist/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7322 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/geometry/geom2d.py
--rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/geometry/geom3d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.666112 stardist-0.8.2/stardist/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/kernels/stardist2d.cl
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/kernels/stardist3d.cl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.670112 stardist-0.8.2/stardist/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.662111 stardist-0.8.2/stardist/lib/external/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.670112 stardist-0.8.2/stardist/lib/external/clipper/
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/clipper/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)   142184 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/clipper/clipper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    15423 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/clipper/clipper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.670112 stardist-0.8.2/stardist/lib/external/nanoflann/
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/nanoflann/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    73558 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/nanoflann/nanoflann.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.670112 stardist-0.8.2/stardist/lib/external/qhull_src/
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/Announce.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21849 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.662111 stardist-0.8.2/stardist/lib/external/qhull_src/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.674112 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/
--rw-r--r--   0 runner    (1001) docker     (121)    73854 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    45785 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
--rw-r--r--   0 runner    (1001) docker     (121)    75784 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
--rw-r--r--   0 runner    (1001) docker     (121)   140430 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
--rw-r--r--   0 runner    (1001) docker     (121)     8707 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
--rw-r--r--   0 runner    (1001) docker     (121)    66346 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    56702 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
--rw-r--r--   0 runner    (1001) docker     (121)    21438 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
--rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
--rw-r--r--   0 runner    (1001) docker     (121)   208318 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    12247 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
--rw-r--r--   0 runner    (1001) docker     (121)   145471 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    47472 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    12127 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
--rw-r--r--   0 runner    (1001) docker     (121)    34690 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    15528 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
--rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
--rw-r--r--   0 runner    (1001) docker     (121)    25609 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    30324 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    12533 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
--rw-r--r--   0 runner    (1001) docker     (121)    20848 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
--rw-r--r--   0 runner    (1001) docker     (121)    33496 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.678112 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/
--rw-r--r--   0 runner    (1001) docker     (121)     4166 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    15929 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
--rw-r--r--   0 runner    (1001) docker     (121)     9577 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
--rw-r--r--   0 runner    (1001) docker     (121)    12043 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
--rw-r--r--   0 runner    (1001) docker     (121)    15508 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7154 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
--rw-r--r--   0 runner    (1001) docker     (121)     4490 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4332 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6853 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
--rw-r--r--   0 runner    (1001) docker     (121)     8054 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
--rw-r--r--   0 runner    (1001) docker     (121)    12637 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
--rw-r--r--   0 runner    (1001) docker     (121)     5606 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7707 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    18839 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
--rw-r--r--   0 runner    (1001) docker     (121)     6626 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4805 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    19140 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
--rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
--rw-r--r--   0 runner    (1001) docker     (121)     6274 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    19957 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/stardist2d.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12832 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/stardist3d.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    47157 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/stardist3d_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/stardist3d_impl.h
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/stardist3d_lib.c
--rw-r--r--   0 runner    (1001) docker     (121)     3891 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/stardist3d_lib.h
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/test_lib3d.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/lib/utils.h
--rw-r--r--   0 runner    (1001) docker     (121)    19434 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.678112 stardist-0.8.2/stardist/models/
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53255 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    27198 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/models/model2d.py
--rw-r--r--   0 runner    (1001) docker     (121)    32133 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/models/model3d.py
--rw-r--r--   0 runner    (1001) docker     (121)    12632 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/nms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.678112 stardist-0.8.2/stardist/plot/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     9310 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (121)    11608 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/rays3d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/sample_patches.py
--rw-r--r--   0 runner    (1001) docker     (121)    15262 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-10 16:23:06.000000 stardist-0.8.2/stardist/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 16:23:20.666112 stardist-0.8.2/stardist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19584 2022-04-10 16:23:20.000000 stardist-0.8.2/stardist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5714 2022-04-10 16:23:20.000000 stardist-0.8.2/stardist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-10 16:23:20.000000 stardist-0.8.2/stardist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-04-10 16:23:20.000000 stardist-0.8.2/stardist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-10 16:23:20.000000 stardist-0.8.2/stardist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.374268 stardist-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-06-03 12:57:39.000000 stardist-0.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-03 12:57:39.000000 stardist-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    19894 2022-06-03 12:57:56.374268 stardist-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18969 2022-06-03 12:57:39.000000 stardist-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-03 12:57:39.000000 stardist-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-03 12:57:56.374268 stardist-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-06-03 12:57:39.000000 stardist-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.358266 stardist-0.8.3/stardist/
+-rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24004 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/big.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19488 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/bioimageio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.358266 stardist-0.8.3/stardist/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/data/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    35505 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/data/images/histo.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   524544 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/data/images/img2d.tif
+-rw-r--r--   0 runner    (1001) docker     (121)   138925 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/data/images/img3d.tif
+-rw-r--r--   0 runner    (1001) docker     (121)   524544 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/data/images/mask2d.tif
+-rw-r--r--   0 runner    (1001) docker     (121)    15419 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/data/images/mask3d.tif
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7322 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/geometry/geom2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/geometry/geom3d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/kernels/
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/kernels/stardist2d.cl
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/kernels/stardist3d.cl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.354266 stardist-0.8.3/stardist/lib/external/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/lib/external/clipper/
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/clipper/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   142184 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/clipper/clipper.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    15423 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/clipper/clipper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/lib/external/nanoflann/
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/nanoflann/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    73558 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/nanoflann/nanoflann.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.362267 stardist-0.8.3/stardist/lib/external/qhull_src/
+-rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/Announce.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21849 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.354266 stardist-0.8.3/stardist/lib/external/qhull_src/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.366267 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/
+-rw-r--r--   0 runner    (1001) docker     (121)    73854 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    45785 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)    75784 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)   140430 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)     8707 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)    66346 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    56702 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)    21438 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)   208318 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    12247 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)   145471 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    47472 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    12127 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
+-rw-r--r--   0 runner    (1001) docker     (121)    34690 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    15528 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)    25609 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    30324 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    12533 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
+-rw-r--r--   0 runner    (1001) docker     (121)    20848 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
+-rw-r--r--   0 runner    (1001) docker     (121)    33496 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.374268 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/
+-rw-r--r--   0 runner    (1001) docker     (121)     4166 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    15929 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9577 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12043 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
+-rw-r--r--   0 runner    (1001) docker     (121)    15508 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7154 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4490 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4332 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6853 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8054 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12637 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5606 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7707 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7186 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    18839 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6626 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4805 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    19140 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5300 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6274 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3158 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    19957 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/stardist2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12832 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/stardist3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    47157 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/stardist3d_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/stardist3d_impl.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/stardist3d_lib.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3891 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/stardist3d_lib.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/test_lib3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/lib/utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19434 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.374268 stardist-0.8.3/stardist/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55632 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27198 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/models/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32133 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/models/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12632 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/nms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.374268 stardist-0.8.3/stardist/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9310 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11608 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/rays3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/sample_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.374268 stardist-0.8.3/stardist/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/scripts/predict2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/scripts/predict3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15262 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-03 12:57:39.000000 stardist-0.8.3/stardist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 12:57:56.358266 stardist-0.8.3/stardist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    19894 2022-06-03 12:57:55.000000 stardist-0.8.3/stardist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-06-03 12:57:56.000000 stardist-0.8.3/stardist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 12:57:55.000000 stardist-0.8.3/stardist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-03 12:57:56.000000 stardist-0.8.3/stardist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-06-03 12:57:56.000000 stardist-0.8.3/stardist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-03 12:57:56.000000 stardist-0.8.3/stardist.egg-info/top_level.txt
```

### Comparing `stardist-0.8.2/LICENSE.txt` & `stardist-0.8.3/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2021, Uwe Schmidt, Martin Weigert
+Copyright (c) 2018-2022, Uwe Schmidt, Martin Weigert
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
@@ -22,8 +22,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `stardist-0.8.2/PKG-INFO` & `stardist-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.8.2
+Version: 0.8.3
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +20,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tf1
 Provides-Extra: test
 Provides-Extra: bioimageio
 License-File: LICENSE.txt
 
 [![PyPI version](https://badge.fury.io/py/stardist.svg)](https://pypi.org/project/stardist)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/stardist/badges/version.svg)](https://anaconda.org/conda-forge/stardist)
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 
 # *StarDist* - Object Detection with Star-convex Shapes
 
 ![](https://github.com/stardist/stardist/raw/master/images/stardist_overview.png)
@@ -269,17 +269,23 @@
 
     CC=gcc-10 CXX=g++-10 pip install stardist
 
 If you use `conda` on macOS and after `import stardist` see errors similar to `Symbol not found: _GOMP_loop_nonmonotonic_dynamic_next`, please see [this issue](https://github.com/stardist/stardist/issues/19#issuecomment-535610758) for a temporary workaround.
 
 ##### Apple Silicon
 
-As of StarDist 0.8.2, we provide `arm64` wheels that should work with macOS on Apple M1.
-For more details about installing TensorFlow and other important packages on the Apple M1 architecture, please see [this excellent post](https://forum.image.sc/t/napari-tensorflow-aicsimageio-stardist-care-n2v-pyclesperanto-running-native-on-apple-silicon-m1/55051/3) by Peter Sobolewski.
-
+As of StarDist 0.8.2, we provide `arm64` wheels that should work with macOS on Apple M1. 
+We recommend setting up an `arm64` `conda` environment with GPU-accelerated TensorFlow following [Apple's instructions](https://developer.apple.com/metal/tensorflow-plugin/) using [conda-forge miniforge3 or mambaforge](https://github.com/conda-forge/miniforge). Then install `stardist` using `pip`.
+```
+conda create -y -n stardist-env python=3.9   
+conda activate stardist-env
+conda install -c apple tensorflow-deps
+pip install tensorflow-macos tensorflow-metal
+pip install stardist
+```
 
 #### Windows
 Please install the [Build Tools for Visual Studio 2019](https://www.visualstudio.com/downloads/#build-tools-for-visual-studio-2019) (or newer) from Microsoft to compile extensions for Python 3.6+ (see [this](https://wiki.python.org/moin/WindowsCompilers) for further information). During installation, make sure to select the *C++ build tools*. Note that the compiler comes with OpenMP support.
 
 ## Plugins for other software
 
 ### ImageJ/Fiji
@@ -319,9 +325,7 @@
   title     = {Star-convex Polyhedra for 3D Object Detection and Segmentation in Microscopy},
   booktitle = {The IEEE Winter Conference on Applications of Computer Vision (WACV)},
   month     = {March},
   year      = {2020},
   doi       = {10.1109/WACV45572.2020.9093435}
 }
 ```
-
-
```

### Comparing `stardist-0.8.2/README.md` & `stardist-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![PyPI version](https://badge.fury.io/py/stardist.svg)](https://pypi.org/project/stardist)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/stardist/badges/version.svg)](https://anaconda.org/conda-forge/stardist)
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 
 # *StarDist* - Object Detection with Star-convex Shapes
 
 ![](https://github.com/stardist/stardist/raw/master/images/stardist_overview.png)
@@ -243,17 +244,23 @@
 
     CC=gcc-10 CXX=g++-10 pip install stardist
 
 If you use `conda` on macOS and after `import stardist` see errors similar to `Symbol not found: _GOMP_loop_nonmonotonic_dynamic_next`, please see [this issue](https://github.com/stardist/stardist/issues/19#issuecomment-535610758) for a temporary workaround.
 
 ##### Apple Silicon
 
-As of StarDist 0.8.2, we provide `arm64` wheels that should work with macOS on Apple M1.
-For more details about installing TensorFlow and other important packages on the Apple M1 architecture, please see [this excellent post](https://forum.image.sc/t/napari-tensorflow-aicsimageio-stardist-care-n2v-pyclesperanto-running-native-on-apple-silicon-m1/55051/3) by Peter Sobolewski.
-
+As of StarDist 0.8.2, we provide `arm64` wheels that should work with macOS on Apple M1. 
+We recommend setting up an `arm64` `conda` environment with GPU-accelerated TensorFlow following [Apple's instructions](https://developer.apple.com/metal/tensorflow-plugin/) using [conda-forge miniforge3 or mambaforge](https://github.com/conda-forge/miniforge). Then install `stardist` using `pip`.
+```
+conda create -y -n stardist-env python=3.9   
+conda activate stardist-env
+conda install -c apple tensorflow-deps
+pip install tensorflow-macos tensorflow-metal
+pip install stardist
+```
 
 #### Windows
 Please install the [Build Tools for Visual Studio 2019](https://www.visualstudio.com/downloads/#build-tools-for-visual-studio-2019) (or newer) from Microsoft to compile extensions for Python 3.6+ (see [this](https://wiki.python.org/moin/WindowsCompilers) for further information). During installation, make sure to select the *C++ build tools*. Note that the compiler comes with OpenMP support.
 
 ## Plugins for other software
 
 ### ImageJ/Fiji
```

### Comparing `stardist-0.8.2/setup.py` & `stardist-0.8.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,8 +133,15 @@
 
     extras_require={
         "tf1":  ["csbdeep[tf1]>=0.6.3"],
         "test": ["pytest"],
         "bioimageio": ["bioimageio.core>=0.5.0","importlib-metadata"],
     },
 
+    entry_points = {
+        'console_scripts': [
+            'stardist-predict2d = stardist.scripts.predict2d:main',
+            'stardist-predict3d = stardist.scripts.predict3d:main',
+        ],
+    }
+
 )
```

### Comparing `stardist-0.8.2/stardist/__init__.py` & `stardist-0.8.3/stardist/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/big.py` & `stardist-0.8.3/stardist/big.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/bioimageio_utils.py` & `stardist-0.8.3/stardist/bioimageio_utils.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/data/__init__.py` & `stardist-0.8.3/stardist/data/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/data/images/histo.jpg` & `stardist-0.8.3/stardist/data/images/histo.jpg`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/data/images/img2d.tif` & `stardist-0.8.3/stardist/data/images/img2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/data/images/img3d.tif` & `stardist-0.8.3/stardist/data/images/img3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/data/images/mask2d.tif` & `stardist-0.8.3/stardist/data/images/mask2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/data/images/mask3d.tif` & `stardist-0.8.3/stardist/data/images/mask3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/geometry/geom2d.py` & `stardist-0.8.3/stardist/geometry/geom2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/geometry/geom3d.py` & `stardist-0.8.3/stardist/geometry/geom3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/kernels/stardist2d.cl` & `stardist-0.8.3/stardist/kernels/stardist2d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/kernels/stardist3d.cl` & `stardist-0.8.3/stardist/kernels/stardist3d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/clipper/LICENSE.txt` & `stardist-0.8.3/stardist/lib/external/clipper/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/clipper/clipper.cpp` & `stardist-0.8.3/stardist/lib/external/clipper/clipper.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/clipper/clipper.hpp` & `stardist-0.8.3/stardist/lib/external/clipper/clipper.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/nanoflann/LICENSE.txt` & `stardist-0.8.3/stardist/lib/external/nanoflann/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/nanoflann/nanoflann.hpp` & `stardist-0.8.3/stardist/lib/external/nanoflann/nanoflann.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/Announce.txt` & `stardist-0.8.3/stardist/lib/external/qhull_src/Announce.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/COPYING.txt` & `stardist-0.8.3/stardist/lib/external/qhull_src/COPYING.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/README.txt` & `stardist-0.8.3/stardist/lib/external/qhull_src/README.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp` & `stardist-0.8.3/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/stardist2d.cpp` & `stardist-0.8.3/stardist/lib/stardist2d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/stardist3d.cpp` & `stardist-0.8.3/stardist/lib/stardist3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/stardist3d_impl.cpp` & `stardist-0.8.3/stardist/lib/stardist3d_impl.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/stardist3d_impl.h` & `stardist-0.8.3/stardist/lib/stardist3d_impl.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/stardist3d_lib.c` & `stardist-0.8.3/stardist/lib/stardist3d_lib.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/stardist3d_lib.h` & `stardist-0.8.3/stardist/lib/stardist3d_lib.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/test_lib3d.cpp` & `stardist-0.8.3/stardist/lib/test_lib3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/lib/utils.cpp` & `stardist-0.8.3/stardist/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/matching.py` & `stardist-0.8.3/stardist/matching.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/models/__init__.py` & `stardist-0.8.3/stardist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/models/base.py` & `stardist-0.8.3/stardist/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import warnings
 import math
 from tqdm import tqdm
 from collections import namedtuple
 from pathlib import Path
 import threading
+import functools
 import scipy.ndimage as ndi
 import numbers
 
 from csbdeep.models.base_model import BaseModel
 from csbdeep.utils.tf import export_SavedModel, keras_import, IS_TF_1, CARETensorBoard
 
 import tensorflow as tf
@@ -427,15 +428,15 @@
                                                     disable=(not _show_tile_progress), total=num_tiles_used)
 
             return tile_generator, tuple(sh), create_empty_output
 
         return x, axes, axes_net, axes_net_div_by, _permute_axes, resizer, n_tiles, grid, grid_dict, channel, predict_direct, tiling_setup
 
 
-    def predict(self, img, axes=None, normalizer=None, n_tiles=None, show_tile_progress=True, **predict_kwargs):
+    def _predict_generator(self, img, axes=None, normalizer=None, n_tiles=None, show_tile_progress=True, **predict_kwargs):
         """Predict.
 
         Parameters
         ----------
         img : :class:`numpy.ndarray`
             Input image
         axes : str or None
@@ -489,14 +490,15 @@
                 # prob and dist have different channel dimensionality than image x
                 s_src[channel] = slice(None)
                 s_dst[channel] = slice(None)
                 s_src, s_dst = tuple(s_src), tuple(s_dst)
                 # print(s_src,s_dst)
                 for part, part_tile in zip(result, result_tile):
                     part[s_dst] = part_tile[s_src]
+                yield  # yield None after each processed tile
         else:
             # predict_direct -> prob, dist, [prob_class if multi_class]
             result = predict_direct(x)
 
         result = [resizer.after(part, axes_net) for part in result]
 
         # result = (prob, dist) for legacy or (prob, dist, prob_class) for multiclass
@@ -507,18 +509,28 @@
         result[1] = np.maximum(1e-3, result[1]) # avoid small dist values to prevent problems with Qhull
         result[1] = np.moveaxis(result[1],channel,-1)
 
         if self._is_multiclass():
             # prob_class
             result[2] = np.moveaxis(result[2],channel,-1)
 
-        return tuple(result)
+        # last "yield" is the actual output that would have been "return"ed if this was a regular function
+        yield tuple(result)
 
 
-    def predict_sparse(self, img, prob_thresh=None, axes=None, normalizer=None, n_tiles=None, show_tile_progress=True, b=2, **predict_kwargs):
+    @functools.wraps(_predict_generator)
+    def predict(self, *args, **kwargs):
+        # return last "yield"ed value of generator
+        r = None
+        for r in self._predict_generator(*args, **kwargs):
+            pass
+        return r
+
+
+    def _predict_sparse_generator(self, img, prob_thresh=None, axes=None, normalizer=None, n_tiles=None, show_tile_progress=True, b=2, **predict_kwargs):
         """ Sparse version of model.predict()
         Returns
         -------
         (prob, dist, [prob_class], points)   flat list of probs, dists, (optional prob_class) and points
         """
         if prob_thresh is None: prob_thresh = self.thresholds.prob
 
@@ -567,14 +579,15 @@
                 _points = _points * np.array(self.config.grid).reshape((1,len(self.config.grid)))
                 pointsa.extend(_points)
 
                 if self._is_multiclass():
                     p = results_tile[2][s_src].copy()
                     p = np.moveaxis(p,channel,-1)
                     prob_classa.extend(p[inds])
+                yield  # yield None after each processed tile
 
         else:
             # predict_direct -> prob, dist, [prob_class if multi_class]
             results = predict_direct(x)
             prob, dist = results[:2]
             prob, dist = _prep(prob, dist)
             inds   = _ind_prob_thresh(prob, prob_thresh, b=b)
@@ -592,33 +605,43 @@
         dista = np.asarray(dista).reshape((-1,self.config.n_rays))
         pointsa = np.asarray(pointsa).reshape((-1,self.config.n_dim))
 
         idx = resizer.filter_points(x.ndim, pointsa, axes_net)
         proba = proba[idx]
         dista = dista[idx]
         pointsa = pointsa[idx]
-        
+
+        # last "yield" is the actual output that would have been "return"ed if this was a regular function
         if self._is_multiclass():
             prob_classa = np.asarray(prob_classa).reshape((-1,self.config.n_classes+1))
             prob_classa = prob_classa[idx]
-            return proba, dista, prob_classa, pointsa
+            yield proba, dista, prob_classa, pointsa
         else:
             prob_classa = None
-            return proba, dista, pointsa
+            yield proba, dista, pointsa
 
 
-    def predict_instances(self, img, axes=None, normalizer=None,
-                          sparse=True,
-                          prob_thresh=None, nms_thresh=None,
-                          scale=None,
-                          n_tiles=None, show_tile_progress=True,
-                          verbose=False,
-                          return_labels=True,
-                          predict_kwargs=None, nms_kwargs=None,
-                          overlap_label=None, return_predict=False):
+    @functools.wraps(_predict_sparse_generator)
+    def predict_sparse(self, *args, **kwargs):
+        # return last "yield"ed value of generator
+        r = None
+        for r in self._predict_sparse_generator(*args, **kwargs):
+            pass
+        return r
+
+
+    def _predict_instances_generator(self, img, axes=None, normalizer=None,
+                                     sparse=True,
+                                     prob_thresh=None, nms_thresh=None,
+                                     scale=None,
+                                     n_tiles=None, show_tile_progress=True,
+                                     verbose=False,
+                                     return_labels=True,
+                                     predict_kwargs=None, nms_kwargs=None,
+                                     overlap_label=None, return_predict=False):
         """Predict instance segmentation from input image.
 
         Parameters
         ----------
         img : :class:`numpy.ndarray`
             Input image
         axes : str or None
@@ -633,15 +656,15 @@
         prob_thresh : float or None
             Consider only object candidates from pixels with predicted object probability
             above this threshold (also see `optimize_thresholds`).
         nms_thresh : float or None
             Perform non-maximum suppression that considers two objects to be the same
             when their area/surface overlap exceeds this threshold (also see `optimize_thresholds`).
         scale: None or float or iterable
-            Scale the input image internally by this factor and rescale the output accordingly. 
+            Scale the input image internally by this factor and rescale the output accordingly.
             All spatial axes (X,Y,Z) will be scaled if a scalar value is provided.
             Alternatively, multiple scale values (compatible with input `axes`) can be used
             for more fine-grained control (scale values for non-spatial axes must be 1).
         n_tiles : iterable or None
             Out of memory (OOM) errors can occur if the input image is too large.
             To avoid this problem, the input image is broken up into (overlapping) tiles
             that are processed independently and re-assembled.
@@ -694,42 +717,68 @@
             for s,a in zip(scale,_axes):
                 s > 0 or _raise(ValueError("scale values must be greater than 0"))
                 (s in (1,None) or a in 'XYZ') or warnings.warn(f"replacing scale value {s} for non-spatial axis {a} with 1")
             scale = tuple(s if a in 'XYZ' else 1 for s,a in zip(scale,_axes))
             verbose and print(f"scaling image by factors {scale} for axes {_axes}")
             img = ndi.zoom(img, scale, order=1)
 
+        yield 'predict'  # indicate that prediction is starting
+        res = None
         if sparse:
-            res = self.predict_sparse(img, axes=axes, normalizer=normalizer, n_tiles=n_tiles,
-                                      prob_thresh=prob_thresh, show_tile_progress=show_tile_progress, **predict_kwargs)
+            for res in self._predict_sparse_generator(img, axes=axes, normalizer=normalizer, n_tiles=n_tiles,
+                                                      prob_thresh=prob_thresh, show_tile_progress=show_tile_progress, **predict_kwargs):
+                if res is None:
+                    yield 'tile'  # yield 'tile' each time a tile has been processed
         else:
-            res = self.predict(img, axes=axes, normalizer=normalizer, n_tiles=n_tiles,
-                               show_tile_progress=show_tile_progress, **predict_kwargs)
+            for res in self._predict_generator(img, axes=axes, normalizer=normalizer, n_tiles=n_tiles,
+                                               show_tile_progress=show_tile_progress, **predict_kwargs):
+                if res is None:
+                    yield 'tile'  # yield 'tile' each time a tile has been processed
             res = tuple(res) + (None,)
 
         if self._is_multiclass():
             prob, dist, prob_class, points = res
         else:
             prob, dist, points = res
             prob_class = None
 
+        yield 'nms'  # indicate that non-maximum suppression is starting
         res_instances = self._instances_from_prediction(_shape_inst, prob, dist,
                                                         points=points,
                                                         prob_class=prob_class,
                                                         prob_thresh=prob_thresh,
                                                         nms_thresh=nms_thresh,
                                                         scale=(None if scale is None else dict(zip(_axes,scale))),
                                                         return_labels=return_labels,
                                                         overlap_label=overlap_label,
                                                         **nms_kwargs)
 
+        # last "yield" is the actual output that would have been "return"ed if this was a regular function
         if return_predict:
-            return res_instances, tuple(res[:-1])
+            yield res_instances, tuple(res[:-1])
         else:
-            return res_instances
+            yield res_instances
+
+
+    @functools.wraps(_predict_instances_generator)
+    def predict_instances(self, *args, **kwargs):
+        # the reason why the actual computation happens as a generator function
+        # (in '_predict_instances_generator') is that the generator is called
+        # from the stardist napari plugin, which has its benefits regarding
+        # control flow and progress display. however, typical use cases should
+        # almost always use this function ('predict_instances'), and shouldn't
+        # even notice (thanks to @functools.wraps) that it wraps the generator
+        # function. note that similar reasoning applies to 'predict' and
+        # 'predict_sparse'.
+
+        # return last "yield"ed value of generator
+        r = None
+        for r in self._predict_instances_generator(*args, **kwargs):
+            pass
+        return r
 
 
     # def _predict_instances_old(self, img, axes=None, normalizer=None,
     #                       sparse = False,
     #                       prob_thresh=None, nms_thresh=None,
     #                       n_tiles=None, show_tile_progress=True,
     #                       verbose = False,
@@ -1136,12 +1185,12 @@
         assert points.ndim==2
         axes = axes_check_and_normalize(axes,ndim)
 
         bounds = np.array(tuple(self.padded_shape[a]-self.pad[a][1] for a in axes if a.lower() in ('z','y','x')))
         idx = np.where(np.all(points< bounds, 1))
         return idx
 
-    
+
 
 def _tf_version_at_least(version_string="1.0.0"):
     from packaging import version
     return version.parse(tf.__version__) >= version.parse(version_string)
```

### Comparing `stardist-0.8.2/stardist/models/model2d.py` & `stardist-0.8.3/stardist/models/model2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/models/model3d.py` & `stardist-0.8.3/stardist/models/model3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/nms.py` & `stardist-0.8.3/stardist/nms.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/plot/plot.py` & `stardist-0.8.3/stardist/plot/plot.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/plot/render.py` & `stardist-0.8.3/stardist/plot/render.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/rays3d.py` & `stardist-0.8.3/stardist/rays3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/sample_patches.py` & `stardist-0.8.3/stardist/sample_patches.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist/utils.py` & `stardist-0.8.3/stardist/utils.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.2/stardist.egg-info/PKG-INFO` & `stardist-0.8.3/stardist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.8.2
+Version: 0.8.3
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +20,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tf1
 Provides-Extra: test
 Provides-Extra: bioimageio
 License-File: LICENSE.txt
 
 [![PyPI version](https://badge.fury.io/py/stardist.svg)](https://pypi.org/project/stardist)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/stardist/badges/version.svg)](https://anaconda.org/conda-forge/stardist)
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 
 # *StarDist* - Object Detection with Star-convex Shapes
 
 ![](https://github.com/stardist/stardist/raw/master/images/stardist_overview.png)
@@ -269,17 +269,23 @@
 
     CC=gcc-10 CXX=g++-10 pip install stardist
 
 If you use `conda` on macOS and after `import stardist` see errors similar to `Symbol not found: _GOMP_loop_nonmonotonic_dynamic_next`, please see [this issue](https://github.com/stardist/stardist/issues/19#issuecomment-535610758) for a temporary workaround.
 
 ##### Apple Silicon
 
-As of StarDist 0.8.2, we provide `arm64` wheels that should work with macOS on Apple M1.
-For more details about installing TensorFlow and other important packages on the Apple M1 architecture, please see [this excellent post](https://forum.image.sc/t/napari-tensorflow-aicsimageio-stardist-care-n2v-pyclesperanto-running-native-on-apple-silicon-m1/55051/3) by Peter Sobolewski.
-
+As of StarDist 0.8.2, we provide `arm64` wheels that should work with macOS on Apple M1. 
+We recommend setting up an `arm64` `conda` environment with GPU-accelerated TensorFlow following [Apple's instructions](https://developer.apple.com/metal/tensorflow-plugin/) using [conda-forge miniforge3 or mambaforge](https://github.com/conda-forge/miniforge). Then install `stardist` using `pip`.
+```
+conda create -y -n stardist-env python=3.9   
+conda activate stardist-env
+conda install -c apple tensorflow-deps
+pip install tensorflow-macos tensorflow-metal
+pip install stardist
+```
 
 #### Windows
 Please install the [Build Tools for Visual Studio 2019](https://www.visualstudio.com/downloads/#build-tools-for-visual-studio-2019) (or newer) from Microsoft to compile extensions for Python 3.6+ (see [this](https://wiki.python.org/moin/WindowsCompilers) for further information). During installation, make sure to select the *C++ build tools*. Note that the compiler comes with OpenMP support.
 
 ## Plugins for other software
 
 ### ImageJ/Fiji
@@ -319,9 +325,7 @@
   title     = {Star-convex Polyhedra for 3D Object Detection and Segmentation in Microscopy},
   booktitle = {The IEEE Winter Conference on Applications of Computer Vision (WACV)},
   month     = {March},
   year      = {2020},
   doi       = {10.1109/WACV45572.2020.9093435}
 }
 ```
-
-
```

### Comparing `stardist-0.8.2/stardist.egg-info/SOURCES.txt` & `stardist-0.8.3/stardist.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 stardist/rays3d.py
 stardist/sample_patches.py
 stardist/utils.py
 stardist/version.py
 stardist.egg-info/PKG-INFO
 stardist.egg-info/SOURCES.txt
 stardist.egg-info/dependency_links.txt
+stardist.egg-info/entry_points.txt
 stardist.egg-info/requires.txt
 stardist.egg-info/top_level.txt
 stardist/data/__init__.py
 stardist/data/images/histo.jpg
 stardist/data/images/img2d.tif
 stardist/data/images/img3d.tif
 stardist/data/images/mask2d.tif
@@ -117,8 +118,11 @@
 stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
 stardist/models/__init__.py
 stardist/models/base.py
 stardist/models/model2d.py
 stardist/models/model3d.py
 stardist/plot/__init__.py
 stardist/plot/plot.py
-stardist/plot/render.py
+stardist/plot/render.py
+stardist/scripts/__init__.py
+stardist/scripts/predict2d.py
+stardist/scripts/predict3d.py
```

