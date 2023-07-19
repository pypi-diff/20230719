# Comparing `tmp/dela-0.1.4.tar.gz` & `tmp/dela-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dela-0.1.4.tar", max compression
+gzip compressed data, was "dela-0.2.0.tar", max compression
```

## Comparing `dela-0.1.4.tar` & `dela-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     1599 2023-07-11 06:05:23.840877 dela-0.1.4/README.md
--rw-r--r--   0        0        0      267 2023-07-11 06:05:23.840877 dela-0.1.4/dela/FileReader.py
--rw-r--r--   0        0        0     3731 2023-07-11 06:05:23.840877 dela-0.1.4/dela/ListCommand.py
--rw-r--r--   0        0        0     1295 2023-07-11 06:05:23.840877 dela-0.1.4/dela/Todo.py
--rw-r--r--   0        0        0      580 2023-07-11 06:05:23.840877 dela-0.1.4/dela/TodoPresentation.py
--rw-r--r--   0        0        0        0 2023-07-11 06:05:23.840877 dela-0.1.4/dela/__init__.py
--rw-r--r--   0        0        0     2030 2023-07-11 06:05:23.840877 dela-0.1.4/dela/__main__.py
--rw-r--r--   0        0        0      123 2023-07-11 06:05:23.840877 dela-0.1.4/dela/logger.py
--rw-r--r--   0        0        0      367 2023-07-11 06:05:23.848877 dela-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 dela-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2496 2023-07-19 11:15:50.660163 dela-0.2.0/README.md
+-rw-r--r--   0        0        0      267 2023-07-19 11:15:50.660163 dela-0.2.0/dela/FileReader.py
+-rw-r--r--   0        0        0     2153 2023-07-19 11:15:50.660163 dela-0.2.0/dela/ListCommand.py
+-rw-r--r--   0        0        0      204 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TagPresentation.py
+-rw-r--r--   0        0        0     1893 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TagsCommand.py
+-rw-r--r--   0        0        0     1131 2023-07-19 11:15:50.660163 dela-0.2.0/dela/Todo.py
+-rw-r--r--   0        0        0      677 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TodoPresentation.py
+-rw-r--r--   0        0        0     1439 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TodoRepo.py
+-rw-r--r--   0        0        0        0 2023-07-19 11:15:50.660163 dela-0.2.0/dela/__init__.py
+-rw-r--r--   0        0        0     2953 2023-07-19 11:15:50.660163 dela-0.2.0/dela/__main__.py
+-rw-r--r--   0        0        0      426 2023-07-19 11:15:50.660163 dela-0.2.0/dela/comparators.py
+-rw-r--r--   0        0        0      754 2023-07-19 11:15:50.660163 dela-0.2.0/dela/filters.py
+-rw-r--r--   0        0        0      187 2023-07-19 11:15:50.660163 dela-0.2.0/dela/logger.py
+-rw-r--r--   0        0        0      367 2023-07-19 11:15:50.664162 dela-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 dela-0.2.0/PKG-INFO
```

### Comparing `dela-0.1.4/README.md` & `dela-0.2.0/dela/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,106 @@
-## Dela
+#! /bin/python
+import pkg_resources
+from docopt import docopt
+from dela.TagsCommand import TagsCommand
+from dela.ListCommand import ListCommand
+from dela.logger import log
 
-![dela](./imgs/dela.png)
+doc = """dela
 
-### Installation
-
-```
-pip install --user dela
-```
-
-### Help
-
-```
 CLI to list todos in markdown files, like Obsidian Vaults.
 
 Usage:
   dela -h | --help
   dela --version
-  dela list [-v] [--all] [--today] [--done] [--someday] [--status=<symbol>] [--tag=<string>...] [--sort_by=<key>] [--format=<string>] [<glob>]
+  dela list [-v] [--today|--upcoming] [--all|--statuses=<str>] [--tags=<str>] [--sort_by=<str>] [--format=<str>] [<glob>]
+
 
 Options:
   -h --help                     Show this screen
   -v --verbose                  Enable logging
+  --version                     Show version.
+
+  -s=<str> --statuses=<str>      Filter by status (someday, backlog, in_progress, etc) [default: ~,n, ]
+  -t=<str> --tags=<str>         Filter by tag (#work, #home, etc)
+
+  --today                       Show only tasks due today or earlier
+  -u --upcoming                 Show future tasks
   -a --all                      Show all todos including closed ones
-  -t --today                    Show only tasks due today or earlier
-  -d --done                     Show only done tasks
-  --someday                     Show someday tasks marked with [s] status
-  -s --status=<symbol>          Filter by status (x, a, c, ~, ...)
-  -tag=<string>                 Filter by tag (#work, #home, etc)
+
   --sort_by=<key>               Sort by given key
+
   --format=<string>             Format result with given template string.
-  --version                     Show version.
 
 
-Template example:
-    dela list --format='- [$status] $file: $title'
+Template and Sorting Keys:
+
+    NOTE: In templates variable should be prefixed with the $ sign.
+
+
+Todo statuses:
+    Todo status is a symbol placed in the square buckets ([x], [ ], [~], etc). You can use
+    whatever you want, `dela` doesn't have eny presets, except default `--status=~,n, `,
+    which you can overwrite.
 
-    NOTE: Unicode colors are supported
 
+Upcoming Tasks
+    If a task has a date in future, it's hidden by default. To see such tasks in the output,
+    add the `--upcoming` flag.
 
-Template and Sorting Keys:
-    - message
+
+Sorting:
+    By default todos are sorted by `--status` value according to the order of given statuses,
+    and then by date to place todos with dates to the top of the list (due date sounds important,
+    right?). You can sort todos by passing an attribute name to the  `--sort_by` flag.
+    Possible values are:
+
+    - title
     - date
     - status
     - tags
     - file
 
-    NOTE: In templates variable should be prefixed with the $ sign.
 
+Formatting output:
+    You can use your own template with the `--format` flag. Unicode colors are supported:
+
+    For example:
+
+        dela list --format='- [$status] $file: $title'
+
+    Next variables are supported:
+
+    - $title
+    - $date
+    - $status
+    - $tags
+    - $file
+
+
+Examples:
+
+    dela list # By default prints all todos with [~], [n] and [ ] checkboxes
+    dela list -s=' ,s' # prints todos only with statuses [ ] and [s]
+    dela list --today # prints only todos with default statuses with a date equal or earliear then today
+    dela list -t=#tag # prints only todos that have tag #tag
+    dela list -u -s='~,n, ,s' #prints todos with given status including upcoming ones
+"""
+
+version = pkg_resources.get_distribution('dela').version
+
+
+def main():
+    args = docopt(doc, version=version)
+
+    if args['--verbose']:
+        log.setLevel('INFO')
+        log.info('Verbose logging has been enabled')
+
+    log.info(f'{args}')
+
+    if args['list'] == True:
+        ListCommand(args).run()
+        exit(0)
 
-Supported todo examples:
-    - [ ] Todo
-    - [x] Done
-    - [n] Next
-    - [~] Pending
-    - [c] Cancelled
-    - [ ] 20230703 Todo with a date. If it's the day, `dela list -t` will list this guy
-    - [ ] Todo with tags #tagone #tagtwo
-    - [ ] 23330101 Future task will be hidden until the day become
-```
+if __name__ == '__main__':
+    main()
```

### Comparing `dela-0.1.4/dela/TodoPresentation.py` & `dela-0.2.0/dela/TodoPresentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from string import Template
 
 
 class TodoPresentation:
     def __init__(self, format) -> None:
         self.template = Template(format)
 
-    def present(self, todo):
+    def present(self, todos):
+        for todo in todos:
+            self.present_one(todo)
+
+    def present_one(self, todo):
         context = todo.__dict__
         context['tags'] = ' '.join(context['tags'])
 
         str = self.template.substitute(context)
 
         # NOTE: This 2 lines are here to add support for unicode escape
         #       characters like terminal colors, tabs, etc
```

### Comparing `dela-0.1.4/dela/__main__.py` & `dela-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,111 @@
-#! /bin/python
-import pkg_resources
-import logging
-from docopt import docopt
-from dela.ListCommand import ListCommand
-from dela.logger import log
+Metadata-Version: 2.1
+Name: dela
+Version: 0.2.0
+Summary: 
+License: MIT
+Author: 'Anton Shuvalov'
+Author-email: anton@shuvalov.info
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: blue (>=0.9.1,<0.10.0)
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Description-Content-Type: text/markdown
+
+## Dela
+
+![dela](./imgs/dela.png)
+
+### Installation
+
+```
+pip install --user dela
+```
+
+### Examples
+
+```bash
+dela list # By default prints all todos with [~], [n] and [ ] checkboxes
+dela list -s=' ,s' # prints todos only with statuses [ ] and [s]
+dela list --today # prints only todos with default statuses with a date equal or earliear then today
+dela list -t=#tag # prints only todos that have tag #tag
+dela list -u -s='~,n, ,s' #prints todos with given status including upcoming ones
+```
 
-doc = """dela
+### Help
 
+```
 CLI to list todos in markdown files, like Obsidian Vaults.
 
 Usage:
   dela -h | --help
   dela --version
-  dela list [-v] [--all] [--today] [--done] [--someday] [--status=<symbol>] [--tag=<string>...] [--sort_by=<key>] [--format=<string>] [<glob>]
+  dela list [-v] [--today|--upcoming] [--all|--statuses=<str>] [--tags=<str>] [--sort_by=<str>] [--format=<str>] [<glob>]
+
 
 Options:
   -h --help                     Show this screen
   -v --verbose                  Enable logging
+  --version                     Show version.
+
+  -s=<str> --statuses=<str>      Filter by status (someday, backlog, in_progress, etc) [default: ~,n, ]
+  -t=<str> --tags=<str>         Filter by tag (#work, #home, etc)
+
+  --today                       Show only tasks due today or earlier
+  -u --upcoming                 Show future tasks
   -a --all                      Show all todos including closed ones
-  -t --today                    Show only tasks due today or earlier
-  -d --done                     Show only done tasks
-  --someday                     Show someday tasks marked with [s] status
-  -s --status=<symbol>          Filter by status (x, a, c, ~, ...)
-  -tag=<string>                 Filter by tag (#work, #home, etc)
+
   --sort_by=<key>               Sort by given key
+
   --format=<string>             Format result with given template string.
-  --version                     Show version.
 
 
-Template example:
-    dela list --format='- [$status] $file: $title'
+Template and Sorting Keys:
+
+    NOTE: In templates variable should be prefixed with the $ sign.
+
 
-    NOTE: Unicode colors are supported
+Todo statuses:
+    Todo status is a symbol placed in the square buckets ([x], [ ], [~], etc). You can use
+    whatever you want, `dela` doesn't have eny presets, except default `--status=~,n, `,
+    which you can overwrite.
 
 
-Template and Sorting Keys:
-    - message
+Upcoming Tasks
+    If a task has a date in future, it's hidden by default. To see such tasks in the output,
+    add the `--upcoming` flag.
+
+
+Sorting:
+    By default todos are sorted by `--status` value according to the order of given statuses,
+    and then by date to place todos with dates to the top of the list (due date sounds important,
+    right?). You can sort todos by passing an attribute name to the  `--sort_by` flag.
+    Possible values are:
+
+    - title
     - date
     - status
     - tags
     - file
 
-    NOTE: In templates variable should be prefixed with the $ sign.
 
+Formatting output:
+    You can use your own template with the `--format` flag. Unicode colors are supported:
+
+    For example:
+
+        dela list --format='- [$status] $file: $title'
 
-Supported todo examples:
-    - [ ] Todo
-    - [x] Done
-    - [n] Next
-    - [~] Pending
-    - [c] Cancelled
-    - [ ] 20230703 Todo with a date. If it's the day, `dela list -t` will list this guy
-    - [ ] Todo with tags #tagone #tagtwo
-    - [ ] 23330101 Future task will be hidden until the day become
-"""
-
-version = pkg_resources.get_distribution("dela").version
-
-def main():
-    args = docopt(doc, version=version)
-
-    if args['--verbose']:
-        log.setLevel(logging.INFO)
-        log.info('Verbose logging has been enabled')
-
-    log.info(f'{args}')
-
-    if args['list'] == True:
-        ListCommand(args).run()
-        exit(0)
+    Next variables are supported:
 
+    - $title
+    - $date
+    - $status
+    - $tags
+    - $file
+```
 
-if __name__ == '__main__':
-    main()
```

