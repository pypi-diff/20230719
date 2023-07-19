# Comparing `tmp/ssh_terminal_manager-0.8.2.tar.gz` & `tmp/ssh_terminal_manager-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.8.2.tar", last modified: Mon Jul 17 08:35:55 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.8.3.tar", last modified: Wed Jul 19 07:59:00 2023, max compression
```

## Comparing `ssh_terminal_manager-0.8.2.tar` & `ssh_terminal_manager-0.8.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:35:55.460568 ssh_terminal_manager-0.8.2/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.2/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-17 08:35:55.456568 ssh_terminal_manager-0.8.2/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.2/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-17 08:35:09.000000 ssh_terminal_manager-0.8.2/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-17 08:35:55.460568 ssh_terminal_manager-0.8.2/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:35:55.456568 ssh_terminal_manager-0.8.2/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:35:55.456568 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8726 2023-07-17 07:25:30.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-17 07:25:30.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:35:55.456568 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-17 08:35:55.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-17 08:35:55.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-17 08:35:55.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-17 08:35:55.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-17 08:35:55.000000 ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.3/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.3/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-19 07:58:10.000000 ssh_terminal_manager-0.8.3/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.678728 ssh_terminal_manager-0.8.3/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8726 2023-07-17 08:57:09.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-17 08:57:09.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.8.2/LICENSE` & `ssh_terminal_manager-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.8.2/PKG-INFO` & `ssh_terminal_manager-0.8.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.8.2/pyproject.toml` & `ssh_terminal_manager-0.8.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,14 +20,14 @@
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.8.2",
+  "terminal-manager >= 0.8.3",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.8.2/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.8.2/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

