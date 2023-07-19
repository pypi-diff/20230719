# Comparing `tmp/FiveMCipherFinder-2.2.0.tar.gz` & `tmp/FiveMCipherFinder-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-2.2.0.tar", last modified: Sun Jul  9 07:11:36 2023, max compression
+gzip compressed data, was "FiveMCipherFinder-2.3.0.tar", last modified: Wed Jul 19 05:38:36 2023, max compression
```

## Comparing `FiveMCipherFinder-2.2.0.tar` & `FiveMCipherFinder-2.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/cipherFinder/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6929 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8278 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/setup.py
```

### Comparing `FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/PKG-INFO` & `FiveMCipherFinder-2.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,75 @@
-Metadata-Version: 2.1
-Name: FiveMCipherFinder
-Version: 2.2.0
-Summary: Finds Cipher in lua scripts.
-Home-page: https://github.com/exersalza/FivemCipherFinder
-Author: exersalza
-License: MIT
-Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
-Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# FivemCipherFinder (v2.3.0)
 
-# FivemCipherFinder (v2.2.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 
-This is a Fivem Cipher remover for those that don't want Ciphers in their scripts :D
+- [Installation](#installation)
+- [Usage](#Usage)
+- [Troubleshooting](#Troubleshooting)
+- [Known false-positives](#known-false-positives)
+- [Todo](#todo)
+- [Contact](#Contact)
 
-The idea behind these scripts is to remove a Cipher or more. Currently, there is only the Python version available, but I will soon add the C++ variant.
+This is a Fivem Cipher finder for those that don't want Ciphers in their scripts :D
+
+The idea behind these scripts is to find one or more Cipher in your script files. 
+Currently, there is only the Python version available, but I will soon add the C++ variant.
 
 Desc:
 The script will walk through your Server's directories and scan, for example, `\x41\x42\x43`. When it found something it will write the line and trigger it into a Log file.
 
-## Languages 
-Planed are Python (Finished so far)
+## Installation
+Py-Version: 3.8 and above
+
+run `pip install FivemCipherFinder` or download the latest release and unpack it.
+
+Make sure to read the [Troubleshooting](#Troubleshooting) page first before you add me on Discord.
+
+## Install instructions for Python
+Py-Version: 3.8 and above
+
+run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
 ## Usage
 
-Syntax: `find-cipher [search path] [exclude paths]... [OPTIONS]...`
+Syntax: `find-cipher [-h] [-p [PATH]] [-x [EXCLUDE_PATH ...]] [-n] [-v] [--v2]`
 Options are:
-- `--verbose` -> To show the found ciphers inside the Console
+- `-p|--path` -> Redirect the search from the current path `.` to another one.
+- `-x|--exclude` -> Exclude paths that you dont want to scan. 
+- `-n|--no-log` -> Prevents that an logfile is being written. Works hand in hand with `-v`
+- `-v|--verbose` -> To show the found ciphers inside the Console as soon as they were found.
 - `--v2` -> For the gibberish search. Like `local fjdlsajfdsancu = ...`
 
 It's a console tool so you can use `find-cipher` just like that in your `Resources` folder or you can specifiy you folder with `find-cipher ~/FiveM/server-data/resources` as example.
 
 Should you struggle with returning ciphers in your script, try using the
 `--v2` flag behind the command like `find-cipher . --v2 cars,mlos`.
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
-## Install instructions for Python
-Py-Version: 3.8 and above
-
-run `pip install FivemCipherFinder` or download the latest release and unpack it.
-
 ### Troubleshooting
 
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
 
-## Known false positives
-- `easy-admin`
-- `encrypted scripts`
+Also make sure (on Windows) that you have your python scripts folder inside your path variable. Should the folder be missing, it shows at the pip installation as a warning. [how to add something to the path variable](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)
+
+
+## Known-false-positives
+
+- `EasyAdmin`
+- `encrypted/obfuscated scripts`
+
 
 ## ToDo
 - Detect cipher spreader
+- Add de obfuscator for detectet cipher
 - ~~Find random generated character variable names~~
 
 ## Contact
 Discord: exersalza / exersalza[>'-']>#1337 | [DE/EN]
```

### Comparing `FiveMCipherFinder-2.2.0/LICENSE` & `FiveMCipherFinder-2.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 exersalza "Julian J."
+Copyright (c) 2022-2023 exersalza "Julian J."
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `FiveMCipherFinder-2.2.0/PKG-INFO` & `FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,92 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.2.0
+Version: 2.3.0
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FivemCipherFinder (v2.2.0)
+# FivemCipherFinder (v2.3.0)
+
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 
-This is a Fivem Cipher remover for those that don't want Ciphers in their scripts :D
+- [Installation](#installation)
+- [Usage](#Usage)
+- [Troubleshooting](#Troubleshooting)
+- [Known false-positives](#known-false-positives)
+- [Todo](#todo)
+- [Contact](#Contact)
+
+This is a Fivem Cipher finder for those that don't want Ciphers in their scripts :D
 
-The idea behind these scripts is to remove a Cipher or more. Currently, there is only the Python version available, but I will soon add the C++ variant.
+The idea behind these scripts is to find one or more Cipher in your script files. 
+Currently, there is only the Python version available, but I will soon add the C++ variant.
 
 Desc:
 The script will walk through your Server's directories and scan, for example, `\x41\x42\x43`. When it found something it will write the line and trigger it into a Log file.
 
-## Languages 
-Planed are Python (Finished so far)
+## Installation
+Py-Version: 3.8 and above
+
+run `pip install FivemCipherFinder` or download the latest release and unpack it.
+
+Make sure to read the [Troubleshooting](#Troubleshooting) page first before you add me on Discord.
+
+## Install instructions for Python
+Py-Version: 3.8 and above
+
+run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
 ## Usage
 
-Syntax: `find-cipher [search path] [exclude paths]... [OPTIONS]...`
+Syntax: `find-cipher [-h] [-p [PATH]] [-x [EXCLUDE_PATH ...]] [-n] [-v] [--v2]`
 Options are:
-- `--verbose` -> To show the found ciphers inside the Console
+- `-p|--path` -> Redirect the search from the current path `.` to another one.
+- `-x|--exclude` -> Exclude paths that you dont want to scan. 
+- `-n|--no-log` -> Prevents that an logfile is being written. Works hand in hand with `-v`
+- `-v|--verbose` -> To show the found ciphers inside the Console as soon as they were found.
 - `--v2` -> For the gibberish search. Like `local fjdlsajfdsancu = ...`
 
 It's a console tool so you can use `find-cipher` just like that in your `Resources` folder or you can specifiy you folder with `find-cipher ~/FiveM/server-data/resources` as example.
 
 Should you struggle with returning ciphers in your script, try using the
 `--v2` flag behind the command like `find-cipher . --v2 cars,mlos`.
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
-## Install instructions for Python
-Py-Version: 3.8 and above
-
-run `pip install FivemCipherFinder` or download the latest release and unpack it.
-
 ### Troubleshooting
 
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
 
-## Known false positives
-- `easy-admin`
-- `encrypted scripts`
+Also make sure (on Windows) that you have your python scripts folder inside your path variable. Should the folder be missing, it shows at the pip installation as a warning. [how to add something to the path variable](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)
+
+
+## Known-false-positives
+
+- `EasyAdmin`
+- `encrypted/obfuscated scripts`
+
 
 ## ToDo
 - Detect cipher spreader
+- Add de obfuscator for detectet cipher
 - ~~Find random generated character variable names~~
 
 ## Contact
 Discord: exersalza / exersalza[>'-']>#1337 | [DE/EN]
```

### Comparing `FiveMCipherFinder-2.2.0/cipherFinder/finder.py` & `FiveMCipherFinder-2.3.0/cipherFinder/finder.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,31 +22,34 @@
 from __future__ import annotations
 from datetime import datetime as dt
 
 import os
 import re
 import sys
 import platform
+import argparse
 import requests
 
 from gibberish_detector import detector
 
 REGEX = r'(((\\x|\\u)([a-fA-F0-9]{2})){2})'
 COLORS = ['\033[0m', '\033[91m', '\033[92m']
 RAW_BIG_MODEL = 'https://raw.githubusercontent.com/exersalza/FivemCipherFinder/main/big.model'
 
 log = []
 
 def get_big_model_file() -> int:
     # Check if the big.model file exists
     if not os.path.exists('./big.model'):
         with open('big.model', 'wb') as _file:
-            for chunk in requests.get(RAW_BIG_MODEL, stream=True, timeout=5) \
+            for chunk in requests.get(RAW_BIG_MODEL, 
+                                      stream=True, timeout=5) \
                     .iter_content(chunk_size=8192):
                 if not chunk: continue
+
                 _file.write(chunk)
 
     return 0
 
 
 def validate_lines(lines: list) -> list[tuple]:
     """ Validate the lines that are given through the 'lines' parameter.
@@ -59,15 +62,15 @@
     Returns
     -------
     list[tuple]
         A list with infected lines 
         (or false positives by AntiCheat or obfuscated code)
     """
 
-    ret = []
+    ret: list[tuple] = []
 
     for ln, line in enumerate(lines, start=1):  # ln: lineNumber
         if re.findall(REGEX, rf'{line}', re.MULTILINE and re.IGNORECASE):
             ret.append((ln, line))
 
     return ret
 
@@ -97,25 +100,27 @@
         if 'local' in i and det.is_gibberish(rf'{i}'):
             matches.append((l_counter, i))
 
         l_counter += 1
     return matches
 
 
-def check_file(d: str, file: str, count: int) -> tuple[int, int]: 
+def check_file(d: str, file: str, count: int, args: argparse.Namespace) -> tuple[int, int]: 
     """ Iterate over a file and check the lines
 
     Parameters
     ----------
     d : str
         Give the path to the file e.g "/home/wildCiphers"
     file : str
         Give a file name to scan e.g "wildCipherInHere.lua"
     count: int
         Give the current cipher count.
+    args: argparse.Namespace
+        Give the arguments delieverd from the Cmd line.
     
     Returns
     -------
     tuple[ret_code, count]
         A Tuple with the return code and the current cipher count.
     """
 
@@ -124,32 +129,35 @@
             lines = f.readlines()
         except UnicodeDecodeError:
             print(f'Can\'t decode `{d}/{file}`.')
             return 1, count
         
         match = validate_lines(lines)
         
-        if '--v2' in sys.argv:
+        if args.v2:
             match += do_gibberish_check(lines)
 
         if match:
             for ln, line in match:
                 path = d.replace('\\', '/') + f'/{file}'
                 to_log = f'File: {path}\nLineNumber: {ln}\n'
 
-                if '--verbose' in sys.argv:  # Log in console.
+                if args.verbose:  # Log in console.
                     print(to_log)
 
 
                 log.append(to_log + f'Line: {line!r}\n----------------\n')
                 count += 1
     return 0, count
 
 
 def write_log_file(**kw) -> int: 
+    if kw.pop('args').no_log:
+        return 0
+
     with open(f'CipherLog-{dt.now():%H-%M-%S}.txt', 'w+', encoding='utf-8') as f:
         f.writelines(log)
         
         print(f'{kw.pop("red")}Oh no, the program found a spy in your files x.x '
           f'Check the CipherLog.txt for location and trigger. {kw.pop("count")} where found!'
           f'{kw.pop("white")}\n#staysafe')
     return 0
@@ -159,74 +167,87 @@
     """ Validates lua files.
 
     Usage:
     ------
     Run the program: `find-cipher [path] [exclude path] [OPTIONS...]`.
 
     args:
-        path : Optional : 
+        --path : Optional : 
             Give the path to search, when no path is given, the 
             current working directory will be used `.`
-        exclude path : Optional : 
+        --exclude-path : Optional : 
             Exclude directory's where you don't want to search.
+        --no-log: Optional :
+            Don't create a log file, can be used hand in hand with --verbose
         --verbose : Optional : 
             Print a Cipher directly to the Command line on found.
         --v2 : Optional : 
             Uses an extra algorithm to find gibberish or randomly generated
             variable/function/table names. It can introduce more palse-positiv
             because of obfuscated scripts, but can help to find ciphers.
 
     Advertisement:
     --------------
     Get your beautiful Cipher today, just smack the play button and find some.
+    Just for $9.99 you can get the Base edition, and just for anohter $49.99
+    you can get yourself access to the Version 2.
     I hope you don't have any but always be sure to have none.
 
     Returns
     -------
     int
         Return code
     """
 
-    if '-h' in sys.argv or '--help' in sys.argv:
-        print(main.__doc__)
-        return 0
+    parser = argparse.ArgumentParser(description='Validates lua files.')
 
-    pattern = ''.join([(i.replace(',', ')|(') if '--' not in i else '') for i in sys.argv[2:]])
-    local_path = '.'
+    parser.add_argument('-p', '--path', nargs='?', default='.',
+                        help='Give the path to search, when no path is given, the current working directory will be used "."')
+    parser.add_argument('-x', '--exclude', nargs='*', default='',
+                        help='Exclude directories where you don\'t want to search.')
+    parser.add_argument('-n', '--no-log', action='store_true',
+                        help='Don\'t create a log file, can be used hand in hand with --verbose')
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='Print a Cipher directly to the Command line on found.')
+    parser.add_argument('--v2', action='store_true',
+                        help='Uses an extra algorithm to find gibberish or randomly generated variable/function/table names. It can introduce more false-positives because of obfuscated scripts but can help find ciphers.')
+
+    args = parser.parse_args()
+
+    pattern = ''.join([(i.replace(',', ')|(') if '--' not in i else '') for i in args.exclude])
+    local_path = args.path
     count = 0 
 
     get_big_model_file()  # sure there are other ways, but python is doing python stuff.
-
-    if len(sys.argv) > 1 and '--' not in sys.argv[1]:
-        local_path = sys.argv[1]
     
     for d, _, files in os.walk(local_path):
         if pattern and re.findall(f'{"(" + pattern + ")"}', 
                                   fr'{d}'.format(d=d), re.MULTILINE and re.IGNORECASE):
             continue
 
         for file in files:
             if '.lua' not in file:
                 continue
 
-            _, count = check_file(d, file, count)
+            _, count = check_file(d, file, count, args)
     # Write log
     
     red = green = white = ''
 
     if 'linux' in platform.platform().lower():
         white, red, green = COLORS
     
     try:
         os.remove('big.model')
     except FileNotFoundError:
         pass
 
     if log:
-        return write_log_file(white=white, red=red, count=count)
+        return write_log_file(white=white, red=red, 
+                              count=count, args=args)
 
     print(f'{green}Nice! There were no Cipher\'s found!{white}')
 
     return 0
 
 
 if __name__ == '__main__':
```

### Comparing `FiveMCipherFinder-2.2.0/setup.cfg` & `FiveMCipherFinder-2.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 2.2.0
+version = 2.3.0
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls =
```

