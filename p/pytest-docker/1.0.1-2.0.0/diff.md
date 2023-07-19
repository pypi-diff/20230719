# Comparing `tmp/pytest-docker-1.0.1.tar.gz` & `tmp/pytest-docker-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-docker-1.0.1.tar", last modified: Wed Sep 14 15:18:48 2022, max compression
+gzip compressed data, was "pytest-docker-2.0.0.tar", last modified: Wed Jul 19 11:57:28 2023, max compression
```

## Comparing `pytest-docker-1.0.1.tar` & `pytest-docker-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:18:48.706017 pytest-docker-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-14 15:18:32.000000 pytest-docker-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2022-09-14 15:18:48.706017 pytest-docker-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-09-14 15:18:32.000000 pytest-docker-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-14 15:18:32.000000 pytest-docker-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-09-14 15:18:48.706017 pytest-docker-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 15:18:32.000000 pytest-docker-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:18:48.698017 pytest-docker-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:18:48.702017 pytest-docker-1.0.1/src/pytest_docker/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-14 15:18:32.000000 pytest-docker-1.0.1/src/pytest_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-09-14 15:18:32.000000 pytest-docker-1.0.1/src/pytest_docker/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:18:48.706017 pytest-docker-1.0.1/src/pytest_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2022-09-14 15:18:48.000000 pytest-docker-1.0.1/src/pytest_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-14 15:18:48.000000 pytest-docker-1.0.1/src/pytest_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 15:18:48.000000 pytest-docker-1.0.1/src/pytest_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-14 15:18:48.000000 pytest-docker-1.0.1/src/pytest_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-14 15:18:48.000000 pytest-docker-1.0.1/src/pytest_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-14 15:18:48.000000 pytest-docker-1.0.1/src/pytest_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:57:28.638912 pytest-docker-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-19 11:57:28.638912 pytest-docker-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-19 11:57:28.638912 pytest-docker-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:57:28.630912 pytest-docker-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:57:28.634912 pytest-docker-2.0.0/src/pytest_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/src/pytest_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/src/pytest_docker/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:57:28.638912 pytest-docker-2.0.0/src/pytest_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-19 11:57:28.000000 pytest-docker-2.0.0/src/pytest_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-19 11:57:28.000000 pytest-docker-2.0.0/src/pytest_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:57:28.000000 pytest-docker-2.0.0/src/pytest_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-19 11:57:28.000000 pytest-docker-2.0.0/src/pytest_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-19 11:57:28.000000 pytest-docker-2.0.0/src/pytest_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 11:57:28.000000 pytest-docker-2.0.0/src/pytest_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:57:28.638912 pytest-docker-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/tests/test_docker_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/tests/test_docker_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/tests/test_dockercomposeexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-19 11:57:09.000000 pytest-docker-2.0.0/tests/test_integration.py
```

### Comparing `pytest-docker-1.0.1/LICENSE.txt` & `pytest-docker-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-docker-1.0.1/PKG-INFO` & `pytest-docker-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-docker
-Version: 1.0.1
-Summary: Simple pytest fixtures for Docker and docker-compose based tests
+Version: 2.0.0
+Summary: Simple pytest fixtures for Docker and Docker Compose based tests
 Home-page: https://github.com/avast/pytest-docker
 Author: Max K., Andre Caron
 Author-email: maxim.kovykov@avast.com
 License: MIT
 Keywords: docker,docker-compose,pytest
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
@@ -30,48 +31,45 @@
 [![Build Status](https://github.com/avast/pytest-docker/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/avast/pytest-docker/actions/workflows/tests.yaml)
 [![Python versions](https://img.shields.io/pypi/pyversions/pytest-docker)](https://pypi.org/project/pytest-docker/)
 [![Code style](https://img.shields.io/badge/formatted%20with-black-black)](https://github.com/psf/black)
 
 
 # Description
 Simple [pytest](http://doc.pytest.org/) fixtures that help you write integration
-tests with Docker and [docker-compose](https://docs.docker.com/compose/).
+tests with Docker and [Docker Compose](https://docs.docker.com/compose/).
 Specify all necessary containers in a `docker-compose.yml` file and and
 `pytest-docker` will spin them up for the duration of your tests.
 
 This package is tested with Python versions `3.6`, `3.7`, `3.8` and
 `3.9`, and `pytest` version 4, 5 and 6. Python 2 is not supported.
 
 `pytest-docker` was originally created by André Caron.
 
 # Installation
-Install `pytest-docker` with `pip` or add it to your test requirements. It is
-recommended to install `docker-compose` python package directly in your
-environment to ensure that it is available during tests. This will prevent
-potential dependency conflicts that can occur when the system wide
-`docker-compose` is used in tests.
-
-The default behavior is not to install `docker-compose` with `pytest-docker`. If you
-want to, you install `pytest-docker` with the `docker-compose-v1`
-extra. You can use the following command:
+Install `pytest-docker` with `pip` or add it to your test requirements.
 
+By default, it uses the `docker compose` command, so it relies on the Compose plugin for Docker (also called Docker Compose V2).
+
+## Docker Compose V1 compatibility
+
+If you want to use the old `docker-compose` command (deprecated since July 2023, not receiving updates since 2021)
+ then you can do it using the [`docker-compose-command`](#docker_compose_command) fixture:
+
+```python
+@pytest.fixture(scope="session")
+def docker_compose_command() -> str:
+    return "docker-compose"
+```
+
+If you want to use the pip-distributed version of `docker-compose` command, you can install it using
 ```
 pip install pytest-docker[docker-compose-v1]
 ```
 
-## Docker Compose v2 compatiblity
-
-`pytest-docker` will work with Docker Compose v2 out of the box if
-[`compose-switch`](https://github.com/docker/compose-switch)
-is installed.
-
-If you want to use the real Docker Compose v2, it has to be installed
-system wide ([more information](https://github.com/docker/compose#linux))
-and you have to modify the [`docker-compose-command`](#docker_compose_command)
-fixture (this behavior might change in the future versions).
+Another option could be usage of [`compose-switch`](https://github.com/docker/compose-switch).
 
 # Usage
 Here is an example of a test that depends on a HTTP service.
 
 With a `docker-compose.yml` file like this (using the
 [httpbin](https://httpbin.org/) service):
 
@@ -157,16 +155,16 @@
 
 Start all services from the docker compose file (`docker-compose up`).
 After test are finished, shutdown all services (`docker-compose down`).
 
 ### `docker_compose_command`
 
 Docker Compose command to use to execute Dockers. Default is to use
-Docker Compose v1 (command is `docker-compose`). If you want to use
-Docker Compose v2, change this fixture to return `docker compose`.
+Docker Compose V2 (command is `docker compose`). If you want to use
+Docker Compose V1, change this fixture to return `docker-compose`.
 
 ### `docker_setup`
 
 Get the docker_compose command to be executed for test spawn actions.
 Override this fixture in your tests if you need to change spawn actions.
 Returning anything that would evaluate to False will skip this command.
```

### Comparing `pytest-docker-1.0.1/README.md` & `pytest-docker-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 [![Build Status](https://github.com/avast/pytest-docker/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/avast/pytest-docker/actions/workflows/tests.yaml)
 [![Python versions](https://img.shields.io/pypi/pyversions/pytest-docker)](https://pypi.org/project/pytest-docker/)
 [![Code style](https://img.shields.io/badge/formatted%20with-black-black)](https://github.com/psf/black)
 
 
 # Description
 Simple [pytest](http://doc.pytest.org/) fixtures that help you write integration
-tests with Docker and [docker-compose](https://docs.docker.com/compose/).
+tests with Docker and [Docker Compose](https://docs.docker.com/compose/).
 Specify all necessary containers in a `docker-compose.yml` file and and
 `pytest-docker` will spin them up for the duration of your tests.
 
 This package is tested with Python versions `3.6`, `3.7`, `3.8` and
 `3.9`, and `pytest` version 4, 5 and 6. Python 2 is not supported.
 
 `pytest-docker` was originally created by André Caron.
 
 # Installation
-Install `pytest-docker` with `pip` or add it to your test requirements. It is
-recommended to install `docker-compose` python package directly in your
-environment to ensure that it is available during tests. This will prevent
-potential dependency conflicts that can occur when the system wide
-`docker-compose` is used in tests.
-
-The default behavior is not to install `docker-compose` with `pytest-docker`. If you
-want to, you install `pytest-docker` with the `docker-compose-v1`
-extra. You can use the following command:
+Install `pytest-docker` with `pip` or add it to your test requirements.
 
+By default, it uses the `docker compose` command, so it relies on the Compose plugin for Docker (also called Docker Compose V2).
+
+## Docker Compose V1 compatibility
+
+If you want to use the old `docker-compose` command (deprecated since July 2023, not receiving updates since 2021)
+ then you can do it using the [`docker-compose-command`](#docker_compose_command) fixture:
+
+```python
+@pytest.fixture(scope="session")
+def docker_compose_command() -> str:
+    return "docker-compose"
+```
+
+If you want to use the pip-distributed version of `docker-compose` command, you can install it using
 ```
 pip install pytest-docker[docker-compose-v1]
 ```
 
-## Docker Compose v2 compatiblity
-
-`pytest-docker` will work with Docker Compose v2 out of the box if
-[`compose-switch`](https://github.com/docker/compose-switch)
-is installed.
-
-If you want to use the real Docker Compose v2, it has to be installed
-system wide ([more information](https://github.com/docker/compose#linux))
-and you have to modify the [`docker-compose-command`](#docker_compose_command)
-fixture (this behavior might change in the future versions).
+Another option could be usage of [`compose-switch`](https://github.com/docker/compose-switch).
 
 # Usage
 Here is an example of a test that depends on a HTTP service.
 
 With a `docker-compose.yml` file like this (using the
 [httpbin](https://httpbin.org/) service):
 
@@ -131,16 +128,16 @@
 
 Start all services from the docker compose file (`docker-compose up`).
 After test are finished, shutdown all services (`docker-compose down`).
 
 ### `docker_compose_command`
 
 Docker Compose command to use to execute Dockers. Default is to use
-Docker Compose v1 (command is `docker-compose`). If you want to use
-Docker Compose v2, change this fixture to return `docker compose`.
+Docker Compose V2 (command is `docker compose`). If you want to use
+Docker Compose V1, change this fixture to return `docker-compose`.
 
 ### `docker_setup`
 
 Get the docker_compose command to be executed for test spawn actions.
 Override this fixture in your tests if you need to change spawn actions.
 Returning anything that would evaluate to False will skip this command.
```

### Comparing `pytest-docker-1.0.1/setup.cfg` & `pytest-docker-2.0.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = pytest-docker
-version = 1.0.1
-description = Simple pytest fixtures for Docker and docker-compose based tests
+version = 2.0.0
+description = Simple pytest fixtures for Docker and Docker Compose based tests
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = docker,docker-compose,pytest
 url = https://github.com/avast/pytest-docker
 author = Max K., Andre Caron
 author_email = maxim.kovykov@avast.com
 license = MIT
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Topic :: Utilities
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: POSIX
 	Operating System :: Microsoft :: Windows
```

### Comparing `pytest-docker-1.0.1/src/pytest_docker/plugin.py` & `pytest-docker-2.0.0/src/pytest_docker/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,19 +127,19 @@
             command += ' -f "{}"'.format(compose_file)
         command += ' -p "{}" {}'.format(self._compose_project_name, subcommand)
         return execute(command)
 
 
 @pytest.fixture(scope="session")
 def docker_compose_command():
-    """Docker Compose command to use, it could be either `docker-compose`
-    for Docker Compose v1 or `docker compose` for Docker Compose
-    v2."""
+    """Docker Compose command to use, it could be either `docker compose`
+    for Docker Compose V2 or `docker-compose` for Docker Compose
+    V1."""
 
-    return "docker-compose"
+    return "docker compose"
 
 
 @pytest.fixture(scope="session")
 def docker_compose_file(pytestconfig):
     """Get an absolute path to the  `docker-compose.yml` file. Override this
     fixture in your tests if you need a custom location."""
```

### Comparing `pytest-docker-1.0.1/src/pytest_docker.egg-info/PKG-INFO` & `pytest-docker-2.0.0/src/pytest_docker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-docker
-Version: 1.0.1
-Summary: Simple pytest fixtures for Docker and docker-compose based tests
+Version: 2.0.0
+Summary: Simple pytest fixtures for Docker and Docker Compose based tests
 Home-page: https://github.com/avast/pytest-docker
 Author: Max K., Andre Caron
 Author-email: maxim.kovykov@avast.com
 License: MIT
 Keywords: docker,docker-compose,pytest
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
@@ -30,48 +31,45 @@
 [![Build Status](https://github.com/avast/pytest-docker/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/avast/pytest-docker/actions/workflows/tests.yaml)
 [![Python versions](https://img.shields.io/pypi/pyversions/pytest-docker)](https://pypi.org/project/pytest-docker/)
 [![Code style](https://img.shields.io/badge/formatted%20with-black-black)](https://github.com/psf/black)
 
 
 # Description
 Simple [pytest](http://doc.pytest.org/) fixtures that help you write integration
-tests with Docker and [docker-compose](https://docs.docker.com/compose/).
+tests with Docker and [Docker Compose](https://docs.docker.com/compose/).
 Specify all necessary containers in a `docker-compose.yml` file and and
 `pytest-docker` will spin them up for the duration of your tests.
 
 This package is tested with Python versions `3.6`, `3.7`, `3.8` and
 `3.9`, and `pytest` version 4, 5 and 6. Python 2 is not supported.
 
 `pytest-docker` was originally created by André Caron.
 
 # Installation
-Install `pytest-docker` with `pip` or add it to your test requirements. It is
-recommended to install `docker-compose` python package directly in your
-environment to ensure that it is available during tests. This will prevent
-potential dependency conflicts that can occur when the system wide
-`docker-compose` is used in tests.
-
-The default behavior is not to install `docker-compose` with `pytest-docker`. If you
-want to, you install `pytest-docker` with the `docker-compose-v1`
-extra. You can use the following command:
+Install `pytest-docker` with `pip` or add it to your test requirements.
 
+By default, it uses the `docker compose` command, so it relies on the Compose plugin for Docker (also called Docker Compose V2).
+
+## Docker Compose V1 compatibility
+
+If you want to use the old `docker-compose` command (deprecated since July 2023, not receiving updates since 2021)
+ then you can do it using the [`docker-compose-command`](#docker_compose_command) fixture:
+
+```python
+@pytest.fixture(scope="session")
+def docker_compose_command() -> str:
+    return "docker-compose"
+```
+
+If you want to use the pip-distributed version of `docker-compose` command, you can install it using
 ```
 pip install pytest-docker[docker-compose-v1]
 ```
 
-## Docker Compose v2 compatiblity
-
-`pytest-docker` will work with Docker Compose v2 out of the box if
-[`compose-switch`](https://github.com/docker/compose-switch)
-is installed.
-
-If you want to use the real Docker Compose v2, it has to be installed
-system wide ([more information](https://github.com/docker/compose#linux))
-and you have to modify the [`docker-compose-command`](#docker_compose_command)
-fixture (this behavior might change in the future versions).
+Another option could be usage of [`compose-switch`](https://github.com/docker/compose-switch).
 
 # Usage
 Here is an example of a test that depends on a HTTP service.
 
 With a `docker-compose.yml` file like this (using the
 [httpbin](https://httpbin.org/) service):
 
@@ -157,16 +155,16 @@
 
 Start all services from the docker compose file (`docker-compose up`).
 After test are finished, shutdown all services (`docker-compose down`).
 
 ### `docker_compose_command`
 
 Docker Compose command to use to execute Dockers. Default is to use
-Docker Compose v1 (command is `docker-compose`). If you want to use
-Docker Compose v2, change this fixture to return `docker compose`.
+Docker Compose V2 (command is `docker compose`). If you want to use
+Docker Compose V1, change this fixture to return `docker-compose`.
 
 ### `docker_setup`
 
 Get the docker_compose command to be executed for test spawn actions.
 Override this fixture in your tests if you need to change spawn actions.
 Returning anything that would evaluate to False will skip this command.
```

