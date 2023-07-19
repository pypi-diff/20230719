# Comparing `tmp/wordx-0.2.9.1.tar.gz` & `tmp/wordx-0.2.9.2.tar.gz`

## Comparing `wordx-0.2.9.1.tar` & `wordx-0.2.9.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.9.1/src/wordx/__init__.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 wordx-0.2.9.1/src/wordx/fake_zip.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.9.1/src/wordx/sheet.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wordx-0.2.9.1/src/wordx/utility.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.9.1/src/wordx/word_file.py
--rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/1.png
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/1.py
--rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/123.docx
--rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/2.docx
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/3.docx
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/footer.docx
--rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/footer.xml
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/haha.xml
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/test_fake_zip.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/文档合并/123.docx
--rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/文档合并/456.docx
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/文档合并/merge.docx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.9.1/tests/文档合并/merge.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.9.1/LICENSE
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 wordx-0.2.9.1/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 wordx-0.2.9.1/pyproject.toml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 wordx-0.2.9.1/PKG-INFO
+-rw-r--r--   0        0        0    62053 2020-02-02 00:00:00.000000 wordx-0.2.9.2/img/word-template.png
+-rw-r--r--   0        0        0    30134 2020-02-02 00:00:00.000000 wordx-0.2.9.2/img/wordx-tool.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.9.2/src/wordx/__init__.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 wordx-0.2.9.2/src/wordx/fake_zip.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.9.2/src/wordx/sheet.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wordx-0.2.9.2/src/wordx/utility.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.9.2/src/wordx/word_file.py
+-rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/1.png
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/1.py
+-rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/123.docx
+-rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/2.docx
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/3.docx
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/footer.docx
+-rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/footer.xml
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/haha.xml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/test_fake_zip.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/文档合并/123.docx
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/文档合并/456.docx
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/文档合并/merge.docx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.9.2/tests/文档合并/merge.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 wordx-0.2.9.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.9.2/LICENSE
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 wordx-0.2.9.2/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 wordx-0.2.9.2/pyproject.toml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 wordx-0.2.9.2/PKG-INFO
```

### Comparing `wordx-0.2.9.1/src/wordx/fake_zip.py` & `wordx-0.2.9.2/src/wordx/fake_zip.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/src/wordx/sheet.py` & `wordx-0.2.9.2/src/wordx/sheet.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/src/wordx/utility.py` & `wordx-0.2.9.2/src/wordx/utility.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/src/wordx/word_file.py` & `wordx-0.2.9.2/src/wordx/word_file.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/1.png` & `wordx-0.2.9.2/tests/1.png`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/1.py` & `wordx-0.2.9.2/tests/1.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/123.docx` & `wordx-0.2.9.2/tests/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/2.docx` & `wordx-0.2.9.2/tests/2.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/3.docx` & `wordx-0.2.9.2/tests/3.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/footer.docx` & `wordx-0.2.9.2/tests/footer.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/footer.xml` & `wordx-0.2.9.2/tests/footer.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/haha.xml` & `wordx-0.2.9.2/tests/haha.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/test_fake_zip.py` & `wordx-0.2.9.2/tests/test_fake_zip.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/文档合并/123.docx` & `wordx-0.2.9.2/tests/文档合并/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/文档合并/456.docx` & `wordx-0.2.9.2/tests/文档合并/456.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/tests/文档合并/merge.docx` & `wordx-0.2.9.2/tests/文档合并/merge.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/LICENSE` & `wordx-0.2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wordx-0.2.9.1/pyproject.toml` & `wordx-0.2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wordx"
-version = "0.2.9.1"
+version = "0.2.9.2"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "generate word documents in a sexy way"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

