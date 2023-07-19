# Comparing `tmp/wordx-0.2.7.tar.gz` & `tmp/wordx-0.2.8.tar.gz`

## Comparing `wordx-0.2.7.tar` & `wordx-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.7/src/wordx/__init__.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 wordx-0.2.7/src/wordx/fake_zip.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.7/src/wordx/sheet.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wordx-0.2.7/src/wordx/utility.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.7/src/wordx/word_file.py
--rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/1.png
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/1.py
--rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/123.docx
--rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/2.docx
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/3.docx
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/footer.docx
--rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/footer.xml
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/haha.xml
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/test_fake_zip.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/文档合并/123.docx
--rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/文档合并/456.docx
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/文档合并/merge.docx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.7/tests/文档合并/merge.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.7/LICENSE
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 wordx-0.2.7/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 wordx-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 wordx-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.8/src/wordx/__init__.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 wordx-0.2.8/src/wordx/fake_zip.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.8/src/wordx/sheet.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wordx-0.2.8/src/wordx/utility.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.8/src/wordx/word_file.py
+-rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/1.png
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/1.py
+-rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/123.docx
+-rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/2.docx
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/3.docx
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/footer.docx
+-rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/footer.xml
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/haha.xml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/test_fake_zip.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/文档合并/123.docx
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/文档合并/456.docx
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/文档合并/merge.docx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.8/tests/文档合并/merge.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.8/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 wordx-0.2.8/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 wordx-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 wordx-0.2.8/PKG-INFO
```

### Comparing `wordx-0.2.7/src/wordx/fake_zip.py` & `wordx-0.2.8/src/wordx/fake_zip.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/src/wordx/sheet.py` & `wordx-0.2.8/src/wordx/sheet.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/src/wordx/utility.py` & `wordx-0.2.8/src/wordx/utility.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/src/wordx/word_file.py` & `wordx-0.2.8/src/wordx/word_file.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/1.png` & `wordx-0.2.8/tests/1.png`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/1.py` & `wordx-0.2.8/tests/1.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/123.docx` & `wordx-0.2.8/tests/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/2.docx` & `wordx-0.2.8/tests/2.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/3.docx` & `wordx-0.2.8/tests/3.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/footer.docx` & `wordx-0.2.8/tests/footer.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/footer.xml` & `wordx-0.2.8/tests/footer.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/haha.xml` & `wordx-0.2.8/tests/haha.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/test_fake_zip.py` & `wordx-0.2.8/tests/test_fake_zip.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/文档合并/123.docx` & `wordx-0.2.8/tests/文档合并/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/文档合并/456.docx` & `wordx-0.2.8/tests/文档合并/456.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/tests/文档合并/merge.docx` & `wordx-0.2.8/tests/文档合并/merge.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/LICENSE` & `wordx-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wordx-0.2.7/pyproject.toml` & `wordx-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wordx"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "generate word documents in a sexy way"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `wordx-0.2.7/PKG-INFO` & `wordx-0.2.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordx
-Version: 0.2.7
+Version: 0.2.8
 Summary: generate word documents in a sexy way
 Project-URL: Homepage, https://github.com/inspirare6/wordx
 Project-URL: Bug Tracker, https://github.com/inspirare6/wordx/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,11 +21,11 @@
 
 
 sheet = Sheet('template.docx')
 sheet.render(data)
 sheet.save('output.docx')
 ```
 制作Word模板需配套使用word模板工具
-![Word模板工具箱](https://storage.heinz97.top/github/wordx-tool.png)
+![Word模板工具箱](https://github.com/inspirare6/lims/blob/master/frontend/src/assets/img/logo.png?raw=True)
 
 Word文件模板示例
 ![Word模板示例](https://storage.heinz97.top/github/word-template.png)
```

