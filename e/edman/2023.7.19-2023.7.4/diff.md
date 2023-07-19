# Comparing `tmp/edman-2023.7.19.tar.gz` & `tmp/edman-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2023.7.19.tar", last modified: Wed Jul 19 02:01:20 2023, max compression
+gzip compressed data, was "edman-2023.7.4.tar", last modified: Thu Jul  6 01:11:38 2023, max compression
```

## Comparing `edman-2023.7.19.tar` & `edman-2023.7.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.597507 edman-2023.7.19/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/.github/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/.github/workflows/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1574 2023-05-24 04:09:58.000000 edman-2023.7.19/.github/workflows/unittest.yml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2022-07-27 01:25:38.000000 edman-2023.7.19/.gitignore
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/.idea/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2023.7.19/.idea/.gitignore
--rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2023.7.19/.idea/edman.iml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/.idea/inspectionProfiles/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2023.7.19/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      254 2023-04-10 07:58:11.000000 edman-2023.7.19/.idea/misc.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2023.7.19/.idea/modules.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2023.7.19/.idea/vcs.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.7.19/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7672 2023-07-19 02:01:20.597507 edman-2023.7.19/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6112 2023-07-19 01:58:48.000000 edman-2023.7.19/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      169 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1448 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16599 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    48577 2023-07-04 02:31:14.000000 edman-2023.7.19/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.7.19/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    24865 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1492 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2023.7.19/edman/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9640 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10900 2023-05-24 04:09:58.000000 edman-2023.7.19/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7672 2023-07-19 02:01:20.000000 edman-2023.7.19/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      986 2023-07-19 02:01:20.000000 edman-2023.7.19/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-07-19 02:01:20.000000 edman-2023.7.19/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-07-19 02:01:20.000000 edman-2023.7.19/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2023-07-19 02:01:20.000000 edman-2023.7.19/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1124 2023-07-19 01:58:48.000000 edman-2023.7.19/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-07-19 01:58:48.000000 edman-2023.7.19/requirements.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-07-19 02:01:20.597507 edman-2023.7.19/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.597507 edman-2023.7.19/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2023.7.19/tests/__init__.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.597507 edman-2023.7.19/tests/ini/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2023.7.19/tests/ini/test_db.ini.sample
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.7.19/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    88352 2023-07-04 02:31:14.000000 edman-2023.7.19/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    40726 2023-05-18 02:16:03.000000 edman-2023.7.19/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.7.19/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.7.19/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7886 2023-05-23 05:52:10.000000 edman-2023.7.19/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.587507 edman-2023.7.19/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:01:20.597507 edman-2023.7.19/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2023.7.19/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      626 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-17 00:07:28.000000 edman-2023.7.19/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.651838 edman-2023.7.4/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.641838 edman-2023.7.4/.github/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.641838 edman-2023.7.4/.github/workflows/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1574 2023-05-24 04:09:58.000000 edman-2023.7.4/.github/workflows/unittest.yml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2022-07-27 01:25:38.000000 edman-2023.7.4/.gitignore
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.641838 edman-2023.7.4/.idea/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2023.7.4/.idea/.gitignore
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2023.7.4/.idea/edman.iml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.641838 edman-2023.7.4/.idea/inspectionProfiles/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2023.7.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      254 2023-04-10 07:58:11.000000 edman-2023.7.4/.idea/misc.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2023.7.4/.idea/modules.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2023.7.4/.idea/vcs.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.7.4/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7612 2023-07-06 01:11:38.651838 edman-2023.7.4/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.7.4/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.651838 edman-2023.7.4/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      169 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1448 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16599 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    48577 2023-07-04 02:31:14.000000 edman-2023.7.4/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.7.4/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    24865 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1492 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2023.7.4/edman/py.typed
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9640 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10900 2023-05-24 04:09:58.000000 edman-2023.7.4/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.651838 edman-2023.7.4/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7612 2023-07-06 01:11:38.000000 edman-2023.7.4/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      986 2023-07-06 01:11:38.000000 edman-2023.7.4/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-07-06 01:11:38.000000 edman-2023.7.4/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-07-06 01:11:38.000000 edman-2023.7.4/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2023-07-06 01:11:38.000000 edman-2023.7.4/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1123 2023-07-04 02:31:14.000000 edman-2023.7.4/pyproject.toml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1039 2023-07-04 02:31:14.000000 edman-2023.7.4/requirements.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-07-06 01:11:38.651838 edman-2023.7.4/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.651838 edman-2023.7.4/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2023.7.4/tests/__init__.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.651838 edman-2023.7.4/tests/ini/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2023.7.4/tests/ini/test_db.ini.sample
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.7.4/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    88352 2023-07-04 02:31:14.000000 edman-2023.7.4/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    40726 2023-05-18 02:16:03.000000 edman-2023.7.4/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.7.4/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.7.4/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7886 2023-05-23 05:52:10.000000 edman-2023.7.4/tests/test_utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.641838 edman-2023.7.4/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 01:11:38.651838 edman-2023.7.4/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2023.7.4/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      626 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-17 00:07:28.000000 edman-2023.7.4/venv/bin/rstpep2html.py
```

### Comparing `edman-2023.7.19/.github/workflows/unittest.yml` & `edman-2023.7.4/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/.gitignore` & `edman-2023.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/.idea/edman.iml` & `edman-2023.7.4/.idea/edman.iml`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/LICENSE.txt` & `edman-2023.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/PKG-INFO` & `edman-2023.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.7.19
+Version: 2023.7.4
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -192,18 +192,14 @@
 -------
 MIT
 
 API Document
 ------------
 https://ryde.github.io/edman/
 
-PyPI Project
-------------
-https://pypi.org/project/edman/
-
 Author
 ------
 
 [ryde](https://github.com/ryde)
 
 [yuskyamada](https://github.com/yuskyamada)
```

### Comparing `edman-2023.7.19/README.rst` & `edman-2023.7.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -167,18 +167,14 @@
 -------
 MIT
 
 API Document
 ------------
 https://ryde.github.io/edman/
 
-PyPI Project
-------------
-https://pypi.org/project/edman/
-
 Author
 ------
 
 [ryde](https://github.com/ryde)
 
 [yuskyamada](https://github.com/yuskyamada)
```

### Comparing `edman-2023.7.19/edman/config.py` & `edman-2023.7.4/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/convert.py` & `edman-2023.7.4/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/db.py` & `edman-2023.7.4/edman/db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/exceptions.py` & `edman-2023.7.4/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/file.py` & `edman-2023.7.4/edman/file.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/json_manager.py` & `edman-2023.7.4/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/search.py` & `edman-2023.7.4/edman/search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman/utils.py` & `edman-2023.7.4/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/edman.egg-info/PKG-INFO` & `edman-2023.7.4/edman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.7.19
+Version: 2023.7.4
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -192,18 +192,14 @@
 -------
 MIT
 
 API Document
 ------------
 https://ryde.github.io/edman/
 
-PyPI Project
-------------
-https://pypi.org/project/edman/
-
 Author
 ------
 
 [ryde](https://github.com/ryde)
 
 [yuskyamada](https://github.com/yuskyamada)
```

### Comparing `edman-2023.7.19/edman.egg-info/SOURCES.txt` & `edman-2023.7.4/edman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/pyproject.toml` & `edman-2023.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
-    "pymongo~=4.4.1",
+    "pymongo~=4.4.0",
     "python-dateutil~=2.8.2",
     "jmespath~=1.0.1",
 ]
-version = "2023.7.19"
+version = "2023.7.4"
 # dynamic = ["version"]
 
 [project.urls]
 "documentation" = "https://ryde.github.io/edman/"
 "repository" = "https://github.com/ryde/edman"
 
 [tool.setuptools.packages.find]
```

### Comparing `edman-2023.7.19/requirements.txt` & `edman-2023.7.4/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-anyio==3.7.1
 attrs==23.1.0
 bleach==6.0.0
 build==0.10.0
 certifi==2023.5.7
 cffi==1.15.1
-charset-normalizer==3.2.0
+charset-normalizer==3.1.0
 commonmark==0.9.1
-cryptography==41.0.2
-dnspython==2.4.0
+cryptography==41.0.1
+dnspython==2.3.0
 docutils==0.20.1
-exceptiongroup==1.1.2
+exceptiongroup==1.1.1
 flake8==6.0.0
-h11==0.14.0
-httpcore==0.17.3
 idna==3.4
-importlib-metadata==6.8.0
+importlib-metadata==6.7.0
 iniconfig==2.0.0
 isort==5.12.0
-jaraco.classes==3.3.0
+jaraco.classes==3.2.3
 jeepney==0.8.0
 jmespath==1.0.1
 keyring==24.2.0
 markdown-it-py==2.2.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==9.1.0
@@ -31,30 +28,29 @@
 pkginfo==1.9.6
 pluggy==1.2.0
 py==1.11.0
 pycodestyle==2.10.0
 pycparser==2.21
 pyflakes==3.0.1
 Pygments==2.15.1
-pymongo==4.4.1
+pymongo==4.4.0
 pyparsing==3.1.0
 pyproject_hooks==1.0.0
 pytest==7.4.0
 python-dateutil==2.8.2
 readme-renderer==40.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.4.2
 SecretStorage==3.3.3
 setuptools-scm==7.1.0
 six==1.16.0
-sniffio==1.3.0
 toml==0.10.2
 tomli==2.0.1
 twine==4.0.2
 types-jmespath==1.0.2.6
 types-python-dateutil==2.8.19.13
 typing_extensions==4.7.1
 urllib3==2.0.3
 webencodings==0.5.1
-zipp==3.16.2
+zipp==3.15.0
```

### Comparing `edman-2023.7.19/tests/test_convert.py` & `edman-2023.7.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/tests/test_db.py` & `edman-2023.7.4/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/tests/test_file.py` & `edman-2023.7.4/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/tests/test_multiuser.py` & `edman-2023.7.4/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/tests/test_search.py` & `edman-2023.7.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/tests/test_utils.py` & `edman-2023.7.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/jp.py` & `edman-2023.7.4/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2html.py` & `edman-2023.7.4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2html4.py` & `edman-2023.7.4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2html5.py` & `edman-2023.7.4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2latex.py` & `edman-2023.7.4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2man.py` & `edman-2023.7.4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2odt.py` & `edman-2023.7.4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2odt_prepstyles.py` & `edman-2023.7.4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2pseudoxml.py` & `edman-2023.7.4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2s5.py` & `edman-2023.7.4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2xetex.py` & `edman-2023.7.4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rst2xml.py` & `edman-2023.7.4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman-2023.7.19/venv/bin/rstpep2html.py` & `edman-2023.7.4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

