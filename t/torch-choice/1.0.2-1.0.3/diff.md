# Comparing `tmp/torch_choice-1.0.2.tar.gz` & `tmp/torch_choice-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_choice-1.0.2.tar", last modified: Mon May 15 17:07:20 2023, max compression
+gzip compressed data, was "torch_choice-1.0.3.tar", last modified: Wed Jul 19 02:36:56 2023, max compression
```

## Comparing `torch_choice-1.0.2.tar` & `torch_choice-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.759558 torch_choice-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-05-15 17:07:20.759558 torch_choice-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-05-15 17:07:07.000000 torch_choice-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:07:20.759558 torch_choice-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-15 17:07:07.000000 torch_choice-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-15 17:07:07.000000 torch_choice-1.0.2/tests/test_choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-15 17:07:07.000000 torch_choice-1.0.2/tests/test_conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-15 17:07:07.000000 torch_choice-1.0.2/tests/test_nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice/data/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/example_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/joint_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice/model/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/formula_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/model/nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.759558 torch_choice-1.0.2/torch_choice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/easy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/run_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/run_helper_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-15 17:07:07.000000 torch_choice-1.0.2/torch_choice/utils/std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:07:20.755557 torch_choice-1.0.2/torch_choice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 17:07:20.000000 torch_choice-1.0.2/torch_choice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-19 02:36:41.000000 torch_choice-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-19 02:36:56.030014 torch_choice-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-19 02:36:41.000000 torch_choice-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:36:56.030014 torch_choice-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-19 02:36:41.000000 torch_choice-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-19 02:36:41.000000 torch_choice-1.0.3/tests/test_choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-19 02:36:41.000000 torch_choice-1.0.3/tests/test_conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-07-19 02:36:41.000000 torch_choice-1.0.3/tests/test_nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23807 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/example_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/joint_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/formula_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/model/nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/easy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/run_helper_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-19 02:36:41.000000 torch_choice-1.0.3/torch_choice/utils/std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:36:56.030014 torch_choice-1.0.3/torch_choice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 02:36:56.000000 torch_choice-1.0.3/torch_choice.egg-info/top_level.txt
```

### Comparing `torch_choice-1.0.2/PKG-INFO` & `torch_choice-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: torch_choice
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Pytorch Backend Library for Choice Modelling
-Home-page: 
-Author: Tianyu Du
+Home-page: https://gsbdbi.github.io/torch-choice/
+Author: Tianyu Du, Ayush Kanodia, and Susan Athey
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Torch-Choice: A PyTorch Package for Large-Scale Choice Modelling with Python
 [![Downloads](https://static.pepy.tech/badge/torch-choice)](https://pepy.tech/project/torch-choice)
 [![Downloads](https://static.pepy.tech/badge/torch-choice/month)](https://pepy.tech/project/torch-choice)
 [![Downloads](https://static.pepy.tech/badge/torch-choice/week)](https://pepy.tech/project/torch-choice)
 
 > Authors: Tianyu Du, Ayush Kanodia and Susan Athey; Contact: tianyudu@stanford.edu
@@ -39,15 +40,15 @@
 
 3. The package leverage GPU acceleration using PyTorch and easily scale to large dataset of millions of choice records. All models are trained using state-of-the-art optimizers by in PyTorch. These optimization algorithms are tested to be scalable by modern machine learning practitioners. However, you can rest assure that the package runs flawlessly when no GPU is used as well.
 
 4. Setting up the PyTorch training pipelines can be frustrating. We provide easy-to-use [PyTorch lightning](https://www.pytorchlightning.ai) wrapper of models to free researchers from the hassle from setting up PyTorch optimizers and training loops.
 
 
 ## Installation
-We offer two ways to install the package. This is a work in progress. We recommend installing the package from source to get the latest version and bug-fix patches.
+We offer two ways to install the package. This is a work in progress. **We recommend installing the package from source to get the latest version and bug-fix patches**.
 We are actively working on this package and will be adding more features and examples. Please feel free to reach out to us with any questions or suggestions.
 
 ### Installation from Pip
 Simply run `pip install torch-choice` to install the package. This will install the latest *stable* version of the package.
 
 ### Installation from Source
 For those wish to leverage the latest feature, you can install `torch-choice` from Github source.
```

### Comparing `torch_choice-1.0.2/README.md` & `torch_choice-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 3. The package leverage GPU acceleration using PyTorch and easily scale to large dataset of millions of choice records. All models are trained using state-of-the-art optimizers by in PyTorch. These optimization algorithms are tested to be scalable by modern machine learning practitioners. However, you can rest assure that the package runs flawlessly when no GPU is used as well.
 
 4. Setting up the PyTorch training pipelines can be frustrating. We provide easy-to-use [PyTorch lightning](https://www.pytorchlightning.ai) wrapper of models to free researchers from the hassle from setting up PyTorch optimizers and training loops.
 
 
 ## Installation
-We offer two ways to install the package. This is a work in progress. We recommend installing the package from source to get the latest version and bug-fix patches.
+We offer two ways to install the package. This is a work in progress. **We recommend installing the package from source to get the latest version and bug-fix patches**.
 We are actively working on this package and will be adding more features and examples. Please feel free to reach out to us with any questions or suggestions.
 
 ### Installation from Pip
 Simply run `pip install torch-choice` to install the package. This will install the latest *stable* version of the package.
 
 ### Installation from Source
 For those wish to leverage the latest feature, you can install `torch-choice` from Github source.
```

### Comparing `torch_choice-1.0.2/setup.py` & `torch_choice-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,30 +7,39 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="torch_choice",
-    version="1.0.2",
+    version="1.0.3",
     description="A Pytorch Backend Library for Choice Modelling",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="",
-    author="Tianyu Du",
+    url="https://gsbdbi.github.io/torch-choice/",
+    author="Tianyu Du, Ayush Kanodia, and Susan Athey",
     author_email="tianyudu@stanford.edu",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     # packages=["torch_choice"],
     packages=setuptools.find_packages(),
     include_package_data=True,
     # install_requires=["torch"],
+    install_requires=[
+        "numpy>=1.22",
+        "termcolor>=1.1.0",
+        "scikit-learn",
+        "pandas>=1.4.3",
+        "tabulate>=0.8.10",
+        "torch>=1.12.0",
+        "pytorch-lightning>=1.6.3",
+    ]
     # entry_points={
     #     "console_scripts": [
     #         "realpython=.__main__:main",
     #     ]
     # },
 )
```

### Comparing `torch_choice-1.0.2/tests/test_choice_dataset.py` & `torch_choice-1.0.3/tests/test_choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/tests/test_conditional_logit_model.py` & `torch_choice-1.0.3/tests/test_conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/tests/test_nested_logit_model.py` & `torch_choice-1.0.3/tests/test_nested_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/data/choice_dataset.py` & `torch_choice-1.0.3/torch_choice/data/choice_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -373,68 +373,84 @@
         return key.startswith('item_') and (key != 'item_availability') and (key != 'item_index')
 
     @staticmethod
     def _is_user_attribute(key: str) -> bool:
         return key.startswith('user_') and (key != 'user_index')
 
     @staticmethod
-    def _is_session_attribute(key: str) -> bool:
-        return key.startswith('session_') and (key != 'session_index')
+    def _is_useritem_attribute(key: str) -> bool:
+        return key.startswith('useritem_')
 
     @staticmethod
-    def _is_taste_attribute(key: str) -> bool:
-        return key.startswith('taste_')
+    def _is_session_attribute(key: str) -> bool:
+        return key.startswith('session_') and (key != 'session_index')
 
     @staticmethod
     def _is_price_attribute(key: str) -> bool:
         return key.startswith('price_') or key.startswith('itemsession_')
 
+    @staticmethod
+    def _is_usersessionitem_attribute(key: str) -> bool:
+        return key.startswith('usersessionitem_')
+
     def _is_attribute(self, key: str) -> bool:
         return self._is_item_attribute(key) \
             or self._is_user_attribute(key) \
+            or self._is_useritem_attribute(key) \
             or self._is_session_attribute(key) \
-            or self._is_taste_attribute(key) \
-            or self._is_price_attribute(key)
+            or self._is_price_attribute(key) \
+            or self._is_usersessionitem_attribute(key)
+
 
     def _expand_tensor(self, key: str, val: torch.Tensor) -> torch.Tensor:
-        """Expands attribute tensor to (num_sessions, num_items, num_params) shape for prediction tasks, this method
+        """Expands attribute tensor to (len(self), num_items, num_params) shape for prediction tasks, this method
         won't reshape the tensor at all if the `key` (i.e., name of the tensor) suggests its not an attribute of any kind.
 
         Args:
             key (str): name of the attribute used to determine the raw shape of the tensor. For example, 'item_obs' means
                 the raw tensor is in shape (num_items, num_params).
             val (torch.Tensor): the attribute tensor to be reshaped.
 
         Returns:
             torch.Tensor: the reshaped tensor with shape (num_sessions, num_items, num_params).
         """
         if not self._is_attribute(key):
-            print(f'Warning: the input key {key} is not an attribute of the dataset, will NOT modify the provided tensor.')
-            # don't expand non-attribute tensors, if any.
-            return val
+            # this is a sanity check.
+            raise ValueError(f'Warning: the input key {key} is not an attribute of the dataset, will NOT modify the provided tensor.')
+
+        num_params = val.shape[-1]  # the number of parameters/coefficients/observables.
 
-        num_params = val.shape[-1]
+        # convert attribute tensors to (len(self), num_items, num_params) shape.
         if self._is_user_attribute(key):
             # user_attribute (num_users, *)
             out = val[self.user_index, :].view(
                 len(self), 1, num_params).expand(-1, self.num_items, -1)
         elif self._is_item_attribute(key):
             # item_attribute (num_items, *)
             out = val.view(1, self.num_items, num_params).expand(
                 len(self), -1, -1)
+        elif self._is_useritem_attribute(key):
+            # useritem_attribute (num_users, num_items, *)
+            out = val[self.user_index, :, :]
         elif self._is_session_attribute(key):
             # session_attribute (num_sessions, *)
             out = val[self.session_index, :].view(
                 len(self), 1, num_params).expand(-1, self.num_items, -1)
-        elif self._is_taste_attribute(key):
-            # taste_attribute (num_users, num_items, *)
-            out = val[self.user_index, :, :]
+        # elif self._is_taste_attribute(key):
+        #     # taste_attribute (num_users, num_items, *)
+        #     out = val[self.user_index, :, :]
         elif self._is_price_attribute(key):
             # price_attribute (num_sessions, num_items, *)
             out = val[self.session_index, :, :]
+        elif self._is_usersessionitem_attribute(key):
+            # usersessionitem_attribute has shape (num_users, num_sessions, num_items, *)
+            out = val[self.user_index, self.session_index, :, :]  # (len(self), num_items, *)
+
+        else:
+            raise ValueError(f'Warning: the input key {key} is not an attribute of the dataset, will NOT modify the provided tensor.')
 
         assert out.shape == (len(self), self.num_items, num_params)
         return out
 
     @staticmethod
     def unique(tensor: torch.Tensor) -> Tuple[np.ndarray]:
         arr = tensor.cpu().numpy()
@@ -477,11 +493,11 @@
         summary.append(string)
 
         summary.append('Attribute Summaries:')
         for key, item in self.__dict__.items():
             if self._is_attribute(key) and torch.is_tensor(item):
                 summary.append("Observable Tensor '{}' with shape {}".format(key, item.shape))
                 # price attributes are 3-dimensional tensors, ignore  for cleanness here.
-                if not self._is_price_attribute(key):
+                if (not self._is_price_attribute(key)) and (not self._is_usersessionitem_attribute(key)) and (not self._is_useritem_attribute(key)):
                     summary.append(str(pd.DataFrame(item.to('cpu').float().numpy()).describe()))
         print('\n'.join(summary) + f"\ndevice={self.device}")
         return None
```

### Comparing `torch_choice-1.0.2/torch_choice/data/example_datasets.py` & `torch_choice-1.0.3/torch_choice/data/example_datasets.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/data/joint_dataset.py` & `torch_choice-1.0.3/torch_choice/data/joint_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/data/utils.py` & `torch_choice-1.0.3/torch_choice/data/utils.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/model/coefficient.py` & `torch_choice-1.0.3/torch_choice/model/coefficient.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/model/conditional_logit_model.py` & `torch_choice-1.0.3/torch_choice/model/conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/model/formula_parser.py` & `torch_choice-1.0.3/torch_choice/model/formula_parser.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/model/nested_logit_model.py` & `torch_choice-1.0.3/torch_choice/model/nested_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/utils/easy_data_wrapper.py` & `torch_choice-1.0.3/torch_choice/utils/easy_data_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,28 @@
                  item_name_column: str,
                  choice_column: str,
                  user_index_column: Optional[str] = None,
                  session_index_column: Optional[str] = None,
                  # Option 1: feed in data-frames of observables.
                  user_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  item_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
+                 useritem_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  session_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  price_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  itemsession_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
+                 useritemsession_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  # Option 2: derive observables from columns of main_data.
                  user_observable_columns: Optional[List[str]] = None,
                  item_observable_columns: Optional[List[str]] = None,
+                 useritem_observable_columns: Optional[List[str]] = None,
                  session_observable_columns: Optional[List[str]] = None,
                  price_observable_columns: Optional[List[str]] = None,
                  itemsession_observable_columns: Optional[List[str]] = None,
+                 useritemsession_observable_columns: Optional[List[str]] = None,
+                 # Misc.
                  device: str = 'cpu'):
         """The initialization method of EasyDatasetWrapper.
 
         Args:
             main_data (pd.DataFrame): the main dataset holding all purchase records in a "long-format", each row of the
                 dataset is an item in a purchase record.
                 The main_data data-frame should contains the following columns:
@@ -84,14 +89,17 @@
 
             The itemsession_observable_column is an alias for the `price_observable_column` argument for backward compatibility,
                 all elements of `itemsession_observable_columns` will be appended to `price_observable_column`.
 
         Raises:
             ValueError: _description_
         """
+        if (useritem_observable_data is not None) or (useritemsession_observable_data is not None) or (useritem_observable_columns is not None) or (useritemsession_observable_columns is not None):
+            raise NotImplementedError("The user-item and user-item-session observables are not yet supported in easy data wrapper. Please construct ChoiceDataset objects directly with tensors using the ChoiceDataset class to include these observables.")
+
         # read in data.
         self.main_data = main_data
         self.purchase_record_column = purchase_record_column
         # in alphabetical order of purchase record indices.
         # this is kept internally.
         self.purchase_record_index = main_data[purchase_record_column].unique()
         self.item_name_column = item_name_column
```

### Comparing `torch_choice-1.0.2/torch_choice/utils/run_helper.py` & `torch_choice-1.0.3/torch_choice/utils/run_helper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice/utils/run_helper_lightning.py` & `torch_choice-1.0.3/torch_choice/utils/run_helper_lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,28 +81,30 @@
         dataset_test: Optional[ChoiceDataset]=None,
         model_optimizer: str='Adam',
         batch_size: int=-1,
         learning_rate: float=0.01,
         num_epochs: int=10,
         num_workers: int=0,
         device: Optional[str]=None,
+        report_std: bool=True,
         **kwargs) -> Union[ConditionalLogitModel, NestedLogitModel]:
     """_summary_
 
     Args:
         model (Union[ConditionalLogitModel, NestedLogitModel]): the constructed model.
         dataset_train (ChoiceDataset): the dataset for training.
         dataset_val (ChoiceDataset): an optional dataset for validation.
         dataset_test (ChoiceDataset): an optional dataset for testing.
         batch_size (int, optional): batch size for model training. Defaults to -1.
         learning_rate (float, optional): learning rate for model training. Defaults to 0.01.
         num_epochs (int, optional): number of epochs for the training. Defaults to 10.
         num_workers (int, optional): number of parallel workers for data loading. Defaults to 0.
         device (Optional[str], optional): the device that trains the model, if None is specified, the function will
             use the current device of the provided model. Defaults to None.
+        report_std (bool, optional): whether to report standard error for the estimated parameters. Defaults to True.
         **kwargs: other keyword arguments for the pytorch lightning trainer, this is for users with experience in
             pytorch lightning and wish to customize the training process.
 
     Returns:
         Union[ConditionalLogitModel, NestedLogitModel]: the trained model.
     """
     # ==================================================================================================================
@@ -146,26 +148,29 @@
     # ==================================================================================================================
     # if the validation dataset is provided, do early stopping.
     callbacks = [EarlyStopping(monitor="val_ll", mode="max", patience=10, min_delta=0.001)] if val_dataloader is not None else []
 
     trainer = pl.Trainer(accelerator="cuda" if "cuda" in device else device,  # note: "cuda:0" is not a accelerator name.
                          devices="auto",
                          max_epochs=num_epochs,
-                         check_val_every_n_epoch=num_epochs // 100,
-                         log_every_n_steps=num_epochs // 100,
+                         check_val_every_n_epoch=max(num_epochs // 100, 1),
+                         log_every_n_steps=max(num_epochs // 100, 1),
                          callbacks=callbacks,
                          **kwargs)
     start_time = time.time()
-    trainer.fit(lightning_model, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader)
+    trainer.fit(lightning_model, train_dataloader, val_dataloader)
     print(f'Time taken for training: {time.time() - start_time}')
     if test_dataloader is not None:
-        trainer.test(lightning_model, test_dataloaders=test_dataloader)
+        trainer.test(lightning_model, test_dataloader)
     else:
         print('Skip testing, no test dataset is provided.')
 
+    if not report_std:
+        return model
+
     # ==================================================================================================================
     # Construct standard error, z-value, and p-value of coefficients.
     # ==================================================================================================================
     # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
     state_dict = deepcopy(lightning_model.model.state_dict())
     model_clone.load_state_dict(state_dict)
 
@@ -191,16 +196,17 @@
     report = list()
     for coef_name, std in std_dict.items():
         std = std.cpu().detach().numpy()
         mean = mean_dict[coef_name].cpu().detach().numpy()
         coef_name = coef_name.replace('coef_dict.', '').replace('.coef', '')
         for i in range(mean.size):
             report.append({'Coefficient': coef_name + f'_{i}',
-                           'Estimation': float(mean[i]),
-                           'Std. Err.': float(std[i])})
+                           'Estimation': float(mean.reshape(-1,)[i]),
+                           'Std. Err.': float(std.reshape(-1,)[i])
+                           })
     report = pd.DataFrame(report).set_index('Coefficient')
 
     # Compute z-value
     report['z-value'] = report['Estimation'] / report['Std. Err.']
 
     # Compute p-value (two tails).
     report['Pr(>|z|)'] = (1 - norm.cdf(abs(report['z-value']))) * 2
```

### Comparing `torch_choice-1.0.2/torch_choice/utils/std.py` & `torch_choice-1.0.3/torch_choice/utils/std.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.2/torch_choice.egg-info/PKG-INFO` & `torch_choice-1.0.3/torch_choice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: torch-choice
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Pytorch Backend Library for Choice Modelling
-Home-page: 
-Author: Tianyu Du
+Home-page: https://gsbdbi.github.io/torch-choice/
+Author: Tianyu Du, Ayush Kanodia, and Susan Athey
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Torch-Choice: A PyTorch Package for Large-Scale Choice Modelling with Python
 [![Downloads](https://static.pepy.tech/badge/torch-choice)](https://pepy.tech/project/torch-choice)
 [![Downloads](https://static.pepy.tech/badge/torch-choice/month)](https://pepy.tech/project/torch-choice)
 [![Downloads](https://static.pepy.tech/badge/torch-choice/week)](https://pepy.tech/project/torch-choice)
 
 > Authors: Tianyu Du, Ayush Kanodia and Susan Athey; Contact: tianyudu@stanford.edu
@@ -39,15 +40,15 @@
 
 3. The package leverage GPU acceleration using PyTorch and easily scale to large dataset of millions of choice records. All models are trained using state-of-the-art optimizers by in PyTorch. These optimization algorithms are tested to be scalable by modern machine learning practitioners. However, you can rest assure that the package runs flawlessly when no GPU is used as well.
 
 4. Setting up the PyTorch training pipelines can be frustrating. We provide easy-to-use [PyTorch lightning](https://www.pytorchlightning.ai) wrapper of models to free researchers from the hassle from setting up PyTorch optimizers and training loops.
 
 
 ## Installation
-We offer two ways to install the package. This is a work in progress. We recommend installing the package from source to get the latest version and bug-fix patches.
+We offer two ways to install the package. This is a work in progress. **We recommend installing the package from source to get the latest version and bug-fix patches**.
 We are actively working on this package and will be adding more features and examples. Please feel free to reach out to us with any questions or suggestions.
 
 ### Installation from Pip
 Simply run `pip install torch-choice` to install the package. This will install the latest *stable* version of the package.
 
 ### Installation from Source
 For those wish to leverage the latest feature, you can install `torch-choice` from Github source.
```

### Comparing `torch_choice-1.0.2/torch_choice.egg-info/SOURCES.txt` & `torch_choice-1.0.3/torch_choice.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+LICENSE
 README.md
 setup.py
 tests/test_choice_dataset.py
 tests/test_conditional_logit_model.py
 tests/test_nested_logit_model.py
 torch_choice/__init__.py
 torch_choice.egg-info/PKG-INFO
 torch_choice.egg-info/SOURCES.txt
 torch_choice.egg-info/dependency_links.txt
+torch_choice.egg-info/requires.txt
 torch_choice.egg-info/top_level.txt
 torch_choice/data/__init__.py
 torch_choice/data/choice_dataset.py
 torch_choice/data/example_datasets.py
 torch_choice/data/joint_dataset.py
 torch_choice/data/utils.py
 torch_choice/model/__init__.py
```

