# Comparing `tmp/replize-0.1.0.tar.gz` & `tmp/replize-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replize-0.1.0.tar", last modified: Wed Jul 19 03:06:16 2023, max compression
+gzip compressed data, was "replize-0.1.1.tar", last modified: Wed Jul 19 03:19:06 2023, max compression
```

## Comparing `replize-0.1.0.tar` & `replize-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:06:16.517050 replize-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 03:05:29.000000 replize-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-19 03:06:16.517050 replize-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-19 03:05:29.000000 replize-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:06:16.513049 replize-0.1.0/replize/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-19 03:05:29.000000 replize-0.1.0/replize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-19 03:06:15.000000 replize-0.1.0/replize/replize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:06:16.517050 replize-0.1.0/replize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-19 03:06:16.000000 replize-0.1.0/replize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 03:06:16.000000 replize-0.1.0/replize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:06:16.000000 replize-0.1.0/replize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:06:16.000000 replize-0.1.0/replize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 03:06:16.000000 replize-0.1.0/replize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-19 03:06:16.517050 replize-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-19 03:05:29.000000 replize-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:19:06.630680 replize-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 03:18:26.000000 replize-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-19 03:19:06.630680 replize-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-19 03:18:26.000000 replize-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:19:06.630680 replize-0.1.1/replize/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-19 03:18:26.000000 replize-0.1.1/replize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-19 03:19:05.000000 replize-0.1.1/replize/replize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:19:06.630680 replize-0.1.1/replize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-19 03:19:06.000000 replize-0.1.1/replize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 03:19:06.000000 replize-0.1.1/replize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:19:06.000000 replize-0.1.1/replize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 03:19:06.000000 replize-0.1.1/replize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:19:06.000000 replize-0.1.1/replize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 03:19:06.000000 replize-0.1.1/replize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-19 03:19:06.630680 replize-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-19 03:18:26.000000 replize-0.1.1/setup.py
```

### Comparing `replize-0.1.0/LICENSE` & `replize-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `replize-0.1.0/replize/replize.py` & `replize-0.1.1/replize/replize.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         -rw-r--r-- 1 user group  0 Jan  1 00:00 __pycache__
         -rw-r--r-- 1 user group  0 Jan  1 00:00 replize.py
         ls >>> exit
         $
 
     Tricks:
 
-    `replize` is meant to be used with `functools.partial` to make the kind of REPL 
-    factory YOU want, by changing the defaults. 
+    `replize` is meant to be used with `functools.partial` to make the kind of REPL
+    factory YOU want, by changing the defaults.
 
-    If you want a given stdout or stderr value to have the effect of exiting the REPL, 
-    you can set the callback to raise an exception that is in the ``exit_exceptions``. 
+    If you want a given stdout or stderr value to have the effect of exiting the REPL,
+    you can set the callback to raise an exception that is in the ``exit_exceptions``.
 
     """
 
     exit_commands = set(exit_commands)
     exit_exceptions = tuple(exit_exceptions)
 
     # TODO: Like this for now, but could make prompt string dynamic in the future
@@ -71,16 +71,16 @@
                     stdout_callback(stdout)
                 if stderr:
                     stderr_callback(stderr)
         except exit_exceptions:  # TODO: Pylance says this is an error. It's not.
             break  # TODO: Enable verbose exit?
 
 
-if __name__ == '__main__':
-    # Script to enter a REPL for a command line program given by name
+def _replize_cli():
+    """Script to enter a REPL for a command line program given by name"""
     from argparse import ArgumentParser, RawTextHelpFormatter
 
     # TODO: Would like to use replize.__doc__ here, but doesn't format well.
     parser = ArgumentParser(
         description=replize.__doc__, formatter_class=RawTextHelpFormatter
     )
 
@@ -102,9 +102,10 @@
 
     replize(
         command=args.command,
         prompt_template=args.prompt_template,
         exit_commands=args.exit_commands,
     )
 
-    # TODO: Could easily give control to prompt_template and exit_commands,
-    # and possibly, as well (through strings), to exit_exceptions.
+
+if __name__ == '__main__':
+    _replize_cli()
```

