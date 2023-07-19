# Comparing `tmp/hotdag-0.6.2.tar.gz` & `tmp/hotdag-0.7.0.tar.gz`

## Comparing `hotdag-0.6.2.tar` & `hotdag-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hotdag-0.6.2/.flake8
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hotdag-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hotdag-0.6.2/dev-requirements.txt
--rw-r--r--   0        0        0    52459 2020-02-02 00:00:00.000000 hotdag-0.6.2/graph.png
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 hotdag-0.6.2/requirements.txt
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hotdag-0.6.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/__about__.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/__init__.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/dbt_cloud.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/dbt_core.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/main.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/manifest.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/renderer.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/test_main.http
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/server/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/server/server.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/server/routers/__init__.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/server/routers/cloud.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/server/routers/manifest.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hotdag-0.6.2/hotdag/server/routers/url.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hotdag-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hotdag-0.6.2/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hotdag-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 hotdag-0.6.2/README.md
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 hotdag-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 hotdag-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hotdag-0.7.0/.flake8
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hotdag-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 hotdag-0.7.0/dev-requirements.txt
+-rw-r--r--   0        0        0    52459 2020-02-02 00:00:00.000000 hotdag-0.7.0/graph.png
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 hotdag-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hotdag-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/__about__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/__init__.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/dbt_cloud.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/dbt_core.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/main.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/manifest.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/renderer.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/test_main.http
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/server/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/server/server.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/server/routers/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/server/routers/cloud.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/server/routers/manifest.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hotdag-0.7.0/hotdag/server/routers/url.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hotdag-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hotdag-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hotdag-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 hotdag-0.7.0/README.md
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 hotdag-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 hotdag-0.7.0/PKG-INFO
```

### Comparing `hotdag-0.6.2/.pre-commit-config.yaml` & `hotdag-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/dev-requirements.txt` & `hotdag-0.7.0/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,92 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
+#    pip-compile
 #
 agate==1.7.0
     # via dbt-core
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 babel==2.12.1
     # via agate
-betterproto==1.2.5
-    # via dbt-core
-black==23.1.0
-    # via hotdag (pyproject.toml)
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via dbt-core
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
-    # via
-    #   black
-    #   dbt-core
+    # via dbt-core
 colorama==0.4.6
     # via dbt-core
-dbt-core==1.4.5
+dbt-core==1.5.3
     # via hotdag (pyproject.toml)
 dbt-extractor==0.4.1
     # via dbt-core
 fastapi==0.95.0
     # via hotdag (pyproject.toml)
-flake8==6.0.0
-    # via hotdag (pyproject.toml)
 future==0.18.3
     # via parsedatetime
 graphviz==0.20.1
     # via hotdag (pyproject.toml)
-grpclib==0.4.3
-    # via betterproto
-h2==4.1.0
-    # via grpclib
 hologram==0.0.15
     # via dbt-core
-hpack==4.0.0
-    # via h2
-hyperframe==6.0.1
-    # via h2
 idna==3.4
     # via
     #   anyio
     #   dbt-core
     #   requests
-iniconfig==2.0.0
-    # via pytest
 isodate==0.6.1
     # via
     #   agate
     #   dbt-core
-isort==5.12.0
-    # via hotdag (pyproject.toml)
 jinja2==3.1.2
     # via dbt-core
 jsonschema==3.2.0
     # via hologram
 leather==0.3.4
     # via agate
 logbook==1.5.3
     # via dbt-core
 loguru==0.6.0
     # via hotdag (pyproject.toml)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
-mashumaro[msgpack]==3.3.1
+mashumaro[msgpack]==3.6
     # via dbt-core
-mccabe==0.7.0
-    # via flake8
 minimal-snowplow-tracker==0.0.2
     # via dbt-core
 msgpack==1.0.5
     # via mashumaro
-multidict==6.0.4
-    # via grpclib
-mypy-extensions==1.0.0
-    # via black
 networkx==2.8.8
     # via dbt-core
 packaging==23.0
-    # via
-    #   black
-    #   dbt-core
-    #   pytest
+    # via dbt-core
 parsedatetime==2.4
     # via agate
 pathspec==0.10.3
-    # via
-    #   black
-    #   dbt-core
-platformdirs==3.2.0
-    # via black
-pluggy==1.0.0
-    # via pytest
-pycodestyle==2.10.0
-    # via flake8
+    # via dbt-core
+protobuf==4.23.4
+    # via dbt-core
 pycparser==2.21
     # via cffi
 pydantic==1.10.7
     # via fastapi
 pydot==1.4.2
     # via hotdag (pyproject.toml)
-pyflakes==3.0.1
-    # via flake8
 pyparsing==3.0.9
     # via pydot
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
-    # via hotdag (pyproject.toml)
 python-dateutil==2.8.2
     # via hologram
 python-slugify==8.0.1
     # via agate
 pytimeparse==1.1.8
     # via agate
 pytz==2023.2
@@ -148,16 +107,14 @@
     #   python-dateutil
 sniffio==1.3.0
     # via anyio
 sqlparse==0.4.3
     # via dbt-core
 starlette==0.26.1
     # via fastapi
-stringcase==1.2.0
-    # via betterproto
 text-unidecode==1.3
     # via python-slugify
 typing-extensions==4.5.0
     # via
     #   dbt-core
     #   mashumaro
     #   pydantic
```

### Comparing `hotdag-0.6.2/graph.png` & `hotdag-0.7.0/graph.png`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/.github/workflows/test.yml` & `hotdag-0.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/__init__.py` & `hotdag-0.7.0/hotdag/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,25 +69,26 @@
 
         if select is None:
             select = "+*+"
 
         # Generate selector from string
         selector_definition = self.string_to_definition(selection=select)
 
-        exclusion_definition = None
+        complete_spec = None
         if exclude:
             exclusion_definition = self.string_to_definition(selection=exclude)
+            complete_spec = SelectionDifference(
+                [selector_definition, exclusion_definition]
+            )
 
         # Generate subgraph
         node_selector = NodeSelector(graph=self.graph, manifest=self.manifest)
 
         direct_nodes, indirect_nodes = node_selector.select_nodes(
-            SelectionDifference([selector_definition, exclusion_definition])
-            if exclusion_definition
-            else selector_definition
+            complete_spec if complete_spec else selector_definition
         )
 
         return direct_nodes
 
     def render(self, selected_nodes: Set[UniqueId], **kwargs) -> str:
         """Render the selection using the provided Renderer."""
         return self.renderer.render(
```

### Comparing `hotdag-0.6.2/hotdag/dbt_cloud.py` & `hotdag-0.7.0/hotdag/dbt_cloud.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/dbt_core.py` & `hotdag-0.7.0/hotdag/dbt_core.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/main.py` & `hotdag-0.7.0/hotdag/main.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/manifest.py` & `hotdag-0.7.0/hotdag/manifest.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/server/routers/cloud.py` & `hotdag-0.7.0/hotdag/server/routers/cloud.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/server/routers/manifest.py` & `hotdag-0.7.0/hotdag/server/routers/manifest.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/hotdag/server/routers/url.py` & `hotdag-0.7.0/hotdag/server/routers/url.py`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/LICENSE.txt` & `hotdag-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/README.md` & `hotdag-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hotdag-0.6.2/pyproject.toml` & `hotdag-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   'fastapi',
-  'dbt-core~=1.4',
+  'dbt-core~=1.5',
   'loguru',
   'pydot',
   'graphviz',
   'requests'
 ]
 dynamic = ["version"]
 
@@ -109,15 +109,15 @@
   "black .",
   "check",
 ]
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.2"
+version = "0.7.0"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "hotdag/__about__.py",
     "pyproject.toml:version"
 ]
```

### Comparing `hotdag-0.6.2/PKG-INFO` & `hotdag-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotdag
-Version: 0.6.2
+Version: 0.7.0
 Summary: Hot evaluation of dbt DAG selectors
 Project-URL: Documentation, https://github.com/nicholasyager/hotdag#readme
 Project-URL: Issues, https://github.com/nicholasyager/hotdag/issues
 Project-URL: Source, https://github.com/nicholasyager/hotdag
 Author-email: Nicholas Yager <yager@nicholasyager.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: dbt-core~=1.4
+Requires-Dist: dbt-core~=1.5
 Requires-Dist: fastapi
 Requires-Dist: graphviz
 Requires-Dist: loguru
 Requires-Dist: pydot
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
```

