# Comparing `tmp/iam_actions-1.2.20230718.tar.gz` & `tmp/iam_actions-1.2.20230719.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230718.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230719.tar", max compression
```

## Comparing `iam_actions-1.2.20230718.tar` & `iam_actions-1.2.20230719.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/README.md
--rw-r--r--   0        0        0      228 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/__init__.py
--rw-r--r--   0        0        0  4368912 2023-07-18 02:55:51.602837 iam_actions-1.2.20230718/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-18 02:54:12.541356 iam_actions-1.2.20230718/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-18 02:54:12.545357 iam_actions-1.2.20230718/iam_actions/generate/services.py
--rw-r--r--   0        0        0   561929 2023-07-18 02:55:51.602837 iam_actions-1.2.20230718/iam_actions/policies.json
--rw-r--r--   0        0        0   197396 2023-07-18 02:55:51.602837 iam_actions-1.2.20230718/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   545040 2023-07-18 02:55:51.602837 iam_actions-1.2.20230718/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-18 02:55:52.418848 iam_actions-1.2.20230718/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230718/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230718/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/README.md
+-rw-r--r--   0        0        0      228 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4369576 2023-07-19 03:40:05.090111 iam_actions-1.2.20230719/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-19 03:38:35.232917 iam_actions-1.2.20230719/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   561944 2023-07-19 03:40:05.090111 iam_actions-1.2.20230719/iam_actions/policies.json
+-rw-r--r--   0        0        0   197396 2023-07-19 03:40:05.090111 iam_actions-1.2.20230719/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   545054 2023-07-19 03:40:05.090111 iam_actions-1.2.20230719/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-19 03:40:05.878121 iam_actions-1.2.20230719/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230719/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230719/PKG-INFO
```

### Comparing `iam_actions-1.2.20230718/LICENSE` & `iam_actions-1.2.20230719/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/README.md` & `iam_actions-1.2.20230719/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/actions.json` & `iam_actions-1.2.20230719/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999414745655346%*

 * *Differences: {"'dms'": "{'GetMetadataModel': {'description': 'Grants permission to list all of the AWS DMS "*

 * *          'attributes for a metadata model. Note. Despite this action requires '*

 * *          'StartMetadataModelImport, the latter does not currently authorize the described Schema '*

 * *          "Conversion operation'}, 'ListMetadataModelAssessmentActionItems': {'description': "*

 * *          "'Grants permission to list the AWS DMS attributes for a metadata model assessment "*

 * *          'action items. Note. Despite this a […]*

```diff
@@ -40141,15 +40141,15 @@
                 "MigrationProject"
             ]
         },
         "GetMetadataModel": {
             "access_level": "Read",
             "action": "GetMetadataModel",
             "condition_keys": [],
-            "description": "Grants permission to list all of the AWS DMS attributes for a metadata model",
+            "description": "Grants permission to list all of the AWS DMS attributes for a metadata model. Note. Despite this action requires StartMetadataModelImport, the latter does not currently authorize the described Schema Conversion operation",
             "orphan": false,
             "resources": [
                 "MigrationProject"
             ]
         },
         "ImportCertificate": {
             "access_level": "Write",
@@ -40192,15 +40192,15 @@
                 "InstanceProfile"
             ]
         },
         "ListMetadataModelAssessmentActionItems": {
             "access_level": "Read",
             "action": "ListMetadataModelAssessmentActionItems",
             "condition_keys": [],
-            "description": "Grants permission to list the AWS DMS attributes for a metadata model assessment action items",
+            "description": "Grants permission to list the AWS DMS attributes for a metadata model assessment action items. Note. Despite this action requires StartMetadataModelImport, the latter does not currently authorize the described Schema Conversion operation",
             "orphan": false,
             "resources": [
                 "MigrationProject"
             ]
         },
         "ListMetadataModelAssessments": {
             "access_level": "Read",
@@ -40232,15 +40232,15 @@
                 "MigrationProject"
             ]
         },
         "ListMigrationProjects": {
             "access_level": "Read",
             "action": "ListMigrationProjects",
             "condition_keys": [],
-            "description": "Grants permission to list the AWS DMS attributes for a migration projects",
+            "description": "Grants permission to list the AWS DMS attributes for a migration projects. Note. Despite this action requires DescribeMigrationProjects and DescribeConversionConfiguration, both required actions do not currently authorize the described Schema Conversion operation",
             "orphan": false,
             "resources": [
                 "DataProvider",
                 "InstanceProfile",
                 "MigrationProject"
             ]
         },
@@ -102129,14 +102129,22 @@
             "condition_keys": [],
             "description": "Grants permission to return a list of all ActiveMQ users",
             "orphan": false,
             "resources": [
                 "brokers"
             ]
         },
+        "Promote": {
+            "access_level": "Undocumented",
+            "action": "Promote",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RebootBroker": {
             "access_level": "Write",
             "action": "RebootBroker",
             "condition_keys": [],
             "description": "Grants permission to reboot a broker",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230718/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230719/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230719/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/generate/generate.py` & `iam_actions-1.2.20230719/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230719/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230719/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/generate/services.py` & `iam_actions-1.2.20230719/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/policies.json` & `iam_actions-1.2.20230719/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999995443277925%*

 * *Differences: {"'serviceMap'": "{'Amazon MQ': {'Actions': {insert: [(19, 'Promote')]}}}"}*

```diff
@@ -15776,14 +15776,15 @@
                 "DescribeConfigurationRevision",
                 "DescribeUser",
                 "ListBrokers",
                 "ListConfigurationRevisions",
                 "ListConfigurations",
                 "ListTags",
                 "ListUsers",
+                "Promote",
                 "RebootBroker",
                 "UpdateBroker",
                 "UpdateConfiguration",
                 "UpdateUser"
             ],
             "HasResource": true,
             "StringPrefix": "mq",
```

### Comparing `iam_actions-1.2.20230718/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230719/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230718/iam_actions/services.json` & `iam_actions-1.2.20230719/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999952304639805%*

 * *Differences: {"'mq'": "{'Actions': {insert: [(19, 'Promote')]}}"}*

```diff
@@ -14272,14 +14272,15 @@
             "DescribeConfigurationRevision",
             "DescribeUser",
             "ListBrokers",
             "ListConfigurationRevisions",
             "ListConfigurations",
             "ListTags",
             "ListUsers",
+            "Promote",
             "RebootBroker",
             "UpdateBroker",
             "UpdateConfiguration",
             "UpdateUser"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230718/pyproject.toml` & `iam_actions-1.2.20230719/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230718"
+version = "1.2.20230719"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230718/setup.py` & `iam_actions-1.2.20230719/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230718',
+    'version': '1.2.20230719',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230718/PKG-INFO` & `iam_actions-1.2.20230719/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230718
+Version: 1.2.20230719
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

