# Comparing `tmp/curtxt-reader-1.2.0.tar.gz` & `tmp/curtxt-reader-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtxt-reader-1.2.0.tar", last modified: Tue Jul 11 17:19:45 2023, max compression
+gzip compressed data, was "curtxt-reader-1.2.1.tar", last modified: Wed Jul 19 12:10:31 2023, max compression
```

## Comparing `curtxt-reader-1.2.0.tar` & `curtxt-reader-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/
--rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.2.0/LICENSE
--rw-r--r--   0 iris      (1000) iris      (1000)    21719 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)     1260 2023-07-11 17:04:49.000000 curtxt-reader-1.2.0/README.md
--rwxr-xr-x   0 iris      (1000) iris      (1000)    11017 2023-07-11 17:01:08.000000 curtxt-reader-1.2.0/curtxt.py
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/curtxt_reader.egg-info/
--rw-r--r--   0 iris      (1000) iris      (1000)    21719 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/SOURCES.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/dependency_links.txt
--rw-r--r--   0 iris      (1000) iris      (1000)       39 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/entry_points.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/top_level.txt
--rw-r--r--   0 iris      (1000) iris      (1000)      902 2023-07-11 17:06:35.000000 curtxt-reader-1.2.0/pyproject.toml
--rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/setup.cfg
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-19 12:10:31.516509 curtxt-reader-1.2.1/
+-rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.2.1/LICENSE
+-rw-r--r--   0 iris      (1000) iris      (1000)    21719 2023-07-19 12:10:31.516509 curtxt-reader-1.2.1/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)     1260 2023-07-11 17:04:49.000000 curtxt-reader-1.2.1/README.md
+-rwxr-xr-x   0 iris      (1000) iris      (1000)    11093 2023-07-19 12:09:26.000000 curtxt-reader-1.2.1/curtxt.py
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-19 12:10:31.513176 curtxt-reader-1.2.1/curtxt_reader.egg-info/
+-rw-r--r--   0 iris      (1000) iris      (1000)    21719 2023-07-19 12:10:31.000000 curtxt-reader-1.2.1/curtxt_reader.egg-info/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-07-19 12:10:31.000000 curtxt-reader-1.2.1/curtxt_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-07-19 12:10:31.000000 curtxt-reader-1.2.1/curtxt_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)       39 2023-07-19 12:10:31.000000 curtxt-reader-1.2.1/curtxt_reader.egg-info/entry_points.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-07-19 12:10:31.000000 curtxt-reader-1.2.1/curtxt_reader.egg-info/top_level.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)      902 2023-07-19 12:09:35.000000 curtxt-reader-1.2.1/pyproject.toml
+-rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-07-19 12:10:31.516509 curtxt-reader-1.2.1/setup.cfg
```

### Comparing `curtxt-reader-1.2.0/LICENSE` & `curtxt-reader-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curtxt-reader-1.2.0/PKG-INFO` & `curtxt-reader-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple ncurses-based plain text reader
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `curtxt-reader-1.2.0/README.md` & `curtxt-reader-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `curtxt-reader-1.2.0/curtxt.py` & `curtxt-reader-1.2.1/curtxt.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,25 +272,26 @@
 Options:
     -h, --help - pring this message and exit
     -v, --version - print version number and exit
     -c, --clear - clear history file"""
     if os.isatty(0) and (len(argv) == 1):
         print(help_text)
         exit()
-    match argv[1]:
-        case "--version" | "-v":
-            print("Version 1.1.2")
-            exit()
-        case "--help" | "-h":
-            print(help_text)
-            exit()
-        case "--clear" | "-c":
-            path = f'{os.environ["HOME"]}/.local/share/curtxt-reader/history'
-            if (os.path.exists(path)):
-                os.remove(path)
-                print("Cleared history")
-            exit()
+    if (len(argv) > 1):
+        match argv[1]:
+            case "--version" | "-v":
+                print("Version 1.2.1")
+                exit()
+            case "--help" | "-h":
+                print(help_text)
+                exit()
+            case "--clear" | "-c":
+                path = f'{os.environ["HOME"]}/.local/share/curtxt-reader/history'
+                if (os.path.exists(path)):
+                    os.remove(path)
+                    print("Cleared history")
+                exit()
     curses.wrapper(main)
 
 
 if __name__ == "__main__":
     init()
```

### Comparing `curtxt-reader-1.2.0/curtxt_reader.egg-info/PKG-INFO` & `curtxt-reader-1.2.1/curtxt_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple ncurses-based plain text reader
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `curtxt-reader-1.2.0/pyproject.toml` & `curtxt-reader-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "curtxt-reader"
-version = "1.2.0"
+version = "1.2.1"
 description = "A simple ncurses-based plain text reader"
 readme = "README.md"
 authors = [{ name = "1256-bits" , email = "128bit@eclipso.eu" }]
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

