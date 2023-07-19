# Comparing `tmp/wpiformat-2023.27.tar.gz` & `tmp/wpiformat-2023.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpiformat-2023.27.tar", last modified: Thu Jul  6 17:46:09 2023, max compression
+gzip compressed data, was "wpiformat-2023.28.tar", last modified: Wed Jul 19 04:35:41 2023, max compression
```

## Comparing `wpiformat-2023.27.tar` & `wpiformat-2023.28.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:09.983296 wpiformat-2023.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-06 17:45:58.000000 wpiformat-2023.27/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-06 17:46:09.983296 wpiformat-2023.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-06 17:45:58.000000 wpiformat-2023.27/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-06 17:45:58.000000 wpiformat-2023.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:46:09.983296 wpiformat-2023.27/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:09.979296 wpiformat-2023.27/wpiformat/
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/bracecomment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/cidentlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/clangformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/clangtidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   144229 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/eofnewline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/gtestname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/includeguard.py
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/includeorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/javaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/jni.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/licenseupdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/pyformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:09.983296 wpiformat-2023.27/wpiformat/test/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_bracecomment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_cidentlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_eofnewline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_gtestname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_includeguard.py
--rw-r--r--   0 runner    (1001) docker     (123)    23206 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_includeorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_javaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29622 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_jni.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_licenseupdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_tasktest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_usingdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_usingnamespacestd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/test/test_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/usingdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/usingnamespacestd.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 17:45:58.000000 wpiformat-2023.27/wpiformat/whitespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:09.979296 wpiformat-2023.27/wpiformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-06 17:46:09.000000 wpiformat-2023.27/wpiformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-06 17:46:09.000000 wpiformat-2023.27/wpiformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:46:09.000000 wpiformat-2023.27/wpiformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 17:46:09.000000 wpiformat-2023.27/wpiformat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 17:46:09.000000 wpiformat-2023.27/wpiformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 17:46:09.000000 wpiformat-2023.27/wpiformat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:35:41.488609 wpiformat-2023.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-19 04:35:29.000000 wpiformat-2023.28/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-19 04:35:41.488609 wpiformat-2023.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-19 04:35:29.000000 wpiformat-2023.28/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-19 04:35:29.000000 wpiformat-2023.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:35:41.488609 wpiformat-2023.28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:35:41.484609 wpiformat-2023.28/wpiformat/
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/bracecomment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/cidentlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/clangformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/clangtidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144241 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/eofnewline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/gtestname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/includeguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/includeorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/javaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/jni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/licenseupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/pyformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:35:41.488609 wpiformat-2023.28/wpiformat/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_bracecomment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_cidentlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_eofnewline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_gtestname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_includeguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23206 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_includeorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_javaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29622 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_jni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_licenseupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_tasktest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_usingdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_usingnamespacestd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/test/test_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/usingdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/usingnamespacestd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-19 04:35:29.000000 wpiformat-2023.28/wpiformat/whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:35:41.484609 wpiformat-2023.28/wpiformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-19 04:35:41.000000 wpiformat-2023.28/wpiformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-19 04:35:41.000000 wpiformat-2023.28/wpiformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:35:41.000000 wpiformat-2023.28/wpiformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 04:35:41.000000 wpiformat-2023.28/wpiformat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 04:35:41.000000 wpiformat-2023.28/wpiformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 04:35:41.000000 wpiformat-2023.28/wpiformat.egg-info/top_level.txt
```

### Comparing `wpiformat-2023.27/LICENSE.txt` & `wpiformat-2023.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/PKG-INFO` & `wpiformat-2023.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpiformat
-Version: 2023.27
+Version: 2023.28
 Summary: Linters and formatters for ensuring WPILib's source code conforms to its style guide
 Maintainer-email: Tyler Veness <calcmogul@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wpilibsuite/styleguide
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `wpiformat-2023.27/README.rst` & `wpiformat-2023.28/README.rst`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/pyproject.toml` & `wpiformat-2023.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/__init__.py` & `wpiformat-2023.28/wpiformat/__init__.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/bracecomment.py` & `wpiformat-2023.28/wpiformat/bracecomment.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/cidentlist.py` & `wpiformat-2023.28/wpiformat/cidentlist.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/clangformat.py` & `wpiformat-2023.28/wpiformat/clangformat.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/clangtidy.py` & `wpiformat-2023.28/wpiformat/clangtidy.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/config.py` & `wpiformat-2023.28/wpiformat/config.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/cpplint.py` & `wpiformat-2023.28/wpiformat/cpplint.py`

 * *Files 0% similar despite different names*

```diff
@@ -3178,15 +3178,15 @@
                   clean_lines.elided[linenum - 2]) or
             Search(r'\bstd::m?function\s*\<\s*$',
                    clean_lines.elided[linenum - 1]))))
 
 
 _HEADERS_CONTAINING_TEMPLATES = (
     ('<deque>', ('deque',)),
-    ('<functional>', ('unary_function', 'binary_function',
+    ('<functional>', ('function', 'unary_function', 'binary_function',
                       'plus', 'minus', 'multiplies', 'divides', 'modulus',
                       'negate',
                       'equal_to', 'not_equal_to', 'greater', 'less',
                       'greater_equal', 'less_equal',
                       'logical_and', 'logical_or', 'logical_not',
                       'unary_negate', 'not1', 'binary_negate', 'not2',
                       'bind1st', 'bind2nd',
```

### Comparing `wpiformat-2023.27/wpiformat/gtestname.py` & `wpiformat-2023.28/wpiformat/gtestname.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/includeguard.py` & `wpiformat-2023.28/wpiformat/includeguard.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/includeorder.py` & `wpiformat-2023.28/wpiformat/includeorder.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/javaclass.py` & `wpiformat-2023.28/wpiformat/javaclass.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/jni.py` & `wpiformat-2023.28/wpiformat/jni.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/licenseupdate.py` & `wpiformat-2023.28/wpiformat/licenseupdate.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/lint.py` & `wpiformat-2023.28/wpiformat/lint.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/pyformat.py` & `wpiformat-2023.28/wpiformat/pyformat.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/stdlib.py` & `wpiformat-2023.28/wpiformat/stdlib.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/task.py` & `wpiformat-2023.28/wpiformat/task.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_bracecomment.py` & `wpiformat-2023.28/wpiformat/test/test_bracecomment.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_cidentlist.py` & `wpiformat-2023.28/wpiformat/test/test_cidentlist.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_config.py` & `wpiformat-2023.28/wpiformat/test/test_config.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_eofnewline.py` & `wpiformat-2023.28/wpiformat/test/test_eofnewline.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_gtestname.py` & `wpiformat-2023.28/wpiformat/test/test_gtestname.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_includeguard.py` & `wpiformat-2023.28/wpiformat/test/test_includeguard.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_includeorder.py` & `wpiformat-2023.28/wpiformat/test/test_includeorder.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_javaclass.py` & `wpiformat-2023.28/wpiformat/test/test_javaclass.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_jni.py` & `wpiformat-2023.28/wpiformat/test/test_jni.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_licenseupdate.py` & `wpiformat-2023.28/wpiformat/test/test_licenseupdate.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_stdlib.py` & `wpiformat-2023.28/wpiformat/test/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_tasktest.py` & `wpiformat-2023.28/wpiformat/test/test_tasktest.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_usingdeclaration.py` & `wpiformat-2023.28/wpiformat/test/test_usingdeclaration.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_usingnamespacestd.py` & `wpiformat-2023.28/wpiformat/test/test_usingnamespacestd.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/test/test_whitespace.py` & `wpiformat-2023.28/wpiformat/test/test_whitespace.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/usingdeclaration.py` & `wpiformat-2023.28/wpiformat/usingdeclaration.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/usingnamespacestd.py` & `wpiformat-2023.28/wpiformat/usingnamespacestd.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat/version.py` & `wpiformat-2023.28/wpiformat/version.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2023.27/wpiformat.egg-info/PKG-INFO` & `wpiformat-2023.28/wpiformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpiformat
-Version: 2023.27
+Version: 2023.28
 Summary: Linters and formatters for ensuring WPILib's source code conforms to its style guide
 Maintainer-email: Tyler Veness <calcmogul@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wpilibsuite/styleguide
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `wpiformat-2023.27/wpiformat.egg-info/SOURCES.txt` & `wpiformat-2023.28/wpiformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

