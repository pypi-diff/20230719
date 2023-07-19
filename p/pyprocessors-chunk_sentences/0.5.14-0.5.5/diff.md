# Comparing `tmp/pyprocessors_chunk_sentences-0.5.14.tar.gz` & `tmp/pyprocessors-chunk_sentences-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_chunk_sentences-0.5.14.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors-chunk_sentences-0.5.5.tar", last modified: Fri Feb 24 14:18:21 2023, max compression
```

## Comparing `pyprocessors_chunk_sentences-0.5.14.tar` & `pyprocessors-chunk_sentences-0.5.5.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0      504 2023-07-19 10:05:16.176625 pyprocessors_chunk_sentences-0.5.14/.bumpversion.cfg
--rw-r--r--   0        0        0     1760 2023-07-19 10:05:16.176625 pyprocessors_chunk_sentences-0.5.14/.gitignore
--rw-r--r--   0        0        0      419 2023-07-19 10:05:16.177625 pyprocessors_chunk_sentences-0.5.14/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2023-07-19 10:05:16.177625 pyprocessors_chunk_sentences-0.5.14/.readthedocs.yml
--rw-r--r--   0        0        0      124 2023-07-19 10:05:16.178625 pyprocessors_chunk_sentences-0.5.14/AUTHORS.md
--rw-r--r--   0        0        0      268 2023-07-19 10:05:16.178625 pyprocessors_chunk_sentences-0.5.14/CHANGELOG.md
--rw-r--r--   0        0        0      476 2023-07-19 10:05:16.179625 pyprocessors_chunk_sentences-0.5.14/Dockerfile
--rw-r--r--   0        0        0    10243 2023-07-19 10:05:16.179625 pyprocessors_chunk_sentences-0.5.14/Jenkinsfile
--rw-r--r--   0        0        0     1082 2023-07-19 10:05:16.180625 pyprocessors_chunk_sentences-0.5.14/LICENSE
--rw-r--r--   0        0        0     1648 2023-07-19 10:05:16.180625 pyprocessors_chunk_sentences-0.5.14/README.md
--rw-r--r--   0        0        0      955 2023-07-19 10:05:16.181625 pyprocessors_chunk_sentences-0.5.14/RELEASE.md
--rw-r--r--   0        0        0     1559 2023-07-19 10:05:16.182625 pyprocessors_chunk_sentences-0.5.14/bumpversion.py
--rw-r--r--   0        0        0       62 2023-07-19 10:05:16.183625 pyprocessors_chunk_sentences-0.5.14/docs/.gitignore
--rw-r--r--   0        0        0      268 2023-07-19 10:05:16.183625 pyprocessors_chunk_sentences-0.5.14/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-07-19 10:05:16.184625 pyprocessors_chunk_sentences-0.5.14/docs/LICENSE
--rw-r--r--   0        0        0        0 2023-07-19 10:05:16.184625 pyprocessors_chunk_sentences-0.5.14/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-07-19 10:05:16.186625 pyprocessors_chunk_sentences-0.5.14/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2914 2023-07-19 10:05:16.187625 pyprocessors_chunk_sentences-0.5.14/docs/conf.py
--rw-r--r--   0        0        0      149 2023-07-19 10:05:16.187625 pyprocessors_chunk_sentences-0.5.14/docs/index.rst
--rw-r--r--   0        0        0       98 2023-07-19 10:05:16.188625 pyprocessors_chunk_sentences-0.5.14/mypy.ini
--rw-r--r--   0        0        0     2304 2023-07-19 10:05:16.188625 pyprocessors_chunk_sentences-0.5.14/pyproject.toml
--rw-r--r--   0        0        0       64 2023-07-19 10:09:08.151265 pyprocessors_chunk_sentences-0.5.14/src/pyprocessors_chunk_sentences/__init__.py
--rw-r--r--   0        0        0     6587 2023-07-19 10:05:16.190625 pyprocessors_chunk_sentences-0.5.14/src/pyprocessors_chunk_sentences/chunk_sentences.py
--rw-r--r--   0        0        0        0 2023-07-19 10:05:16.190625 pyprocessors_chunk_sentences-0.5.14/tests/__init__.py
--rw-r--r--   0        0        0     3286 2023-07-19 10:05:16.191625 pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr.json
--rw-r--r--   0        0        0     3002 2023-07-19 10:09:04.541161 pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_char_chunked.json
--rw-r--r--   0        0        0     2900 2023-07-19 10:09:04.542162 pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_char_chunked2.json
--rw-r--r--   0        0        0     3102 2023-07-19 10:09:04.545162 pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_token_chunked.json
--rw-r--r--   0        0        0     2900 2023-07-19 10:09:04.552162 pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_token_chunked2.json
--rw-r--r--   0        0        0     2798 2023-07-19 10:09:05.101178 pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_token_chunked3.json
--rw-r--r--   0        0        0     5369 2023-07-19 10:05:16.199626 pyprocessors_chunk_sentences-0.5.14/tests/test_chunk_sentences.py
--rw-r--r--   0        0        0      927 2023-07-19 10:05:16.199626 pyprocessors_chunk_sentences-0.5.14/tox.ini
--rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 pyprocessors_chunk_sentences-0.5.14/setup.py
--rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 pyprocessors_chunk_sentences-0.5.14/PKG-INFO
+-rw-r--r--   0        0        0      504 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.bumpversion.cfg
+-rw-r--r--   0        0        0     1760 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.gitignore
+-rw-r--r--   0        0        0      419 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.readthedocs.yml
+-rw-r--r--   0        0        0      124 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/AUTHORS.md
+-rw-r--r--   0        0        0      268 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0      476 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/Dockerfile
+-rw-r--r--   0        0        0    10243 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1648 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/README.md
+-rw-r--r--   0        0        0      955 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/RELEASE.md
+-rw-r--r--   0        0        0     1559 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/bumpversion.py
+-rw-r--r--   0        0        0       62 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/.gitignore
+-rw-r--r--   0        0        0      268 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/LICENSE
+-rw-r--r--   0        0        0        0 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2914 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/conf.py
+-rw-r--r--   0        0        0      149 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/index.rst
+-rw-r--r--   0        0        0       98 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/mypy.ini
+-rw-r--r--   0        0        0     2289 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-02-24 14:18:20.466203 pyprocessors-chunk_sentences-0.5.5/src/pyprocessors_chunk_sentences/__init__.py
+-rw-r--r--   0        0        0     6283 2023-02-24 10:23:31.993033 pyprocessors-chunk_sentences-0.5.5/src/pyprocessors_chunk_sentences/chunk_sentences.py
+-rw-r--r--   0        0        0        0 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0     3286 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr.json
+-rw-r--r--   0        0        0     3002 2023-02-24 14:18:17.620129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked.json
+-rw-r--r--   0        0        0     2900 2023-02-24 14:18:17.621129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked2.json
+-rw-r--r--   0        0        0     3102 2023-02-24 14:18:17.624129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked.json
+-rw-r--r--   0        0        0     2900 2023-02-24 14:18:17.630129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked2.json
+-rw-r--r--   0        0        0     4671 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/tests/test_chunk_sentences.py
+-rw-r--r--   0        0        0      927 2023-02-24 10:10:11.845208 pyprocessors-chunk_sentences-0.5.5/tox.ini
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 pyprocessors-chunk_sentences-0.5.5/setup.py
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 pyprocessors-chunk_sentences-0.5.5/PKG-INFO
```

### Comparing `pyprocessors_chunk_sentences-0.5.14/.gitignore` & `pyprocessors-chunk_sentences-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/Jenkinsfile` & `pyprocessors-chunk_sentences-0.5.5/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/LICENSE` & `pyprocessors-chunk_sentences-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/README.md` & `pyprocessors-chunk_sentences-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/RELEASE.md` & `pyprocessors-chunk_sentences-0.5.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/bumpversion.py` & `pyprocessors-chunk_sentences-0.5.5/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/docs/LICENSE` & `pyprocessors-chunk_sentences-0.5.5/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/docs/conf.py` & `pyprocessors-chunk_sentences-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/pyproject.toml` & `pyprocessors-chunk_sentences-0.5.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "Programming Language :: Python :: 3.8",
 ]
 requires = [
     "pymultirole-plugins>=0.5.0,<0.6.0",
     "collections-extended",
     "numpy",
     "blingfire",
-    "tiktoken"
 ]
 dist-name = "pyprocessors-chunk_sentences"
 
 [tool.flit.entrypoints."pyprocessors.plugins"]
 chunk_sentences = "pyprocessors_chunk_sentences.chunk_sentences:ChunkSentencesProcessor"
```

### Comparing `pyprocessors_chunk_sentences-0.5.14/src/pyprocessors_chunk_sentences/chunk_sentences.py` & `pyprocessors-chunk_sentences-0.5.5/src/pyprocessors_chunk_sentences/chunk_sentences.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from enum import Enum
 from functools import lru_cache
 from typing import Type, List, cast
 
 import blingfire
-import tiktoken
 from collections_extended import RangeMap
 from pydantic import BaseModel, Field
 from pymultirole_plugins.v1.processor import ProcessorParameters, ProcessorBase
 from pymultirole_plugins.v1.schema import Document, Sentence
 
 
 class ChunkingUnit(str, Enum):
@@ -20,16 +19,14 @@
     wbd = "wbd"
     bert_base_tok = "bert_base_tok"
     bert_base_cased_tok = "bert_base_cased_tok"
     bert_chinese = "bert_chinese"
     bert_multi_cased = "bert_multi_cased"
     xlm_roberta_base = "xlm_roberta_base"
     gpt2 = "gpt2"
-    gpt_4 = "gpt-4"
-    gpt_3_5_turbo = "gpt-3.5-turbo"
     roberta = "roberta"
     laser100k = "laser100k"
     laser250k = "laser250k"
     laser500k = "laser500k"
 
 
 class ChunkSentencesParameters(ProcessorParameters):
@@ -80,27 +77,26 @@
                 sentences.append(Sentence(start=0, end=len(document.text)))
             document.sentences = sentences
         return documents
 
     @classmethod
     def group_sentences(cls, text: str, sentences: List[Sentence], params: ChunkSentencesParameters):
         uncase = 'bert' in params.model.value and 'cased' not in params.model.value
-        h = get_model(params.model.value) if params.unit == ChunkingUnit.token else None
+        h = get_blingfire(params.model.value) if params.unit == ChunkingUnit.token else None
         chunk_size = params.chunk_token_max_length if params.unit == ChunkingUnit.token else params.chunk_char_max_length
         chunks = RangeMap()
         start = 0
         text_length = 0 if params.unit == ChunkingUnit.token else len(text)
         for sent in sentences:
             if h is not None:
                 stext = text[sent.start:sent.end].lower() if uncase else text[sent.start:sent.end]
                 tokens = cls.tokenize_with_model(h, stext)
                 text_length += len(tokens)
                 end = start + len(tokens)
-                if end > start:
-                    chunks[start:end] = WrappedSentence(sent, start=start, end=end)
+                chunks[start:end] = WrappedSentence(sent, start=start, end=end)
                 start = end
             else:
                 chunks[sent.start:sent.end] = WrappedSentence(sent)
 
         cstart = 0
         cend = 0
         while cend < text_length:
@@ -119,20 +115,17 @@
                     cend = chunk[-2].end
                     csend = chunk[-2].sentence.end
             yield (csstart, csend)
             cstart = cend
 
     @classmethod
     def tokenize_with_model(cls, model, stext):
-        if isinstance(model, int):
-            tokens = blingfire.text_to_ids(model, stext, len(stext), unk=0,
-                                           no_padding=True) if model != -1 else blingfire.text_to_words(
-                stext).split(' ')
-        else:
-            tokens = model.encode(stext)
+        tokens = blingfire.text_to_ids(model, stext, len(stext), unk=0,
+                                       no_padding=True) if model != -1 else blingfire.text_to_words(
+            stext).split(' ')
         return tokens
 
     @classmethod
     def get_model(cls) -> Type[BaseModel]:
         return ChunkSentencesParameters
 
 
@@ -140,16 +133,13 @@
     def __init__(self, sentence: Sentence, start=None, end=None):
         self.sentence = sentence
         self.start = start or sentence.start
         self.end = end or sentence.end
 
 
 @lru_cache(maxsize=None)
-def get_model(model: str):
+def get_blingfire(model: str):
     # load a provided with the package model
-    if model == TokenModel.wbd.value:
+    if model == TokenModel.wbd:
         return -1
-    elif model.startswith("gpt-"):
-        h = tiktoken.encoding_for_model(model)
-    else:
-        h = blingfire.load_model(os.path.join(os.path.dirname(blingfire.__file__), f"{model}.bin"))
+    h = blingfire.load_model(os.path.join(os.path.dirname(blingfire.__file__), f"{model}.bin"))
     return h
```

### Comparing `pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_char_chunked.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_char_chunked2.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked2.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_token_chunked.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/tests/data/news_fr_token_chunked2.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked2.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/tests/test_chunk_sentences.py` & `pyprocessors-chunk_sentences-0.5.5/tests/test_chunk_sentences.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import pytest
 from pymultirole_plugins.v1.schema import Document
 
 from pyprocessors_chunk_sentences.chunk_sentences import (
     ChunkSentencesProcessor,
-    ChunkSentencesParameters, ChunkingUnit, TokenModel, get_model,
+    ChunkSentencesParameters, ChunkingUnit, TokenModel, get_blingfire,
 )
 
 
 def test_model():
     model = ChunkSentencesProcessor.get_model()
     model_class = model.construct().__class__
     assert model_class == ChunkSentencesParameters
@@ -47,51 +47,38 @@
     testdir = Path(__file__).parent
     source = Path(testdir, "data/news_fr.json")
     with source.open("r") as fin:
         doc = json.load(fin)
         original_doc = Document(**doc)
     processor = ChunkSentencesProcessor()
     parameters = ChunkSentencesParameters(unit=ChunkingUnit.token)
-    h = get_model(parameters.model.value)
+    h = get_blingfire(parameters.model.value)
     docs = processor.process([Document(**doc)], parameters)
     chunked: Document = docs[0]
     assert len(original_doc.sentences) > len(chunked.sentences)
     for sent in chunked.sentences:
         stokens = ChunkSentencesProcessor.tokenize_with_model(h, chunked.text[sent.start:sent.end])
         assert len(stokens) <= parameters.chunk_token_max_length
     result = Path(testdir, "data/news_fr_token_chunked.json")
     with result.open("w") as fout:
         json.dump(chunked.dict(), fout, indent=2)
 
     parameters = ChunkSentencesParameters(unit=ChunkingUnit.token, model=TokenModel.bert_multi_cased,
                                           chunk_token_max_length=512)
-    h = get_model(parameters.model.value)
+    h = get_blingfire(parameters.model.value)
     docs = processor.process([Document(**doc)], parameters)
     chunked2: Document = docs[0]
     assert len(original_doc.sentences) > len(chunked2.sentences)
     for sent in chunked2.sentences:
         stokens = ChunkSentencesProcessor.tokenize_with_model(h, chunked2.text[sent.start:sent.end])
         assert len(stokens) <= parameters.chunk_token_max_length
     result = Path(testdir, "data/news_fr_token_chunked2.json")
     with result.open("w") as fout:
         json.dump(chunked2.dict(), fout, indent=2)
 
-    parameters = ChunkSentencesParameters(unit=ChunkingUnit.token, model=TokenModel.gpt_4,
-                                          chunk_token_max_length=8000)
-    h = get_model(parameters.model.value)
-    docs = processor.process([Document(**doc)], parameters)
-    chunked2: Document = docs[0]
-    assert len(original_doc.sentences) > len(chunked2.sentences)
-    for sent in chunked2.sentences:
-        stokens = ChunkSentencesProcessor.tokenize_with_model(h, chunked2.text[sent.start:sent.end])
-        assert len(stokens) <= parameters.chunk_token_max_length
-    result = Path(testdir, "data/news_fr_token_chunked3.json")
-    with result.open("w") as fout:
-        json.dump(chunked2.dict(), fout, indent=2)
-
 
 @pytest.mark.skip(reason="Not a test")
 def test_blingfire():
     import blingfire
     s = "Эpple pie. How do I renew my virtual smart card?: /Microsoft IT/ 'virtual' smart card certificates for DirectAccess are valid for one year. In order to get to microsoft.com we need to type pi@1.2.1.2."
 
     print('-----------------------')
@@ -99,15 +86,15 @@
     words = blingfire.text_to_words(s).split(' ')  # sequence length: 128, oov id: 100
     print(len(words))
     print(words)
 
     for m in TokenModel:
         if m != TokenModel.wbd:
             # one time load the model (we are using the one that comes with the package)
-            h = get_model(m.value)
+            h = get_blingfire(m.value)
             print('-----------------------')
             print("Model: %s" % m.value)
 
             # use the model from one or more threads
             ids = blingfire.text_to_ids(h, s, len(s), unk=0, no_padding=True)  # sequence length: 128, oov id: 100
             print(len(ids))  # returns a numpy array of length 128 (padded or trimmed)
             print(ids)  # returns a numpy array of length 128 (padded or trimmed)
```

### Comparing `pyprocessors_chunk_sentences-0.5.14/tox.ini` & `pyprocessors-chunk_sentences-0.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_chunk_sentences-0.5.14/setup.py` & `pyprocessors-chunk_sentences-0.5.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 package_dir = \
 {'': 'src'}
 
 install_requires = \
 ['pymultirole-plugins>=0.5.0,<0.6.0',
  'collections-extended',
  'numpy',
- 'blingfire',
- 'tiktoken']
+ 'blingfire']
 
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
  'docs': ['sphinx',
           'sphinx-rtd-theme',
           'm2r2',
           'sphinxcontrib.apidoc',
@@ -35,15 +34,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['chunk_sentences = '
                           'pyprocessors_chunk_sentences.chunk_sentences:ChunkSentencesProcessor']}
 
 setup(name='pyprocessors-chunk_sentences',
-      version='0.5.14',
+      version='0.5.5',
       description='Sherpa sentence chunking processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_chunk_sentences/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors_chunk_sentences-0.5.14/PKG-INFO` & `pyprocessors-chunk_sentences-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-chunk_sentences
-Version: 0.5.14
+Version: 0.5.5
 Summary: Sherpa sentence chunking processor
 Home-page: https://github.com/oterrier/pyprocessors_chunk_sentences/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -19,15 +19,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: pymultirole-plugins>=0.5.0,<0.6.0
 Requires-Dist: collections-extended
 Requires-Dist: numpy
 Requires-Dist: blingfire
-Requires-Dist: tiktoken
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinxcontrib.apidoc ; extra == "docs"
```

