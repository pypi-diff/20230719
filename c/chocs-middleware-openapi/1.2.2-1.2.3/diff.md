# Comparing `tmp/chocs_middleware_openapi-1.2.2.tar.gz` & `tmp/chocs_middleware_openapi-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chocs_middleware_openapi-1.2.2.tar", max compression
+gzip compressed data, was "chocs_middleware_openapi-1.2.3.tar", max compression
```

## Comparing `chocs_middleware_openapi-1.2.2.tar` & `chocs_middleware_openapi-1.2.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-02-24 15:08:21.110437 chocs_middleware_openapi-1.2.2/LICENSE
--rw-r--r--   0        0        0     4812 2023-02-24 15:08:21.110437 chocs_middleware_openapi-1.2.2/README.md
--rw-r--r--   0        0        0       42 2023-02-24 15:08:21.110437 chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/__init__.py
--rw-r--r--   0        0        0     1108 2023-02-24 15:08:21.110437 chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/error.py
--rw-r--r--   0        0        0     4407 2023-02-24 15:08:21.110437 chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/middleware.py
--rw-r--r--   0        0        0     3923 2023-02-24 15:08:21.114436 chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/validators.py
--rw-r--r--   0        0        0     1211 2023-02-24 15:08:21.114436 chocs_middleware_openapi-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 chocs_middleware_openapi-1.2.2/setup.py
--rw-r--r--   0        0        0     6162 1970-01-01 00:00:00.000000 chocs_middleware_openapi-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/LICENSE
+-rw-r--r--   0        0        0     4812 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/README.md
+-rw-r--r--   0        0        0       42 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/__init__.py
+-rw-r--r--   0        0        0     1108 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/error.py
+-rw-r--r--   0        0        0     4407 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/middleware.py
+-rw-r--r--   0        0        0     3923 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/validators.py
+-rw-r--r--   0        0        0     1212 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 chocs_middleware_openapi-1.2.3/PKG-INFO
```

### Comparing `chocs_middleware_openapi-1.2.2/LICENSE` & `chocs_middleware_openapi-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.2/README.md` & `chocs_middleware_openapi-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/error.py` & `chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/error.py`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/middleware.py` & `chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.2/chocs_middleware/openapi/validators.py` & `chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/validators.py`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.2/pyproject.toml` & `chocs_middleware_openapi-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chocs_middleware.openapi"
-version = "1.2.2"
+version = "1.2.3"
 description = "Middleware to validate incoming requests with openapi spec."
 authors = [
     "Dawid Kraczkowski <dawid.kraczkowski@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 packages = [
@@ -28,15 +28,16 @@
     "Topic :: Utilities",
 ]
 
 # Requirements
 [tool.poetry.dependencies]
 python = "^3.8"
 chocs = "^1.6.1"
-opyapi = "^1.3.2"
+opyapi = "^1.3.3"
+
 
 [tool.poetry.dev-dependencies]
 pytest = "^4.1.0"
 pytest-cov = "^2.5"
 pytest-mock = "^1.9"
 black = "^22.10.0"
 isort = "^5.6.4"
```

### Comparing `chocs_middleware_openapi-1.2.2/setup.py` & `chocs_middleware_openapi-1.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,161 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: chocs-middleware-openapi
+Version: 1.2.3
+Summary: Middleware to validate incoming requests with openapi spec.
+Home-page: https://github.com/kodemore/chocs-openapi
+License: MIT
+Keywords: openapi,json-schema,chocs,http,middleware
+Author: Dawid Kraczkowski
+Author-email: dawid.kraczkowski@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Dist: chocs (>=1.6.1,<2.0.0)
+Requires-Dist: opyapi (>=1.3.3,<2.0.0)
+Project-URL: Documentation, https://github.com/kodemore/chocs-openapi
+Project-URL: Repository, https://github.com/kodemore/chocs-openapi
+Description-Content-Type: text/markdown
+
+# Chocs-OpenApi <br> [![PyPI version](https://badge.fury.io/py/chocs-middleware.openapi.svg)](https://pypi.org/project/chocs-middleware.openapi/) [![CI](https://github.com/kodemore/chocs-openapi/actions/workflows/main.yaml/badge.svg)](https://github.com/kodemore/chocs-openapi/actions/workflows/main.yaml) [![Release](https://github.com/kodemore/chocs-openapi/actions/workflows/release.yml/badge.svg)](https://github.com/kodemore/chocs-openapi/actions/workflows/release.yml) [![codecov](https://codecov.io/gh/kodemore/chocs-openapi/branch/main/graph/badge.svg?token=GWMTNY5G0N)](https://codecov.io/gh/kodemore/chocs-openapi) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+OpenApi middleware for chocs library.
+
+Newest OpenAPI Specification (v.3.x) can be easily integrated into Chocs through application's middleware. 
+Validation is performed via [JsonSchema Draft-7.0 specification](https://json-schema.org) and all commonly 
+used features are supported.
+
+## Features
+
+Open api integration can be used to:
+- validate request's body
+- validate request's path parameters
+- validate request's headers
+- validate request's query parameters
+- validate request's cookies  
+- generate dtos from openapi file
+
+## Installation
+
+With pip,
+```shell
+pip install chocs-middleware.openapi
+```
+or through poetry
+```shell
+poetry add chocs-middleware.openapi
+```
+
+# Usage
+
+## Using your OpenAPI file
+
+Chocs can read json and yaml files, this example will cover yaml usage although the only difference is the file extension.
+
+```python
+import chocs
+from chocs_middleware.openapi import OpenApiMiddleware
+from os import path
+
+# absolute path to file containing open api documentation; yaml and json files are supported
+openapi_filename = path.join(path.dirname(__file__), "/openapi.yml")
+
+# instantiating application and passing open api middleware
+app = chocs.Application(OpenApiMiddleware(openapi_filename, validate_body=True, validate_query=True))
+
+# the registered route must correspond to open api route within `path` section.
+# if request body is invalid the registered controller will not be invoked
+@app.post("/pets")
+def create_pet(request: chocs.HttpRequest) -> chocs.HttpResponse:
+  ...
+  return chocs.HttpResponse(status=200)
+```
+Complete integration example can be [found here](./examples/input_validation_with_open_api/openapi.yml)
+
+> Keep in mind registered route has to match 1:1 the specified route inside `paths` section inside your OpenApi documentation
+
+## Validating request body
+
+Below is very simple schema to validate request body of a `POST /pet` request. Request body is required, should be valid json request and contain the following properties:
+- name (string)
+- tags (array of string)
+- id (optional string)
+
+`openapi.yml`
+```yaml
+openapi: "3.0.0"
+info:
+  version: "1.0.0"
+  title: "Pet Store"
+paths:
+  /pets:
+    post:
+      description: Creates a new Pet
+      requestBody:
+        description: Pet
+        required: true
+        content:
+          application/json:
+            schema:
+              $ref: "#/components/schemas/Pet"
+      responses:
+        200:
+          description: "Success"
+components:
+  schemas:
+    Pet:
+      type: object
+      required:
+        - name
+        - tag
+      properties:
+        id:
+          type: integer
+        name:
+          type: string
+        tag:
+          type: array
+          items:
+            type: string
+```
+
+`app.py`
+```python
+import chocs
+from chocs_middleware.openapi import OpenApiMiddleware
+from os import path
+
+openapi_filename = path.join(path.dirname(__file__), "/openapi.yml")
+app = chocs.Application(OpenApiMiddleware(openapi_filename, validate_body=True))
+
+@app.post("/pets")
+def create_pet(request: chocs.HttpRequest) -> chocs.HttpResponse:
+  pet = request.parsed_body # here we will get valid pet
+  return chocs.HttpResponse(status=200)
+
+chocs.serve(app)
+```
+
+`create_pet` controller will be only invoked if request contains valid body. Pet's data can be accessed through `request.parsed_body` which is a dict-like object.
+
+## Json schema support
+
+Chocs uses JSON Schema to validate your open api definitions with full draft-7 support and almost complete 2019-09 standard support. 
+This means you can use almost every feature described on the [understanding json schema](https://json-schema.org/understanding-json-schema/reference/index.html) webpage. 
+The webpage is a great resource full of examples and detailed descriptions around JSON Schema. 
+
+
+> There are some caveats around `allOf` validator:
+> - all object schemas inside `allOf` definition are automatically composed into a single object definition
+> - when combining string validators make sure format validator is the last validator in the pipeline otherwise validation might fail due to string casting
 
-packages = \
-['chocs_middleware', 'chocs_middleware.openapi']
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['chocs>=1.6.1,<2.0.0', 'opyapi>=1.3.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'chocs-middleware-openapi',
-    'version': '1.2.2',
-    'description': 'Middleware to validate incoming requests with openapi spec.',
-    'long_description': '# Chocs-OpenApi <br> [![PyPI version](https://badge.fury.io/py/chocs-middleware.openapi.svg)](https://pypi.org/project/chocs-middleware.openapi/) [![CI](https://github.com/kodemore/chocs-openapi/actions/workflows/main.yaml/badge.svg)](https://github.com/kodemore/chocs-openapi/actions/workflows/main.yaml) [![Release](https://github.com/kodemore/chocs-openapi/actions/workflows/release.yml/badge.svg)](https://github.com/kodemore/chocs-openapi/actions/workflows/release.yml) [![codecov](https://codecov.io/gh/kodemore/chocs-openapi/branch/main/graph/badge.svg?token=GWMTNY5G0N)](https://codecov.io/gh/kodemore/chocs-openapi) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\nOpenApi middleware for chocs library.\n\nNewest OpenAPI Specification (v.3.x) can be easily integrated into Chocs through application\'s middleware. \nValidation is performed via [JsonSchema Draft-7.0 specification](https://json-schema.org) and all commonly \nused features are supported.\n\n## Features\n\nOpen api integration can be used to:\n- validate request\'s body\n- validate request\'s path parameters\n- validate request\'s headers\n- validate request\'s query parameters\n- validate request\'s cookies  \n- generate dtos from openapi file\n\n## Installation\n\nWith pip,\n```shell\npip install chocs-middleware.openapi\n```\nor through poetry\n```shell\npoetry add chocs-middleware.openapi\n```\n\n# Usage\n\n## Using your OpenAPI file\n\nChocs can read json and yaml files, this example will cover yaml usage although the only difference is the file extension.\n\n```python\nimport chocs\nfrom chocs_middleware.openapi import OpenApiMiddleware\nfrom os import path\n\n# absolute path to file containing open api documentation; yaml and json files are supported\nopenapi_filename = path.join(path.dirname(__file__), "/openapi.yml")\n\n# instantiating application and passing open api middleware\napp = chocs.Application(OpenApiMiddleware(openapi_filename, validate_body=True, validate_query=True))\n\n# the registered route must correspond to open api route within `path` section.\n# if request body is invalid the registered controller will not be invoked\n@app.post("/pets")\ndef create_pet(request: chocs.HttpRequest) -> chocs.HttpResponse:\n  ...\n  return chocs.HttpResponse(status=200)\n```\nComplete integration example can be [found here](./examples/input_validation_with_open_api/openapi.yml)\n\n> Keep in mind registered route has to match 1:1 the specified route inside `paths` section inside your OpenApi documentation\n\n## Validating request body\n\nBelow is very simple schema to validate request body of a `POST /pet` request. Request body is required, should be valid json request and contain the following properties:\n- name (string)\n- tags (array of string)\n- id (optional string)\n\n`openapi.yml`\n```yaml\nopenapi: "3.0.0"\ninfo:\n  version: "1.0.0"\n  title: "Pet Store"\npaths:\n  /pets:\n    post:\n      description: Creates a new Pet\n      requestBody:\n        description: Pet\n        required: true\n        content:\n          application/json:\n            schema:\n              $ref: "#/components/schemas/Pet"\n      responses:\n        200:\n          description: "Success"\ncomponents:\n  schemas:\n    Pet:\n      type: object\n      required:\n        - name\n        - tag\n      properties:\n        id:\n          type: integer\n        name:\n          type: string\n        tag:\n          type: array\n          items:\n            type: string\n```\n\n`app.py`\n```python\nimport chocs\nfrom chocs_middleware.openapi import OpenApiMiddleware\nfrom os import path\n\nopenapi_filename = path.join(path.dirname(__file__), "/openapi.yml")\napp = chocs.Application(OpenApiMiddleware(openapi_filename, validate_body=True))\n\n@app.post("/pets")\ndef create_pet(request: chocs.HttpRequest) -> chocs.HttpResponse:\n  pet = request.parsed_body # here we will get valid pet\n  return chocs.HttpResponse(status=200)\n\nchocs.serve(app)\n```\n\n`create_pet` controller will be only invoked if request contains valid body. Pet\'s data can be accessed through `request.parsed_body` which is a dict-like object.\n\n## Json schema support\n\nChocs uses JSON Schema to validate your open api definitions with full draft-7 support and almost complete 2019-09 standard support. \nThis means you can use almost every feature described on the [understanding json schema](https://json-schema.org/understanding-json-schema/reference/index.html) webpage. \nThe webpage is a great resource full of examples and detailed descriptions around JSON Schema. \n\n\n> There are some caveats around `allOf` validator:\n> - all object schemas inside `allOf` definition are automatically composed into a single object definition\n> - when combining string validators make sure format validator is the last validator in the pipeline otherwise validation might fail due to string casting\n\n',
-    'author': 'Dawid Kraczkowski',
-    'author_email': 'dawid.kraczkowski@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kodemore/chocs-openapi',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

