# Comparing `tmp/streamingcli-2.0.0.tar.gz` & `tmp/streamingcli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamingcli-2.0.0.tar", last modified: Wed Jul 19 07:38:30 2023, max compression
+gzip compressed data, was "streamingcli-2.0.1.tar", last modified: Wed Jul 19 10:03:15 2023, max compression
```

## Comparing `streamingcli-2.0.0.tar` & `streamingcli-2.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 07:38:19.000000 streamingcli-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 07:38:19.000000 streamingcli-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 07:38:30.318848 streamingcli-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-19 07:38:19.000000 streamingcli-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-19 07:38:29.000000 streamingcli-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 07:38:30.318848 streamingcli-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-19 07:38:19.000000 streamingcli-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.302847 streamingcli-2.0.0/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.302847 streamingcli-2.0.0/streamingcli/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/docker/login_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/docker_response_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.306847 streamingcli-2.0.0/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/jupyter/jar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/jupyter/notebook_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.306847 streamingcli-2.0.0/streamingcli/platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/jinja_prettifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.306847 streamingcli-2.0.0/streamingcli/platform/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/k8s/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/k8s/deployment_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.310848 streamingcli-2.0.0/streamingcli/platform/ververica/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/ververica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/ververica/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/ververica/deployment_target_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.310848 streamingcli-2.0.0/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/profile/profile_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/deploy_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/jupyter/jupyter_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/local_project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/project_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/publish_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/python/python_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/template_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/templates/flink_app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/yaml_merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.302847 streamingcli-2.0.0/streamingcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/jupyter/test_notebook_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/profile/test_profile_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/project/test_yaml_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/test_k82_deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/test_vvp_deployment_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.240241 streamingcli-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 10:03:04.000000 streamingcli-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 10:03:04.000000 streamingcli-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 10:03:15.240241 streamingcli-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-19 10:03:04.000000 streamingcli-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-19 10:03:14.000000 streamingcli-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 10:03:15.240241 streamingcli-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-19 10:03:04.000000 streamingcli-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.228241 streamingcli-2.0.1/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.232241 streamingcli-2.0.1/streamingcli/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/docker/login_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/docker_response_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.232241 streamingcli-2.0.1/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/jupyter/jar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/jupyter/notebook_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.232241 streamingcli-2.0.1/streamingcli/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/jinja_prettifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.232241 streamingcli-2.0.1/streamingcli/platform/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/k8s/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/k8s/deployment_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.232241 streamingcli-2.0.1/streamingcli/platform/ververica/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/ververica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/ververica/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/platform/ververica/deployment_target_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.236241 streamingcli-2.0.1/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/profile/profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.236241 streamingcli-2.0.1/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/deploy_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.236241 streamingcli-2.0.1/streamingcli/project/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/jupyter/jupyter_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/local_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/publish_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.236241 streamingcli-2.0.1/streamingcli/project/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/python/python_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/template_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.236241 streamingcli-2.0.1/streamingcli/project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/templates/flink_app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-19 10:03:04.000000 streamingcli-2.0.1/streamingcli/project/yaml_merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.232241 streamingcli-2.0.1/streamingcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 10:03:15.000000 streamingcli-2.0.1/streamingcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-19 10:03:15.000000 streamingcli-2.0.1/streamingcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:03:15.000000 streamingcli-2.0.1/streamingcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 10:03:15.000000 streamingcli-2.0.1/streamingcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-19 10:03:15.000000 streamingcli-2.0.1/streamingcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 10:03:15.000000 streamingcli-2.0.1/streamingcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.240241 streamingcli-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.240241 streamingcli-2.0.1/tests/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.240241 streamingcli-2.0.1/tests/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/jupyter/test_notebook_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.240241 streamingcli-2.0.1/tests/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/profile/test_profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:15.240241 streamingcli-2.0.1/tests/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/project/test_yaml_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/test_k82_deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-19 10:03:04.000000 streamingcli-2.0.1/tests/streamingcli/test_vvp_deployment_adapter.py
```

### Comparing `streamingcli-2.0.0/LICENSE` & `streamingcli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/PKG-INFO` & `streamingcli-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Streaming platform CLI
 Home-page: https://github.com/getindata/streaming-cli
 Author: GetInData
 Author-email: office@getindata.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamingcli-2.0.0/README.md` & `streamingcli-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/requirements.txt` & `streamingcli-2.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/setup.cfg` & `streamingcli-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.0
+current_version = 2.0.1
 
 [flake8]
 exclude = .git,__pycache__,build,dist,*.yml
 max-line-length = 120
 extend-ignore = E203
 
 [mypy]
```

### Comparing `streamingcli-2.0.0/setup.py` & `streamingcli-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import List
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def get_requirements(filename: str) -> List[str]:
     with open(filename, "r", encoding="utf-8") as fp:
```

### Comparing `streamingcli-2.0.0/streamingcli/config.py` & `streamingcli-2.0.1/streamingcli/config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/docker/login_command.py` & `streamingcli-2.0.1/streamingcli/docker/login_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/docker_response_reader.py` & `streamingcli-2.0.1/streamingcli/docker_response_reader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/jupyter/jar_handler.py` & `streamingcli-2.0.1/streamingcli/jupyter/jar_handler.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/jupyter/notebook_converter.py` & `streamingcli-2.0.1/streamingcli/jupyter/notebook_converter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/main.py` & `streamingcli-2.0.1/streamingcli/main.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/platform/deployment_adapter.py` & `streamingcli-2.0.1/streamingcli/platform/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/platform/k8s/config_loader.py` & `streamingcli-2.0.1/streamingcli/platform/k8s/config_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/platform/k8s/deployment_adapter.py` & `streamingcli-2.0.1/streamingcli/platform/k8s/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/platform/ververica/deployment_adapter.py` & `streamingcli-2.0.1/streamingcli/platform/ververica/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/platform/ververica/deployment_target_adapter.py` & `streamingcli-2.0.1/streamingcli/platform/ververica/deployment_target_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/profile/profile_adapter.py` & `streamingcli-2.0.1/streamingcli/profile/profile_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/build_command.py` & `streamingcli-2.0.1/streamingcli/project/build_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/deploy_command.py` & `streamingcli-2.0.1/streamingcli/project/deploy_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/jupyter/jupyter_project_factory.py` & `streamingcli-2.0.1/streamingcli/project/jupyter/jupyter_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/local_project_config.py` & `streamingcli-2.0.1/streamingcli/project/local_project_config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/publish_command.py` & `streamingcli-2.0.1/streamingcli/project/publish_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/python/python_project_factory.py` & `streamingcli-2.0.1/streamingcli/project/python/python_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/template_loader.py` & `streamingcli-2.0.1/streamingcli/project/template_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli/project/templates/flink_app.py.template` & `streamingcli-2.0.1/streamingcli/project/templates/flink_app.py.template`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli.egg-info/PKG-INFO` & `streamingcli-2.0.1/streamingcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Streaming platform CLI
 Home-page: https://github.com/getindata/streaming-cli
 Author: GetInData
 Author-email: office@getindata.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamingcli-2.0.0/streamingcli.egg-info/SOURCES.txt` & `streamingcli-2.0.1/streamingcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/streamingcli.egg-info/requires.txt` & `streamingcli-2.0.1/streamingcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/tests/streamingcli/jupyter/test_notebook_converter.py` & `streamingcli-2.0.1/tests/streamingcli/jupyter/test_notebook_converter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/tests/streamingcli/profile/test_profile_adapter.py` & `streamingcli-2.0.1/tests/streamingcli/profile/test_profile_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/tests/streamingcli/test_k82_deployment_adapter.py` & `streamingcli-2.0.1/tests/streamingcli/test_k82_deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.0/tests/streamingcli/test_vvp_deployment_adapter.py` & `streamingcli-2.0.1/tests/streamingcli/test_vvp_deployment_adapter.py`

 * *Files identical despite different names*

