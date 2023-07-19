# Comparing `tmp/autotrain-advanced-0.5.7.tar.gz` & `tmp/autotrain-advanced-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.5.7.tar", last modified: Tue Jul 18 10:49:53 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.5.8.tar", last modified: Tue Jul 18 11:39:03 2023, max compression
```

## Comparing `autotrain-advanced-0.5.7.tar` & `autotrain-advanced-0.5.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.360645 autotrain-advanced-0.5.7/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.7/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-18 10:49:53.360645 autotrain-advanced-0.5.7/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.7/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-18 10:49:53.360645 autotrain-advanced-0.5.7/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.7/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.356645 autotrain-advanced-0.5.7/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.356645 autotrain-advanced-0.5.7/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-18 10:49:48.000000 autotrain-advanced-0.5.7/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.5.7/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.356645 autotrain-advanced-0.5.7/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.7/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.7/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.7/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.5.7/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14109 2023-07-11 10:08:31.000000 autotrain-advanced-0.5.7/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.7/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.7/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.7/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.7/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.7/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.356645 autotrain-advanced-0.5.7/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.7/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.7/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.7/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.7/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.7/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.7/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.7/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.7/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.356645 autotrain-advanced-0.5.7/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9966 2023-07-11 12:12:06.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/clm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5525 2023-07-13 15:02:50.000000 autotrain-advanced-0.5.7/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.7/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 10:49:53.360645 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-18 10:49:53.000000 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1223 2023-07-18 10:49:53.000000 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-18 10:49:53.000000 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-18 10:49:53.000000 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2849 2023-07-18 10:49:53.000000 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-18 10:49:53.000000 autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.041414 autotrain-advanced-0.5.8/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.8/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-18 11:39:03.041414 autotrain-advanced-0.5.8/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.8/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-18 11:39:03.041414 autotrain-advanced-0.5.8/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.8/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.037414 autotrain-advanced-0.5.8/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.037414 autotrain-advanced-0.5.8/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-18 11:38:59.000000 autotrain-advanced-0.5.8/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.5.8/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.037414 autotrain-advanced-0.5.8/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.8/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.8/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.8/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.5.8/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14456 2023-07-18 11:15:05.000000 autotrain-advanced-0.5.8/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.8/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.8/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.8/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.8/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.8/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.037414 autotrain-advanced-0.5.8/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.8/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.8/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.8/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.8/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.8/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.8/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.8/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.8/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.037414 autotrain-advanced-0.5.8/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9955 2023-07-18 11:12:58.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/clm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-18 11:14:03.000000 autotrain-advanced-0.5.8/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.8/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-18 11:39:03.041414 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-18 11:39:02.000000 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1223 2023-07-18 11:39:03.000000 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-18 11:39:02.000000 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-18 11:39:02.000000 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2849 2023-07-18 11:39:02.000000 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-18 11:39:02.000000 autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.5.7/LICENSE` & `autotrain-advanced-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/PKG-INFO` & `autotrain-advanced-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.7
+Version: 0.5.8
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.7/setup.py` & `autotrain-advanced-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/__init__.py` & `autotrain-advanced-0.5.8/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Lint as: python3
 # pylint: enable=line-too-long
 
-__version__ = "0.5.7"
+__version__ = "0.5.8"
```

### Comparing `autotrain-advanced-0.5.7/src/autotrain/app.py` & `autotrain-advanced-0.5.8/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.5.8/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.5.8/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.5.8/src/autotrain/cli/run_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         args.fp16,
         args.push_to_hub,
         args.use_int8,
         args.model_max_length,
         args.repo_id,
         args.use_int4,
         args.trainer,
+        args.target_modules,
     )
 
 
 class RunAutoTrainLLMCommand(BaseAutoTrainCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         run_llm_parser = parser.add_parser(
@@ -320,14 +321,21 @@
         run_llm_parser.add_argument(
             "--trainer",
             help="Trainer type to use",
             required=False,
             type=str,
             default="default",
         )
+        run_llm_parser.add_argument(
+            "--target_modules",
+            help="Target modules to use",
+            required=False,
+            type=str,
+            default=None,
+        )
 
         run_llm_parser.set_defaults(func=run_llm_command_factory)
 
     def __init__(
         self,
         train,
         deploy,
@@ -365,14 +373,15 @@
         fp16,
         push_to_hub,
         use_int8,
         model_max_length,
         repo_id,
         use_int4,
         trainer,
+        target_modules,
     ):
         self.train = train
         self.deploy = deploy
         self.inference = inference
         self.data_path = data_path
         self.train_split = train_split
         self.valid_split = valid_split
@@ -406,14 +415,15 @@
         self.fp16 = fp16
         self.push_to_hub = push_to_hub
         self.use_int8 = use_int8
         self.model_max_length = model_max_length
         self.repo_id = repo_id
         self.use_int4 = use_int4
         self.trainer = trainer
+        self.target_modules = target_modules
 
         if self.train:
             if self.project_name is None:
                 raise ValueError("Project name must be specified")
             if self.data_path is None:
                 raise ValueError("Data path must be specified")
             if self.model is None:
@@ -460,9 +470,10 @@
                 fp16=self.fp16,
                 push_to_hub=self.push_to_hub,
                 use_int8=self.use_int8,
                 model_max_length=self.model_max_length,
                 repo_id=self.repo_id,
                 use_int4=self.use_int4,
                 trainer=self.trainer,
+                target_modules=self.target_modules,
             )
             train_llm(params)
```

### Comparing `autotrain-advanced-0.5.7/src/autotrain/dataset.py` & `autotrain-advanced-0.5.8/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/help.py` & `autotrain-advanced-0.5.8/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/params.py` & `autotrain-advanced-0.5.8/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.5.8/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.5.8/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.5.8/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.5.8/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/project.py` & `autotrain-advanced-0.5.8/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/tasks.py` & `autotrain-advanced-0.5.8/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/clm.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             model = prepare_model_for_int8_training(model)
         peft_config = LoraConfig(
             r=config.lora_r,
             lora_alpha=config.lora_alpha,
             lora_dropout=config.lora_dropout,
             bias="none",
             task_type="CAUSAL_LM",
-            target_modules=utils.TARGET_MODULES.get(config.model_name),
+            target_modules=utils.get_target_modules(config),
         )
         model = get_peft_model(model, peft_config)
 
     if config.block_size == -1:
         config.block_size = None
 
     if config.block_size is None:
```

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/dreambooth.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.5.8/src/autotrain/trainers/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,21 @@
     fp16: bool = Field(False, title="FP16")
     push_to_hub: bool = Field(False, title="Push to hub")
     use_int8: bool = Field(False, title="Use int8")
     model_max_length: int = Field(1024, title="Model max length")
     repo_id: str = Field(None, title="Repo id")
     use_int4: bool = Field(False, title="Use int4")
     trainer: str = Field("default", title="Trainer type")
+    target_modules: str = Field(None, title="Target modules")
+
+
+def get_target_modules(config):
+    if config.target_modules is None:
+        return TARGET_MODULES.get(config.model_name)
+    return config.target_modules.split(",")
 
 
 def process_data(data, tokenizer, config):
     data = data.to_pandas()
     data = data.fillna("")
 
     data = data[[config.text_column]]
```

### Comparing `autotrain-advanced-0.5.7/src/autotrain/utils.py` & `autotrain-advanced-0.5.8/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.7
+Version: 0.5.8
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.7/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.5.8/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

