# Comparing `tmp/hserv-0.0.1.tar.gz` & `tmp/hserv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hserv-0.0.1.tar", last modified: Mon Jul 17 15:17:11 2023, max compression
+gzip compressed data, was "hserv-0.0.2.tar", last modified: Wed Jul 19 06:39:00 2023, max compression
```

## Comparing `hserv-0.0.1.tar` & `hserv-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-07-17 15:17:11.277353 hserv-0.0.1/
--rw-r--r--   0 mirko      (501) staff       (20)    35149 2023-07-17 15:06:39.000000 hserv-0.0.1/LICENSE
--rw-r--r--   0 mirko      (501) staff       (20)      187 2023-07-17 15:17:11.277147 hserv-0.0.1/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)       69 2023-07-17 15:06:39.000000 hserv-0.0.1/README.md
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-07-17 15:17:11.275884 hserv-0.0.1/hserv/
--rw-r--r--   0 mirko      (501) staff       (20)       36 2023-07-17 15:10:25.000000 hserv-0.0.1/hserv/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)       20 2023-07-17 15:10:15.000000 hserv-0.0.1/hserv/__version__.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-07-17 15:17:11.276778 hserv-0.0.1/hserv.egg-info/
--rw-r--r--   0 mirko      (501) staff       (20)      187 2023-07-17 15:17:11.000000 hserv-0.0.1/hserv.egg-info/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)      181 2023-07-17 15:17:11.000000 hserv-0.0.1/hserv.egg-info/SOURCES.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2023-07-17 15:17:11.000000 hserv-0.0.1/hserv.egg-info/dependency_links.txt
--rw-r--r--   0 mirko      (501) staff       (20)        6 2023-07-17 15:17:11.000000 hserv-0.0.1/hserv.egg-info/top_level.txt
--rw-r--r--   0 mirko      (501) staff       (20)       38 2023-07-17 15:17:11.277415 hserv-0.0.1/setup.cfg
--rw-r--r--   0 mirko      (501) staff       (20)      438 2023-07-17 15:17:01.000000 hserv-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:39:00.333733 hserv-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-19 06:38:49.000000 hserv-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-19 06:38:49.000000 hserv-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 06:39:00.333733 hserv-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-19 06:38:49.000000 hserv-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:39:00.333733 hserv-0.0.2/hserv/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-19 06:38:49.000000 hserv-0.0.2/hserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-19 06:38:49.000000 hserv-0.0.2/hserv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-19 06:38:49.000000 hserv-0.0.2/hserv/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 06:39:00.333733 hserv-0.0.2/hserv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-19 06:39:00.000000 hserv-0.0.2/hserv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-19 06:38:49.000000 hserv-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 06:39:00.333733 hserv-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-19 06:38:49.000000 hserv-0.0.2/setup.py
```

### Comparing `hserv-0.0.1/LICENSE` & `hserv-0.0.2/LICENSE`

 * *Files identical despite different names*

