# Comparing `tmp/gaiacalc-0.2.2.tar.gz` & `tmp/gaiacalc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiacalc-0.2.2.tar", last modified: Mon Dec 19 21:11:26 2022, max compression
+gzip compressed data, was "gaiacalc-1.0.0.tar", last modified: Wed Jul 19 11:15:43 2023, max compression
```

## Comparing `gaiacalc-0.2.2.tar` & `gaiacalc-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.686634 gaiacalc-0.2.2/
--rw-rw-r--   0 loutre     (501) staff       (20)     1074 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/LICENCE
--rw-rw-r--   0 loutre     (501) staff       (20)      151 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/MANIFEST.in
--rw-r--r--   0 loutre     (501) staff       (20)     1581 2022-12-19 21:11:26.686413 gaiacalc-0.2.2/PKG-INFO
--rw-rw-r--   0 loutre     (501) staff       (20)     1157 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/README.txt
--rw-rw-r--   0 loutre     (501) staff       (20)      705 2022-12-19 21:09:24.000000 gaiacalc-0.2.2/pyproject.toml
--rw-r--r--   0 loutre     (501) staff       (20)       38 2022-12-19 21:11:26.686690 gaiacalc-0.2.2/setup.cfg
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.631797 gaiacalc-0.2.2/src/
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.635093 gaiacalc-0.2.2/src/gaiacalc/
--rw-rw-r--   0 loutre     (501) staff       (20)        0 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/__init__.py
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.644734 gaiacalc-0.2.2/src/gaiacalc/data/
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.670175 gaiacalc-0.2.2/src/gaiacalc/data/DA/
--rw-rw-r--   0 loutre     (501) staff       (20)   197356 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/024DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   297389 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/027DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   345908 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/032DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   377655 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/036DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   399219 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/043DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   843078 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/045DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   203346 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/053DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   193163 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/058DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   193163 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/066DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   212331 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/083DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   205143 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/095DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   206341 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/09DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   193762 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/100DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   203346 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/105DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   365076 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/110DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   354893 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/116DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   336923 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/122DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   390234 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA/129DA.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   766467 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DA.grid
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.685183 gaiacalc-0.2.2/src/gaiacalc/data/DB/
--rw-rw-r--   0 loutre     (501) staff       (20)   413398 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/051DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   210322 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/054DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   189686 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/058DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   170457 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/066DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   237993 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/074DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   258160 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/087DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   162015 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/095DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   165298 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/100DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   169519 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/110DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   264726 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/116DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   442008 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/122DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   238462 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB/129DB.dat
--rw-rw-r--   0 loutre     (501) staff       (20)   751111 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/DB.grid
--rw-rw-r--   0 loutre     (501) staff       (20)      499 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/bye.html
--rw-rw-r--   0 loutre     (501) staff       (20)    84806 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/gaiacalc.png
--rw-rw-r--   0 loutre     (501) staff       (20)     1241 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/guide.html
--rw-rw-r--   0 loutre     (501) staff       (20)     6744 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/guide.png
--rw-rw-r--   0 loutre     (501) staff       (20)     3681 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/install.html
--rw-rw-r--   0 loutre     (501) staff       (20)    17103 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/logoUPC.jpg
--rw-rw-r--   0 loutre     (501) staff       (20)     5635 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/page.html
--rw-rw-r--   0 loutre     (501) staff       (20)     1710 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/question.jpg
--rw-rw-r--   0 loutre     (501) staff       (20)     7503 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/quit.jpg
--rw-rw-r--   0 loutre     (501) staff       (20)   981440 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/data/samples.csv
--rw-rw-r--   0 loutre     (501) staff       (20)     4394 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/gaiacalc.py
--rw-rw-r--   0 loutre     (501) staff       (20)    16031 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/index.py
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.686068 gaiacalc-0.2.2/src/gaiacalc/log/
--rw-rw-r--   0 loutre     (501) staff       (20)       71 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/log/empty.log
--rw-rw-r--   0 loutre     (501) staff       (20)     7124 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/loop.py
--rw-rw-r--   0 loutre     (501) staff       (20)     6348 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/show.py
--rw-rw-r--   0 loutre     (501) staff       (20)     4668 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/util.py
--rw-rw-r--   0 loutre     (501) staff       (20)     4036 2022-12-19 20:48:57.000000 gaiacalc-0.2.2/src/gaiacalc/webserver.py
-drwxr-xr-x   0 loutre     (501) staff       (20)        0 2022-12-19 21:11:26.636196 gaiacalc-0.2.2/src/gaiacalc.egg-info/
--rw-r--r--   0 loutre     (501) staff       (20)     1581 2022-12-19 21:11:26.000000 gaiacalc-0.2.2/src/gaiacalc.egg-info/PKG-INFO
--rw-r--r--   0 loutre     (501) staff       (20)     1724 2022-12-19 21:11:26.000000 gaiacalc-0.2.2/src/gaiacalc.egg-info/SOURCES.txt
--rw-r--r--   0 loutre     (501) staff       (20)        1 2022-12-19 21:11:26.000000 gaiacalc-0.2.2/src/gaiacalc.egg-info/dependency_links.txt
--rw-r--r--   0 loutre     (501) staff       (20)       56 2022-12-19 21:11:26.000000 gaiacalc-0.2.2/src/gaiacalc.egg-info/entry_points.txt
--rw-r--r--   0 loutre     (501) staff       (20)       75 2022-12-19 21:11:26.000000 gaiacalc-0.2.2/src/gaiacalc.egg-info/requires.txt
--rw-r--r--   0 loutre     (501) staff       (20)        9 2022-12-19 21:11:26.000000 gaiacalc-0.2.2/src/gaiacalc.egg-info/top_level.txt
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.142588 gaiacalc-1.0.0/
+-rw-rw-r--   0 loutre     (501) staff       (20)     1074 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/LICENCE
+-rw-rw-r--   0 loutre     (501) staff       (20)      151 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/MANIFEST.in
+-rw-r--r--   0 loutre     (501) staff       (20)     1581 2023-07-19 11:15:43.142399 gaiacalc-1.0.0/PKG-INFO
+-rw-rw-r--   0 loutre     (501) staff       (20)     1157 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/README.txt
+-rw-rw-r--   0 loutre     (501) staff       (20)      705 2023-07-19 11:15:26.000000 gaiacalc-1.0.0/pyproject.toml
+-rw-r--r--   0 loutre     (501) staff       (20)       38 2023-07-19 11:15:43.142641 gaiacalc-1.0.0/setup.cfg
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.079686 gaiacalc-1.0.0/src/
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.082923 gaiacalc-1.0.0/src/gaiacalc/
+-rw-rw-r--   0 loutre     (501) staff       (20)        0 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/__init__.py
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.092973 gaiacalc-1.0.0/src/gaiacalc/data/
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.125372 gaiacalc-1.0.0/src/gaiacalc/data/DA/
+-rw-rw-r--   0 loutre     (501) staff       (20)   197356 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/024DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   297389 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/027DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   345908 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/032DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   377655 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/036DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   399219 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/043DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   843078 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/045DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   203346 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/053DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   193163 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/058DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   193163 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/066DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   212331 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/083DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   205143 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/095DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   206341 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/09DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   193762 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/100DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   203346 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/105DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   365076 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/110DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   354893 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/116DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   336923 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/122DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   390234 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA/129DA.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   766467 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DA.grid
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.138830 gaiacalc-1.0.0/src/gaiacalc/data/DB/
+-rw-rw-r--   0 loutre     (501) staff       (20)   413398 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/051DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   210322 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/054DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   189686 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/058DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   170457 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/066DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   237993 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/074DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   258160 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/087DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   162015 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/095DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   165298 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/100DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   169519 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/110DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   264726 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/116DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   442008 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/122DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   238462 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB/129DB.dat
+-rw-rw-r--   0 loutre     (501) staff       (20)   751111 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/DB.grid
+-rw-rw-r--   0 loutre     (501) staff       (20)      499 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/bye.html
+-rw-rw-r--   0 loutre     (501) staff       (20)    84806 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/gaiacalc.png
+-rw-rw-r--   0 loutre     (501) staff       (20)     1241 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/guide.html
+-rw-rw-r--   0 loutre     (501) staff       (20)     6744 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/guide.png
+-rw-rw-r--   0 loutre     (501) staff       (20)     4053 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/install.html
+-rw-rw-r--   0 loutre     (501) staff       (20)    17103 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/logoUPC.jpg
+-rw-rw-r--   0 loutre     (501) staff       (20)     5613 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/page.html
+-rw-rw-r--   0 loutre     (501) staff       (20)     1710 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/question.jpg
+-rw-rw-r--   0 loutre     (501) staff       (20)     7503 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/quit.jpg
+-rw-rw-r--   0 loutre     (501) staff       (20)   981440 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/data/samples.csv
+-rw-rw-r--   0 loutre     (501) staff       (20)     4394 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/gaiacalc.py
+-rw-rw-r--   0 loutre     (501) staff       (20)    16031 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/index.py
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.142047 gaiacalc-1.0.0/src/gaiacalc/log/
+-rw-rw-r--   0 loutre     (501) staff       (20)       71 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/log/empty.log
+-rw-rw-r--   0 loutre     (501) staff       (20)     7124 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/loop.py
+-rw-rw-r--   0 loutre     (501) staff       (20)     6348 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/show.py
+-rw-rw-r--   0 loutre     (501) staff       (20)     4668 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/util.py
+-rw-rw-r--   0 loutre     (501) staff       (20)     4036 2023-07-19 11:05:23.000000 gaiacalc-1.0.0/src/gaiacalc/webserver.py
+drwxr-xr-x   0 loutre     (501) staff       (20)        0 2023-07-19 11:15:43.084037 gaiacalc-1.0.0/src/gaiacalc.egg-info/
+-rw-r--r--   0 loutre     (501) staff       (20)     1581 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/PKG-INFO
+-rw-r--r--   0 loutre     (501) staff       (20)     1724 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/SOURCES.txt
+-rw-r--r--   0 loutre     (501) staff       (20)        1 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/dependency_links.txt
+-rw-r--r--   0 loutre     (501) staff       (20)       56 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/entry_points.txt
+-rw-r--r--   0 loutre     (501) staff       (20)       75 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/requires.txt
+-rw-r--r--   0 loutre     (501) staff       (20)        9 2023-07-19 11:15:43.000000 gaiacalc-1.0.0/src/gaiacalc.egg-info/top_level.txt
```

### Comparing `gaiacalc-0.2.2/LICENCE` & `gaiacalc-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/PKG-INFO` & `gaiacalc-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiacalc
-Version: 0.2.2
+Version: 1.0.0
 Summary: Gaia white dwarfs parameter interpolator
 Author-email: Julie Doligez <julie@doligez.fr>
 Project-URL: Homepage, http://gaia.doligez.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `gaiacalc-0.2.2/README.txt` & `gaiacalc-1.0.0/README.txt`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/pyproject.toml` & `gaiacalc-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaiacalc"
-version = "0.2.2"
+version = "1.0.0"
 authors = [
 { name="Julie Doligez", email="julie@doligez.fr" }
 ]
 description = "Gaia white dwarfs parameter interpolator"
 readme = "README.txt"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/024DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/024DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/027DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/027DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/032DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/032DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/036DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/036DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/043DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/043DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/045DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/045DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/053DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/053DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/058DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/058DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/066DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/066DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/083DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/083DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/095DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/095DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/09DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/09DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/100DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/100DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/105DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/105DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/110DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/110DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/116DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/116DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/122DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/122DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA/129DA.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DA/129DA.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DA.grid` & `gaiacalc-1.0.0/src/gaiacalc/data/DA.grid`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/051DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/051DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/054DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/054DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/058DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/058DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/066DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/066DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/074DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/074DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/087DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/087DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/095DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/095DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/100DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/100DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/110DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/110DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/116DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/116DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/122DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/122DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB/129DB.dat` & `gaiacalc-1.0.0/src/gaiacalc/data/DB/129DB.dat`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/DB.grid` & `gaiacalc-1.0.0/src/gaiacalc/data/DB.grid`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/gaiacalc.png` & `gaiacalc-1.0.0/src/gaiacalc/data/gaiacalc.png`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/guide.html` & `gaiacalc-1.0.0/src/gaiacalc/data/guide.html`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/guide.png` & `gaiacalc-1.0.0/src/gaiacalc/data/guide.png`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/install.html` & `gaiacalc-1.0.0/src/gaiacalc/data/install.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       - <a href="#exe">Download Windows exe file</a>
       - <a href="#pip">Install a python package with the classical pip tool</a>
       - <a href="#deb">Install a linux debian package to build a gaiacalc server</a>
       - <a href="#git">Get the source code on GitHub</a>
 			  
       ------------------------------------------------------------------------------------------------------
 
-      <a id=app href=http://gaia.doligez.fr/drop?file=gaiacalc.dmg>Download app for MacOS</a>
+      <a id=app href=drop?file=gaiacalc.dmg>Download app for MacOS</a>
 
       You will get the file gaiacalc.dmg.
       This is a virtual disk including the app.
       
       Installation:
       - double click gaiacalc.dmg
       - you get a new disk in your finder window, click on it
@@ -28,17 +28,18 @@
       - choose the "open" item
       - you get a window with a security warning
       - now click the "Open" button
       - first launching may be quite long, give it some time (seconds, not minutes :)
       
       ------------------------------------------------------------------------------------------------------
       
-      <a id=exe href=http://gaia.doligez.fr/drop?file=gaiacalc.exe>Download exe for Windows</a>
+      <a id=exe href=drop?file=gaiacalc.exe>Download exe for Windows</a>
 
       You will get the file gaiacalc.exe
+      Windows will complain about security risks and you have to keep the file anyway
       Double click to open gaiacalc
       First launching may be quite long, give it some time (seconds, not minutes :)
       
       ------------------------------------------------------------------------------------------------------
       
       <a id=pip href=https://pypi.org/project/gaiacalc>Download pip package for python</a>
 
@@ -50,24 +51,31 @@
       
       On Windows, use a cmd window and type this:
       py -m pip install gaiacalc
       Then you get a gaiacalc command : type "gaiacalc" then RETURN key
       
       ------------------------------------------------------------------------------------------------------
       
-      <a id=deb></a>Download deb package for linux deban
+      <a id=deb></a>Download deb package for linux debian
 
-      Not yet available
       This package is for IT administrators.
-      It will turn your debian server as a gaiacalc server.
+      It will turn your debian 11 server as a gaiacalc server.
       The user will access gaiacalc web page with URL : http://yourservername.com
       
+      First ensure that pip3 is installed (not included in debian11 on OVH cloud)
+      Otherwise type this :
+      sudo apt-get update
+      sudo apt-get install python3-pip
+      
       After downloading the file gaiacalc.deb, install it with command:
       sudo dpkg -i gaiacalc.deb
       That's it, nothing more is needed
+
+      In order to deliver the gaiacalc.deb archive itself from your new server,
+      you should copy or move it to /usr/local/lib/python3.9/dist-packages/gaiacalc/data
       
       If you want to change the server port, you can edit file /etc/init.d/gaiacalc
       Find there the args --tcpport in the line DAEMON_ARGS.
       You can change the value 80 to 8080 for example.
       Save the change and reboot your server with command : sudo reboot
       Users will now access to http://yourservername.com:8080
```

#### html2text {}

```diff
@@ -32,14 +32,16 @@
 
       -------------------------------------------------------------------------
 -----------------------------
 
       Download_exe_for_Windows
 
       You will get the file gaiacalc.exe
+      Windows will complain about security risks and you have to keep the file
+anyway
       Double click to open gaiacalc
       First launching may be quite long, give it some time (seconds, not
 minutes :)
 
       -------------------------------------------------------------------------
 -----------------------------
 
@@ -54,26 +56,35 @@
       On Windows, use a cmd window and type this:
       py -m pip install gaiacalc
       Then you get a gaiacalc command : type "gaiacalc" then RETURN key
 
       -------------------------------------------------------------------------
 -----------------------------
 
-      Download deb package for linux deban
+      Download deb package for linux debian
 
-      Not yet available
       This package is for IT administrators.
-      It will turn your debian server as a gaiacalc server.
+      It will turn your debian 11 server as a gaiacalc server.
       The user will access gaiacalc web page with URL : http://
 yourservername.com
 
+      First ensure that pip3 is installed (not included in debian11 on OVH
+cloud)
+      Otherwise type this :
+      sudo apt-get update
+      sudo apt-get install python3-pip
+
       After downloading the file gaiacalc.deb, install it with command:
       sudo dpkg -i gaiacalc.deb
       That's it, nothing more is needed
 
+      In order to deliver the gaiacalc.deb archive itself from your new server,
+      you should copy or move it to /usr/local/lib/python3.9/dist-packages/
+gaiacalc/data
+
       If you want to change the server port, you can edit file /etc/init.d/
 gaiacalc
       Find there the args --tcpport in the line DAEMON_ARGS.
       You can change the value 80 to 8080 for example.
       Save the change and reboot your server with command : sudo reboot
       Users will now access to http://yourservername.com:8080
```

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/logoUPC.jpg` & `gaiacalc-1.0.0/src/gaiacalc/data/logoUPC.jpg`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/page.html` & `gaiacalc-1.0.0/src/gaiacalc/data/page.html`

 * *Files 2% similar despite different names*

```diff
@@ -161,24 +161,24 @@
       </form>
       </div>
 
       <br>or you can get the complete story at once :
       <div class="tooltip">
 	<img src=page?name=question.jpg>
 	<span class="tooltiptext">
-	  This is a bigfile : 300 MBytes
+	  This is a bigfile : 700 MBytes
 	</span>
       </div>
       <br>
-      download the 10 millions white dwarfs known from Gaia EDR3
+      download the 1.3 millions white dwarfs known from Gaia EDR3
       with their mass and temperature :)
 
       <br><br>
       <div style="margin-left: 200">
-	<a href=http://gaia.doligez.fr/drop?file=bigfile.csv.gz>oh yeah, I want this one</a>
+	<a href=drop?file=bigfile.csv.gz>oh yeah, I want this one</a>
       </div>
 
       <div id="rectangle">
       Download your gaiacalc<br><br>
       <a href=page?name=install.html#app>app for MacOS</a><br>
       <a href=page?name=install.html#exe>exe for Windows</a><br>
       <a href=page?name=install.html#pip>python pip3 package</a><br>
```

#### html2text {}

```diff
@@ -36,17 +36,17 @@
 [page?name=question.jpg]  Name of column (if header)
 or rank of column (zero-based) or uncheck to compute both DA/DB
 
 [send file and download computing result] %s
 [show data on HRD diagram]
 
 or you can get the complete story at once :
-[page?name=question.jpg]  This is a bigfile : 300 MBytes
+[page?name=question.jpg]  This is a bigfile : 700 MBytes
 
-download the 10 millions white dwarfs known from Gaia EDR3 with their mass and
+download the 1.3 millions white dwarfs known from Gaia EDR3 with their mass and
 temperature :)
 
 oh_yeah,_I_want_this_one
 Download your gaiacalc
 
 app_for_MacOS
 exe_for_Windows
```

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/question.jpg` & `gaiacalc-1.0.0/src/gaiacalc/data/question.jpg`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/quit.jpg` & `gaiacalc-1.0.0/src/gaiacalc/data/quit.jpg`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/data/samples.csv` & `gaiacalc-1.0.0/src/gaiacalc/data/samples.csv`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/gaiacalc.py` & `gaiacalc-1.0.0/src/gaiacalc/gaiacalc.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/index.py` & `gaiacalc-1.0.0/src/gaiacalc/index.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/loop.py` & `gaiacalc-1.0.0/src/gaiacalc/loop.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/show.py` & `gaiacalc-1.0.0/src/gaiacalc/show.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/util.py` & `gaiacalc-1.0.0/src/gaiacalc/util.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc/webserver.py` & `gaiacalc-1.0.0/src/gaiacalc/webserver.py`

 * *Files identical despite different names*

### Comparing `gaiacalc-0.2.2/src/gaiacalc.egg-info/PKG-INFO` & `gaiacalc-1.0.0/src/gaiacalc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiacalc
-Version: 0.2.2
+Version: 1.0.0
 Summary: Gaia white dwarfs parameter interpolator
 Author-email: Julie Doligez <julie@doligez.fr>
 Project-URL: Homepage, http://gaia.doligez.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `gaiacalc-0.2.2/src/gaiacalc.egg-info/SOURCES.txt` & `gaiacalc-1.0.0/src/gaiacalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

