# Comparing `tmp/streamingcli-1.9.1.tar.gz` & `tmp/streamingcli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamingcli-1.9.1.tar", last modified: Thu Mar  2 10:16:59 2023, max compression
+gzip compressed data, was "streamingcli-2.0.0.tar", last modified: Wed Jul 19 07:38:30 2023, max compression
```

## Comparing `streamingcli-1.9.1.tar` & `streamingcli-2.0.0.tar`

### file list

```diff
@@ -1,86 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-02 10:16:53.000000 streamingcli-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-02 10:16:53.000000 streamingcli-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-02 10:16:59.856937 streamingcli-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-02 10:16:53.000000 streamingcli-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-02 10:16:59.000000 streamingcli-1.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-02 10:16:59.856937 streamingcli-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-02 10:16:53.000000 streamingcli-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.848937 streamingcli-1.9.1/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.848937 streamingcli-1.9.1/streamingcli/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/docker/login_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/docker_response_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/jupyter/jar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/jupyter/notebook_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/apitoken_create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/apitoken_remove_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/deployment_target_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/platform/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/secret_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/platform/ververica/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/apitoken_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/deployment_target_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/profile/profile_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/profile/profile_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/cicd_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/deploy_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/project/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/jupyter/jupyter_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/local_project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/project_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/publish_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/project/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/python/python_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/template_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/streamingcli/project/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/deployment_target.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/flink_app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/k8s_flink_deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/vvp_flink_deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/yaml_merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.848937 streamingcli-1.9.1/streamingcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/jupyter/test_notebook_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/profile/test_profile_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/project/test_yaml_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/test_k82_deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/test_k8s_secret_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 07:38:19.000000 streamingcli-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 07:38:19.000000 streamingcli-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 07:38:30.318848 streamingcli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-19 07:38:19.000000 streamingcli-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-19 07:38:29.000000 streamingcli-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 07:38:30.318848 streamingcli-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-19 07:38:19.000000 streamingcli-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.302847 streamingcli-2.0.0/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.302847 streamingcli-2.0.0/streamingcli/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/docker/login_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/docker_response_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.306847 streamingcli-2.0.0/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/jupyter/jar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/jupyter/notebook_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.306847 streamingcli-2.0.0/streamingcli/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/jinja_prettifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.306847 streamingcli-2.0.0/streamingcli/platform/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/k8s/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/k8s/deployment_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.310848 streamingcli-2.0.0/streamingcli/platform/ververica/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/ververica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/ververica/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/platform/ververica/deployment_target_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.310848 streamingcli-2.0.0/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/profile/profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/deploy_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/jupyter/jupyter_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/local_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/publish_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/python/python_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/template_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/streamingcli/project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/templates/flink_app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-19 07:38:19.000000 streamingcli-2.0.0/streamingcli/project/yaml_merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.302847 streamingcli-2.0.0/streamingcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 07:38:30.000000 streamingcli-2.0.0/streamingcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.314848 streamingcli-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/jupyter/test_notebook_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/profile/test_profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:30.318848 streamingcli-2.0.0/tests/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/project/test_yaml_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/test_k82_deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-19 07:38:19.000000 streamingcli-2.0.0/tests/streamingcli/test_vvp_deployment_adapter.py
```

### Comparing `streamingcli-1.9.1/LICENSE` & `streamingcli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/requirements.txt` & `streamingcli-2.0.0/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 -i https://pypi.org/simple
-attrs==22.2.0 ; python_version >= '3.6'
+attrs==22.2.0; python_version >= '3.6'
 autopep8==2.0.1
-cachetools==5.2.1 ; python_version ~= '3.7'
-certifi==2022.12.7 ; python_version >= '3.6'
-charset-normalizer==3.0.1 ; python_version >= '3.6'
+cachetools==5.2.1; python_version ~= '3.7'
+certifi==2022.12.7; python_version >= '3.6'
+charset-normalizer==3.0.1; python_version >= '3.6'
 click==8.1.3
-colorama==0.4.6 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
+colorama==0.4.6; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
 copier==2.5.1
 dataclasses-json==0.5.7
 docker==6.0.1
 fastjsonschema==2.16.2
-google-auth==2.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+google-auth==2.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 hiyapyco==0.4.16
-idna==3.4 ; python_version >= '3.5'
+idna==3.4; python_version >= '3.5'
 importlib-metadata==6.0.0
-importlib-resources==5.10.2 ; python_version < '3.9'
+importlib-resources==5.10.2; python_version < '3.9'
 jinja2==2.11.3
-jsonschema==4.17.3 ; python_version >= '3.7'
-jupyter-core==5.1.3 ; python_version >= '3.8'
+jsonschema==4.17.3; python_version >= '3.7'
+jupyter-core==5.1.3; python_version >= '3.8'
 kubernetes==25.3.0
 markupsafe==2.0.1
 marshmallow==3.19.0
 marshmallow-dataclass==8.5.11
 marshmallow-enum==1.5.1
 mypy-extensions==0.4.3
 nbformat==5.7.3
-oauthlib==3.2.2 ; python_version >= '3.6'
-packaging==23.0 ; python_version >= '3.7'
-pkgutil-resolve-name==1.3.10 ; python_version < '3.9'
-platformdirs==2.6.2 ; python_version >= '3.7'
+oauthlib==3.2.2; python_version >= '3.6'
+packaging==23.0; python_version >= '3.7'
+pkgutil-resolve-name==1.3.10; python_version < '3.9'
+platformdirs==2.6.2; python_version >= '3.7'
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
-pycodestyle==2.10.0 ; python_version >= '3.6'
-pyrsistent==0.19.3 ; python_version >= '3.7'
+pycodestyle==2.10.0; python_version >= '3.6'
+pyrsistent==0.19.3; python_version >= '3.7'
 python-dateutil==2.8.0
 pyyaml==6.0
 requests==2.28.2
-requests-oauthlib==1.3.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-rsa==4.9 ; python_version >= '3.6'
-ruamel.yaml==0.17.21 ; python_version >= '3'
-ruamel.yaml.clib==0.2.7 ; python_version < '3.11' and platform_python_implementation == 'CPython'
+requests-oauthlib==1.3.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+rsa==4.9; python_version >= '3.6'
+ruamel.yaml==0.17.21; python_version >= '3'
+ruamel.yaml.clib==0.2.7; python_version < '3.11' and platform_python_implementation == 'CPython'
 setuptools==66.0.0
-six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 sqlparse==0.4.3
-toml==0.10.2 ; python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'
-tomli==2.0.1 ; python_version < '3.11'
-traitlets==5.8.1 ; python_version >= '3.7'
-typing-extensions==4.4.0 ; python_version >= '3.7'
+toml==0.10.2; python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'
+tomli==2.0.1; python_version < '3.11'
+traitlets==5.8.1; python_version >= '3.7'
+typing-extensions==4.4.0; python_version >= '3.7'
 typing-inspect==0.8.0
-urllib3==1.26.14 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
-websocket-client==1.4.2 ; python_version >= '3.7'
+urllib3==1.26.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+websocket-client==1.4.2; python_version >= '3.7'
 wget==3.2
 wheel==0.38.4
-zipp==3.11.0 ; python_version >= '3.7'
+zipp==3.11.0; python_version >= '3.7'
```

### Comparing `streamingcli-1.9.1/setup.cfg` & `streamingcli-2.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.1
+current_version = 2.0.0
 
 [flake8]
 exclude = .git,__pycache__,build,dist,*.yml
 max-line-length = 120
 extend-ignore = E203
 
 [mypy]
```

### Comparing `streamingcli-1.9.1/setup.py` & `streamingcli-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import List
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-__version__ = "1.9.1"
+__version__ = "2.0.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def get_requirements(filename: str) -> List[str]:
     with open(filename, "r", encoding="utf-8") as fp:
```

### Comparing `streamingcli-1.9.1/streamingcli/config.py` & `streamingcli-2.0.0/streamingcli/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from pathlib import Path
-
-PROJECT_LOCAL_CONFIG_FILE_NAME = ".streaming_config.yml"
+PROJECT_LOCAL_CONFIG_FILE_NAME = "config/general.yml"
+PROJECT_DEPLOYMENT_TEMPLATE = "config/flink_deployment.yml"
 PROJECT_K8S_CONFIGMAP_KEY = "project_configmap.json"
 PLATFORM_K8S_CONFIGMAP_NAME = "streaming-platform-config"
 PLATFORM_K8S_CONFIGMAP_KEY = "platform_config.json"
 PLATFORM_K8S_SECRET_NAME = "streaming-platform-secret"
 PLATFORM_DEFAULT_DEPLOYMENT_TARGET_NAME = "default"
-PROFILE_ENV_VARIABLE_NAME = "SCLI_PROFILE"
+PROFILE_ENV_VARIABLE_NAME = "SCLI_ENV"
 SCLI_CONFIG_DIR_NAME = ".scli"
-DEFAULT_PROFILE_DIR = f"{str(Path.home())}/{SCLI_CONFIG_DIR_NAME}"
-DEFAULT_PROFILE_PATH = f"{DEFAULT_PROFILE_DIR}/profiles.yml"
+DEFAULT_PROFILE_PATH = "config"
+DEFAULT_PROFILE = "base"
+PROFILE_CONFIG_FILE = "profile.yml"
 PYTHON_TEMPLATE_PROJECT = "PYTHON_TEMPLATE_PROJECT"
 JUPYTER_TEMPLATE_PROJECT = "JUPYTER_TEMPLATE_PROJECT"
 DEFAULT_FLINK_APP_NAME = "flink_app.py"
 DEFAULT_NOTEBOOK_NAME = "notebook.ipynb"
 ADDITIONAL_DEPENDENCIES_DIR = "/app/lib"
```

### Comparing `streamingcli-1.9.1/streamingcli/docker/login_command.py` & `streamingcli-2.0.0/streamingcli/docker/login_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 import base64
 import json
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 import click
 import docker
 from docker import auth
 from docker.utils import config
 
+from streamingcli.profile.profile_adapter import ProfileAdapter
+from streamingcli.project.deploy_command import ProjectDeployer
+
 
 class LoginCommand:
     @staticmethod
-    def docker_login(username: str, password: str, docker_registry_url: str) -> None:
+    def docker_login(
+        username: str, password: str, profile: Optional[str] = None
+    ) -> None:
+        profile_name = ProjectDeployer.get_profile_name(profile_name=profile)
+        profile_data = ProfileAdapter.get_profile(profile_name=profile_name)
+        if not profile_data.docker_registry_url:
+            raise click.ClickException("Missing docker_registry_url")
+
         client = docker.from_env()
-        client.login(username, password, registry=docker_registry_url, reauth=True)
-        click.echo(f"Successfully logged in to {docker_registry_url}")
+        client.login(
+            username, password, registry=profile_data.docker_registry_url, reauth=True
+        )
+        click.echo(f"Successfully logged in to {profile_data.docker_registry_url}")
         # it's a bit of a hack, docker-py login method does not update auth credentials in Docker config file
-        LoginCommand.update_docker_auths_config(username, password, docker_registry_url)
+        LoginCommand.update_docker_auths_config(
+            username, password, profile_data.docker_registry_url
+        )
 
     @staticmethod
     def update_docker_auths_config(
         username: str, password: str, docker_registry_url: str
     ) -> None:
         config_file = config.find_config_file()
         with open(config_file, "r+") as f:
```

### Comparing `streamingcli-1.9.1/streamingcli/docker_response_reader.py` & `streamingcli-2.0.0/streamingcli/docker_response_reader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/jupyter/jar_handler.py` & `streamingcli-2.0.0/streamingcli/jupyter/jar_handler.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/jupyter/notebook_converter.py` & `streamingcli-2.0.0/streamingcli/jupyter/notebook_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 @dataclass
 class Sql(NotebookEntry):
     value: str = ""
     type: str = "SQL"
 
 
 @dataclass
+class SqlSet(NotebookEntry):
+    value: List[str] = field(default_factory=lambda: [])
+    type: str = "SQL_SET"
+
+
+@dataclass
 class RegisterUdf(NotebookEntry):
     function_name: str = ""
     object_name: str = ""
     type: str = "REGISTER_UDF"
 
 
 @dataclass
@@ -150,14 +156,17 @@
         else:
             return []
 
     def _handle_magic_cell(
         self, cell: nbformat.NotebookNode, notebook_dir: str
     ) -> Sequence[NotebookEntry]:
         source = cell.source
+        if source.startswith("%%flink_execute_sql_set"):
+            sql_statements = "\n".join(source.split("\n")[1:])
+            return [SqlSet(value=sqlparse.split(sql_statements))]
         if source.startswith("%%flink_execute_sql"):
             sql_statement = "\n".join(source.split("\n")[1:])
             if NotebookConverter._skip_statement(sql_statement):
                 return []
             return self._convert_sql_statement_to_python_instructions(sql_statement)
         if source.startswith("%%flink_execute"):
             code = "\n".join(source.split("\n")[1:])
```

### Comparing `streamingcli-1.9.1/streamingcli/platform/deployment_adapter.py` & `streamingcli-2.0.0/streamingcli/platform/deployment_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
 from jinja2 import Environment
 
+from streamingcli.config import PROJECT_DEPLOYMENT_TEMPLATE
+from streamingcli.platform.jinja_prettifier import yaml_pretty
 from streamingcli.profile.profile_adapter import ScliProfile
 from streamingcli.project.template_loader import TemplateLoader
 
 
 class DeploymentAdapter(ABC):
     def __init__(
         self, profile_data: ScliProfile, docker_image_tag: str, project_name: str
@@ -21,19 +23,20 @@
     def deploy(self, deployment_yml: str) -> Optional[str]:
         pass
 
     @abstractmethod
     def validate_profile_data(self) -> None:
         pass
 
-    @staticmethod
-    @abstractmethod
-    def get_template_name() -> str:
-        pass
+    def generate_project_template(
+        self, dependencies: List[str], file_descriptor_path: Optional[str] = None
+    ) -> str:
+        descriptor_path = file_descriptor_path or PROJECT_DEPLOYMENT_TEMPLATE
+        template = TemplateLoader.load_project_template(descriptor_path)
 
-    def generate_project_template(self, dependencies: List[str]) -> str:
-        template = TemplateLoader.load_project_template(self.get_template_name())
         params = self.profile_data.__dict__.copy()
         params["project_name"] = self.project_name
         params["docker_image_tag"] = self.docker_image_tag
         params["dependencies"] = dependencies
-        return Environment().from_string(template).render(params)
+        env = Environment()
+        env.filters["pretty"] = yaml_pretty
+        return env.from_string(template).render(params)
```

### Comparing `streamingcli-1.9.1/streamingcli/platform/k8s/config_loader.py` & `streamingcli-2.0.0/streamingcli/platform/k8s/config_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/platform/k8s/deployment_adapter.py` & `streamingcli-2.0.0/streamingcli/platform/k8s/deployment_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,22 @@
         if stderr:
             raise click.ClickException(
                 f"Failed to kubectl apply deployment.yaml file: {str(stderr)}"
             )
         return str(stdout) if stdout else None
 
     def validate_profile_data(self) -> None:
-        if self.profile_data.k8s_namespace is None:
+        if self.profile_data.config["k8s"]["namespace"] is None:
             raise click.ClickException("Missing K8S Namespace attribute or profile")
         if self.profile_data.docker_registry_url is None:
             raise click.ClickException(
                 "Missing Docker repository URL attribute or profile"
             )
         if self.docker_image_tag is None or len(self.docker_image_tag) == 0:
             raise click.ClickException("Missing Docker image tag attribute")
 
     @staticmethod
-    def get_template_name() -> str:
-        return "k8s_flink_deployment.yml"
-
-    @staticmethod
     def _kubectl_apply(deployment_yml: str) -> Tuple[bytes, bytes]:
         cmd = subprocess.Popen(
             ["kubectl apply -f -"], stdin=subprocess.PIPE, shell=True
         )
         return cmd.communicate(bytes(deployment_yml, "utf-8"), timeout=120)
```

### Comparing `streamingcli-1.9.1/streamingcli/platform/ververica/deployment_target_adapter.py` & `streamingcli-2.0.0/streamingcli/platform/ververica/deployment_target_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/project/build_command.py` & `streamingcli-2.0.0/streamingcli/project/build_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/project/deploy_command.py` & `streamingcli-2.0.0/streamingcli/project/deploy_command.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,59 @@
 import os
 from typing import Any, Optional
 
 import click
 
-from streamingcli.config import PROFILE_ENV_VARIABLE_NAME
+from streamingcli.config import DEFAULT_PROFILE, PROFILE_ENV_VARIABLE_NAME
 from streamingcli.platform.deployment_adapter import DeploymentAdapter
 from streamingcli.platform.k8s.deployment_adapter import K8SDeploymentAdapter
 from streamingcli.platform.ververica.deployment_adapter import (
     VervericaDeploymentAdapter,
 )
-from streamingcli.profile.profile_adapter import (
-    DeploymentMode,
-    ProfileAdapter,
-    ScliProfile,
-)
+from streamingcli.profile.profile_adapter import DeploymentMode, ProfileAdapter
 from streamingcli.project.local_project_config import LocalProjectConfigIO
-from streamingcli.project.yaml_merger import YamlMerger
 
 
 class ProjectDeployer:
     @staticmethod
-    def get_profile_name(profile_name: Optional[str]) -> Optional[str]:
-        if profile_name is not None:
-            return profile_name
-        else:
-            return os.getenv(PROFILE_ENV_VARIABLE_NAME)
+    def get_profile_name(profile_name: Optional[str]) -> str:
+        return profile_name or os.getenv(PROFILE_ENV_VARIABLE_NAME) or DEFAULT_PROFILE
 
     @staticmethod
     def deploy_project(
         docker_image_tag: str,
-        docker_registry_url: Optional[str] = None,
-        docker_image_repository: Optional[str] = None,
-        profile: Optional[str] = None,
-        deployment_mode: Optional[DeploymentMode] = None,
-        ververica_url: Optional[str] = None,
-        ververica_namespace: Optional[str] = None,
-        ververica_deployment_target_name: Optional[str] = None,
+        env: Optional[str] = None,
         ververica_webtoken_secret: Optional[str] = None,
-        k8s_namespace: Optional[str] = None,
-        overrides_from_yaml: Optional[str] = None,
+        file_descriptor_path: Optional[str] = None,
     ) -> None:
 
-        profile_name = ProjectDeployer.get_profile_name(profile_name=profile)
-        if profile_name is None:
-            profile_data = ScliProfile(profile_name="temporary")
-        else:
-            profile_data = ProfileAdapter.get_profile(
-                profile_name=profile_name
-            ) or ScliProfile(profile_name="temporary")
+        profile_name = ProjectDeployer.get_profile_name(profile_name=env)
+        profile_data = ProfileAdapter.get_profile(profile_name=profile_name)
 
         local_project_config = LocalProjectConfigIO.load_project_config()
-        project_name = docker_image_repository or local_project_config.project_name
-        profile_data = ProfileAdapter.update_profile_data(
+        profile_data = ProfileAdapter.update_token(
             profile_data=profile_data,
-            deployment_mode=deployment_mode,
-            ververica_url=ververica_url,
-            ververica_namespace=ververica_namespace,
-            ververica_deployment_target_name=ververica_deployment_target_name,
             ververica_webtoken_secret=ververica_webtoken_secret,
-            docker_registry_url=docker_registry_url,
-            k8s_namespace=k8s_namespace,
         )
         deployment_adapter = DeploymentAdapterFactory.get_adapter(
             profile_data.deployment_mode,
             profile_data=profile_data,
             docker_image_tag=docker_image_tag,
-            project_name=project_name,
+            project_name=local_project_config.project_name,
         )
 
         # Generate deployment YAML
         deployment_yml = deployment_adapter.generate_project_template(
-            local_project_config.dependencies
+            local_project_config.dependencies,
+            file_descriptor_path,
         )
 
-        if overrides_from_yaml:
-            deployment_yml = YamlMerger.merge_two_yaml(
-                deployment_yml, overrides_from_yaml
-            )
-
-        click.echo(f"Deploying streaming project: {project_name} ...")
+        click.echo(
+            f"Deploying streaming project: {local_project_config.project_name} ..."
+        )
         msg = deployment_adapter.deploy(deployment_yml)
         click.echo(msg)
 
 
 class DeploymentAdapterFactory:
     @staticmethod
     def get_adapter(
```

### Comparing `streamingcli-1.9.1/streamingcli/project/jupyter/jupyter_project_factory.py` & `streamingcli-2.0.0/streamingcli/project/jupyter/jupyter_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/project/local_project_config.py` & `streamingcli-2.0.0/streamingcli/project/local_project_config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/project/publish_command.py` & `streamingcli-2.0.0/streamingcli/project/publish_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,40 +4,49 @@
 
 import click
 import docker
 from docker.client import DockerClient
 from docker.errors import DockerException
 from docker.models.images import Image
 
+from streamingcli.profile.profile_adapter import ProfileAdapter
+from streamingcli.project.deploy_command import ProjectDeployer
 from streamingcli.project.local_project_config import LocalProjectConfigIO
 
 
 @dataclass
 class UserCredentials:
     username: str = field()
     password: str
 
 
 class ProjectPublisher:
     @staticmethod
     def publish(
-        docker_repository_url: str,
+        profile: Optional[str] = None,
         docker_image_tag: Optional[str] = None,
         docker_credentials: Optional[UserCredentials] = None,
     ) -> None:
         local_project_config = LocalProjectConfigIO.load_project_config()
+        profile_name = ProjectDeployer.get_profile_name(profile_name=profile)
+        profile_data = ProfileAdapter.get_profile(profile_name=profile_name)
 
         client = docker.from_env()
         image_tag = docker_image_tag if docker_image_tag is not None else "latest"
         local_image_tag = f"{local_project_config.project_name}:{image_tag}"
-        repository_name = f"{docker_repository_url}/{local_project_config.project_name}"
+        repository_name = (
+            f"{profile_data.docker_registry_url}/{local_project_config.project_name}"
+        )
+
+        if not profile_data.docker_registry_url:
+            raise click.ClickException("Missing docker_registry_url")
 
         if docker_credentials is not None:
             ProjectPublisher.authenticate(
-                client, docker_credentials, docker_repository_url
+                client, docker_credentials, profile_data.docker_registry_url
             )
 
         image = ProjectPublisher.get_image(client, local_image_tag)
         if image is None:
             raise click.ClickException(
                 f"No project image {local_image_tag} in local registry! "
                 "Firstly build image with command 'scli project build'"
```

### Comparing `streamingcli-1.9.1/streamingcli/project/python/python_project_factory.py` & `streamingcli-2.0.0/streamingcli/project/python/python_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/streamingcli/project/templates/flink_app.py.template` & `streamingcli-2.0.0/streamingcli/project/templates/flink_app.py.template`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from pyflink.datastream import StreamExecutionEnvironment
 from pyflink.table import StreamTableEnvironment
 
 stream_env = StreamExecutionEnvironment.get_execution_environment()
 stream_env.set_parallelism(1)
 table_env = StreamTableEnvironment.create(stream_env)
+
 {% for entry in notebook_entries %}
 {% if entry.type == 'SQL' %}
 table_env.execute_sql(f"""{{entry.value}}""")
 {% endif %}
+{% if entry.type == 'SQL_SET' %}
+stmt_set = table_env.create_statement_set()
+{% for val in entry.value %}
+stmt_set.add_insert_sql(f"""{{val}}""")
+{% endfor %}
+stmt_set.execute()
+{% endif %}
 {% if entry.type == 'REGISTER_UDF' %}
 table_env.create_temporary_function("{{entry.function_name}}", {{entry.object_name}})
 {% endif %}
 {% if entry.type == 'REGISTER_JAVA_UDF' %}
 table_env.create_java_temporary_function("{{entry.function_name}}", "{{entry.object_name}}")
 {% endif %}
 {% if entry.type == 'CODE' %}
```

### Comparing `streamingcli-1.9.1/streamingcli.egg-info/SOURCES.txt` & `streamingcli-2.0.0/streamingcli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,51 +17,41 @@
 streamingcli.egg-info/top_level.txt
 streamingcli/docker/__init__.py
 streamingcli/docker/login_command.py
 streamingcli/jupyter/__init__.py
 streamingcli/jupyter/jar_handler.py
 streamingcli/jupyter/notebook_converter.py
 streamingcli/platform/__init__.py
-streamingcli/platform/apitoken_create_command.py
-streamingcli/platform/apitoken_remove_command.py
 streamingcli/platform/deployment_adapter.py
-streamingcli/platform/deployment_target_command.py
+streamingcli/platform/jinja_prettifier.py
 streamingcli/platform/k8s/__init__.py
 streamingcli/platform/k8s/config_loader.py
 streamingcli/platform/k8s/deployment_adapter.py
-streamingcli/platform/k8s/secret_adapter.py
 streamingcli/platform/ververica/__init__.py
-streamingcli/platform/ververica/apitoken_adapter.py
 streamingcli/platform/ververica/deployment_adapter.py
 streamingcli/platform/ververica/deployment_target_adapter.py
 streamingcli/profile/__init__.py
 streamingcli/profile/profile_adapter.py
-streamingcli/profile/profile_command.py
 streamingcli/project/__init__.py
 streamingcli/project/build_command.py
-streamingcli/project/cicd_command.py
 streamingcli/project/deploy_command.py
 streamingcli/project/local_project_config.py
 streamingcli/project/project_type.py
 streamingcli/project/publish_command.py
 streamingcli/project/template_loader.py
 streamingcli/project/yaml_merger.py
 streamingcli/project/jupyter/__init__.py
 streamingcli/project/jupyter/jupyter_project_factory.py
 streamingcli/project/python/__init__.py
 streamingcli/project/python/python_project_factory.py
 streamingcli/project/templates/__init__.py
-streamingcli/project/templates/deployment_target.yml
 streamingcli/project/templates/flink_app.py.template
-streamingcli/project/templates/gitlab-ci.yml
-streamingcli/project/templates/k8s_flink_deployment.yml
-streamingcli/project/templates/vvp_flink_deployment.yml
 tests/__init__.py
 tests/streamingcli/__init__.py
 tests/streamingcli/test_k82_deployment_adapter.py
-tests/streamingcli/test_k8s_secret_validation.py
+tests/streamingcli/test_vvp_deployment_adapter.py
 tests/streamingcli/jupyter/__init__.py
 tests/streamingcli/jupyter/test_notebook_converter.py
 tests/streamingcli/profile/__init__.py
 tests/streamingcli/profile/test_profile_adapter.py
 tests/streamingcli/project/__init__.py
 tests/streamingcli/project/test_yaml_merger.py
```

### Comparing `streamingcli-1.9.1/streamingcli.egg-info/requires.txt` & `streamingcli-2.0.0/streamingcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.1/tests/streamingcli/jupyter/test_notebook_converter.py` & `streamingcli-2.0.0/tests/streamingcli/jupyter/test_notebook_converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+import os
 import unittest
+from pathlib import Path
+
+import pytest
 
 from streamingcli.error import FailedToOpenNotebookFile
 from streamingcli.jupyter.notebook_converter import convert_notebook
 
 
 class TestNotebookConverter(unittest.TestCase):
     """Test converting full Jupyter Notebook with udf to Python class"""
 
+    @pytest.fixture(scope="session", autouse=True)
+    def chdir(self):
+        os.chdir(Path(__file__).parent.parent.parent.parent)
+
     def test_converter(self):
         # given
         file_path = "tests/streamingcli/resources/jupyter/notebook1.ipynb"
         # expect
         converted_notebook = convert_notebook(file_path)
         assert (
             converted_notebook.content
@@ -346,7 +354,53 @@
 
 execution_output = stream_env.from_collection(
     collection=[(1, 'aaa'), (2, 'bb'), (3, 'cccc')],
     type_info=Types.ROW([Types.INT(), Types.STRING()])
 )
 """
         )
+
+    def test_notebook_with_multiple_insert_statements(self):
+        # given
+        file_path = "tests/streamingcli/resources/jupyter/notebook8.ipynb"
+        # expect
+        converted_notebook = convert_notebook(file_path)
+        assert (
+            converted_notebook.content
+            == '''from pyflink.datastream import StreamExecutionEnvironment
+from pyflink.table import StreamTableEnvironment
+
+stream_env = StreamExecutionEnvironment.get_execution_environment()
+stream_env.set_parallelism(1)
+table_env = StreamTableEnvironment.create(stream_env)
+
+
+table_env.execute_sql(f"""CREATE TABLE source1 (
+ num INT
+) WITH (
+    'connector' = 'datagen'
+)""")
+
+
+table_env.execute_sql(f"""CREATE TABLE source2 (
+ num INT
+) WITH (
+    'connector' = 'datagen'
+)""")
+
+
+table_env.execute_sql(f"""CREATE TABLE sink (
+ num INT
+) WITH (
+    'connector' = 'blackhole'
+)""")
+
+
+stmt_set = table_env.create_statement_set()
+
+stmt_set.add_insert_sql(f"""INSERT INTO sink SELECT * FROM source1;""")
+
+stmt_set.add_insert_sql(f"""INSERT INTO sink SELECT * FROM source2;""")
+
+stmt_set.execute()
+'''
+        )
```

### Comparing `streamingcli-1.9.1/tests/streamingcli/test_k82_deployment_adapter.py` & `streamingcli-2.0.0/tests/streamingcli/test_k82_deployment_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 import copy
+import os
 import unittest
 from pathlib import Path
 
+import pytest
 from click import ClickException
 
 from streamingcli.platform.k8s.deployment_adapter import K8SDeploymentAdapter
-from streamingcli.profile.profile_adapter import DeploymentMode, ScliProfile
+from streamingcli.profile.profile_adapter import (
+    DeploymentMode,
+    ProfileAdapter,
+    ScliProfile,
+)
 
 
 class TestK8SProfileAdapter(unittest.TestCase):
     K8S_TEST_PROFILE = ScliProfile(
         profile_name="test_profile",
         deployment_mode=DeploymentMode.K8S_OPERATOR,
         docker_registry_url="docker_registry_url",
-        k8s_namespace="test_ns",
+        config={"k8s": {"namespace": "test_ns"}},
     )
     PROJECT_NAME = "test"
     DOCKER_TAG = "latest"
 
+    @pytest.fixture(scope="session", autouse=True)
+    def chdir(self):
+        os.chdir(Path(Path(__file__).parent, "resources/platform/profile_k8s"))
+
     def test_init_with_valid_profile(self):
         k8s_deployment_adapter = K8SDeploymentAdapter(
             self.K8S_TEST_PROFILE, self.DOCKER_TAG, self.PROJECT_NAME
         )
         self.assertEqual(k8s_deployment_adapter.profile_data, self.K8S_TEST_PROFILE)
         self.assertEqual(k8s_deployment_adapter.project_name, self.PROJECT_NAME)
         self.assertEqual(k8s_deployment_adapter.docker_image_tag, self.DOCKER_TAG)
 
     def test_init_with_invalid_profile(self):
         invalid_profile = copy.deepcopy(self.K8S_TEST_PROFILE)
-        invalid_profile.k8s_namespace = None
+        invalid_profile.config["k8s"]["namespace"] = None
         with self.assertRaises(ClickException):
             K8SDeploymentAdapter(invalid_profile, self.DOCKER_TAG, self.PROJECT_NAME)
 
     def test_generating_project_template(self):
         k8s_deployment_adapter = K8SDeploymentAdapter(
-            self.K8S_TEST_PROFILE, self.DOCKER_TAG, self.PROJECT_NAME
+            ProfileAdapter.get_profile("base"), self.DOCKER_TAG, self.PROJECT_NAME
         )
-        print(k8s_deployment_adapter.generate_project_template([]))
-        file_path = "tests/streamingcli/resources/platform/k8s_flink_deployment.yml"
+        result = k8s_deployment_adapter.generate_project_template([])
+        print(result)
+        file_path = "../k8s_flink_deployment.yml"
         self.assertEqual(
-            k8s_deployment_adapter.generate_project_template([]),
             Path(file_path).read_text(),
+            "\n".join([s for s in result.split("\n") if s.strip()]),
         )
```

