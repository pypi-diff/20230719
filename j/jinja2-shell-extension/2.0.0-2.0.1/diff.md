# Comparing `tmp/jinja2_shell_extension-2.0.0.tar.gz` & `tmp/jinja2_shell_extension-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_shell_extension-2.0.0.tar", last modified: Fri Jan 13 14:51:32 2023, max compression
+gzip compressed data, was "jinja2_shell_extension-2.0.1.tar", last modified: Wed Jul 19 11:27:22 2023, max compression
```

## Comparing `jinja2_shell_extension-2.0.0.tar` & `jinja2_shell_extension-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:51:32.961189 jinja2_shell_extension-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-13 14:51:22.000000 jinja2_shell_extension-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-13 14:51:22.000000 jinja2_shell_extension-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-13 14:51:32.961189 jinja2_shell_extension-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-01-13 14:51:22.000000 jinja2_shell_extension-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:51:32.961189 jinja2_shell_extension-2.0.0/jinja2_shell_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-01-13 14:51:22.000000 jinja2_shell_extension-2.0.0/jinja2_shell_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:51:32.961189 jinja2_shell_extension-2.0.0/jinja2_shell_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-13 14:51:32.000000 jinja2_shell_extension-2.0.0/jinja2_shell_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-13 14:51:32.000000 jinja2_shell_extension-2.0.0/jinja2_shell_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 14:51:32.000000 jinja2_shell_extension-2.0.0/jinja2_shell_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 14:51:32.000000 jinja2_shell_extension-2.0.0/jinja2_shell_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-13 14:51:32.000000 jinja2_shell_extension-2.0.0/jinja2_shell_extension.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 14:51:22.000000 jinja2_shell_extension-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 14:51:32.961189 jinja2_shell_extension-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-13 14:51:22.000000 jinja2_shell_extension-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:27:22.656541 jinja2_shell_extension-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-19 11:27:12.000000 jinja2_shell_extension-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 11:27:12.000000 jinja2_shell_extension-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-19 11:27:22.656541 jinja2_shell_extension-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-19 11:27:12.000000 jinja2_shell_extension-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:27:22.656541 jinja2_shell_extension-2.0.1/jinja2_shell_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-19 11:27:12.000000 jinja2_shell_extension-2.0.1/jinja2_shell_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:27:22.656541 jinja2_shell_extension-2.0.1/jinja2_shell_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-19 11:27:22.000000 jinja2_shell_extension-2.0.1/jinja2_shell_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 11:27:22.000000 jinja2_shell_extension-2.0.1/jinja2_shell_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:27:22.000000 jinja2_shell_extension-2.0.1/jinja2_shell_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 11:27:22.000000 jinja2_shell_extension-2.0.1/jinja2_shell_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 11:27:22.000000 jinja2_shell_extension-2.0.1/jinja2_shell_extension.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 11:27:12.000000 jinja2_shell_extension-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:27:22.656541 jinja2_shell_extension-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-19 11:27:12.000000 jinja2_shell_extension-2.0.1/setup.py
```

### Comparing `jinja2_shell_extension-2.0.0/LICENSE` & `jinja2_shell_extension-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_shell_extension-2.0.0/jinja2_shell_extension/__init__.py` & `jinja2_shell_extension-2.0.1/jinja2_shell_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jinja2_shell_extension-2.0.0/setup.py` & `jinja2_shell_extension-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     author="Fabien MARTY",
     author_email="fabien.marty@gmail.com",
     name="jinja2_shell_extension",
-    version="2.0.0",
+    version="2.0.1",
     license="BSD",
     packages=find_packages(),
     install_requires=install_requires,
     python_requires='>=3.0',
     description="a jinja2 extension to access to system environment variables",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

