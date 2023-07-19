# Comparing `tmp/zhcevanstest-1.0.tar.gz` & `tmp/zhcevanstest-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcevanstest-1.0.tar", last modified: Wed Jul 19 12:55:51 2023, max compression
+gzip compressed data, was "zhcevanstest-1.1.1.tar", last modified: Wed Jul 19 13:16:30 2023, max compression
```

## Comparing `zhcevanstest-1.0.tar` & `zhcevanstest-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 12:55:51.501696 zhcevanstest-1.0/
--rw-r--r--   0 evans      (501) staff       (20)      499 2023-07-19 12:55:51.501437 zhcevanstest-1.0/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 12:55:51.501769 zhcevanstest-1.0/setup.cfg
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 12:55:51.501082 zhcevanstest-1.0/zhcevanstest.egg-info/
--rw-r--r--   0 evans      (501) staff       (20)      499 2023-07-19 12:55:51.000000 zhcevanstest-1.0/zhcevanstest.egg-info/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)      143 2023-07-19 12:55:51.000000 zhcevanstest-1.0/zhcevanstest.egg-info/SOURCES.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 12:55:51.000000 zhcevanstest-1.0/zhcevanstest.egg-info/dependency_links.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 12:55:51.000000 zhcevanstest-1.0/zhcevanstest.egg-info/top_level.txt
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 13:16:30.549902 zhcevanstest-1.1.1/
+-rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 13:16:30.549535 zhcevanstest-1.1.1/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 13:16:30.550059 zhcevanstest-1.1.1/setup.cfg
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 13:16:30.549075 zhcevanstest-1.1.1/zhcevanstest.egg-info/
+-rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)      178 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/SOURCES.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/dependency_links.txt
+-rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/requires.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/top_level.txt
```

