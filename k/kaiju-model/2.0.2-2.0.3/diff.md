# Comparing `tmp/kaiju_model-2.0.2-py3-none-any.whl.zip` & `tmp/kaiju_model-2.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12586 bytes, number of entries: 12
--rw-r--r--  2.0 unx       94 b- defN 23-Jul-03 21:32 kaiju_model/__init__.py
--rw-r--r--  2.0 unx    19051 b- defN 23-Jul-03 21:32 kaiju_model/fields.py
--rw-r--r--  2.0 unx    18202 b- defN 23-Jul-03 21:32 kaiju_model/model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 21:32 kaiju_model/grid/__init__.py
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-03 21:32 kaiju_model/grid/base.py
--rw-r--r--  2.0 unx    10281 b- defN 23-Jul-03 21:32 kaiju_model/grid/constructor.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 21:32 kaiju_model/tests/__init__.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-03 21:33 kaiju_model-2.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2012 b- defN 23-Jul-03 21:33 kaiju_model-2.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 21:33 kaiju_model-2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-03 21:33 kaiju_model-2.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      974 b- defN 23-Jul-03 21:33 kaiju_model-2.0.2.dist-info/RECORD
-12 files, 51689 bytes uncompressed, 10942 bytes compressed:  78.8%
+Zip file size: 13147 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       94 b- defN 23-Jul-19 10:48 kaiju_model/__init__.py
+-rw-r--r--  2.0 unx    21343 b- defN 23-Jul-19 10:48 kaiju_model/fields.py
+-rw-r--r--  2.0 unx    18433 b- defN 23-Jul-19 10:48 kaiju_model/model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 10:48 kaiju_model/grid/__init__.py
+-rw-r--r--  2.0 unx      361 b- defN 23-Jul-19 10:48 kaiju_model/grid/base.py
+-rw-r--r--  2.0 unx    10281 b- defN 23-Jul-19 10:48 kaiju_model/grid/constructor.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 10:48 kaiju_model/tests/__init__.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      974 b- defN 23-Jul-19 10:48 kaiju_model-2.0.3.dist-info/RECORD
+12 files, 54212 bytes uncompressed, 11503 bytes compressed:  78.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_model/grid/constructor.py
 Comment: 
 
 Filename: kaiju_model/tests/__init__.py
 Comment: 
 
-Filename: kaiju_model-2.0.2.dist-info/LICENSE
+Filename: kaiju_model-2.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_model-2.0.2.dist-info/METADATA
+Filename: kaiju_model-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_model-2.0.2.dist-info/WHEEL
+Filename: kaiju_model-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_model-2.0.2.dist-info/top_level.txt
+Filename: kaiju_model-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_model-2.0.2.dist-info/RECORD
+Filename: kaiju_model-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_model/__init__.py

```diff
@@ -1,4 +1,4 @@
 __author__ = 'antonnidhoggr@me.com'
 __email__ = 'antonnidhoggr@me.com'
-__version__ = '2.0.2'
+__version__ = '2.0.3'
```

## kaiju_model/fields.py

```diff
@@ -54,27 +54,37 @@
         grid_handler=None,
         normalizer: Callable = None,
         normalizer_es: Callable = None,
         validator: Callable = None,
         field_validator: Callable = None,
         dependence: list = None,
         nested=None,
+        label: str = None,
+        label_key: str = None,
+        helper_text: str = None,
+        helper_key: str = None,
+        view_condition: dict = None
     ):
         """
         :param required:
         :param default:
         :param disabled:
         :param read_only:
         :param grid_handler:
         :param group: attribute parameter group, default is base
         :param normalizer: custom normalizer function
         :param validator: custom validation function
         :param dependence: dependence of fields
         :param field_validator: custom validation function for field parameter
         :param normalizer_es:
+        :param label:
+        :param nested:
+        :param label_key:
+        :param helper_text:
+        :param helper_key:
         """
 
         if group is None:
             self.group = FieldGroups.BASE.value
         elif isinstance(group, enum.Enum):
             self.group = group.value
         else:
@@ -84,14 +94,19 @@
         self.dependence = dependence
         self.is_system = is_system
         self.default = default
         self.disabled = disabled
         self.read_only = read_only
         self.grid_handler = grid_handler
         self.nested = nested
+        self.label = label
+        self.label_key = label_key
+        self.helper_key = helper_key
+        self.helper_text = helper_text
+        self.view_condition = view_condition
 
         # normalizer settings
 
         if normalizer:
             if not callable(normalizer):
                 raise TypeError('Normalizer "%s" must be callable.' % normalizer)
             self.normalize = normalizer
@@ -122,14 +137,19 @@
     def repr(self):
         return {
             'default': self.default,
             'disabled': self.disabled,
             'kind': self._name,
             'required': self.required,
             'dependence': self.dependence,
+            'label': self.label,
+            'label_key': self.label_key,
+            'view_condition': self.view_condition,
+            'helper_key': self.helper_key,
+            'helper_text': self.helper_text,
         }
 
     @property
     def type(self):
         return self._name
 
     @staticmethod
@@ -155,26 +175,32 @@
     def repr(self):
         return self._repr
 
 
 class StringField(BaseField):
     _name = 'string'
 
-    def __init__(self, *args, regex=None, behavior=None, field_type=None, **kwargs):
+    def __init__(self, *args, regex=None, behavior=None, field_type=None, min: int = None, max: int = None,
+                 **kwargs):
         super(StringField, self).__init__(*args, **kwargs)
         self.behavior = behavior
-        self.field_type = field_type  # "password", "email"
-
+        self.field_type = field_type  # 'password', 'email'
+        self.min = min
+        self.max = max
         if regex:
             self.regex = RegExp(*regex)
         else:
             self.regex = None
 
     def repr(self):
         _r = super(StringField, self).repr()
+        _r.update({
+            'min': self.min,
+            'max': self.max,
+        })
 
         if self.regex:
             _r['regex'] = self.regex.repr()
 
         _r['behavior'] = self.behavior
 
         if self.field_type:
@@ -238,28 +264,34 @@
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
 
 class IntegerField(BaseField):
     _name = 'integer'
 
-    def __init__(self, *args, negative_value=True, **kwargs):
+    def __init__(self, *args, negative_value=True, min: int = None, max: int = None, **kwargs):
         super(IntegerField, self).__init__(*args, **kwargs)
         self.negative_value = negative_value
+        self.min = min
+        self.max = max
 
     @staticmethod
     def normalize(value, **_):
         try:
             return int(value)
         except ValueError as exc:
             raise NormalizationError(str(exc))
 
     def repr(self):
         _repr = super(IntegerField, self).repr()
         _repr['negative_value'] = self.negative_value
+        _repr.update({
+            'min': self.min,
+            'max': self.max,
+        })
         return _repr
 
 
 class DecimalField(IntegerField):
     _name = 'decimal'
 
     @staticmethod
@@ -718,7 +750,59 @@
         if val1 is not None:
             val1.sort()
 
         if val2 is not None:
             val2.sort()
 
         return val1 == val2
+
+
+class NestedField(BaseField):
+    _name = 'nested'
+
+    def __init__(self, *args, **kwargs):
+        self._fields = []
+        self.init_fields(kwargs)
+        super(NestedField).__init__(*args, **kwargs)
+
+    def init_fields(self, fields: dict):
+        for k, field in list(fields.items()):
+            if isinstance(field, BaseField):
+                fields.pop(k)
+                self._fields.append({
+                    'id': k,
+                    **field.repr()
+                })
+
+    def repr(self):
+        _r = super().repr()
+        _r['fields'] = self._fields
+        return _r
+
+    @staticmethod
+    def normalize(value, **_):
+        # TODO NEED FIELD NOMALIZER
+
+        return value
+
+
+class NestedListField(NestedField):
+    _name = 'nested_list'
+
+    def normalize(self, value, **_):
+        # TODO NEED FIELD NORMALIZER
+        return value
+
+
+class TextBlock(BaseField):
+    _name = 'text_block'
+
+    def __init__(self, *args, text: str = None, text_key: str = None, **kwargs):
+        super(TextBlock).__init__(*args, **kwargs)
+        self.text = text
+        self.text_key = text_key
+
+    def repr(self):
+        _r = super(TextBlock).repr()
+        _r['text'] = self.text
+        _r['text_key'] = self.text_key
+        return _r
```

## kaiju_model/model.py

```diff
@@ -220,14 +220,15 @@
                 elif k in self._optional_fields:
                     self.settings[k] = v
                 setattr(self, k, v)
 
         else:
             for k, field in self._fields.items():
                 nested = getattr(field, 'nested', None)
+                default = getattr(field, 'default', None)
                 in_kws = False
                 v = None
                 if k in kws:
                     v = kws[k]
                     in_kws = True
 
                 if (
@@ -242,14 +243,18 @@
                 ):
                     nested_values = kws[nested]
 
                     if isinstance(nested_values, dict):
                         v = nested_values.get(k)
                         in_kws = True
 
+                if v is None and default is not None:
+                    v = default
+                    in_kws = True
+
                 if in_kws:
                     if k in self._base_fields:
                         self.base[k] = v
                     elif k in self._optional_fields:
                         self.settings[k] = v
                     setattr(self, k, v)
 
@@ -289,14 +294,16 @@
     def __iter__(self):
         return iter(self.params.items())
 
     def to_dict(self):
         result = {}
 
         for key, field in self._fields.items():
+            if field._name == 'text_block':
+                continue
             if key in self.params:
                 value = self.params[key]
                 nested = getattr(field, 'nested', None)
                 if nested:
                     result[f'{nested}.{key}'] = value
                 else:
                     result[key] = value
@@ -311,40 +318,43 @@
         return self.__class__.name
 
     @property
     def type(self):
         return self.__class__.type
 
     @classmethod
-    def get_fields(cls, default_values=None):
+    def get_fields(cls, default_values=None, exclude=None):
         """Returns attribute fields spec."""
         if type(default_values) is not dict:
             default_values = {}
 
+        if type(exclude) is not set:
+            exclude = set()
+
         base = {
-            'key': FieldGroups.BASE.value,
+            'id': FieldGroups.BASE.value,
             'fields': [
-                {'key': name, **field.repr(), **default_values.get(name, {})}
+                {'id': name, **field.repr(), **default_values.get(name, {})}
                 for name, field in cls._base_fields.items()
-                if not field.is_system
-            ],
+                if not field.is_system and name not in exclude
+            ]
         }
 
         optional = {}
 
         for name, field in cls._optional_fields.items():
-            if not field.is_system:
-                data = {'key': name, **field.repr(), **default_values.get(name, {})}
+            if not field.is_system and name not in exclude:
+                data = {'id': name, **field.repr(), **default_values.get(name, {})}
 
                 if field.group in optional:
                     optional[field.group].append(data)
                 else:
                     optional[field.group] = [data]
 
-        optional = [{'key': key, 'fields': values} for key, values in optional.items()]
+        optional = [{'id': key, 'fields': values} for key, values in optional.items()]
 
         return [base, *optional]
 
     def _is_required(self, value):
 
         if isinstance(value, list):
             is_empty = not all(value) and value
@@ -500,46 +510,39 @@
         return
 
     @property
     def fields(self):
         """Returns attribute fields spec."""
 
         base = {
-            'key': FieldGroups.BASE.value,
+            'id': FieldGroups.BASE.value,
             'fields': [
-                {
-                    'key': name,
-                    'value': self.params.get(name),
-                    **field.repr(),
-                    **self.modify(name, field),
-                    'disabled': self._fields[name].read_only,
-                }
-                for name, field in self._base_fields.items()
-                if not field.is_system
-            ],
+                {'id': name, "value": self.params.get(name), **field.repr(), **self.modify(name, field), "disabled": self._fields[name].read_only}
+                for name, field in self._base_fields.items() if not field.is_system
+            ]
         }
 
         optional = {}
 
         for name, field in self._optional_fields.items():
             _modify = self.modify(name, field)
             if not _modify.get('is_system', field.is_system):
                 data = {
-                    'key': name,
+                    'id': name,
                     'value': self.params.get(name),
                     **field.repr(),
                     'disabled': self._fields[name].read_only,
                     **self.modify(name, field),
                 }
                 if field.group in optional:
                     optional[field.group].append(data)
                 else:
                     optional[field.group] = [data]
 
-        optional = [{'key': key, 'fields': values} for key, values in optional.items()]
+        optional = [{'id': key, 'fields': values} for key, values in optional.items()]
 
         return [base, *optional]
 
     def modify(self, *_, **__):
         return {}
 
     def form_normalize(self):
```

## Comparing `kaiju_model-2.0.2.dist-info/LICENSE` & `kaiju_model-2.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_model-2.0.2.dist-info/METADATA` & `kaiju_model-2.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-model
-Version: 2.0.2
+Version: 2.0.3
 Summary: Web interface related classes.
 Home-page: https://gitlab.com/kaiju-python/kaiju-model
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_model-2.0.2.dist-info/RECORD` & `kaiju_model-2.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_model/__init__.py,sha256=SE5KlutwrqwfjLk6T5gjU_gDHAN8kvohPxtB5obbXXs,94
-kaiju_model/fields.py,sha256=1jFb5YaKIYdizh_rxkJG6200llTl9YHRuwGmVNmlOdU,19051
-kaiju_model/model.py,sha256=QeST7_TGU-Qv-WJAh8ZYExY-V6Y3UR6Qy5EEGghwjvA,18202
+kaiju_model/__init__.py,sha256=S8fabmHBIhc1vIb1axXUW4ToBnCSxlUEF4875FIi47A,94
+kaiju_model/fields.py,sha256=NKcbM3EJGZdSZIMr2gkFQzIHJfHlgdiyIvZ5tg8Ov8M,21343
+kaiju_model/model.py,sha256=GjaXAC797LNrtVD-CXB6O7G2ng05fScrkf3E90SC5II,18433
 kaiju_model/grid/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_model/grid/base.py,sha256=-RxkDq__VSR5w_yXCpa74LNAj-4BNr8NVheKae0rjUE,361
 kaiju_model/grid/constructor.py,sha256=e8m37QUuUxA_drXaFkXhtwBj7iVsQcoF2jr4t_H1WNY,10281
 kaiju_model/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kaiju_model-2.0.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_model-2.0.2.dist-info/METADATA,sha256=-xmHefTTosiqXJxImgbTQlngXKuwiL3Bj2QCrj83ZSA,2012
-kaiju_model-2.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_model-2.0.2.dist-info/top_level.txt,sha256=3lm68s9XtN4zbuKIVlAbnzbqzxqSplKrNmLX6s2CD-Y,12
-kaiju_model-2.0.2.dist-info/RECORD,,
+kaiju_model-2.0.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_model-2.0.3.dist-info/METADATA,sha256=9fjjTa7lgvl-ULiULKzp2NvzvKoClV0fxp9WEeiPgNo,2012
+kaiju_model-2.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_model-2.0.3.dist-info/top_level.txt,sha256=3lm68s9XtN4zbuKIVlAbnzbqzxqSplKrNmLX6s2CD-Y,12
+kaiju_model-2.0.3.dist-info/RECORD,,
```

