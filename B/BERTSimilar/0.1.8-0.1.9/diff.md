# Comparing `tmp/BERTSimilar-0.1.8.tar.gz` & `tmp/BERTSimilar-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BERTSimilar-0.1.8.tar", last modified: Tue Jul 18 19:01:26 2023, max compression
+gzip compressed data, was "BERTSimilar-0.1.9.tar", last modified: Wed Jul 19 00:54:55 2023, max compression
```

## Comparing `BERTSimilar-0.1.8.tar` & `BERTSimilar-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 19:01:26.396838 BERTSimilar-0.1.8/
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 19:01:26.395609 BERTSimilar-0.1.8/BERTSimilar/
--rw-r--r--   0 rdp        (501) staff       (20)    25880 2023-07-18 19:01:01.000000 BERTSimilar-0.1.8/BERTSimilar/BERTSimilar.py
--rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.8/BERTSimilar/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 19:01:26.396391 BERTSimilar-0.1.8/BERTSimilar.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      161 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.8/LICENSE.txt
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 19:01:26.396625 BERTSimilar-0.1.8/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.8/README.md
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 19:01:26.396891 BERTSimilar-0.1.8/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-18 19:01:18.000000 BERTSimilar-0.1.8/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 00:54:55.148974 BERTSimilar-0.1.9/
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 00:54:55.147767 BERTSimilar-0.1.9/BERTSimilar/
+-rw-r--r--   0 rdp        (501) staff       (20)    25884 2023-07-19 00:33:13.000000 BERTSimilar-0.1.9/BERTSimilar/BERTSimilar.py
+-rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.9/BERTSimilar/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 00:54:55.148568 BERTSimilar-0.1.9/BERTSimilar.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-19 00:54:55.000000 BERTSimilar-0.1.9/BERTSimilar.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-19 00:54:55.000000 BERTSimilar-0.1.9/BERTSimilar.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-19 00:54:55.000000 BERTSimilar-0.1.9/BERTSimilar.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      161 2023-07-19 00:54:55.000000 BERTSimilar-0.1.9/BERTSimilar.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-19 00:54:55.000000 BERTSimilar-0.1.9/BERTSimilar.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.9/LICENSE.txt
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-19 00:54:55.148791 BERTSimilar-0.1.9/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.9/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-19 00:54:55.149023 BERTSimilar-0.1.9/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-19 00:54:52.000000 BERTSimilar-0.1.9/setup.py
```

### Comparing `BERTSimilar-0.1.8/BERTSimilar/BERTSimilar.py` & `BERTSimilar-0.1.9/BERTSimilar/BERTSimilar.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,20 +135,20 @@
         self.cv_words = self.count_vectorizer.get_feature_names_out()
         self.bert_words_all = np.array(list(itertools.chain.from_iterable(self.bert_words_ngram)))
         self.bert_vectors_all = np.array(list(itertools.chain.from_iterable(self.bert_vectors_ngram)))
         if self.scaler is not None:
             df = pd.DataFrame(self.bert_vectors_all, columns=self.scaler_col_names)
             self.bert_vectors_all = self.scaler.transform(df)
             del df
-            for i in tqdmn(range(self.max_ngram), desc='Creating', postfix='N-gram Words and Embeddings'):
+            for i in tqdmn(range(self.max_ngram), desc='Generating', postfix='N-gram Words and Embeddings'):
                 df = pd.DataFrame(self.bert_vectors_ngram[i], columns=self.scaler_col_names)
                 self.bert_vectors_ngram[i] = self.scaler.transform(df)
                 del df
         else:
-            for i in tqdmn(range(self.max_ngram), desc='Creating', postfix='N-gram Words and Embeddings'):
+            for i in tqdmn(range(self.max_ngram), desc='Generating', postfix='N-gram Words and Embeddings'):
                 self.bert_vectors_ngram[i] = np.array(self.bert_vectors_ngram[i])
         return self
 
     def _process_wikipedia_dataset(self, page_content):
 
         document_list = []
         for section in page_content:
```

### Comparing `BERTSimilar-0.1.8/BERTSimilar.egg-info/PKG-INFO` & `BERTSimilar-0.1.9/BERTSimilar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.8/LICENSE.txt` & `BERTSimilar-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.8/PKG-INFO` & `BERTSimilar-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.8/README.md` & `BERTSimilar-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.8/setup.py` & `BERTSimilar-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='BERTSimilar',
-    version='0.1.8',
+    version='0.1.9',
     description="Get Similar Words and Embeddings using BERT Models",
     keywords="BERT NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

