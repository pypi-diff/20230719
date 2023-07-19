# Comparing `tmp/raspi_gpio-0.1.7.tar.gz` & `tmp/raspi_gpio-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.7.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.8.tar", max compression
```

## Comparing `raspi_gpio-0.1.7.tar` & `raspi_gpio-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-01 03:19:43.247951 raspi_gpio-0.1.7/LICENSE
--rw-r--r--   0        0        0      270 2023-07-01 03:19:43.247951 raspi_gpio-0.1.7/README.md
--rw-r--r--   0        0        0      741 2023-07-01 03:20:07.257930 raspi_gpio-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-07-01 03:19:43.247951 raspi_gpio-0.1.7/raspi_gpio/GPIO_mock.py
--rw-r--r--   0        0        0      268 2023-07-01 03:19:43.247951 raspi_gpio-0.1.7/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      715 2023-07-01 03:19:43.247951 raspi_gpio-0.1.7/raspi_gpio/spidev_mock.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 12:53:45.951187 raspi_gpio-0.1.8/LICENSE
+-rw-r--r--   0        0        0      270 2023-07-19 12:53:45.951187 raspi_gpio-0.1.8/README.md
+-rw-r--r--   0        0        0      741 2023-07-19 12:54:08.591309 raspi_gpio-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-07-19 12:53:45.955186 raspi_gpio-0.1.8/raspi_gpio/GPIO_mock.py
+-rw-r--r--   0        0        0      311 2023-07-19 12:53:45.955186 raspi_gpio-0.1.8/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      715 2023-07-19 12:53:45.955186 raspi_gpio-0.1.8/raspi_gpio/spidev_mock.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.8/PKG-INFO
```

### Comparing `raspi_gpio-0.1.7/LICENSE` & `raspi_gpio-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.7/pyproject.toml` & `raspi_gpio-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raspi-gpio"
-version = "0.1.7"
+version = "0.1.8"
 description = "RPi.GPIO wrapper with mocks for developmennt on any platform"
 authors = ["Mark Parker <mark@parker-programs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "raspi_gpio"}]
 homepage = "https://pypi.org/project/raspi-gpio/"
 repository = "https://github.com/MarkParker5/raspi-gpio"
```

### Comparing `raspi_gpio-0.1.7/raspi_gpio/GPIO_mock.py` & `raspi_gpio-0.1.8/raspi_gpio/GPIO_mock.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.7/raspi_gpio/spidev_mock.py` & `raspi_gpio-0.1.8/raspi_gpio/spidev_mock.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.7/PKG-INFO` & `raspi_gpio-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-gpio
-Version: 0.1.7
+Version: 0.1.8
 Summary: RPi.GPIO wrapper with mocks for developmennt on any platform
 Home-page: https://pypi.org/project/raspi-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,rpi,rpi-gpio,RPi.GPIO
 Author: Mark Parker
 Author-email: mark@parker-programs.com
 Requires-Python: >=3.10,<4.0
```

