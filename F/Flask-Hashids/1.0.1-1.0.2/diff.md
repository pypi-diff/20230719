# Comparing `tmp/Flask-Hashids-1.0.1.tar.gz` & `tmp/Flask-Hashids-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Hashids-1.0.1.tar", last modified: Mon Feb 13 16:11:16 2023, max compression
+gzip compressed data, was "Flask-Hashids-1.0.2.tar", last modified: Wed Jul 19 07:32:47 2023, max compression
```

## Comparing `Flask-Hashids-1.0.1.tar` & `Flask-Hashids-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-02-13 16:11:16.745538 Flask-Hashids-1.0.1/
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-02-13 16:11:16.745538 Flask-Hashids-1.0.1/Flask_Hashids.egg-info/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3596 2023-02-13 16:11:16.000000 Flask-Hashids-1.0.1/Flask_Hashids.egg-info/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      227 2023-02-13 16:11:16.000000 Flask-Hashids-1.0.1/Flask_Hashids.egg-info/SOURCES.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-02-13 16:11:16.000000 Flask-Hashids-1.0.1/Flask_Hashids.egg-info/dependency_links.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       21 2023-02-13 16:11:16.000000 Flask-Hashids-1.0.1/Flask_Hashids.egg-info/requires.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       14 2023-02-13 16:11:16.000000 Flask-Hashids-1.0.1/Flask_Hashids.egg-info/top_level.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2022-06-22 08:37:38.000000 Flask-Hashids-1.0.1/LICENSE
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3596 2023-02-13 16:11:16.745538 Flask-Hashids-1.0.1/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3109 2023-02-13 15:48:51.000000 Flask-Hashids-1.0.1/README.md
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3803 2023-02-13 15:50:29.000000 Flask-Hashids-1.0.1/flask_hashids.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-02-13 16:11:16.745538 Flask-Hashids-1.0.1/setup.cfg
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      749 2023-02-13 15:59:43.000000 Flask-Hashids-1.0.1/setup.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-19 07:32:47.913291 Flask-Hashids-1.0.2/
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-19 07:32:47.913291 Flask-Hashids-1.0.2/Flask_Hashids.egg-info/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3596 2023-07-19 07:32:47.000000 Flask-Hashids-1.0.2/Flask_Hashids.egg-info/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      227 2023-07-19 07:32:47.000000 Flask-Hashids-1.0.2/Flask_Hashids.egg-info/SOURCES.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-07-19 07:32:47.000000 Flask-Hashids-1.0.2/Flask_Hashids.egg-info/dependency_links.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       26 2023-07-19 07:32:47.000000 Flask-Hashids-1.0.2/Flask_Hashids.egg-info/requires.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       14 2023-07-19 07:32:47.000000 Flask-Hashids-1.0.2/Flask_Hashids.egg-info/top_level.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2022-06-22 08:37:38.000000 Flask-Hashids-1.0.2/LICENSE
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3596 2023-07-19 07:32:47.913291 Flask-Hashids-1.0.2/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3109 2023-02-13 15:48:51.000000 Flask-Hashids-1.0.2/README.md
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     4998 2023-07-19 07:27:08.000000 Flask-Hashids-1.0.2/flask_hashids.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-07-19 07:32:47.913291 Flask-Hashids-1.0.2/setup.cfg
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      756 2023-07-18 14:09:12.000000 Flask-Hashids-1.0.2/setup.py
```

### Comparing `Flask-Hashids-1.0.1/Flask_Hashids.egg-info/PKG-INFO` & `Flask-Hashids-1.0.2/Flask_Hashids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Hashids
-Version: 1.0.1
+Version: 1.0.2
 Summary: Hashids integration for Flask applications.
 Home-page: https://github.com/Pevtrick/Flask-Hashids
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Flask-Hashids-1.0.1/LICENSE` & `Flask-Hashids-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Hashids-1.0.1/PKG-INFO` & `Flask-Hashids-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Hashids
-Version: 1.0.1
+Version: 1.0.2
 Summary: Hashids integration for Flask applications.
 Home-page: https://github.com/Pevtrick/Flask-Hashids
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Flask-Hashids-1.0.1/README.md` & `Flask-Hashids-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Flask-Hashids-1.0.1/flask_hashids.py` & `Flask-Hashids-1.0.2/flask_hashids.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,127 @@
 from flask import current_app, Flask
 from hashids import Hashids as _Hashids
-from typing import Any, Dict, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 from werkzeug.routing import BaseConverter, ValidationError
 
 
 class HashidMixin:
-    '''
-    Thx HashidMixin class adds a hashid property to a class instance. This
-    property will compute a hashid based on the attribute specified by a
-    special class variable called __id_attribute__ (defaults to "id").
+    ''' Hashid Mixin class.
+
+    The HashidMixin class adds a hashid property to a class. This property
+    will compute a hashid based on the attribute specified by the class
+    variable `__id_attribute__: str = 'id'`.
     
     The class can be used with SQLAlchemy models.
-    This won't add a column to the model, the hashid is computed on runtime.
+    This won't add a column to the table, the hashid is implemented as a
+    property and computed on runtime.
 
     NOTE: The extended class must have an attribute named after the value of
-    __id_attribute__ and must be of type int!
+    `__id_attribute__: str` and must be of type `int`!
     '''
 
     __id_attribute__: str = 'id'
 
     @property
     def hashid(self) -> str:
-        id: int = getattr(self, self.__class__.__id_attribute__)
-        return current_app.extensions['hashids'].encode(id)
+        ''' Hashid property.
+
+        Runtime computed hashid based on the attribute specified by the class
+        variable `__id_attribute__: str`.
+        '''
+        id_attribute: int = getattr(self, self.__class__.__id_attribute__)
+        hashids_extension: Hashids = current_app.extensions['hashids']
+        return hashids_extension.encode(id_attribute)
 
 
 class HashidConverter(BaseConverter):
     ''' Hashid Converter.
 
-    Converts and decodes a hashid from routes.
+    Converts and decodes a hashid from routes.\n
     Examples:
+        ```python
         @app.route('/resources/<hashid:resource_id')
         def get_resource(resource_id: int):
             print(isinstance(resource_id, int))  # True
 
         @app.route('/resources/<hashid:resource_ids')
         def get_resources(resource_ids: Tuple[int, ...]):
             print(isinstance(resource_ids, tuple))  # True
             print(all(isinstance(i, int) for i in resource_ids))  # True
+        ```
 
-    Converts and encodes values when generating urls.
+    Converts and encodes values when generating urls.\n
     Examples:
+        ```python
         url_for('get_resource', resource_id=123)  # /resources/Mj3
 
         url_for('get_resource', resource_id=(123, 456))  # /resources/Nk4
+        ```
     '''
 
     def to_python(self, hashid: str) -> Union[int, Tuple[int, ...]]:
-        decoded_hashid = current_app.extensions['hashids'].decode(hashid)
+        ''' Decodes matched hashid in a URL to an int or tuple of ints '''
+        hashids_extension: Hashids = current_app.extensions['hashids']
+        decoded_hashid: Union[int, Tuple[int, ...], Tuple[()]] = hashids_extension.decode(hashid)
         if isinstance(decoded_hashid, tuple) and len(decoded_hashid) == 0:
             raise ValidationError()
         return decoded_hashid
 
-    def to_url(self, value_or_values: Union[int, Tuple[int, ...]]) -> str:
-        if isinstance(value_or_values, int):
-            return current_app.extensions['hashids'].encode(value_or_values)
-        return current_app.extensions['hashids'].encode(*value_or_values)
+    def to_url(self, value: Union[int, Tuple[int, ...]]) -> str:
+        ''' Encodes an int or tuple of ints to a hashid when building a URL '''
+        hashids_extension: Hashids = current_app.extensions['hashids']
+        if isinstance(value, int):
+            return hashids_extension.encode(value)
+        elif isinstance(value, tuple):
+            if len(value) == 0:
+                raise ValueError('Tuple must not be empty')
+            if not all(isinstance(v, int) for v in value):
+                raise TypeError('Tuple must only contain integers')
+            return hashids_extension.encode(*value)
+        else:
+            raise TypeError('Value must be int or tuple of ints')
 
 
 class Hashids:
-    ''' Wrapper class to easily integrate hashids in Flask '''
+    ''' Wrapper class to easily integrate Hashids in Flask '''
 
-    def __init__(self, app: Flask = None):
-        self.app = app
+    def __init__(self, app: Optional[Flask] = None) -> None:
+        self.app: Optional[Flask] = app
         if app is not None:
             self.init_app(app)
 
-    def init_app(self, app: Flask):
-        ''' Setup Hashids, includes the integration of the HashidConverter. '''
-        hashids_config: Dict[str, Any] = {}
+    def init_app(self, app: Flask) -> None:
+        ''' Initialize Hashids extension
+        
+        This method will configure the Hashids extension according to the
+        `config` attribute of the passed `app` object. It will also register
+        the HashidConverter.
+        '''
+        hashids_config: Dict = {}
         if 'HASHIDS_ALPHABET' in app.config:
-            hashids_config['alphabet'] = app.config['HASHIDS_ALPHABET']
+            hashids_config['alphabet']: str = app.config['HASHIDS_ALPHABET']
         if 'HASHIDS_MIN_LENGTH' in app.config:
-            hashids_config['min_length'] = \
-                int(app.config['HASHIDS_MIN_LENGTH'])
+            hashids_config['min_length']: int = int(app.config['HASHIDS_MIN_LENGTH'])
         if 'HASHIDS_SALT' in app.config:
-            hashids_config['salt'] = app.config['HASHIDS_SALT']
-        self._hashids = _Hashids(**hashids_config)
+            hashids_config['salt']: str = app.config['HASHIDS_SALT']
+        self._hashids: _Hashids = _Hashids(**hashids_config)
         if not hasattr(app, 'extensions'):
-            app.extensions = {}
-        app.extensions['hashids'] = self
-        app.url_map.converters['hashid'] = HashidConverter
+            app.extensions: Dict = {}
+        app.extensions['hashids']: Hashids = self
+        app.url_map.converters['hashid']: HashidConverter = HashidConverter
 
     def decode(self, hashid: str) -> Union[int, Tuple[int, ...], Tuple[()]]:
         ''' Decode the passed `hashid`.
-        
+
         Possible return values:
             - `int` if the hashid contains only one value.
             - `Tuple[int, ...]` if the hashid contains multiple values.
             - `Tuple[()]` if the hashid is invalid.
         '''
-        decoded_hashid = self._hashids.decode(hashid)
+        decoded_hashid: Union[Tuple[int, ...], Tuple[()]] = self._hashids.decode(hashid)
         if len(decoded_hashid) == 1:
             return decoded_hashid[0]
         return decoded_hashid
 
     def encode(self, *values: int) -> str:
         ''' Encode the passed `values`. '''
         return self._hashids.encode(*values)
```

### Comparing `Flask-Hashids-1.0.1/setup.py` & `Flask-Hashids-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 
 setup(
     name='Flask-Hashids',
-    version='1.0.1',
+    version='1.0.2',
     url='https://github.com/Pevtrick/Flask-Hashids',
     author='Patrick Jentsch',
     author_email='patrickjentsch@gmx.net',
     description='Hashids integration for Flask applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=['flask_hashids'],
-    install_requires=['Flask', 'Hashids >= 1.0.2'],
+    install_requires=['Flask >= 0.7', 'Hashids >= 1.0.2'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Framework :: Flask',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.5',
```

