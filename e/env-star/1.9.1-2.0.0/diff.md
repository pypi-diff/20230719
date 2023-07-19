# Comparing `tmp/env-star-1.9.1.tar.gz` & `tmp/env_star-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env-star-1.9.1.tar", last modified: Sat Sep 24 18:23:31 2022, max compression
+gzip compressed data, was "env_star-2.0.0.tar", max compression
```

## Comparing `env-star-1.9.1.tar` & `env_star-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,13 @@
-drwxr-xr-x   0 guscardvs  (1000) guscardvs  (1000)        0 2022-09-24 18:23:31.540514 env-star-1.9.1/
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)     1071 2022-08-21 05:18:02.000000 env-star-1.9.1/LICENSE
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      519 2022-09-24 18:23:31.540514 env-star-1.9.1/PKG-INFO
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      280 2022-08-21 05:18:02.000000 env-star-1.9.1/README.md
-drwxr-xr-x   0 guscardvs  (1000) guscardvs  (1000)        0 2022-09-24 18:23:31.540514 env-star-1.9.1/config/
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      565 2022-09-24 18:23:08.000000 env-star-1.9.1/config/__init__.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      551 2022-09-15 13:07:59.000000 env-star-1.9.1/config/_helpers.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)     3620 2022-09-15 13:12:21.000000 env-star-1.9.1/config/config.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      202 2022-08-21 05:18:02.000000 env-star-1.9.1/config/enums.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)     3799 2022-09-24 18:22:30.000000 env-star-1.9.1/config/envconfig.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      342 2022-08-21 05:18:02.000000 env-star-1.9.1/config/exceptions.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)     1175 2022-09-15 13:09:10.000000 env-star-1.9.1/config/helpers.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)     1450 2022-08-28 07:03:10.000000 env-star-1.9.1/config/mapping.py
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)        0 2022-08-21 05:18:02.000000 env-star-1.9.1/config/py.typed
-drwxr-xr-x   0 guscardvs  (1000) guscardvs  (1000)        0 2022-09-24 18:23:31.540514 env-star-1.9.1/env_star.egg-info/
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      519 2022-09-24 18:23:31.000000 env-star-1.9.1/env_star.egg-info/PKG-INFO
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      374 2022-09-24 18:23:31.000000 env-star-1.9.1/env_star.egg-info/SOURCES.txt
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)        1 2022-09-24 18:23:31.000000 env-star-1.9.1/env_star.egg-info/dependency_links.txt
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)       25 2022-09-24 18:23:31.000000 env-star-1.9.1/env_star.egg-info/requires.txt
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)        7 2022-09-24 18:23:31.000000 env-star-1.9.1/env_star.egg-info/top_level.txt
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)       78 2022-08-21 05:18:02.000000 env-star-1.9.1/pyproject.toml
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)      685 2022-09-24 18:23:31.540514 env-star-1.9.1/setup.cfg
--rw-r--r--   0 guscardvs  (1000) guscardvs  (1000)       38 2022-09-15 13:07:05.000000 env-star-1.9.1/setup.py
+-rw-r--r--   0        0        0     1071 2023-07-18 19:51:05.220720 env_star-2.0.0/LICENSE
+-rw-r--r--   0        0        0      280 2023-07-18 19:51:05.220720 env_star-2.0.0/README.md
+-rw-r--r--   0        0        0      495 2023-07-19 13:37:50.704759 env_star-2.0.0/config/__init__.py
+-rw-r--r--   0        0        0     4128 2023-07-19 13:37:50.704759 env_star-2.0.0/config/_helpers.py
+-rw-r--r--   0        0        0     3407 2023-07-19 13:37:50.704759 env_star-2.0.0/config/config.py
+-rw-r--r--   0        0        0      812 2023-07-19 13:37:50.704759 env_star-2.0.0/config/enums.py
+-rw-r--r--   0        0        0     2682 2023-07-19 13:37:50.704759 env_star-2.0.0/config/envconfig.py
+-rw-r--r--   0        0        0      501 2023-07-19 13:37:50.704759 env_star-2.0.0/config/exceptions.py
+-rw-r--r--   0        0        0      926 2023-07-19 13:37:50.704759 env_star-2.0.0/config/interface.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:51:05.220720 env_star-2.0.0/config/py.typed
+-rw-r--r--   0        0        0     1224 2023-07-19 13:37:50.704759 env_star-2.0.0/config/utils.py
+-rw-r--r--   0        0        0     1015 2023-07-19 14:11:30.576403 env_star-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 env_star-2.0.0/PKG-INFO
```

### Comparing `env-star-1.9.1/LICENSE` & `env_star-2.0.0/LICENSE`

 * *Files identical despite different names*

