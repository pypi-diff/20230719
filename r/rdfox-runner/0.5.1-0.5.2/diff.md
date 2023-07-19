# Comparing `tmp/rdfox_runner-0.5.1.tar.gz` & `tmp/rdfox_runner-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfox_runner-0.5.1.tar", max compression
+gzip compressed data, was "rdfox_runner-0.5.2.tar", max compression
```

## Comparing `rdfox_runner-0.5.1.tar` & `rdfox_runner-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2022-09-22 22:12:50.581454 rdfox_runner-0.5.1/LICENSE
--rw-r--r--   0        0        0      704 2023-02-27 13:00:56.300119 rdfox_runner-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      626 2022-09-22 22:12:50.587333 rdfox_runner-0.5.1/src/rdfox_runner/__init__.py
--rw-r--r--   0        0        0    11122 2023-02-26 22:51:13.795239 rdfox_runner-0.5.1/src/rdfox_runner/command_runner.py
--rw-r--r--   0        0        0     8815 2023-02-23 15:56:44.278706 rdfox_runner-0.5.1/src/rdfox_runner/rdfox_endpoint.py
--rw-r--r--   0        0        0    12015 2023-02-26 22:50:50.464757 rdfox_runner-0.5.1/src/rdfox_runner/run_rdfox.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 rdfox_runner-0.5.1/setup.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 rdfox_runner-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-09-22 22:12:50.581454 rdfox_runner-0.5.2/LICENSE
+-rw-r--r--   0        0        0      720 2023-07-19 15:53:59.103582 rdfox_runner-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      626 2022-09-22 22:12:50.587333 rdfox_runner-0.5.2/src/rdfox_runner/__init__.py
+-rw-r--r--   0        0        0    11122 2023-02-26 22:51:13.795239 rdfox_runner-0.5.2/src/rdfox_runner/command_runner.py
+-rw-r--r--   0        0        0     9748 2023-07-19 15:43:57.865140 rdfox_runner-0.5.2/src/rdfox_runner/rdfox_endpoint.py
+-rw-r--r--   0        0        0    12015 2023-02-26 22:50:50.464757 rdfox_runner-0.5.2/src/rdfox_runner/run_rdfox.py
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 rdfox_runner-0.5.2/setup.py
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 rdfox_runner-0.5.2/PKG-INFO
```

### Comparing `rdfox_runner-0.5.1/LICENSE` & `rdfox_runner-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.1/pyproject.toml` & `rdfox_runner-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rdfox_runner"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Rick Lupton <mail@ricklupton.name>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 rdflib = "^5.0.0"
 importlib-metadata = {version = ">= 1.0", python = "<3.8"}
@@ -16,11 +16,12 @@
 # updating to use rdflib v6 this dependency can be removed.
 pyparsing = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 Sphinx = "^3.5.2"
 sphinx-rtd-theme = "^0.5.1"
+nox = "^2023.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rdfox_runner-0.5.1/src/rdfox_runner/__init__.py` & `rdfox_runner-0.5.2/src/rdfox_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.1/src/rdfox_runner/command_runner.py` & `rdfox_runner-0.5.2/src/rdfox_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.1/src/rdfox_runner/rdfox_endpoint.py` & `rdfox_runner-0.5.2/src/rdfox_runner/rdfox_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 import logging
 import re
 import requests
 from textwrap import indent
 from rdflib import Graph, Literal, URIRef
+from rdflib.plugins.stores.sparqlstore import SPARQLUpdateStore
 
 # Pandas is optional, but convenient if available
 try:
     import pandas as pd
 except ImportError:
     pd = None
 
@@ -45,14 +46,37 @@
         self.query = query
         self.message = message
 
     def __str__(self):
         return f"ParsingError: {self.message}"
 
 
+# This is the value before version 6.0. After version 6.0, don't pass a value
+# for the default graph at all in queries.
+#
+RDFOX_DEFAULT_GRAPH = URIRef("http://oxfordsemantic.tech/RDFox#DefaultTriples")
+
+class RDFoxSPARQLUpdateStore(SPARQLUpdateStore):
+    """Avoid passing `default-graph-uri` in SPARQL queries.
+
+    Before version 6.0 of RDFox, this parameter had to be set to the default
+    graph URI if it was present. After version 6.0 it's not clear what the
+    default graph URI is, so we just avoid passing this parameter.
+
+    """
+
+    def _query(self, *args, **kwargs):
+        """Remove the `default_graph` kwarg that is used to set the
+        `default-graph-uri` parameter."""
+        if kwargs.get("default_graph") == RDFOX_DEFAULT_GRAPH:
+            del kwargs["default_graph"]
+        return super()._query(*args, **kwargs)
+
+
+
 class RDFoxEndpoint:
     """Interface to interact with a running RDFox endpoint.
 
     :param namespaces: dict of RDFlib namespaces to bind
     """
 
     # Allow short names for mime types, copying rdflib
@@ -64,15 +88,15 @@
         'ttl': 'test/turtle',
     }
 
     def __init__(self, namespaces: Optional[Mapping] = None):
         self.namespaces = namespaces or {}
         self.server = None
         self.datastore = None
-        self.graph = Graph("SPARQLUpdateStore", identifier="http://oxfordsemantic.tech/RDFox#DefaultTriples")
+        self.graph = Graph(RDFoxSPARQLUpdateStore(), identifier=RDFOX_DEFAULT_GRAPH)  #"https://rdfox.com/vocabulary#DefaultTriples")
         for k, v in self.namespaces.items():
             self.graph.bind(k, v)
 
     def connect(self, url: str):
         """Connect to RDFox at given base URL.
 
         The SPARQL endpoint is at `{url}/datastores/default/sparql`.
```

### Comparing `rdfox_runner-0.5.1/src/rdfox_runner/run_rdfox.py` & `rdfox_runner-0.5.2/src/rdfox_runner/run_rdfox.py`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.1/setup.py` & `rdfox_runner-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'requests>=2.25.1,<3.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=1.0']}
 
 setup_kwargs = {
     'name': 'rdfox-runner',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': '',
     'long_description': 'None',
     'author': 'Rick Lupton',
     'author_email': 'mail@ricklupton.name',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdfox_runner-0.5.1/PKG-INFO` & `rdfox_runner-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfox-runner
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

