# Comparing `tmp/easylaser-0.1.3.tar.gz` & `tmp/easylaser-0.1.4.tar.gz`

## Comparing `easylaser-0.1.3.tar` & `easylaser-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/__init__.py
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/align.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/get_model.py
--rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/laser.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/embed.py
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/encoder.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/laserLstmEncoder.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/laserTransformerEncoder.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/multiGpuEncoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/lib/constants.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/lib/text_processing.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.3/test/fake_data.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.3/test/test_laser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 easylaser-0.1.3/.gitignore
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.3/LICENSE
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.3/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 easylaser-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 easylaser-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/__init__.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/align.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/get_model.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/laser.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/embed/embed.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/lib/constants.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 easylaser-0.1.4/easylaser/lib/text_processing.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.4/test/fake_data.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.4/test/test_laser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 easylaser-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.4/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 easylaser-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 easylaser-0.1.4/PKG-INFO
```

### Comparing `easylaser-0.1.3/easylaser/align.py` & `easylaser-0.1.4/easylaser/align.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/get_model.py` & `easylaser-0.1.4/easylaser/get_model.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/laser.py` & `easylaser-0.1.4/easylaser/laser.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             raise RuntimeError(
                 "Encoder not started, please start it with start_encoder"
             )
         embeddings = embed_sentences(
             sentences=sentences,
             encoder=self.encoder,
             verbose=self.verbose,
-            spm_model=self.spm,
+            sp=self.sp,
         )
         return embeddings
 
     def align_sentences(
         self,
         sentences_lang0: list[str],
         sentences_lang1: list[str],
```

### Comparing `easylaser-0.1.3/easylaser/embed/embed.py` & `easylaser-0.1.4/easylaser/embed/embed.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/embed/encoder.py` & `easylaser-0.1.4/easylaser/embed/encoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/embed/laserLstmEncoder.py` & `easylaser-0.1.4/easylaser/embed/laserLstmEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/embed/laserTransformerEncoder.py` & `easylaser-0.1.4/easylaser/embed/laserTransformerEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/embed/multiGpuEncoder.py` & `easylaser-0.1.4/easylaser/embed/multiGpuEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/lib/constants.py` & `easylaser-0.1.4/easylaser/lib/constants.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/easylaser/lib/text_processing.py` & `easylaser-0.1.4/easylaser/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/test/fake_data.py` & `easylaser-0.1.4/test/fake_data.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/test/test_laser.py` & `easylaser-0.1.4/test/test_laser.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/LICENSE` & `easylaser-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/README.md` & `easylaser-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.3/pyproject.toml` & `easylaser-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "easylaser"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Lingua Custodia", email="it@linguacustodia.com" },
 ]
 description = "An easy to use interface to LASER"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `easylaser-0.1.3/PKG-INFO` & `easylaser-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylaser
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy to use interface to LASER
 Author-email: Lingua Custodia <it@linguacustodia.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

