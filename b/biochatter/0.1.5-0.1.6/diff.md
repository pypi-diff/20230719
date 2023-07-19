# Comparing `tmp/biochatter-0.1.5.tar.gz` & `tmp/biochatter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biochatter-0.1.5.tar", max compression
+gzip compressed data, was "biochatter-0.1.6.tar", max compression
```

## Comparing `biochatter-0.1.5.tar` & `biochatter-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.5/LICENSE
--rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.5/biochatter/__init__.py
--rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.5/biochatter/_stats.py
--rw-r--r--   0        0        0    18302 2023-07-07 08:35:59.679816 biochatter-0.1.5/biochatter/llm_connect.py
--rw-r--r--   0        0        0     5839 2023-07-06 14:40:38.478959 biochatter-0.1.5/biochatter/podcast.py
--rw-r--r--   0        0        0     5788 2023-07-06 14:40:38.479205 biochatter-0.1.5/biochatter/vectorstore.py
--rw-r--r--   0        0        0      740 2023-07-07 08:36:14.273345 biochatter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 biochatter-0.1.5/setup.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 biochatter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.6/LICENSE
+-rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.6/biochatter/__init__.py
+-rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.6/biochatter/_stats.py
+-rw-r--r--   0        0        0    18302 2023-07-07 08:35:59.679816 biochatter-0.1.6/biochatter/llm_connect.py
+-rw-r--r--   0        0        0     5922 2023-07-19 11:17:00.987814 biochatter-0.1.6/biochatter/podcast.py
+-rw-r--r--   0        0        0     7150 2023-07-19 11:48:37.917691 biochatter-0.1.6/biochatter/vectorstore.py
+-rw-r--r--   0        0        0      765 2023-07-19 11:48:37.919179 biochatter-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 biochatter-0.1.6/setup.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 biochatter-0.1.6/PKG-INFO
```

### Comparing `biochatter-0.1.5/LICENSE` & `biochatter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.5/biochatter/_stats.py` & `biochatter-0.1.6/biochatter/_stats.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.5/biochatter/llm_connect.py` & `biochatter-0.1.6/biochatter/llm_connect.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.5/biochatter/podcast.py` & `biochatter-0.1.6/biochatter/podcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     "You are tasked with summarising a scientific manuscript for consumption as"
     "a podcast. You will receive a collection of sentences from the"
     "manuscript, from which you will remove any information not relevant to the"
     "content, such as references, figure legends, tables, author information, "
     "journal metadata, and so on. You will then be asked to summarise the"
     "section of the manuscript, making the wording more suitable for listening."
     "Remove all content in brackets that is of technical nature, such as"
-    "p-values, statistical tests, and so on."
+    "p-values, statistical tests, and so on. If the given text contains only "
+    "literature references, return 'No content'."
 )
 
 
 class Podcaster:
     def __init__(self, document: Document) -> None:
         """
         Orchestrates the podcasting of a document.
```

### Comparing `biochatter-0.1.5/biochatter/vectorstore.py` & `biochatter-0.1.6/biochatter/vectorstore.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 from langchain.schema import Document
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.document_loaders import TextLoader
 from langchain.vectorstores import Milvus
 
 import fitz  # this is PyMuPDF (PyPI pymupdf package, not fitz)
-
+from transformers import GPT2TokenizerFast
 
 class DocumentEmbedder:
     def __init__(
         self,
         use_prompt: bool = True,
         used: bool = False,
         online: bool = False,
         chunk_size: int = 1000,
         chunk_overlap: int = 0,
+        split_by_characters: bool = True,
         document: Optional[Document] = None,
         separators: Optional[list] = None,
         n_results: int = 3,
         model: Optional[str] = None,
         vector_db_vendor: Optional[str] = None,
         connection_args: Optional[dict] = None,
         api_key: Optional[str] = None,
@@ -34,14 +35,16 @@
         self.use_prompt = use_prompt
         self.used = used
         self.online = online
         self.chunk_size = chunk_size
         self.chunk_overlap = chunk_overlap
         self.separators = separators or [" ", ",", "\n"]
         self.n_results = n_results
+        self.split_by_characters = split_by_characters
+        self.model_name = model
 
         # TODO: variable embeddings depending on model
         # for now, just use ada-002
         # TODO API Key handling to central config
         if not self.online:
             self.embeddings = OpenAIEmbeddings(openai_api_key=api_key)
         else:
@@ -70,20 +73,43 @@
     def set_document(self, document: List[Document]) -> None:
         self.document = document
 
     def _load_document(self, path: str) -> None:
         reader = DocumentReader()
         self.document = reader.load_document(path)
 
-    def split_document(self) -> None:
-        text_splitter = RecursiveCharacterTextSplitter(
+    def _characters_splitter(self) -> RecursiveCharacterTextSplitter:
+        return RecursiveCharacterTextSplitter(
             chunk_size=self.chunk_size,
             chunk_overlap=self.chunk_overlap,
-            separators=self.separators,
+            separators=self.separators
         )
+    def _tokens_splitter(self) -> RecursiveCharacterTextSplitter:
+        DEFAULT_OPENAI_MODEL = "gpt-3.5-turbo"
+        HUGGINGFACE_MODELS = ["bigscience/bloom"]
+        if self.model_name and self.model_name in HUGGINGFACE_MODELS:
+            tokenizer = GPT2TokenizerFast.from_pretrained("gpt2")
+            return RecursiveCharacterTextSplitter.from_huggingface_tokenizer(
+                tokenizer, 
+                chunk_size=self.chunk_size,
+                chunk_overlap=self.chunk_overlap,
+                separators=self.separators
+            )
+        else:
+            return RecursiveCharacterTextSplitter.from_tiktoken_encoder(
+                encoding_name="",
+                model_name=DEFAULT_OPENAI_MODEL if not self.model_name else self.model_name,
+                chunk_size=self.chunk_size,
+                chunk_overlap=self.chunk_overlap,
+                separators=self.separators
+            )
+    def _text_splitter(self) -> RecursiveCharacterTextSplitter:
+        return self._characters_splitter() if self.split_by_characters else self._tokens_splitter()
+    def split_document(self) -> None:
+        text_splitter = self._text_splitter()
         self.split = text_splitter.split_documents(self.document)
 
     def store_embeddings(self) -> None:
         if self.vector_db_vendor == "milvus":
             self.vector_db = Milvus.from_documents(
                 documents=self.split,
                 embedding=self.embeddings,
```

### Comparing `biochatter-0.1.5/pyproject.toml` & `biochatter-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biochatter"
-version = "0.1.5"
+version = "0.1.6"
 description = "Backend library for conversational AI in biomedicine"
 authors = ["Sebastian Lobentanzer <sebastian.lobentanzer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -12,14 +12,15 @@
 openai = "^0.27.8"
 pymupdf = "^1.22.3"
 pymilvus = "2.2.8"
 tiktoken = "^0.4.0"
 nltk = "^3.8.1"
 redis = "^4.5.5"
 retry = "^0.9.2"
+transformers = "^4.30.2"
 streamlit = { version = "^1.23.1", optional = true }
 gTTS = { version = "^2.3.2", optional = true }
 
 [tool.poetry.extras]
 streamlit = ["streamlit"]
 podcast = ["gTTS"]
```

### Comparing `biochatter-0.1.5/setup.py` & `biochatter-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 ['langchain>=0.0.146,<0.0.147',
  'nltk>=3.8.1,<4.0.0',
  'openai>=0.27.8,<0.28.0',
  'pymilvus==2.2.8',
  'pymupdf>=1.22.3,<2.0.0',
  'redis>=4.5.5,<5.0.0',
  'retry>=0.9.2,<0.10.0',
- 'tiktoken>=0.4.0,<0.5.0']
+ 'tiktoken>=0.4.0,<0.5.0',
+ 'transformers>=4.30.2,<5.0.0']
 
 extras_require = \
 {'podcast': ['gTTS>=2.3.2,<3.0.0'], 'streamlit': ['streamlit>=1.23.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'biochatter',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Backend library for conversational AI in biomedicine',
     'long_description': '# biochatter\nThis repository contains the `biochatter` Python package, a generic backend library for the connection of biomedical applications to conversational AI. Used in [ChatGSE](https://chat.biocypher.org), which is being developed at https://github.com/biocypher/ChatGSE. More to come, so stay tuned!\n\n## Installation\nTo use the package, install it from PyPI, for instance using pip (`pip install biochatter`) or Poetry (`poetry add biochatter`).\n',
     'author': 'Sebastian Lobentanzer',
     'author_email': 'sebastian.lobentanzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `biochatter-0.1.5/PKG-INFO` & `biochatter-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biochatter
-Version: 0.1.5
+Version: 0.1.6
 Summary: Backend library for conversational AI in biomedicine
 License: MIT
 Author: Sebastian Lobentanzer
 Author-email: sebastian.lobentanzer@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pymilvus (==2.2.8)
 Requires-Dist: pymupdf (>=1.22.3,<2.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: streamlit (>=1.23.1,<2.0.0); extra == "streamlit"
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # biochatter
 This repository contains the `biochatter` Python package, a generic backend library for the connection of biomedical applications to conversational AI. Used in [ChatGSE](https://chat.biocypher.org), which is being developed at https://github.com/biocypher/ChatGSE. More to come, so stay tuned!
 
 ## Installation
 To use the package, install it from PyPI, for instance using pip (`pip install biochatter`) or Poetry (`poetry add biochatter`).
```

