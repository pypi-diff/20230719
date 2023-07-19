# Comparing `tmp/pasteboard2-0.0.4.tar.gz` & `tmp/pasteboard2-0.0.5.tar.gz`

## Comparing `pasteboard2-0.0.4.tar` & `pasteboard2-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.idea/pasteboard.iml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/src/pasteboard2/__init__.py
--rwxr-xr-x   0        0        0     4157 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/src/pasteboard2/pasteboard2.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/tests/test_pasteboard2.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 pasteboard2-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.github/workflows/black.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.idea/pasteboard.iml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/pasteboard2/__init__.py
+-rwxr-xr-x   0        0        0     1542 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/pasteboard2/__main__.py
+-rwxr-xr-x   0        0        0     1820 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/pasteboard2/pasteboard2.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/tests/test_pasteboard2.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/README.md
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 pasteboard2-0.0.5/PKG-INFO
```

### Comparing `pasteboard2-0.0.4/tests/test_pasteboard2.py` & `pasteboard2-0.0.5/tests/test_pasteboard2.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     assert is_empty()
 
 
 def test_pasteboard_types_empty_at_start():
     assert get_types() == []
 
 
+def test_pasteboard_types_str_empty_at_start():
+    assert get_types_str() == ""
+
+
 def test_pasteboard_set_content():
     # Set content to pasteboard
     set_content("Hello, World!")
     # Assert that the content has been correctly set
     assert get_content() == "Hello, World!"
 
 
@@ -78,8 +82,8 @@
     clear_pb()
     # Assert that the pasteboard is empty after clearing
     assert is_empty()
 
     # Set content to pasteboard
     set_content("Hello, World!")
     # Assert that the list includes PLAIN_TEXT_UTF8 after adding text content
-    assert PLAIN_TEXT_UTF8 in get_types()
+    assert pasteboard2.PLAIN_TEXT_UTF8 in get_types()
```

### Comparing `pasteboard2-0.0.4/.gitignore` & `pasteboard2-0.0.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 __pycache__/
 *.py[cod]
+dist/
 
 .idea/git_toolbox_prj.xml
 
 # User-specific stuff
 .idea/**/workspace.xml
 .idea/**/tasks.xml
 .idea/**/usage.statistics.xml
```

### Comparing `pasteboard2-0.0.4/LICENSE.txt` & `pasteboard2-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pasteboard2-0.0.4/README.md` & `pasteboard2-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,53 +4,68 @@
 [PyObjC](https://pypi.org/project/pyobjc/) and is modeled after the
 [Swift](https://en.wikipedia.org/wiki/Swift_(programming_language)) program
 [pbv](https://github.com/chee/pbv).
 
 ## Command Line Usage
 ### Top Level
 ```
- Usage: pasteboard2.py [OPTIONS] COMMAND [ARGS]...
+ Usage: pb2 [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
 │ --help          Show this message and exit.                                        │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ─────────────────────────────────────────────────────────────────────────╮
 │ clear            Empties the pasteboard.                                           │
 │ clip             Print the content of the pasteboard if it's a string.             │
-│ test             Run tests with pytest and doctest.                                │
 │ types            List the content types of the current pasteboard.                 │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ### Clip Subcommand
 ```
- Usage: pasteboard2.py clip [OPTIONS]
+ Usage: pb2 clip [OPTIONS]
 
  Print the content of the pasteboard if it's a string.
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
 │ --type  -t      TEXT  The type of content to get [default: public.utf8-plain-text] │
 │ --help                Show this message and exit.                                  │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ## Test
 ```
 git clone https://github.com/bwagner/pasteboard2.git
 cd pasteboard2
 python -m venv ~/venv/pb2
 source ~/venv/pb2/bin/activate
+python -m pip install --upgrade pip setuptools wheel
 pip install -r requirements.txt
-./src/pasteboard2/pasteboard2.py test
+pytest
 deactivate
 rm -rf ~/venv/pb2
 ```
+## TODO
+[pbv](https://github.com/chee/pbv) offers reading from
+several pasteboards. We should, too.
+
 ## Requirements
 - pyobjc
 - typer
 - pytest (for development)
+
+## Contribute
+```
+git clone https://github.com/bwagner/pasteboard2.git
+cd pasteboard2
+source ~/venv/pb2/bin/activate
+python -m pip install --upgrade pip setuptools wheel
+pip install -r requirements.txt
+pre-commit install
+
+```
+
 ## Alternatives
 - https://pypi.org/project/pasteboard/ \
   https://github.com/tobywf/pasteboard \
   but it's no longer maintained (checked 20230710)
 
 - https://pypi.org/project/tacky/ \
   https://github.com/friedenberg/tacky
-
```

### Comparing `pasteboard2-0.0.4/PKG-INFO` & `pasteboard2-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasteboard2
-Version: 0.0.4
+Version: 0.0.5
 Summary: access macOS pasteboard
 Project-URL: Homepage, https://github.com/bwagner/pasteboard2
 Project-URL: Bug Tracker, https://github.com/bwagner/pasteboard2/issues
 Author-email: Bernhard Wagner <pasteboard2@nosuch.biz>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,53 +40,68 @@
 [PyObjC](https://pypi.org/project/pyobjc/) and is modeled after the
 [Swift](https://en.wikipedia.org/wiki/Swift_(programming_language)) program
 [pbv](https://github.com/chee/pbv).
 
 ## Command Line Usage
 ### Top Level
 ```
- Usage: pasteboard2.py [OPTIONS] COMMAND [ARGS]...
+ Usage: pb2 [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
 │ --help          Show this message and exit.                                        │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ─────────────────────────────────────────────────────────────────────────╮
 │ clear            Empties the pasteboard.                                           │
 │ clip             Print the content of the pasteboard if it's a string.             │
-│ test             Run tests with pytest and doctest.                                │
 │ types            List the content types of the current pasteboard.                 │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ### Clip Subcommand
 ```
- Usage: pasteboard2.py clip [OPTIONS]
+ Usage: pb2 clip [OPTIONS]
 
  Print the content of the pasteboard if it's a string.
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
 │ --type  -t      TEXT  The type of content to get [default: public.utf8-plain-text] │
 │ --help                Show this message and exit.                                  │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ## Test
 ```
 git clone https://github.com/bwagner/pasteboard2.git
 cd pasteboard2
 python -m venv ~/venv/pb2
 source ~/venv/pb2/bin/activate
+python -m pip install --upgrade pip setuptools wheel
 pip install -r requirements.txt
-./src/pasteboard2/pasteboard2.py test
+pytest
 deactivate
 rm -rf ~/venv/pb2
 ```
+## TODO
+[pbv](https://github.com/chee/pbv) offers reading from
+several pasteboards. We should, too.
+
 ## Requirements
 - pyobjc
 - typer
 - pytest (for development)
+
+## Contribute
+```
+git clone https://github.com/bwagner/pasteboard2.git
+cd pasteboard2
+source ~/venv/pb2/bin/activate
+python -m pip install --upgrade pip setuptools wheel
+pip install -r requirements.txt
+pre-commit install
+
+```
+
 ## Alternatives
 - https://pypi.org/project/pasteboard/ \
   https://github.com/tobywf/pasteboard \
   but it's no longer maintained (checked 20230710)
 
 - https://pypi.org/project/tacky/ \
   https://github.com/friedenberg/tacky
-
```

