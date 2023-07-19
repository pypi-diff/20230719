# Comparing `tmp/ei_cli-0.3.0.tar.gz` & `tmp/ei_cli-0.3.1.tar.gz`

## Comparing `ei_cli-0.3.0.tar` & `ei_cli-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ei_cli-0.3.0/codecov.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 ei_cli-0.3.0/requirements-dev.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ei_cli-0.3.0/requirements.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.github/workflows/ci-py310.yml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.github/workflows/ci-py311.yml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.github/workflows/ci-py37.yml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.github/workflows/ci-py38.yml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.github/workflows/ci-py39.yml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0    87795 2020-02-02 00:00:00.000000 ei_cli-0.3.0/assets/ei.png
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/__init__.py
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/cli.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/concurrency.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/defaults.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/exceptions.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/fields.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/service.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/session.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/table.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/aws/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/aws/ec2.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/aws/elasticache.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/aws/elb.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/aws/rds.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/services/aws/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/cli/__init__.py
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/cli/ec2.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/cli/elasticache.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/cli/elb.py
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/cli/rds.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ei_cli-0.3.0/ei/views/cli/s3.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ei_cli-0.3.0/scripts/_utils.sh
--rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 ei_cli-0.3.0/scripts/publish.sh
--rwxr-xr-x   0        0        0      939 2020-02-02 00:00:00.000000 ei_cli-0.3.0/scripts/release.sh
--rwxr-xr-x   0        0        0      549 2020-02-02 00:00:00.000000 ei_cli-0.3.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/core/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/core/test_cli.py
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/core/test_fields.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/core/test_service.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/core/test_utils.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 ei_cli-0.3.0/tests/mocks/app.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ei_cli-0.3.0/.gitignore
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 ei_cli-0.3.0/README.md
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ei_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 ei_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ei_cli-0.3.1/codecov.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 ei_cli-0.3.1/requirements-dev.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ei_cli-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.github/workflows/ci-py310.yml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.github/workflows/ci-py311.yml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.github/workflows/ci-py37.yml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.github/workflows/ci-py38.yml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.github/workflows/ci-py39.yml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0    87795 2020-02-02 00:00:00.000000 ei_cli-0.3.1/assets/ei.png
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/__init__.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/cli.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/concurrency.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/defaults.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/exceptions.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/fields.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/service.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/session.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/table.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/aws/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/aws/ec2.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/aws/elasticache.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/aws/elb.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/aws/rds.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/services/aws/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/cli/__init__.py
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/cli/ec2.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/cli/elasticache.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/cli/elb.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/cli/rds.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ei_cli-0.3.1/ei/views/cli/s3.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ei_cli-0.3.1/scripts/_utils.sh
+-rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 ei_cli-0.3.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0      939 2020-02-02 00:00:00.000000 ei_cli-0.3.1/scripts/release.sh
+-rwxr-xr-x   0        0        0      549 2020-02-02 00:00:00.000000 ei_cli-0.3.1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/core/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/core/test_cli.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/core/test_fields.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/core/test_service.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/core/test_utils.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 ei_cli-0.3.1/tests/mocks/app.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ei_cli-0.3.1/.gitignore
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 ei_cli-0.3.1/README.md
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ei_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 ei_cli-0.3.1/PKG-INFO
```

### Comparing `ei_cli-0.3.0/.github/workflows/ci-py311.yml` & `ei_cli-0.3.1/.github/workflows/ci-py311.yml`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/assets/ei.png` & `ei_cli-0.3.1/assets/ei.png`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/core/cli.py` & `ei_cli-0.3.1/ei/core/cli.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/core/concurrency.py` & `ei_cli-0.3.1/ei/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/core/defaults.py` & `ei_cli-0.3.1/ei/core/defaults.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/core/fields.py` & `ei_cli-0.3.1/ei/core/fields.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/core/service.py` & `ei_cli-0.3.1/ei/core/service.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/core/session.py` & `ei_cli-0.3.1/ei/core/session.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/services/aws/ec2.py` & `ei_cli-0.3.1/ei/services/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/services/aws/elasticache.py` & `ei_cli-0.3.1/ei/services/aws/elasticache.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/services/aws/elb.py` & `ei_cli-0.3.1/ei/services/aws/elb.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/services/aws/s3.py` & `ei_cli-0.3.1/ei/services/aws/s3.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/views/cli/ec2.py` & `ei_cli-0.3.1/ei/views/cli/ec2.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/views/cli/elasticache.py` & `ei_cli-0.3.1/ei/views/cli/elasticache.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/views/cli/elb.py` & `ei_cli-0.3.1/ei/views/cli/elb.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/views/cli/rds.py` & `ei_cli-0.3.1/ei/views/cli/rds.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/ei/views/cli/s3.py` & `ei_cli-0.3.1/ei/views/cli/s3.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/scripts/release.sh` & `ei_cli-0.3.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/scripts/test.sh` & `ei_cli-0.3.1/scripts/test.sh`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/tests/core/test_cli.py` & `ei_cli-0.3.1/tests/core/test_cli.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/tests/core/test_fields.py` & `ei_cli-0.3.1/tests/core/test_fields.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/tests/core/test_service.py` & `ei_cli-0.3.1/tests/core/test_service.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/tests/mocks/app.py` & `ei_cli-0.3.1/tests/mocks/app.py`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/README.md` & `ei_cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/pyproject.toml` & `ei_cli-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ei_cli-0.3.0/PKG-INFO` & `ei_cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ei-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: aws cli for human
 Project-URL: Documentation, https://github.com/unknown/ei#readme
 Project-URL: Issues, https://github.com/unknown/ei/issues
 Project-URL: Source, https://github.com/unknown/ei
 Author-email: Ashon <ashon8813@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

