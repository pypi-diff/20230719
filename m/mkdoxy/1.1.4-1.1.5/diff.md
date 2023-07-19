# Comparing `tmp/mkdoxy-1.1.4.tar.gz` & `tmp/mkdoxy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.1.4.tar", last modified: Mon Jul 17 11:27:48 2023, max compression
+gzip compressed data, was "mkdoxy-1.1.5.tar", last modified: Wed Jul 19 14:36:02 2023, max compression
```

## Comparing `mkdoxy-1.1.4.tar` & `mkdoxy-1.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.756512 mkdoxy-1.1.4/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.4/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-17 11:27:48.756381 mkdoxy-1.1.4/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.4/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.752667 mkdoxy-1.1.4/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.4/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.4/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.4/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     4393 2023-07-17 11:27:23.000000 mkdoxy-1.1.4/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     4443 2023-07-17 11:24:21.000000 mkdoxy-1.1.4/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-07-17 11:27:25.000000 mkdoxy-1.1.4/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    12051 2023-07-13 14:03:02.000000 mkdoxy-1.1.4/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.4/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    21472 2023-07-17 11:27:29.000000 mkdoxy-1.1.4/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     7770 2023-07-17 11:24:21.000000 mkdoxy-1.1.4/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-17 11:27:30.000000 mkdoxy-1.1.4/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.756165 mkdoxy-1.1.4/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.4/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4632 2023-07-17 11:23:05.000000 mkdoxy-1.1.4/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.4/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-07-17 11:27:32.000000 mkdoxy-1.1.4/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.753476 mkdoxy-1.1.4/mkdoxy.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      131 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-17 11:27:48.756546 mkdoxy-1.1.4/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1838 2023-07-17 11:24:52.000000 mkdoxy-1.1.4/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.495192 mkdoxy-1.1.5/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.5/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-19 14:36:02.495052 mkdoxy-1.1.5/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.5/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.490581 mkdoxy-1.1.5/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.5/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.5/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.5/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4393 2023-07-17 11:27:23.000000 mkdoxy-1.1.5/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4443 2023-07-17 11:24:21.000000 mkdoxy-1.1.5/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-07-17 11:27:25.000000 mkdoxy-1.1.5/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    12051 2023-07-13 14:03:02.000000 mkdoxy-1.1.5/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.5/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    21472 2023-07-17 11:27:29.000000 mkdoxy-1.1.5/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7770 2023-07-17 11:24:21.000000 mkdoxy-1.1.5/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-17 11:27:30.000000 mkdoxy-1.1.5/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.494821 mkdoxy-1.1.5/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.5/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4632 2023-07-17 11:23:05.000000 mkdoxy-1.1.5/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.5/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.5/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-07-17 11:27:32.000000 mkdoxy-1.1.5/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-19 14:36:02.491569 mkdoxy-1.1.5/mkdoxy.egg-info/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      143 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-19 14:36:02.000000 mkdoxy-1.1.5/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-19 14:36:02.495227 mkdoxy-1.1.5/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1853 2023-07-19 14:34:47.000000 mkdoxy-1.1.5/setup.py
```

### Comparing `mkdoxy-1.1.4/LICENSE` & `mkdoxy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/PKG-INFO` & `mkdoxy-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.4
+Version: 1.1.5
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.4 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.5 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.1.4/README.md` & `mkdoxy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.1.5/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/constants.py` & `mkdoxy-1.1.5/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/doxygen.py` & `mkdoxy-1.1.5/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/doxyrun.py` & `mkdoxy-1.1.5/mkdoxy/doxyrun.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/finder.py` & `mkdoxy-1.1.5/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/generatorAuto.py` & `mkdoxy-1.1.5/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/generatorBase.py` & `mkdoxy-1.1.5/mkdoxy/generatorBase.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/generatorSnippets.py` & `mkdoxy-1.1.5/mkdoxy/generatorSnippets.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/markdown.py` & `mkdoxy-1.1.5/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/node.py` & `mkdoxy-1.1.5/mkdoxy/node.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/plugin.py` & `mkdoxy-1.1.5/mkdoxy/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/property.py` & `mkdoxy-1.1.5/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/code.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/error.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/templates/member.jinja2` & `mkdoxy-1.1.5/mkdoxy/templates/member.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/utils.py` & `mkdoxy-1.1.5/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy/xml_parser.py` & `mkdoxy-1.1.5/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.1.5/mkdoxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.4
+Version: 1.1.5
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.4 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.5 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.1.4/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.1.5/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.4/setup.py` & `mkdoxy-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name='mkdoxy',
-    version='1.1.4',
+    version='1.1.5',
     description='MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator',
     url='https://github.com/JakubAndrysek/MkDoxy',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
@@ -25,15 +25,15 @@
     project_urls={
         'Source': 'https://github.com/JakubAndrysek/MkDoxy',
         'Documentation': 'https://mkdoxy.kubaandrysek.cz/',
         'Tracker': 'https://github.com/JakubAndrysek/MkDoxy/issues',
         'Funding': 'https://github.com/sponsors/jakubandrysek',
     },
 
-    install_requires=['mkdocs'],
+    install_requires=['mkdocs', 'ruamel.yaml'],
     extras_require={
         "dev": [
             "mkdocs-material==9.1.18",
             "Jinja2~=3.1.2",
             "ruamel.yaml~=0.17.32",
             "mkdocs-open-in-new-tab~=1.0.2",
             "pathlib~=1.0.1",
```

