# Comparing `tmp/testforBCIplot-2.0.tar.gz` & `tmp/testforBCIplot-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testforBCIplot-2.0.tar", last modified: Wed Jul 19 11:23:39 2023, max compression
+gzip compressed data, was "testforBCIplot-2.1.tar", last modified: Wed Jul 19 11:36:17 2023, max compression
```

## Comparing `testforBCIplot-2.0.tar` & `testforBCIplot-2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 11:23:39.513635 testforBCIplot-2.0/
--rw-r--r--   0 evans      (501) staff       (20)      150 2023-07-19 11:23:39.513149 testforBCIplot-2.0/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 11:23:39.513794 testforBCIplot-2.0/setup.cfg
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 11:23:39.512613 testforBCIplot-2.0/testforBCIplot.egg-info/
--rw-r--r--   0 evans      (501) staff       (20)      150 2023-07-19 11:23:39.000000 testforBCIplot-2.0/testforBCIplot.egg-info/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)      257 2023-07-19 11:23:39.000000 testforBCIplot-2.0/testforBCIplot.egg-info/SOURCES.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 11:23:39.000000 testforBCIplot-2.0/testforBCIplot.egg-info/dependency_links.txt
--rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 11:23:39.000000 testforBCIplot-2.0/testforBCIplot.egg-info/requires.txt
--rw-r--r--   0 evans      (501) staff       (20)       57 2023-07-19 11:23:39.000000 testforBCIplot-2.0/testforBCIplot.egg-info/top_level.txt
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 11:36:17.450679 testforBCIplot-2.1/
+-rw-r--r--   0 evans      (501) staff       (20)      150 2023-07-19 11:36:17.450417 testforBCIplot-2.1/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 11:36:17.450753 testforBCIplot-2.1/setup.cfg
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 11:36:17.450110 testforBCIplot-2.1/testforBCIplot.egg-info/
+-rw-r--r--   0 evans      (501) staff       (20)      150 2023-07-19 11:36:17.000000 testforBCIplot-2.1/testforBCIplot.egg-info/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)      326 2023-07-19 11:36:17.000000 testforBCIplot-2.1/testforBCIplot.egg-info/SOURCES.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 11:36:17.000000 testforBCIplot-2.1/testforBCIplot.egg-info/dependency_links.txt
+-rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 11:36:17.000000 testforBCIplot-2.1/testforBCIplot.egg-info/requires.txt
+-rw-r--r--   0 evans      (501) staff       (20)       57 2023-07-19 11:36:17.000000 testforBCIplot-2.1/testforBCIplot.egg-info/top_level.txt
```

