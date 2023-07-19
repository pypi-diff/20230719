# Comparing `tmp/keras_model_cv-0.3.1.tar.gz` & `tmp/keras_model_cv-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_model_cv-0.3.1.tar", last modified: Tue Feb  7 06:45:05 2023, max compression
+gzip compressed data, was "keras_model_cv-0.5.4.tar", last modified: Wed Jul 19 11:18:32 2023, max compression
```

## Comparing `keras_model_cv-0.3.1.tar` & `keras_model_cv-0.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 padu      (1000) padu      (1000)        0 2023-02-07 06:45:05.557702 keras_model_cv-0.3.1/
--rw-r--r--   0 padu      (1000) padu      (1000)     3472 2023-02-07 06:45:05.557702 keras_model_cv-0.3.1/PKG-INFO
--rw-rw-r--   0 padu      (1000) padu      (1000)     3117 2023-02-02 12:48:32.000000 keras_model_cv-0.3.1/README.md
-drwxr-xr-x   0 padu      (1000) padu      (1000)        0 2023-02-07 06:45:05.553702 keras_model_cv-0.3.1/keras_model_cv/
--rw-r--r--   0 padu      (1000) padu      (1000)       26 2023-01-31 12:25:27.000000 keras_model_cv-0.3.1/keras_model_cv/__init__.py
--rw-r--r--   0 padu      (1000) padu      (1000)    11168 2023-02-06 21:49:45.000000 keras_model_cv-0.3.1/keras_model_cv/core.py
-drwxr-xr-x   0 padu      (1000) padu      (1000)        0 2023-02-07 06:45:05.557702 keras_model_cv-0.3.1/keras_model_cv.egg-info/
--rw-r--r--   0 padu      (1000) padu      (1000)     3472 2023-02-07 06:45:05.000000 keras_model_cv-0.3.1/keras_model_cv.egg-info/PKG-INFO
--rw-r--r--   0 padu      (1000) padu      (1000)      257 2023-02-07 06:45:05.000000 keras_model_cv-0.3.1/keras_model_cv.egg-info/SOURCES.txt
--rw-r--r--   0 padu      (1000) padu      (1000)        1 2023-02-07 06:45:05.000000 keras_model_cv-0.3.1/keras_model_cv.egg-info/dependency_links.txt
--rw-r--r--   0 padu      (1000) padu      (1000)       54 2023-02-07 06:45:05.000000 keras_model_cv-0.3.1/keras_model_cv.egg-info/requires.txt
--rw-r--r--   0 padu      (1000) padu      (1000)       15 2023-02-07 06:45:05.000000 keras_model_cv-0.3.1/keras_model_cv.egg-info/top_level.txt
--rw-r--r--   0 padu      (1000) padu      (1000)       38 2023-02-07 06:45:05.557702 keras_model_cv-0.3.1/setup.cfg
--rw-rw-r--   0 padu      (1000) padu      (1000)      846 2023-02-06 21:51:15.000000 keras_model_cv-0.3.1/setup.py
+drwxr-xr-x   0 paveldubovik   (501) staff       (20)        0 2023-07-19 11:18:32.735417 keras_model_cv-0.5.4/
+-rw-r--r--   0 paveldubovik   (501) staff       (20)     3472 2023-07-19 11:18:32.735117 keras_model_cv-0.5.4/PKG-INFO
+-rw-r--r--   0 paveldubovik   (501) staff       (20)     3117 2023-07-13 14:53:16.000000 keras_model_cv-0.5.4/README.md
+drwxr-xr-x   0 paveldubovik   (501) staff       (20)        0 2023-07-19 11:18:32.732129 keras_model_cv-0.5.4/keras_model_cv/
+-rw-r--r--   0 paveldubovik   (501) staff       (20)       26 2023-07-13 14:53:16.000000 keras_model_cv-0.5.4/keras_model_cv/__init__.py
+-rw-r--r--   0 paveldubovik   (501) staff       (20)    13399 2023-07-19 10:54:32.000000 keras_model_cv-0.5.4/keras_model_cv/core.py
+drwxr-xr-x   0 paveldubovik   (501) staff       (20)        0 2023-07-19 11:18:32.734572 keras_model_cv-0.5.4/keras_model_cv.egg-info/
+-rw-r--r--   0 paveldubovik   (501) staff       (20)     3472 2023-07-19 11:18:32.000000 keras_model_cv-0.5.4/keras_model_cv.egg-info/PKG-INFO
+-rw-r--r--   0 paveldubovik   (501) staff       (20)      257 2023-07-19 11:18:32.000000 keras_model_cv-0.5.4/keras_model_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 paveldubovik   (501) staff       (20)        1 2023-07-19 11:18:32.000000 keras_model_cv-0.5.4/keras_model_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 paveldubovik   (501) staff       (20)       54 2023-07-19 11:18:32.000000 keras_model_cv-0.5.4/keras_model_cv.egg-info/requires.txt
+-rw-r--r--   0 paveldubovik   (501) staff       (20)       15 2023-07-19 11:18:32.000000 keras_model_cv-0.5.4/keras_model_cv.egg-info/top_level.txt
+-rw-r--r--   0 paveldubovik   (501) staff       (20)       38 2023-07-19 11:18:32.735521 keras_model_cv-0.5.4/setup.cfg
+-rw-r--r--   0 paveldubovik   (501) staff       (20)      846 2023-07-19 10:54:32.000000 keras_model_cv-0.5.4/setup.py
```

### Comparing `keras_model_cv-0.3.1/PKG-INFO` & `keras_model_cv-0.5.4/keras_model_cv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: keras_model_cv
-Version: 0.3.1
+Name: keras-model-cv
+Version: 0.5.4
 Summary: Cross-validation for keras models
 Home-page: https://github.com/dubovikmaster/keras-model-cv
 Author: Pavel Dubovik
 Author-email: geometryk@gmail.com
 License: MIT
 Keywords: keras cross-validate,validation keras modelscross-validation
 Platform: any
```

### Comparing `keras_model_cv-0.3.1/README.md` & `keras_model_cv-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `keras_model_cv-0.3.1/keras_model_cv/core.py` & `keras_model_cv-0.5.4/keras_model_cv/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,89 +10,121 @@
     Union,
     List,
     Tuple,
     Iterable,
     Any
 
 )
+import copy
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import tensorflow as tf
 import yaml
 from sklearn.model_selection import BaseCrossValidator
 from tensorflow import keras
 
 NAMES = ['mysterious', 'incredible', 'beautiful', 'graceful']
 STATUS = {'RUNNING': 0, 'OK': 1}
 
+logger = tf.get_logger()
+logger.propagate = False
+
 
 class KerasCV:
 
     def __init__(
             self,
             model_builder: Callable,
             cv: BaseCrossValidator,
             params: dict,
             preprocessor: Optional[Union[Callable, List[Callable]]] = None,
+            supervised_preprocessor: Optional[Union[bool, List[bool]]] = None,
             save_history: bool = False,
             directory: Optional[Union[str, PathLike]] = None,
             name: Optional[str] = None,
             custom_evaluate: Optional[Callable] = None,
             overwrite: bool = False,
             distribution_strategy: Optional[tf.distribute.Strategy] = None
 
 
     ):
         self.model_builder = model_builder
         self.cv = cv
         self.params = params
         self.preprocessor = preprocessor
+        self.supervised_preprocessor = supervised_preprocessor
         self.save_history = save_history
         self.directory = directory
         self.name = name
         self.history = None
         self.overwrite = overwrite
         self.cv_results = None
         self.distribution_strategy = distribution_strategy
         self.splits_info = None
         self._multiple_input = None
         self._custom_eval = custom_evaluate
+        self._model_checkpoint_deepcopy = None
+        self._model_checkpoint_new_filepath = None
 
         if self.save_history:
             if self.name is None:
                 self.name = random.choice(NAMES) + '_project'
             if self.directory is None:
                 raise ValueError('directory must be specified if save_history is "True".')
             self.project_path = Path(self.directory).joinpath(self.name)
             self.project_path.mkdir(exist_ok=True, parents=True)
 
     @staticmethod
-    def preprocess_data(x: Iterable, preprocessor: Callable, fit_transform: bool):
+    def preprocess_data(x: Iterable, y: Iterable, preprocessor: Callable, supervised: bool,  fit_transform: bool):
         if preprocessor is None:
             return x
         if fit_transform:
             if isinstance(preprocessor, keras.layers.Layer):
                 preprocessor.adapt(x)
                 return preprocessor(x)
-            preprocessor.fit(x)
-            return preprocessor.transform(x)
+            if supervised:
+                new_x = preprocessor.fit_transform(x, y)
+            else:
+                new_x = preprocessor.fit_transform(x)
+            return new_x
         if isinstance(preprocessor, keras.layers.Layer):
             return preprocessor(x)
         return preprocessor.transform(x)
 
     @staticmethod
     def _save_yaml(obj: dict, filename: PathLike):
         yaml.dump(obj, stream=open(filename, 'w'), default_flow_style=False)
 
     @staticmethod
     def _load_yaml(filename: PathLike):
         yml = yaml.load(stream=open(filename, 'r'), Loader=yaml.FullLoader)
         return yml
 
+    def _load_best_model(self, model):
+        if self._model_checkpoint_deepcopy.save_best_only:
+            model = tf.keras.models.load_model(self._model_checkpoint_new_filepath)
+        else:
+            model.load_weights(self._model_checkpoint_new_filepath)
+        return model
+
+    def _find_model_checkpoint(self, kwargs):
+        if 'callbacks' in kwargs:
+            if isinstance(kwargs['callbacks'], list):
+                callbacks = list(kwargs['callbacks'])
+                for callback in callbacks:
+                    if isinstance(callback, tf.keras.callbacks.ModelCheckpoint):
+                        self._model_checkpoint_deepcopy = copy.deepcopy(callback)
+                        kwargs['callbacks'].remove(callback)
+                        break
+            else:
+                if isinstance(kwargs['callbacks'], tf.keras.callbacks.ModelCheckpoint):
+                    self._model_checkpoint_deepcopy = copy.deepcopy(kwargs['callbacks'])
+                    kwargs['callbacks'] = []
+
     def _get_split_path(self, split_number: int):
         split_path = self.project_path.joinpath(f'split_{split_number}')
         if not split_path.exists():
             split_path.mkdir(exist_ok=True, parents=True)
         return split_path
 
     def _del_split_folders(self):
@@ -122,45 +154,56 @@
             ValueError(f"Can't find history for split {split_number}")
         self.history.append(self._load_yaml(history_yml))
         metrics_yml = split_path.joinpath('validation_metric.yml')
         if not metrics_yml.exists():
             ValueError(f"Can't find validate metrics  for split {split_number}")
         self.cv_results.append(self._load_yaml(metrics_yml))
 
-    def _prepare_data(self, x, idx: List[int], fit_transform: bool):
+    def _prepare_data(self, x: Iterable, y: Iterable, idx: List[int], fit_transform: bool):
+        y_new = y[idx]
         if self._multiple_input:
             x_new = [i[idx] for i in x]
             if self.preprocessor is not None:
-                x_new = [self.preprocess_data(x_new[i], self.preprocessor[i], fit_transform) for i in
+                x_new = [self.preprocess_data(x_new[i], y_new, self.preprocessor[i], self.supervised_preprocessor[i],
+                                              fit_transform) for i in
                          range(len(self.preprocessor))]
         else:
             x_new = x[idx]
             if self.preprocessor is not None:
-                x_new = self.preprocess_data(x_new, self.preprocessor, fit_transform)
+                x_new = self.preprocess_data(x_new, y_new, self.preprocessor, self.supervised_preprocessor,
+                                             fit_transform)
         return x_new
 
     def get_model(self):
         with maybe_distribute(self.distribution_strategy):
             model = self.model_builder(**self.params)
             return model
 
     def fit(self, x, y, **kwargs):
+        self._model_checkpoint_deepcopy = None
+        self._model_checkpoint_new_filepath = None
         self.history = []
         self.cv_results = []
         self.splits_info = []
         if self.save_history:
             self._del_split_folders()
         if isinstance(x, list):
             self._multiple_input = True
             n_sample = len(x[0])
         else:
             self._multiple_input = False
             n_sample = len(x)
+        self._find_model_checkpoint(kwargs)
         for split, (train_index, test_index) in enumerate(
                 self.cv.split(range(n_sample), y)):
+            if self._model_checkpoint_deepcopy:
+                callback = copy.deepcopy(self._model_checkpoint_deepcopy)
+                callback.filepath = self._model_checkpoint_deepcopy.filepath + f'/split_{split}'
+                self._model_checkpoint_new_filepath = callback.filepath
+                kwargs['callbacks'].append(callback)
             if self.save_history and not self.overwrite:
                 split_status = self._check_split_status(split)
                 if split_status:
                     self._load_history(split)
                     continue
             start = time.perf_counter()
             split_info = {'start_time': time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
@@ -168,42 +211,43 @@
                           'status': 'RUNNING'
                           }
             if self.save_history:
                 split_path = self._get_split_path(split_number=split)
                 self._save_yaml(split_info, split_path.joinpath('split_info.yml'))
             keras.backend.clear_session()
             if kwargs.get('verbose', 0):
-                tf.get_logger().info(
+                logger.info(
                     "\n" + "-" * 31 + "\n"
                                       f"Cross-Validation {split + 1}/{self.cv.get_n_splits()}"
                     + "\n"
                     + "-" * 31
                     + "\n"
                 )
             # prepare train data
-            x_train = self._prepare_data(x, train_index, fit_transform=True)
+            x_train = self._prepare_data(x, y, train_index, fit_transform=True)
             y_train = y[train_index]
 
             # prepare test data
-            x_test = self._prepare_data(x, test_index, fit_transform=False)
+            x_test = self._prepare_data(x, y,  test_index, fit_transform=False)
             y_test = y[test_index]
             # get model
             model = self.get_model()
-
             # train model
             history = model.fit(x_train, y_train, **kwargs)
             self.history.append(history.history)
 
-            tf.get_logger().info(
+            logger.info(
                 "\n" + "-" * 31 + "\n"
                                   "Evaluate validation performance"
                 + "\n"
                 + "-" * 31
                 + "\n"
             )
+            if self._model_checkpoint_deepcopy:
+                model = self._load_best_model(model)
             if self._custom_eval:
                 y_pred = model.predict(
                     x_test,
                     batch_size=kwargs.get('batch_size', 32),
                     verbose=kwargs.get('verbose', 0),
                 )
                 val_res = self._custom_eval(y_test, y_pred)
@@ -217,15 +261,15 @@
                     batch_size=kwargs.get('batch_size', 32),
                     return_dict=True,
                     verbose=kwargs.get('verbose', 0),
                 )
                 self.cv_results.append(val_res)
             val_res['split'] = split
             end = round(time.perf_counter() - start, 1)
-            tf.get_logger().info(
+            logger.info(
                 "\n" + "-" * 31 + "\n"
                                   f"Split {split + 1}/{self.cv.get_n_splits()} time took: {end} s."
                 + "\n"
             )
 
             split_info['status'] = 'OK'
             split_info['end_time'] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
```

### Comparing `keras_model_cv-0.3.1/keras_model_cv.egg-info/PKG-INFO` & `keras_model_cv-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: keras-model-cv
-Version: 0.3.1
+Name: keras_model_cv
+Version: 0.5.4
 Summary: Cross-validation for keras models
 Home-page: https://github.com/dubovikmaster/keras-model-cv
 Author: Pavel Dubovik
 Author-email: geometryk@gmail.com
 License: MIT
 Keywords: keras cross-validate,validation keras modelscross-validation
 Platform: any
```

### Comparing `keras_model_cv-0.3.1/setup.py` & `keras_model_cv-0.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="keras_model_cv",
-    version="0.3.1",
+    version="0.5.4",
     description="Cross-validation for keras models",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files="LICENSE",
     dec="README.md",
     author="Pavel Dubovik",
```

