# Comparing `tmp/datawords-0.5.0rc2.tar.gz` & `tmp/datawords-0.5.0rc3.tar.gz`

## Comparing `datawords-0.5.0rc2.tar` & `datawords-0.5.0rc3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/.pylintrc
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/_utils.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/constants.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/index_old.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/indexes.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/install_pytorch.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/models.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/models_old.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/parsers.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/ranking.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/deepnlp/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/deepnlp/core.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/deepnlp/translators.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/deepnlp/translators2.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/deepnlp/utils.py
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/files/stop_en.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/files/stop_es.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/datawords/files/stop_pt.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/make.bat
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/api_reference.rst
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/conf.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/index.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/api/deepnlp.rst
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/api/indexes.rst
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/api/models.rst
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/api/parsers.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/docs/source/api/ranking.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/tests/__init__.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/tests/test_indexes.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/tests/test_models.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/tests/test_parsers.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/tests/test_rankings.py
--rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/tests/texts.txt
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/LICENSE
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/NOTICE.md
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/README.md
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/.pylintrc
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/_utils.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/constants.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/index_old.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/indexes.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/install_pytorch.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/models.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/models_old.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/parsers.py
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/ranking.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/deepnlp/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/deepnlp/core.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/deepnlp/translators.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/deepnlp/translators2.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/deepnlp/utils.py
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/files/stop_en.txt
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/files/stop_es.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/datawords/files/stop_pt.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/make.bat
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/api_reference.rst
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/conf.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/index.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/api/deepnlp.rst
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/api/indexes.rst
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/api/models.rst
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/api/parsers.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/docs/source/api/ranking.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/shared.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/test_indexes.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/test_models.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/test_parsers.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/test_rankings.py
+-rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/tests/texts.txt
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/LICENSE
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/NOTICE.md
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/README.md
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 datawords-0.5.0rc3/PKG-INFO
```

### Comparing `datawords-0.5.0rc2/.pylintrc` & `datawords-0.5.0rc3/.pylintrc`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/Makefile` & `datawords-0.5.0rc3/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/_utils.py` & `datawords-0.5.0rc3/datawords/_utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/constants.py` & `datawords-0.5.0rc3/datawords/constants.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/index_old.py` & `datawords-0.5.0rc3/datawords/index_old.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/indexes.py` & `datawords-0.5.0rc3/datawords/indexes.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/install_pytorch.py` & `datawords-0.5.0rc3/datawords/install_pytorch.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/models.py` & `datawords-0.5.0rc3/datawords/models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/models_old.py` & `datawords-0.5.0rc3/datawords/models_old.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/parsers.py` & `datawords-0.5.0rc3/datawords/parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/ranking.py` & `datawords-0.5.0rc3/datawords/ranking.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 class PageRankTFIDF:
     # pylint: disable=too-few-public-methods
     """PageRank based on TFIDF"""
 
     def __init__(
-        self, tokenizer, barrier=0.7, min_df=1, max_df=0.9, ngram_range=(1, 1)
+        self, tokenizer=None, barrier=0.7, min_df=1, max_df=0.9, ngram_range=(1, 1)
     ):
         # pylint: disable=too-many-arguments
         self.tf = TfidfVectorizer(
             analyzer="word",
             ngram_range=ngram_range,
             # stop_words=stopw,
             tokenizer=tokenizer,
@@ -185,16 +185,16 @@
 
     def fit_transform(self, X: np.ndarray):
         self.fit(X)
         scores = self.transform()
         return scores
 
     def rank(self, index: List[Any], top_n=5):
-        """ given a `index` build a ranking using the scores created
-        by PageRank. """
+        """given a `index` build a ranking using the scores created
+        by PageRank."""
         ranking = zip(index, self.scores)
         best = sorted(ranking, key=lambda tup: tup[1], reverse=True)[:top_n]
         return best
 
     @property
     def scores(self):
         return self._scores
@@ -202,7 +202,32 @@
     @property
     def edges(self):
         return self._edges
 
     @property
     def adjacency(self):
         return self._adj
+
+
+def rank(index: List[Any], scores: np.ndarray, top_n=5):
+    """
+    given a score result from any of the PageRank models
+    an a index which correlates with the data used to calculate
+    pagerank then, reorder score from top to bottom.
+
+    To produce a simple numeric index, :function:`datawords.ranking.numeric_index`
+    could be used. 
+    """
+    ranking = zip(index, scores)
+    best = sorted(ranking, key=lambda tup: tup[1], reverse=True)
+    if top_n:
+        return best[:top_n]
+    return best
+
+
+def numeric_index(values: List[Any]) -> List[int]:
+    """
+    given a list of values of any type it produce
+    an incremental index of int.
+    useful for :function:`datawords.ranking.rank`
+    """
+    return list(range(0, len(values)))
```

### Comparing `datawords-0.5.0rc2/datawords/utils.py` & `datawords-0.5.0rc3/datawords/utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/deepnlp/core.py` & `datawords-0.5.0rc3/datawords/deepnlp/core.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/deepnlp/translators.py` & `datawords-0.5.0rc3/datawords/deepnlp/translators.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/deepnlp/translators2.py` & `datawords-0.5.0rc3/datawords/deepnlp/translators2.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/files/stop_en.txt` & `datawords-0.5.0rc3/datawords/files/stop_en.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/files/stop_es.txt` & `datawords-0.5.0rc3/datawords/files/stop_es.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/datawords/files/stop_pt.txt` & `datawords-0.5.0rc3/datawords/files/stop_pt.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/Makefile` & `datawords-0.5.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/make.bat` & `datawords-0.5.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/source/conf.py` & `datawords-0.5.0rc3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/source/index.rst` & `datawords-0.5.0rc3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/source/api/deepnlp.rst` & `datawords-0.5.0rc3/docs/source/api/deepnlp.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/source/api/indexes.rst` & `datawords-0.5.0rc3/docs/source/api/indexes.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/docs/source/api/parsers.rst` & `datawords-0.5.0rc3/docs/source/api/parsers.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/tests/test_indexes.py` & `datawords-0.5.0rc3/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/tests/test_models.py` & `datawords-0.5.0rc3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/tests/test_parsers.py` & `datawords-0.5.0rc3/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/tests/texts.txt` & `datawords-0.5.0rc3/tests/texts.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/.gitignore` & `datawords-0.5.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/LICENSE` & `datawords-0.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/README.md` & `datawords-0.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `datawords-0.5.0rc2/pyproject.toml` & `datawords-0.5.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	"langdetect~=1.0.9",
 	"python-Levenshtein~=0.12.2",
 	"emoji~=1.5.0",
 	"gensim~=4.3.0",
 	"nltk~=3.6.4",
 	"scikit-learn~=1.2.0",
 	"spacy~=3.4.4",
-	"pytextrank~=3.2.1",
+	# "pytextrank~=3.2.1",
 	"scikit-network~=0.28.3",
 	"langcodes[data]~=3.2.1",
 	"annoy~=1.17.0",
 	"pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0",
 	"toolz",
 	"tqdm",
 ]
```

### Comparing `datawords-0.5.0rc2/PKG-INFO` & `datawords-0.5.0rc3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawords
-Version: 0.5.0rc2
+Version: 0.5.0rc3
 Summary: A library to work with text data
 Project-URL: Documentation, https://github.com/unknown/datawords#readme
 Project-URL: Issues, https://github.com/unknown/datawords/issues
 Project-URL: Source, https://github.com/unknown/datawords
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
@@ -25,15 +25,14 @@
 Requires-Dist: annoy~=1.17.0
 Requires-Dist: emoji~=1.5.0
 Requires-Dist: gensim~=4.3.0
 Requires-Dist: langcodes[data]~=3.2.1
 Requires-Dist: langdetect~=1.0.9
 Requires-Dist: nltk~=3.6.4
 Requires-Dist: pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4
-Requires-Dist: pytextrank~=3.2.1
 Requires-Dist: python-levenshtein~=0.12.2
 Requires-Dist: scikit-learn~=1.2.0
 Requires-Dist: scikit-network~=0.28.3
 Requires-Dist: spacy~=3.4.4
 Requires-Dist: toolz
 Requires-Dist: tqdm
 Requires-Dist: unidecode~=1.3.2
```

