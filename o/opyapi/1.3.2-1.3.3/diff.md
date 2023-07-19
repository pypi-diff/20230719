# Comparing `tmp/opyapi-1.3.2.tar.gz` & `tmp/opyapi-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyapi-1.3.2.tar", max compression
+gzip compressed data, was "opyapi-1.3.3.tar", max compression
```

## Comparing `opyapi-1.3.2.tar` & `opyapi-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1065 2023-02-03 14:10:49.560292 opyapi-1.3.2/LICENSE
--rw-r--r--   0        0        0    13038 2023-02-03 14:10:49.560292 opyapi-1.3.2/README.md
--rw-r--r--   0        0        0      623 2023-02-03 14:10:49.560292 opyapi-1.3.2/opyapi/__init__.py
--rw-r--r--   0        0        0       22 2023-02-03 14:10:49.560292 opyapi-1.3.2/opyapi/__version__.py
--rw-r--r--   0        0        0      150 2023-02-03 14:10:49.560292 opyapi-1.3.2/opyapi/_yaml_support.py
--rw-r--r--   0        0        0      326 2023-02-03 14:10:49.560292 opyapi-1.3.2/opyapi/console/application.py
--rw-r--r--   0        0        0     4587 2023-02-03 14:10:49.560292 opyapi-1.3.2/opyapi/console/dto_generator/generator.py
--rw-r--r--   0        0        0     5570 2023-02-03 14:10:49.560292 opyapi-1.3.2/opyapi/console/dto_generator/processor.py
--rw-r--r--   0        0        0     2188 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/console/generate_dto.py
--rw-r--r--   0        0        0     5050 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/errors.py
--rw-r--r--   0        0        0    13982 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/json_schema.py
--rw-r--r--   0        0        0    13558 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/schema_validator.py
--rw-r--r--   0        0        0     2525 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/string_format.py
--rw-r--r--   0        0        0     3713 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/__init__.py
--rw-r--r--   0        0        0     3542 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/array_validators.py
--rw-r--r--   0        0        0     1898 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/combining_validators.py
--rw-r--r--   0        0        0     6660 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/format_validators.py
--rw-r--r--   0        0        0     3009 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/number_validators.py
--rw-r--r--   0        0        0     4036 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/object_validators.py
--rw-r--r--   0        0        0     1807 2023-02-03 14:10:49.564292 opyapi-1.3.2/opyapi/validators/string_validators.py
--rw-r--r--   0        0        0     1179 2023-02-03 14:10:49.564292 opyapi-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    14380 1970-01-01 00:00:00.000000 opyapi-1.3.2/setup.py
--rw-r--r--   0        0        0    14337 1970-01-01 00:00:00.000000 opyapi-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-19 13:44:24.905453 opyapi-1.3.3/LICENSE
+-rw-r--r--   0        0        0    13038 2023-07-19 13:44:24.905453 opyapi-1.3.3/README.md
+-rw-r--r--   0        0        0      623 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/__version__.py
+-rw-r--r--   0        0        0      150 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/_yaml_support.py
+-rw-r--r--   0        0        0      326 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/console/application.py
+-rw-r--r--   0        0        0     4587 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/console/dto_generator/generator.py
+-rw-r--r--   0        0        0     5570 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/console/dto_generator/processor.py
+-rw-r--r--   0        0        0     2188 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/console/generate_dto.py
+-rw-r--r--   0        0        0     5050 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/errors.py
+-rw-r--r--   0        0        0    13982 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/json_schema.py
+-rw-r--r--   0        0        0    13558 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/schema_validator.py
+-rw-r--r--   0        0        0     2525 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/string_format.py
+-rw-r--r--   0        0        0     3713 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/__init__.py
+-rw-r--r--   0        0        0     3542 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/array_validators.py
+-rw-r--r--   0        0        0     1898 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/combining_validators.py
+-rw-r--r--   0        0        0     6660 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/format_validators.py
+-rw-r--r--   0        0        0     3009 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/number_validators.py
+-rw-r--r--   0        0        0     4036 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/object_validators.py
+-rw-r--r--   0        0        0     1807 2023-07-19 13:44:24.909453 opyapi-1.3.3/opyapi/validators/string_validators.py
+-rw-r--r--   0        0        0     1179 2023-07-19 13:44:24.909453 opyapi-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    14237 1970-01-01 00:00:00.000000 opyapi-1.3.3/PKG-INFO
```

### Comparing `opyapi-1.3.2/LICENSE` & `opyapi-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/README.md` & `opyapi-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/__init__.py` & `opyapi-1.3.3/opyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/console/dto_generator/generator.py` & `opyapi-1.3.3/opyapi/console/dto_generator/generator.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/console/dto_generator/processor.py` & `opyapi-1.3.3/opyapi/console/dto_generator/processor.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/console/generate_dto.py` & `opyapi-1.3.3/opyapi/console/generate_dto.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/errors.py` & `opyapi-1.3.3/opyapi/errors.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/json_schema.py` & `opyapi-1.3.3/opyapi/json_schema.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/schema_validator.py` & `opyapi-1.3.3/opyapi/schema_validator.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/string_format.py` & `opyapi-1.3.3/opyapi/string_format.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/__init__.py` & `opyapi-1.3.3/opyapi/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/array_validators.py` & `opyapi-1.3.3/opyapi/validators/array_validators.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/combining_validators.py` & `opyapi-1.3.3/opyapi/validators/combining_validators.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/format_validators.py` & `opyapi-1.3.3/opyapi/validators/format_validators.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/number_validators.py` & `opyapi-1.3.3/opyapi/validators/number_validators.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/object_validators.py` & `opyapi-1.3.3/opyapi/validators/object_validators.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/opyapi/validators/string_validators.py` & `opyapi-1.3.3/opyapi/validators/string_validators.py`

 * *Files identical despite different names*

### Comparing `opyapi-1.3.2/pyproject.toml` & `opyapi-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opyapi"
-version = "1.3.2"
+version = "1.3.3"
 description = "JsonSchem and OpenAPI tools for python."
 authors = [
     "Dawid Kraczkowski <dawid.kraczkowski@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kodemore/opyapi"
@@ -24,15 +24,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
 # Requirements
 [tool.poetry.dependencies]
 python = "^3.8"
-pyyaml = "^5.4.1"
+pyyaml = "^6.0.1"
 cleo = "^2.0.1"
 
 [tool.poetry.scripts]
 opyapi="opyapi.console.application:main"
 
 [tool.poetry.dev-dependencies]
 pytest = "^4.1.0"
```

### Comparing `opyapi-1.3.2/setup.py` & `opyapi-1.3.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,487 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: opyapi
+Version: 1.3.3
+Summary: JsonSchem and OpenAPI tools for python.
+Home-page: https://github.com/kodemore/opyapi
+License: MIT
+Keywords: JsonSchema,OpenAPI,validation,json,schema,rest,api
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
+Requires-Dist: cleo (>=2.0.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Project-URL: Documentation, https://github.com/kodemore/opyapi
+Project-URL: Repository, https://github.com/kodemore/opyapi
+Description-Content-Type: text/markdown
 
-packages = \
-['opyapi',
- 'opyapi.console',
- 'opyapi.console.dto_generator',
- 'opyapi.validators']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cleo>=2.0.1,<3.0.0', 'pyyaml>=5.4.1,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['opyapi = opyapi.console.application:main']}
-
-setup_kwargs = {
-    'name': 'opyapi',
-    'version': '1.3.2',
-    'description': 'JsonSchem and OpenAPI tools for python.',
-    'long_description': '# OpyAPI - JsonSchema and OpenAPI tools for python <br> [![CI](https://github.com/kodemore/opyapi/actions/workflows/main.yaml/badge.svg)](https://github.com/kodemore/opyapi/actions/workflows/main.yaml) [![Release](https://github.com/kodemore/opyapi/actions/workflows/release.yml/badge.svg)](https://github.com/kodemore/opyapi/actions/workflows/release.yml) [![codecov](https://codecov.io/gh/kodemore/opyapi/branch/main/graph/badge.svg?token=KWFTWSKPKJ)](https://codecov.io/gh/kodemore/opyapi) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\nJsonSchema and OpenAPI tools for python.\n\n## Features\n- Validation builder for json schema\n- Custom string formatters support\n- Full JsonSchema draft-7 support\n- Support for JsonReferences, $anchor\n- Dataclass generation from OpenAPI schema\n- Great performance\n\n## Installation\n\nWith pip,\n```shell\npip install opyapi\n```\nor through poetry\n```shell\npoetry add opyapi\n```\n\n# Usage\n\n> It is recommended to get familiar with json-schema if you haven\'t yet. \n> [Understanding Json Schema](https://json-schema.org/understanding-json-schema/index.html) is a great place to start and learn Json Schema\'s basics\n## Simple usage\nLibrary can be used to validate data, against defined json-schema like so:\n\n```python\nfrom opyapi import validate\n\nassert validate(\n    {"name": "Test", "age":12}, \n    {\n        "type": "object",\n        "properties": {\n            "name": {\n                "type": "string",\n            },\n            "age": {\n              "type": "integer",  \n            }\n        }\n    }\n)\n```\n\n## Using references\nValidating documents against complex schemas is also possible,\nplease consider the following example with json references:\n\n```python\nfrom opyapi import validate\n\nschema = {\n    "type": "object",\n    "properties": {\n        "name": {\n            "type": "string",\n            "minLength": 2,\n        },\n        "email": {\n            "$ref": "#/$defs/email"\n        }\n    },\n    "$defs": {\n        "email": {\n            "type": "string",\n            "format": "email"\n        }\n    }\n}\n\nvalidate({"name": "Bob", "email": "bob@test.com"}, schema)\n```\n\n## Custom string formats support\n\n```python\nfrom opyapi import StringFormat, validate\nimport re\n\ndef my_format_validator(value: str) -> str:\n    if re.match("^my-", value):\n        return value\n    raise ValueError(f"Could not validate {value}")\n\nStringFormat["my-format"] = my_format_validator\n\nvalidate("my-test", {"type": "string", "format": "my-format"})  # passes\nvalidate("test", {"type": "string", "format": "my-format"})  # fails\n```\n\n> In the above example `opyapi.StringFormat` is used to register new custom format,\n> which is recognised during validation.\n\n## Re-using validators\n\nThere are scenarios where same validator should be used multiple times,\nin these scenarios to improve performance it is better to use `build_validator_for` \nwhich returns a validator function for the passed schema:\n\n```python\nfrom opyapi import build_validator_for\n\nmy_validator = build_validator_for({\n    "type": "object",\n    "properties": {\n        "name": {\n            "type": "string",\n            "minLength": 2,\n        },\n        "email": {\n            "type": "string",\n            "format": "email",\n        }\n    },\n})\n\nassert my_validator({"name": "Bob", "email": "bob@email.com"})\n```\n\n## Catching errors\n\n`opyapi` provides versatile error package, which is really simple to use. You are only required to define try/except \nblock within you can catch one of the errors defined in the package depending on your scenario.\n\n```python\nfrom opyapi import build_validator_for\nfrom opyapi.errors import ValidationError\n\nmy_validator = build_validator_for({\n    "type": "object",\n    "properties": {\n        "name": {\n            "type": "string",\n            "minLength": 2,\n        },\n        "email": {\n            "type": "string",\n            "format": "email",\n        }\n    },\n})\n\ntry:\n    my_validator({"name": "Bob", "email": "invalid"})\nexcept ValidationError as e:\n    print(f"Validation failed from the reason: {e}")\n\n```\n\n### Errors structure\n\nThe following graph represents exception used in `opyapi`. \nAll exceptions are part of `opyapi.errors` module.\n\n```\nValueError\n    ┗━ ValidationError\n            ┣━ TypeValidationError\n            ┣━ EnumValidationError\n            ┣━ FormatValidationError\n            ┣━ ItemsValidationError\n            ┃           ┣━ UniqueItemsValidationError\n            ┃           ┣━ AdditionalItemsValidationError\n            ┃           ┣━ MinimumItemsValidationError\n            ┃           ┗━ MaximumItemsValidationError\n            ┣━ MultipleOfValidationError\n            ┣━ ComparisonValidationError\n            ┃           ┣━ EqualityValidationError\n            ┃           ┗━ RangeValidationError\n            ┃                       ┣━ MinimumValidationError\n            ┃                       ┣━ MaximumValidationError\n            ┃                       ┣━ ExclusiveMinimumValidationError\n            ┃                       ┗━ ExclusiveMaximumValidationError\n            ┗━ ObjectValidationError\n                        ┣━ PropertyValidationError\n                        ┃           ┣━ RequiredPropertyValidationError\n                        ┃           ┣━ PropertyValueValidationError\n                        ┃           ┣━ PropertyNameValidationError\n                        ┃           ┗━ AdditionalPropertiesValidationError\n                        ┣━ ObjectSizeValidationError\n                        ┃           ┣━ MinimumPropertiesValidationError\n                        ┃           ┗━ MaximumPropertiesValidationError\n                        ┗━ DependencyValidationError\n```\n\n#### `opyapi.errors.ValidationError`\nGeneric validation error.\n\n#### `opyapi.errors.TypeValidationError`\nRaised when passed type does not conform type defined in the schema.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "type": "integer"\n> }\n> ```\n\n#### `opyapi.errors.EnumValidationError`\nRaised when value does not conform enum definition.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "enum": ["integer", "string", "boolean"]\n> }\n> ```\n\n#### `opyapi.errors.FormatValidationError`\nRaised when value does not conform defined format in string schema.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "type": "string",\n>   "format": "date-time"\n> }\n> ```\n\n#### `opyapi.errors.ItemsValidationError`\nGeneric Exception raised when validation of an array fails for some reason.\n\n#### `opyapi.errors.UniqueItemsValidationError`\nRaised when items in an array are expected to be unique but passed value does not conform the requirement. \nThis exception extends generic `opyapi.errors.ItemsValidationError` exception.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "type": "array",\n>   "uniqueItems": true\n> }\n> ```\n\n#### `opyapi.errors.AdditionalItemsValidationError`\nRaised when additional items in an array either does not conform the schema or are not expected.\nThis exception extends generic `opyapi.errors.ItemsValidationError` exception.\n\n> Can be triggered by the following schema:\n> ```json\n> {\n>   "type": "array",\n>   "items": [\n>     {"type": "string"},\n>     {"type":  "integer"}        \n>   ],\n>   "additionalItems": false\n> }\n> ```\n\n#### `opyapi.errors.MinimumItemsValidationError`, `opyapi.errors.MaximumItemsValidationError`\nRaised when number of items in an array does not conform maximum or minimum items specified in schema.\nThis exception extends generic `opyapi.errors.ItemsValidationError` exception.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "type": "array",\n>   "minimumItems": 2,\n>   "MaximumItems": 10\n> }\n> ```\n\n\n#### `opyapi.errors.MultipleOfValidationError`\nRaised when validated number is not multiplication of passed value.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "type": "numerical",\n>   "multipleOf": 2\n> }\n> ```\n\n#### `opyapi.errors.ComparisonValidationError`\nRaised when comparison operation fails. This is a generic exception used by other comparison errors.\n\n#### `opyapi.errors.EqualityValidationError`\nRaised when validated value is not the same as defined expected value. This exception extends `opyapi.errors.ComparisonValidationError`.\n\n> Can be triggered by following example schema:\n> ```json\n> {\n>   "const": "test"\n> }\n> ```\n\n#### `opyapi.errors.RangeValidationError`\nRaised when (exclusive) minimum, (exclusive) maximum comparisons fail. This exception extends `opyapi.errors.ComparisonValidationError`.\n\n#### `opyapi.errors.MinimumValidationError`, `opyapi.errors.MaximumValidationError`, `opyapi.errors.ExclusiveMinimumValidationError`, `opyapi.errors.ExclusiveMaximumValidationError`\nRaised when passed numerical (or integer) value is not within expected range defined in schema.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "numerical",\n>   "minimum": 2\n> }\n> ```\n\n\n#### `opyapi.errors.ObjectValidationError`\nGeneric exception raised when validation of an object fails for some reason.\n\n#### `opyapi.errors.PropertyValidationError`\nGeneric exception raised when validation of object\'s property fails for some reason. \nThis exception extends `opyapi.errors.ObjectValidationError` exception.\n\n#### `opyapi.errors.RequiredPropertyValidationError`\nRaised when required property is not present in passed object.\nThis exception extends `opyapi.errors.PropertyValidationError` exception.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "object",\n>   "properties": {\n>     "name" : {"type": "string"}\n>   },\n>   "required": ["name"]\n> }\n> ```\n\n#### `opyapi.errors.PropertyValueValidationError`\nRaised when property contains invalid value. \nThis exception extends `opyapi.errors.PropertyValidationError` exception.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "object",\n>   "properties": {\n>     "name" : {"type": "string"}\n>   }\n> }\n> ```\n\n#### `opyapi.errors.PropertyNameValidationError`\nRaised when property\'s names does not conform defined schema. \nThis exception extends `opyapi.errors.PropertyValidationError` exception.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "object",\n>   "properties": {\n>     "name" : {"type": "string"}\n>   },\n>   "propertyNames": {\n>     "pattern": "^x-" \n>   }\n> }\n> ```\n\n#### `opyapi.errors.AdditionalPropertiesValidationError`\nRaised when additional properties are not allowed or set schema is not followed. \nThis exception extends `opyapi.errors.PropertyValidationError` exception.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "object",\n>   "properties": {\n>     "name" : {"type": "string"}\n>   },\n>   "additionalProperties": false\n> }\n> ```\n\n#### `opyapi.errors.ObjectSizeValidationError`\nGeneric exception raised when number of properties does not conform defined schema. \nThis exception extends `opyapi.errors.ObjectValidationError` exception.\n\n#### `opyapi.errors.MinimumPropertiesValidationError`, `opyapi.errors.MaximumPropertiesValidationError`\nGeneric exception raised when number of properties does not conform defined schema. \nThese exceptions extend `opyapi.errors.ObjectSizeValidationError`exception.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "object",\n>   "properties": {\n>     "name" : {"type": "string"}\n>   },\n>   "minProperties": 2,\n>   "maxProperties": 10\n> }\n> ```\n\n#### `opyapi.errors.DependencyValidationError`\n\nRaised when dependent properties are defined in the schema but not provided in a passed object. \nThis exception extends `opyapi.errors.ObjectValidationError` exception.\n\n> Can be triggered by the following example schema:\n> ```json\n> {\n>   "type": "object",\n>   "properties": {\n>     "name" : {"type": "string"}\n>   },\n>   "dependentRequired": {\n>     "name": ["first_name", "last_name"]\n>   }\n> }\n> ```\n\n## API\n\n### `validate(obj: typing.Any, schema: typing.Union[dict, opyapi.JsonSchema]): typing.Any`\n\nValidates passed object `obj`, and if valid returns the object, otherwise raises a `ValueError` exception.\n\n```python\nfrom opyapi import validate\n\nassert validate(\n    {"name": "Test", "age":12}, \n    {\n        "type": "object",\n        "properties": {\n            "name": {\n                "type": "string",\n            },\n            "age": {\n              "type": "integer",  \n            }\n        }\n    }\n)\n```\n\n### `build_validator_for(schema: typing.Union[dict, JsonSchema]) -> Callable`\n\nCreates validator function for passed json schema and returns it as a result.\n\n```python\nfrom opyapi import build_validator_for\n\nvalidator =  build_validator_for({\n    "type": "object",\n    "properties": {\n        "name": {\n            "type": "string",\n        },\n        "age": {\n          "type": "integer",  \n        }\n    }\n})\n```\n',
-    'author': 'Dawid Kraczkowski',
-    'author_email': 'dawid.kraczkowski@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kodemore/opyapi',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+# OpyAPI - JsonSchema and OpenAPI tools for python <br> [![CI](https://github.com/kodemore/opyapi/actions/workflows/main.yaml/badge.svg)](https://github.com/kodemore/opyapi/actions/workflows/main.yaml) [![Release](https://github.com/kodemore/opyapi/actions/workflows/release.yml/badge.svg)](https://github.com/kodemore/opyapi/actions/workflows/release.yml) [![codecov](https://codecov.io/gh/kodemore/opyapi/branch/main/graph/badge.svg?token=KWFTWSKPKJ)](https://codecov.io/gh/kodemore/opyapi) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+JsonSchema and OpenAPI tools for python.
+
+## Features
+- Validation builder for json schema
+- Custom string formatters support
+- Full JsonSchema draft-7 support
+- Support for JsonReferences, $anchor
+- Dataclass generation from OpenAPI schema
+- Great performance
+
+## Installation
+
+With pip,
+```shell
+pip install opyapi
+```
+or through poetry
+```shell
+poetry add opyapi
+```
+
+# Usage
+
+> It is recommended to get familiar with json-schema if you haven't yet. 
+> [Understanding Json Schema](https://json-schema.org/understanding-json-schema/index.html) is a great place to start and learn Json Schema's basics
+## Simple usage
+Library can be used to validate data, against defined json-schema like so:
+
+```python
+from opyapi import validate
+
+assert validate(
+    {"name": "Test", "age":12}, 
+    {
+        "type": "object",
+        "properties": {
+            "name": {
+                "type": "string",
+            },
+            "age": {
+              "type": "integer",  
+            }
+        }
+    }
+)
+```
+
+## Using references
+Validating documents against complex schemas is also possible,
+please consider the following example with json references:
+
+```python
+from opyapi import validate
+
+schema = {
+    "type": "object",
+    "properties": {
+        "name": {
+            "type": "string",
+            "minLength": 2,
+        },
+        "email": {
+            "$ref": "#/$defs/email"
+        }
+    },
+    "$defs": {
+        "email": {
+            "type": "string",
+            "format": "email"
+        }
+    }
 }
 
+validate({"name": "Bob", "email": "bob@test.com"}, schema)
+```
+
+## Custom string formats support
+
+```python
+from opyapi import StringFormat, validate
+import re
+
+def my_format_validator(value: str) -> str:
+    if re.match("^my-", value):
+        return value
+    raise ValueError(f"Could not validate {value}")
+
+StringFormat["my-format"] = my_format_validator
+
+validate("my-test", {"type": "string", "format": "my-format"})  # passes
+validate("test", {"type": "string", "format": "my-format"})  # fails
+```
+
+> In the above example `opyapi.StringFormat` is used to register new custom format,
+> which is recognised during validation.
+
+## Re-using validators
+
+There are scenarios where same validator should be used multiple times,
+in these scenarios to improve performance it is better to use `build_validator_for` 
+which returns a validator function for the passed schema:
+
+```python
+from opyapi import build_validator_for
+
+my_validator = build_validator_for({
+    "type": "object",
+    "properties": {
+        "name": {
+            "type": "string",
+            "minLength": 2,
+        },
+        "email": {
+            "type": "string",
+            "format": "email",
+        }
+    },
+})
+
+assert my_validator({"name": "Bob", "email": "bob@email.com"})
+```
+
+## Catching errors
+
+`opyapi` provides versatile error package, which is really simple to use. You are only required to define try/except 
+block within you can catch one of the errors defined in the package depending on your scenario.
+
+```python
+from opyapi import build_validator_for
+from opyapi.errors import ValidationError
+
+my_validator = build_validator_for({
+    "type": "object",
+    "properties": {
+        "name": {
+            "type": "string",
+            "minLength": 2,
+        },
+        "email": {
+            "type": "string",
+            "format": "email",
+        }
+    },
+})
+
+try:
+    my_validator({"name": "Bob", "email": "invalid"})
+except ValidationError as e:
+    print(f"Validation failed from the reason: {e}")
+
+```
+
+### Errors structure
+
+The following graph represents exception used in `opyapi`. 
+All exceptions are part of `opyapi.errors` module.
+
+```
+ValueError
+    ┗━ ValidationError
+            ┣━ TypeValidationError
+            ┣━ EnumValidationError
+            ┣━ FormatValidationError
+            ┣━ ItemsValidationError
+            ┃           ┣━ UniqueItemsValidationError
+            ┃           ┣━ AdditionalItemsValidationError
+            ┃           ┣━ MinimumItemsValidationError
+            ┃           ┗━ MaximumItemsValidationError
+            ┣━ MultipleOfValidationError
+            ┣━ ComparisonValidationError
+            ┃           ┣━ EqualityValidationError
+            ┃           ┗━ RangeValidationError
+            ┃                       ┣━ MinimumValidationError
+            ┃                       ┣━ MaximumValidationError
+            ┃                       ┣━ ExclusiveMinimumValidationError
+            ┃                       ┗━ ExclusiveMaximumValidationError
+            ┗━ ObjectValidationError
+                        ┣━ PropertyValidationError
+                        ┃           ┣━ RequiredPropertyValidationError
+                        ┃           ┣━ PropertyValueValidationError
+                        ┃           ┣━ PropertyNameValidationError
+                        ┃           ┗━ AdditionalPropertiesValidationError
+                        ┣━ ObjectSizeValidationError
+                        ┃           ┣━ MinimumPropertiesValidationError
+                        ┃           ┗━ MaximumPropertiesValidationError
+                        ┗━ DependencyValidationError
+```
+
+#### `opyapi.errors.ValidationError`
+Generic validation error.
+
+#### `opyapi.errors.TypeValidationError`
+Raised when passed type does not conform type defined in the schema.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "type": "integer"
+> }
+> ```
+
+#### `opyapi.errors.EnumValidationError`
+Raised when value does not conform enum definition.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "enum": ["integer", "string", "boolean"]
+> }
+> ```
+
+#### `opyapi.errors.FormatValidationError`
+Raised when value does not conform defined format in string schema.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "type": "string",
+>   "format": "date-time"
+> }
+> ```
+
+#### `opyapi.errors.ItemsValidationError`
+Generic Exception raised when validation of an array fails for some reason.
+
+#### `opyapi.errors.UniqueItemsValidationError`
+Raised when items in an array are expected to be unique but passed value does not conform the requirement. 
+This exception extends generic `opyapi.errors.ItemsValidationError` exception.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "type": "array",
+>   "uniqueItems": true
+> }
+> ```
+
+#### `opyapi.errors.AdditionalItemsValidationError`
+Raised when additional items in an array either does not conform the schema or are not expected.
+This exception extends generic `opyapi.errors.ItemsValidationError` exception.
+
+> Can be triggered by the following schema:
+> ```json
+> {
+>   "type": "array",
+>   "items": [
+>     {"type": "string"},
+>     {"type":  "integer"}        
+>   ],
+>   "additionalItems": false
+> }
+> ```
+
+#### `opyapi.errors.MinimumItemsValidationError`, `opyapi.errors.MaximumItemsValidationError`
+Raised when number of items in an array does not conform maximum or minimum items specified in schema.
+This exception extends generic `opyapi.errors.ItemsValidationError` exception.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "type": "array",
+>   "minimumItems": 2,
+>   "MaximumItems": 10
+> }
+> ```
+
+
+#### `opyapi.errors.MultipleOfValidationError`
+Raised when validated number is not multiplication of passed value.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "type": "numerical",
+>   "multipleOf": 2
+> }
+> ```
+
+#### `opyapi.errors.ComparisonValidationError`
+Raised when comparison operation fails. This is a generic exception used by other comparison errors.
+
+#### `opyapi.errors.EqualityValidationError`
+Raised when validated value is not the same as defined expected value. This exception extends `opyapi.errors.ComparisonValidationError`.
+
+> Can be triggered by following example schema:
+> ```json
+> {
+>   "const": "test"
+> }
+> ```
+
+#### `opyapi.errors.RangeValidationError`
+Raised when (exclusive) minimum, (exclusive) maximum comparisons fail. This exception extends `opyapi.errors.ComparisonValidationError`.
+
+#### `opyapi.errors.MinimumValidationError`, `opyapi.errors.MaximumValidationError`, `opyapi.errors.ExclusiveMinimumValidationError`, `opyapi.errors.ExclusiveMaximumValidationError`
+Raised when passed numerical (or integer) value is not within expected range defined in schema.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "numerical",
+>   "minimum": 2
+> }
+> ```
+
+
+#### `opyapi.errors.ObjectValidationError`
+Generic exception raised when validation of an object fails for some reason.
+
+#### `opyapi.errors.PropertyValidationError`
+Generic exception raised when validation of object's property fails for some reason. 
+This exception extends `opyapi.errors.ObjectValidationError` exception.
+
+#### `opyapi.errors.RequiredPropertyValidationError`
+Raised when required property is not present in passed object.
+This exception extends `opyapi.errors.PropertyValidationError` exception.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "object",
+>   "properties": {
+>     "name" : {"type": "string"}
+>   },
+>   "required": ["name"]
+> }
+> ```
+
+#### `opyapi.errors.PropertyValueValidationError`
+Raised when property contains invalid value. 
+This exception extends `opyapi.errors.PropertyValidationError` exception.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "object",
+>   "properties": {
+>     "name" : {"type": "string"}
+>   }
+> }
+> ```
+
+#### `opyapi.errors.PropertyNameValidationError`
+Raised when property's names does not conform defined schema. 
+This exception extends `opyapi.errors.PropertyValidationError` exception.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "object",
+>   "properties": {
+>     "name" : {"type": "string"}
+>   },
+>   "propertyNames": {
+>     "pattern": "^x-" 
+>   }
+> }
+> ```
+
+#### `opyapi.errors.AdditionalPropertiesValidationError`
+Raised when additional properties are not allowed or set schema is not followed. 
+This exception extends `opyapi.errors.PropertyValidationError` exception.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "object",
+>   "properties": {
+>     "name" : {"type": "string"}
+>   },
+>   "additionalProperties": false
+> }
+> ```
+
+#### `opyapi.errors.ObjectSizeValidationError`
+Generic exception raised when number of properties does not conform defined schema. 
+This exception extends `opyapi.errors.ObjectValidationError` exception.
+
+#### `opyapi.errors.MinimumPropertiesValidationError`, `opyapi.errors.MaximumPropertiesValidationError`
+Generic exception raised when number of properties does not conform defined schema. 
+These exceptions extend `opyapi.errors.ObjectSizeValidationError`exception.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "object",
+>   "properties": {
+>     "name" : {"type": "string"}
+>   },
+>   "minProperties": 2,
+>   "maxProperties": 10
+> }
+> ```
+
+#### `opyapi.errors.DependencyValidationError`
+
+Raised when dependent properties are defined in the schema but not provided in a passed object. 
+This exception extends `opyapi.errors.ObjectValidationError` exception.
+
+> Can be triggered by the following example schema:
+> ```json
+> {
+>   "type": "object",
+>   "properties": {
+>     "name" : {"type": "string"}
+>   },
+>   "dependentRequired": {
+>     "name": ["first_name", "last_name"]
+>   }
+> }
+> ```
+
+## API
+
+### `validate(obj: typing.Any, schema: typing.Union[dict, opyapi.JsonSchema]): typing.Any`
+
+Validates passed object `obj`, and if valid returns the object, otherwise raises a `ValueError` exception.
+
+```python
+from opyapi import validate
+
+assert validate(
+    {"name": "Test", "age":12}, 
+    {
+        "type": "object",
+        "properties": {
+            "name": {
+                "type": "string",
+            },
+            "age": {
+              "type": "integer",  
+            }
+        }
+    }
+)
+```
+
+### `build_validator_for(schema: typing.Union[dict, JsonSchema]) -> Callable`
+
+Creates validator function for passed json schema and returns it as a result.
+
+```python
+from opyapi import build_validator_for
+
+validator =  build_validator_for({
+    "type": "object",
+    "properties": {
+        "name": {
+            "type": "string",
+        },
+        "age": {
+          "type": "integer",  
+        }
+    }
+})
+```
 
-setup(**setup_kwargs)
```

