# Comparing `tmp/idkwhttph-0.1.1.tar.gz` & `tmp/idkwhttph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.1.1.tar", max compression
+gzip compressed data, was "idkwhttph-0.1.2.tar", max compression
```

## Comparing `idkwhttph-0.1.1.tar` & `idkwhttph-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0    19450 2023-07-19 12:57:29.753088 idkwhttph-0.1.1/idkwhttph/__init__.py
--rw-r--r--   0        0        0    17691 2023-07-19 12:29:56.022607 idkwhttph-0.1.1/idkwhttph/replit_sync.py
--rw-r--r--   0        0        0      295 2023-07-19 13:00:16.128912 idkwhttph-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-19 13:00:30.437182 idkwhttph-0.1.1/setup.py
--rw-r--r--   0        0        0      239 2023-07-19 13:00:30.437590 idkwhttph-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    37180 2023-07-19 13:09:24.076551 idkwhttph-0.1.2/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-19 13:09:13.364557 idkwhttph-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-19 13:10:17.714866 idkwhttph-0.1.2/setup.py
+-rw-r--r--   0        0        0      239 2023-07-19 13:10:17.715195 idkwhttph-0.1.2/PKG-INFO
```

