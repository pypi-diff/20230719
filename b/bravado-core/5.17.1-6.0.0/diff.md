# Comparing `tmp/bravado-core-5.17.1.tar.gz` & `tmp/bravado-core-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bravado-core-5.17.1.tar", last modified: Fri Sep  2 17:27:10 2022, max compression
+gzip compressed data, was "bravado-core-6.0.0.tar", last modified: Tue Jul 18 23:30:47 2023, max compression
```

## Comparing `bravado-core-5.17.1.tar` & `bravado-core-6.0.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2022-09-02 17:27:10.000000 bravado-core-5.17.1/
--rw-r--r--   0 bariteau  (3176) users      (100)    28531 2022-09-01 22:21:26.000000 bravado-core-5.17.1/CHANGELOG.rst
--rw-r--r--   0 bariteau  (3176) users      (100)     1587 2022-09-01 22:21:26.000000 bravado-core-5.17.1/LICENSE.txt
--rw-r--r--   0 bariteau  (3176) users      (100)       61 2022-09-01 22:21:26.000000 bravado-core-5.17.1/MANIFEST.in
--rw-r--r--   0 bariteau  (3176) users      (100)     3957 2022-09-02 17:27:10.000000 bravado-core-5.17.1/PKG-INFO
--rw-r--r--   0 bariteau  (3176) users      (100)     2460 2022-09-01 22:21:26.000000 bravado-core-5.17.1/README.rst
-drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2022-09-02 17:27:10.000000 bravado-core-5.17.1/bravado_core/
--rw-r--r--   0 bariteau  (3176) users      (100)       43 2022-09-02 17:25:10.000000 bravado-core-5.17.1/bravado_core/__init__.py
--rw-r--r--   0 bariteau  (3176) users      (100)      676 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/_compat.py
--rw-r--r--   0 bariteau  (3176) users      (100)      456 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/_compat_typing.py
--rw-r--r--   0 bariteau  (3176) users      (100)     3428 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/_decorators.py
--rw-r--r--   0 bariteau  (3176) users      (100)       90 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/content_type.py
--rw-r--r--   0 bariteau  (3176) users      (100)     5289 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/docstring.py
--rw-r--r--   0 bariteau  (3176) users      (100)     1986 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/exception.py
--rw-r--r--   0 bariteau  (3176) users      (100)     7541 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/formatter.py
--rw-r--r--   0 bariteau  (3176) users      (100)    16058 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/marshal.py
--rw-r--r--   0 bariteau  (3176) users      (100)    35645 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/model.py
--rw-r--r--   0 bariteau  (3176) users      (100)     9718 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/operation.py
--rw-r--r--   0 bariteau  (3176) users      (100)    14518 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/param.py
--rw-r--r--   0 bariteau  (3176) users      (100)        0 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/py.typed
--rw-r--r--   0 bariteau  (3176) users      (100)     2687 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/request.py
--rw-r--r--   0 bariteau  (3176) users      (100)     6523 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/resource.py
--rw-r--r--   0 bariteau  (3176) users      (100)     8920 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/response.py
--rw-r--r--   0 bariteau  (3176) users      (100)     8520 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/schema.py
--rw-r--r--   0 bariteau  (3176) users      (100)     2771 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/security_definition.py
--rw-r--r--   0 bariteau  (3176) users      (100)     2537 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/security_requirement.py
--rw-r--r--   0 bariteau  (3176) users      (100)    26681 2022-09-02 17:24:42.000000 bravado-core-5.17.1/bravado_core/spec.py
--rw-r--r--   0 bariteau  (3176) users      (100)    19039 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/spec_flattening.py
--rw-r--r--   0 bariteau  (3176) users      (100)    12598 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/swagger20_validator.py
--rw-r--r--   0 bariteau  (3176) users      (100)    16765 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/unmarshal.py
--rw-r--r--   0 bariteau  (3176) users      (100)    10813 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/util.py
--rw-r--r--   0 bariteau  (3176) users      (100)     7466 2022-09-01 22:21:26.000000 bravado-core-5.17.1/bravado_core/validate.py
-drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2022-09-02 17:27:10.000000 bravado-core-5.17.1/bravado_core.egg-info/
--rw-r--r--   0 bariteau  (3176) users      (100)     3957 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/PKG-INFO
--rw-r--r--   0 bariteau  (3176) users      (100)      943 2022-09-02 17:27:10.000000 bravado-core-5.17.1/bravado_core.egg-info/SOURCES.txt
--rw-r--r--   0 bariteau  (3176) users      (100)        1 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/dependency_links.txt
--rw-r--r--   0 bariteau  (3176) users      (100)        1 2022-09-01 22:27:29.000000 bravado-core-5.17.1/bravado_core.egg-info/not-zip-safe
--rw-r--r--   0 bariteau  (3176) users      (100)      232 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/requires.txt
--rw-r--r--   0 bariteau  (3176) users      (100)       13 2022-09-02 17:27:09.000000 bravado-core-5.17.1/bravado_core.egg-info/top_level.txt
--rw-r--r--   0 bariteau  (3176) users      (100)      106 2022-09-02 17:27:10.000000 bravado-core-5.17.1/setup.cfg
--rwxr-xr-x   0 bariteau  (3176) users      (100)     1894 2022-09-02 17:24:42.000000 bravado-core-5.17.1/setup.py
+drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-07-18 23:30:47.122728 bravado-core-6.0.0/
+-rw-r--r--   0 ckuehl    (3119) users      (100)    28531 2023-07-18 20:00:57.000000 bravado-core-6.0.0/CHANGELOG.rst
+-rw-r--r--   0 ckuehl    (3119) users      (100)     1587 2023-07-18 20:00:57.000000 bravado-core-6.0.0/LICENSE.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)       61 2023-07-18 20:00:57.000000 bravado-core-6.0.0/MANIFEST.in
+-rw-r--r--   0 ckuehl    (3119) users      (100)     3426 2023-07-18 23:30:47.122728 bravado-core-6.0.0/PKG-INFO
+-rw-r--r--   0 ckuehl    (3119) users      (100)     2461 2023-07-18 23:29:45.000000 bravado-core-6.0.0/README.rst
+drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-07-18 23:30:47.122728 bravado-core-6.0.0/bravado_core/
+-rw-r--r--   0 ckuehl    (3119) users      (100)       42 2023-07-18 23:30:13.000000 bravado-core-6.0.0/bravado_core/__init__.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)      223 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/_compat.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)      457 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/_compat_typing.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     3460 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/_decorators.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)       90 2023-07-18 20:00:57.000000 bravado-core-6.0.0/bravado_core/content_type.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     5289 2023-07-18 20:00:57.000000 bravado-core-6.0.0/bravado_core/docstring.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     1986 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/exception.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     7541 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/formatter.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    16058 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/marshal.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    35645 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/model.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     9718 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/operation.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    14518 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/param.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)        0 2023-07-18 20:00:57.000000 bravado-core-6.0.0/bravado_core/py.typed
+-rw-r--r--   0 ckuehl    (3119) users      (100)     2687 2023-07-18 20:00:57.000000 bravado-core-6.0.0/bravado_core/request.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     6523 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/resource.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     8920 2023-07-18 20:00:57.000000 bravado-core-6.0.0/bravado_core/response.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     8520 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/schema.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     2770 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/security_definition.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     2537 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/security_requirement.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    26697 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/spec.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    19039 2023-07-18 20:00:57.000000 bravado-core-6.0.0/bravado_core/spec_flattening.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    12598 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/swagger20_validator.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    16765 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/unmarshal.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    10813 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/util.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)     7466 2023-07-18 23:29:45.000000 bravado-core-6.0.0/bravado_core/validate.py
+drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-07-18 23:30:47.122728 bravado-core-6.0.0/bravado_core.egg-info/
+-rw-r--r--   0 ckuehl    (3119) users      (100)     3426 2023-07-18 23:30:47.000000 bravado-core-6.0.0/bravado_core.egg-info/PKG-INFO
+-rw-r--r--   0 ckuehl    (3119) users      (100)      908 2023-07-18 23:30:47.000000 bravado-core-6.0.0/bravado_core.egg-info/SOURCES.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)        1 2023-07-18 23:30:47.000000 bravado-core-6.0.0/bravado_core.egg-info/dependency_links.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)      131 2023-07-18 23:30:47.000000 bravado-core-6.0.0/bravado_core.egg-info/requires.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)       13 2023-07-18 23:30:47.000000 bravado-core-6.0.0/bravado_core.egg-info/top_level.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)      106 2023-07-18 23:30:47.122728 bravado-core-6.0.0/setup.cfg
+-rwxr-xr-x   0 ckuehl    (3119) users      (100)     1676 2023-07-18 23:30:03.000000 bravado-core-6.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bravado-core-5.17.1/CHANGELOG.rst` & `bravado-core-6.0.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.1/LICENSE.txt` & `bravado-core-6.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.1/README.rst` & `bravado-core-6.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 ::
 
     # Run tests
     tox
 
     # Install git pre-commit hooks
-    .tox/py27/bin/pre-commit install
+    .tox/py310/bin/pre-commit install
 
 
 Contributing
 ------------
 
 1. Fork it ( http://github.com/Yelp/bravado-core/fork )
 2. Create your feature branch (``git checkout -b my-new-feature``)
```

### Comparing `bravado-core-5.17.1/bravado_core/_decorators.py` & `bravado-core-6.0.0/bravado_core/_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                         raise SwaggerMappingError(
                             'Spec {0} is a required value'.format(object_schema),
                         )
                 elif is_marshaling_operation:
                     return value
             return func(value)
 
-        return wrapper
+        return wrapper  # type: ignore
 
     return external_wrapper
 
 
 def wrap_recursive_call_exception(func):
     # type: (FuncType) -> FuncType
     """
@@ -78,8 +78,8 @@
     def wrapper(*args, **kwargs):
         # type: (typing.Any, typing.Any) -> typing.Any
         try:
             return func(*args, **kwargs)
         except RecursiveCallException:
             return lambda *new_args, **new_kawrgs: func(*args, **kwargs)(*new_args, **new_kawrgs)
 
-    return wrapper
+    return wrapper  # type: ignore
```

### Comparing `bravado-core-5.17.1/bravado_core/docstring.py` & `bravado-core-6.0.0/bravado_core/docstring.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.1/bravado_core/exception.py` & `bravado-core-6.0.0/bravado_core/exception.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import sys
+import typing
 
 import six
-import typing
 
 
 if getattr(typing, 'TYPE_CHECKING', False):
     from bravado_core._compat_typing import FuncType
 
 
 class SwaggerError(Exception):
```

### Comparing `bravado-core-5.17.1/bravado_core/formatter.py` & `bravado-core-6.0.0/bravado_core/formatter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 Support for the 'format' key in the swagger spec as outlined in
 https://github.com/swagger-api/swagger-spec/blob/master/versions/2.0.md#dataTypeFormat
 """
 from __future__ import unicode_literals
 
 import base64
 import functools
+import typing
 
 import dateutil.parser
 import pytz
 import six
-import typing
 
 from bravado_core import schema
 from bravado_core.exception import SwaggerMappingError
 
 
 if getattr(typing, 'TYPE_CHECKING', False):
     from bravado_core._compat_typing import JSONDict
```

### Comparing `bravado-core-5.17.1/bravado_core/marshal.py` & `bravado-core-6.0.0/bravado_core/marshal.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
+import typing
 import warnings
 from functools import partial
 
-import typing
 from six import iteritems
 
 from bravado_core import _decorators
 from bravado_core import schema
 from bravado_core.exception import SwaggerMappingError
 from bravado_core.model import Model
 from bravado_core.model import MODEL_MARKER
```

### Comparing `bravado-core-5.17.1/bravado_core/model.py` & `bravado-core-6.0.0/bravado_core/model.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 import abc
 import functools
 import logging
 import re
+import typing
 from copy import deepcopy
 from warnings import warn
 
-import typing
 from six import add_metaclass
 from six import iteritems
 from six import string_types
 from swagger_spec_validator.ref_validators import attach_scope
 
 from bravado_core.schema import collapsed_properties
 from bravado_core.schema import is_dict_like
```

### Comparing `bravado-core-5.17.1/bravado_core/operation.py` & `bravado-core-6.0.0/bravado_core/operation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import logging
-
 import typing
+
 from six import iteritems
 from six import PY2
 
 from bravado_core.exception import SwaggerSchemaError
 from bravado_core.param import Param
 from bravado_core.security_requirement import SecurityRequirement
 from bravado_core.util import AliasKeyDict
```

### Comparing `bravado-core-5.17.1/bravado_core/param.py` & `bravado-core-6.0.0/bravado_core/param.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import logging
+import typing
 from functools import partial
 
 import simplejson as json
 import six
-import typing
 from six.moves.urllib.parse import quote
 
 from bravado_core import schema
 from bravado_core.content_type import APP_JSON
 from bravado_core.exception import SwaggerMappingError
 from bravado_core.marshal import marshal_schema_object
 from bravado_core.unmarshal import unmarshal_schema_object
```

### Comparing `bravado-core-5.17.1/bravado_core/request.py` & `bravado-core-6.0.0/bravado_core/request.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.1/bravado_core/resource.py` & `bravado-core-6.0.0/bravado_core/resource.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import logging
+import typing
 from collections import defaultdict
 from copy import deepcopy
 from itertools import chain
 
-import typing
 from six import iteritems
 from six import iterkeys
 from six import PY2
 
 from bravado_core.exception import SwaggerMappingError
 from bravado_core.operation import Operation
 from bravado_core.util import AliasKeyDict
```

### Comparing `bravado-core-5.17.1/bravado_core/response.py` & `bravado-core-6.0.0/bravado_core/response.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.1/bravado_core/schema.py` & `bravado-core-6.0.0/bravado_core/schema.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import copy
-
 import typing
+
 from six import iteritems
 from six import string_types
 
 from bravado_core._compat import Mapping
 from bravado_core.exception import SwaggerMappingError
```

### Comparing `bravado-core-5.17.1/bravado_core/security_definition.py` & `bravado-core-6.0.0/bravado_core/security_definition.py`

 * *Files identical despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 import logging
-from copy import deepcopy
-
 import typing
+from copy import deepcopy
 
 
 if getattr(typing, 'TYPE_CHECKING', False):
     from bravado_core._compat_typing import JSONDict
     from bravado_core.spec import Spec
```

### Comparing `bravado-core-5.17.1/bravado_core/security_requirement.py` & `bravado-core-6.0.0/bravado_core/security_requirement.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import logging
+import typing
 
 import six
-import typing
 
 from bravado_core.exception import SwaggerSchemaError
 
 if getattr(typing, 'TYPE_CHECKING', False):
     from bravado_core._compat_typing import JSONDict
     from bravado_core.security_definition import SecurityDefinition
     from bravado_core.spec import Spec
```

### Comparing `bravado-core-5.17.1/bravado_core/spec.py` & `bravado-core-6.0.0/bravado_core/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 import json
 import logging
 import os.path
+import typing
 import warnings
 from copy import deepcopy
 from itertools import chain
 
 import requests
-import typing
 import yaml
 from jsonref import JsonRef
 from jsonschema import FormatChecker
 from jsonschema.validators import RefResolver
 from six import iteritems
 from six import iterkeys
 from six.moves import range
@@ -406,15 +406,15 @@
         """
         if ref_dict is None or not is_ref(ref_dict):
             return ref_dict
 
         # Restore attached resolution scope before resolving since the
         # resolver doesn't have a traversal history (accumulated scope_stack)
         # when asked to resolve.
-        with in_scope(self.resolver, ref_dict):
+        with in_scope(self.resolver, ref_dict):  # type: ignore
             reference_value = ref_dict['$ref']  # type: ignore
             _, target = self.resolver.resolve(reference_value)
             return target
 
     # NOTE: deref gets overridden, if internally_dereference_refs is enabled, after calling build
     deref = _force_deref
```

### Comparing `bravado-core-5.17.1/bravado_core/spec_flattening.py` & `bravado-core-6.0.0/bravado_core/spec_flattening.py`

 * *Files identical despite different names*

### Comparing `bravado-core-5.17.1/bravado_core/swagger20_validator.py` & `bravado-core-6.0.0/bravado_core/swagger20_validator.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import functools
-
 import typing
+
 from jsonschema import FormatChecker
 from jsonschema import RefResolver
 from jsonschema import validators
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import Draft4Validator
 from swagger_spec_validator.ref_validators import in_scope
```

### Comparing `bravado-core-5.17.1/bravado_core/unmarshal.py` & `bravado-core-6.0.0/bravado_core/unmarshal.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 The module exposes unmarshaling capabilities.
 
 Unmarshaling is the operation that converts a "JSON" object into its python representation.
 The operation should also take care of converting types accordingly to the defined :class:`bravado_core.formatter.SwaggerFormat`s.
 """
+import typing
 import warnings
 from functools import partial
 
-import typing
 from six import iteritems
 
 from bravado_core import _decorators
 from bravado_core import schema
 from bravado_core.exception import SwaggerMappingError
 from bravado_core.model import MODEL_MARKER
 from bravado_core.schema import collapsed_properties
```

### Comparing `bravado-core-5.17.1/bravado_core/util.py` & `bravado-core-6.0.0/bravado_core/util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import copy
 import inspect
 import re
-
 import typing
 from enum import Enum
+
 from six import iteritems
 from six import iterkeys
 
 from bravado_core._compat import get_function_spec
 from bravado_core._compat import wraps
 from bravado_core.schema import is_dict_like
 from bravado_core.schema import is_list_like
```

### Comparing `bravado-core-5.17.1/bravado_core/validate.py` & `bravado-core-6.0.0/bravado_core/validate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 Delegate as much validation as possible out to jsonschema. This module serves
 as the single point of entry for validations should we need to further
 customize the behavior.
 """
 import sys
+import typing
 
 import jsonschema
-import typing
 from six import itervalues
 from six import reraise
 
 from bravado_core._compat import wraps
 from bravado_core.exception import SwaggerMappingError
 from bravado_core.exception import SwaggerSecurityValidationError
 from bravado_core.model import is_object
```

### Comparing `bravado-core-5.17.1/bravado_core.egg-info/SOURCES.txt` & `bravado-core-6.0.0/bravado_core.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -28,10 +28,9 @@
 bravado_core/swagger20_validator.py
 bravado_core/unmarshal.py
 bravado_core/util.py
 bravado_core/validate.py
 bravado_core.egg-info/PKG-INFO
 bravado_core.egg-info/SOURCES.txt
 bravado_core.egg-info/dependency_links.txt
-bravado_core.egg-info/not-zip-safe
 bravado_core.egg-info/requires.txt
 bravado_core.egg-info/top_level.txt
```

### Comparing `bravado-core-5.17.1/setup.py` & `bravado-core-6.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013, Digium, Inc.
 # Copyright (c) 2014-2015, Yelp, Inc.
 import os
-import sys
 
 from setuptools import setup
 
 import bravado_core
 
-install_requires = [
-    "jsonref",
-    "jsonschema[format]>=2.5.1",
-    "python-dateutil",
-    "pyyaml",
-    'requests',
-    "simplejson",
-    "six",
-    "swagger-spec-validator>=2.0.1",
-    "pytz",
-    "msgpack>=0.5.2",
-]
-
-# pyrsistent dropped python2 support in 0.17.0
-if sys.version_info < (3, 5):
-    install_requires.append('pyrsistent<0.17')
 
 setup(
     name="bravado-core",
     version=bravado_core.version,
     license="BSD 3-Clause License",
     description="Library for adding Swagger support to clients and servers",
     long_description=open(
         os.path.join(
             os.path.dirname(__file__),
             "README.rst",
         ),
     ).read(),
+    long_description_content_type='text/markdown',
     author="Digium, Inc. and Yelp, Inc.",
     author_email="opensource+bravado-core@yelp.com",
     url="https://github.com/Yelp/bravado-core",
     packages=["bravado_core"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    install_requires=[
+        "jsonref",
+        "jsonschema[format]>=2.5.1",
+        "python-dateutil",
+        "pyyaml",
+        'requests',
+        "simplejson",
+        "six",
+        "swagger-spec-validator>=2.0.1",
+        "pytz",
+        "msgpack>=0.5.2",
     ],
-    install_requires=install_requires,
     package_data={
         'bravado_core': ['py.typed'],
     },
-    # https://mypy.readthedocs.io/en/latest/installed_packages.html
-    zip_safe=False,
-    extras_require={
-        ':python_version<"3.5"': ['typing'],
-        ':python_version<"3.4"': ['enum34'],
-        ':python_version<"3.2"': ['functools32'],
-    },
-    python_requires='!=3.0,!=3.1,!=3.2,!=3.3,!=3.4,!=3.5.0',
+    python_requires='>=3.7',
 )
```

