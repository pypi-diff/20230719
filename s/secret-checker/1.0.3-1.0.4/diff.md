# Comparing `tmp/secret_checker-1.0.3.tar.gz` & `tmp/secret_checker-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_checker-1.0.3.tar", last modified: Sun Jul 16 17:31:51 2023, max compression
+gzip compressed data, was "secret_checker-1.0.4.tar", last modified: Wed Jul 19 07:26:12 2023, max compression
```

## Comparing `secret_checker-1.0.3.tar` & `secret_checker-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 17:31:51.970001 secret_checker-1.0.3/
--rw-rw-rw-   0        0        0      242 2023-07-16 17:31:51.969000 secret_checker-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-15 01:11:16.000000 secret_checker-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 17:31:51.947938 secret_checker-1.0.3/secret_checker/
--rw-rw-rw-   0        0        0        2 2023-07-15 18:14:03.000000 secret_checker-1.0.3/secret_checker/__init__.py
--rw-rw-rw-   0        0        0     3862 2023-07-16 17:29:06.000000 secret_checker-1.0.3/secret_checker/check_var.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:31:51.967994 secret_checker-1.0.3/secret_checker.egg-info/
--rw-rw-rw-   0        0        0      242 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 17:31:51.970001 secret_checker-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      356 2023-07-16 17:31:26.000000 secret_checker-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:26:12.985323 secret_checker-1.0.4/
+-rw-rw-rw-   0        0        0      242 2023-07-19 07:26:12.985323 secret_checker-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-15 01:11:16.000000 secret_checker-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:26:12.951860 secret_checker-1.0.4/secret_checker/
+-rw-rw-rw-   0        0        0        2 2023-07-15 18:14:03.000000 secret_checker-1.0.4/secret_checker/__init__.py
+-rw-rw-rw-   0        0        0     3928 2023-07-19 07:26:03.000000 secret_checker-1.0.4/secret_checker/check_var.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:26:12.985323 secret_checker-1.0.4/secret_checker.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-07-19 07:26:12.000000 secret_checker-1.0.4/secret_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-19 07:26:12.000000 secret_checker-1.0.4/secret_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:26:12.000000 secret_checker-1.0.4/secret_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-19 07:26:12.000000 secret_checker-1.0.4/secret_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:26:12.985323 secret_checker-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      356 2023-07-19 07:25:02.000000 secret_checker-1.0.4/setup.py
```

