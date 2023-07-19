# Comparing `tmp/dct_package-0.1.1.tar.gz` & `tmp/dct_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dct_package-0.1.1.tar", max compression
+gzip compressed data, was "dct_package-0.2.0.tar", max compression
```

## Comparing `dct_package-0.1.1.tar` & `dct_package-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       46 2023-07-19 09:23:34.975819 dct_package-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-19 09:15:06.226224 dct_package-0.1.1/dct_package/__init__.py
--rw-r--r--   0        0        0      165 2023-07-19 09:26:33.647407 dct_package-0.1.1/dct_package/scrapper.py
--rw-r--r--   0        0        0      303 2023-07-19 09:26:39.191467 dct_package-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 dct_package-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-07-19 09:23:34.975819 dct_package-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 09:15:06.226224 dct_package-0.2.0/dct_package/__init__.py
+-rw-r--r--   0        0        0      202 2023-07-19 09:27:14.917908 dct_package-0.2.0/dct_package/scrapper.py
+-rw-r--r--   0        0        0      303 2023-07-19 09:27:19.602041 dct_package-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 dct_package-0.2.0/PKG-INFO
```

