# Comparing `tmp/pybenutils-3.2.3.tar.gz` & `tmp/pybenutils-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybenutils-3.2.3.tar", last modified: Wed Jul 12 12:48:40 2023, max compression
+gzip compressed data, was "pybenutils-3.3.0.tar", last modified: Wed Jul 19 09:54:21 2023, max compression
```

## Comparing `pybenutils-3.2.3.tar` & `pybenutils-3.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.362550 pybenutils-3.2.3/
--rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.2.3/LICENSE
--rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4061 2023-07-12 12:48:40.362550 pybenutils-3.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.2.3/README.md
--rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.2.3/deploy_requirements.txt
--rw-rw-rw-   0        0        0      559 2023-07-06 12:04:25.000000 pybenutils-3.2.3/deployment_checklist.md
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.302710 pybenutils-3.2.3/pybenutils/
--rw-rw-rw-   0        0        0      153 2023-07-12 12:33:03.000000 pybenutils-3.2.3/pybenutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.313681 pybenutils-3.2.3/pybenutils/amazon_boto3/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/amazon_boto3/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/amazon_boto3/amazon_obj.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.320662 pybenutils-3.2.3/pybenutils/autogui/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/autogui/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/autogui/__main__.py
--rw-rw-rw-   0        0        0     6044 2023-07-12 12:33:03.000000 pybenutils-3.2.3/pybenutils/autogui/auto_gui_cls.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.331632 pybenutils-3.2.3/pybenutils/browsers/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/chrome.py
--rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/firefox.py
--rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/selenium_utils.py
--rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/simple_browser_controller_cls.py
--rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/web_driver.py
--rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/browsers/windows_browsers_keywords.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.339611 pybenutils-3.2.3/pybenutils/network/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/download_manager.py
--rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/http_cert_info.py
--rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/s3_bucket_cls.py
--rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/network/ssh_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.354571 pybenutils-3.2.3/pybenutils/os_operations/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/__init__.py
--rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/files_and_directories.py
--rw-rw-rw-   0        0        0    18745 2023-07-06 12:12:38.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_application_control.py
--rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_input_control.py
--rw-rw-rw-   0        0        0     5506 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_operations.py
--rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/mac_popup_handler.py
--rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/os_operations/window_operations.py
--rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/useful.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.358561 pybenutils-3.2.3/pybenutils/utils_logger/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/utils_logger/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.2.3/pybenutils/utils_logger/config_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.310689 pybenutils-3.2.3/pybenutils.egg-info/
--rw-rw-rw-   0        0        0     4061 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 12:48:40.000000 pybenutils-3.2.3/pybenutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.2.3/requirements.txt
--rw-rw-rw-   0        0        0      243 2023-07-12 12:48:40.364544 pybenutils-3.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1965 2023-07-06 12:04:25.000000 pybenutils-3.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:48:40.360556 pybenutils-3.2.3/tests/
--rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.2.3/tests/test_self_import.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.024885 pybenutils-3.3.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.3.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4311 2023-07-19 09:54:21.025882 pybenutils-3.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.3.0/README.md
+-rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.3.0/deploy_requirements.txt
+-rw-rw-rw-   0        0        0      559 2023-07-06 12:04:25.000000 pybenutils-3.3.0/deployment_checklist.md
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.922160 pybenutils-3.3.0/pybenutils/
+-rw-rw-rw-   0        0        0      153 2023-07-19 08:57:33.000000 pybenutils-3.3.0/pybenutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.952080 pybenutils-3.3.0/pybenutils/amazon_boto3/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/amazon_boto3/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/amazon_boto3/amazon_obj.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.960061 pybenutils-3.3.0/pybenutils/autogui/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/autogui/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/autogui/__main__.py
+-rw-rw-rw-   0        0        0     6044 2023-07-19 08:57:24.000000 pybenutils-3.3.0/pybenutils/autogui/auto_gui_cls.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.979010 pybenutils-3.3.0/pybenutils/browsers/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/chrome.py
+-rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/firefox.py
+-rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/selenium_utils.py
+-rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/simple_browser_controller_cls.py
+-rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/web_driver.py
+-rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/windows_browsers_keywords.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.990976 pybenutils-3.3.0/pybenutils/network/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/download_manager.py
+-rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/http_cert_info.py
+-rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/s3_bucket_cls.py
+-rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/ssh_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.013914 pybenutils-3.3.0/pybenutils/os_operations/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/__init__.py
+-rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/files_and_directories.py
+-rw-rw-rw-   0        0        0    18804 2023-07-19 08:57:33.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_application_control.py
+-rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_input_control.py
+-rw-rw-rw-   0        0        0     5506 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_operations.py
+-rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_popup_handler.py
+-rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/window_operations.py
+-rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/useful.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.019899 pybenutils-3.3.0/pybenutils/utils_logger/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/utils_logger/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/utils_logger/config_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.946097 pybenutils-3.3.0/pybenutils.egg-info/
+-rw-rw-rw-   0        0        0     4311 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.3.0/requirements.txt
+-rw-rw-rw-   0        0        0      243 2023-07-19 09:54:21.027879 pybenutils-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2311 2023-07-19 08:57:33.000000 pybenutils-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.022891 pybenutils-3.3.0/tests/
+-rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.3.0/tests/test_self_import.py
```

### Comparing `pybenutils-3.2.3/LICENSE` & `pybenutils-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/PKG-INFO` & `pybenutils-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: pybenutils
-Version: 3.2.3
+Version: 3.3.0
 Summary: PyBEN Utilities repository
 Home-page: https://github.com/DarkFlameBEN/pybenutils.git
 Author: Ben Moskovitch
 Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
 License: MIT License
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pybenutils
 PyBEN Utilities repository, Contains a variety of useful methods and classes designed to allow easy access to high level operations
```

### Comparing `pybenutils-3.2.3/README.md` & `pybenutils-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/deployment_checklist.md` & `pybenutils-3.3.0/deployment_checklist.md`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/amazon_boto3/amazon_obj.py` & `pybenutils-3.3.0/pybenutils/amazon_boto3/amazon_obj.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/autogui/__main__.py` & `pybenutils-3.3.0/pybenutils/autogui/__main__.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/autogui/auto_gui_cls.py` & `pybenutils-3.3.0/pybenutils/autogui/auto_gui_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/browsers/chrome.py` & `pybenutils-3.3.0/pybenutils/browsers/chrome.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/browsers/firefox.py` & `pybenutils-3.3.0/pybenutils/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/browsers/selenium_utils.py` & `pybenutils-3.3.0/pybenutils/browsers/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/browsers/simple_browser_controller_cls.py` & `pybenutils-3.3.0/pybenutils/browsers/simple_browser_controller_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/browsers/web_driver.py` & `pybenutils-3.3.0/pybenutils/browsers/web_driver.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/browsers/windows_browsers_keywords.py` & `pybenutils-3.3.0/pybenutils/browsers/windows_browsers_keywords.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/network/download_manager.py` & `pybenutils-3.3.0/pybenutils/network/download_manager.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/network/http_cert_info.py` & `pybenutils-3.3.0/pybenutils/network/http_cert_info.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/network/s3_bucket_cls.py` & `pybenutils-3.3.0/pybenutils/network/s3_bucket_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/network/ssh_helper.py` & `pybenutils-3.3.0/pybenutils/network/ssh_helper.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/files_and_directories.py` & `pybenutils-3.3.0/pybenutils/os_operations/files_and_directories.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/mac_application_control.py` & `pybenutils-3.3.0/pybenutils/os_operations/mac_application_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,22 @@
         self.application_process_name = None  # dynamically inserted in the launch method
         self.bundle_id = None
         self.system_level_application_name = system_level_application
         self.elements_in_current_view = []
 
     def get_application_process_name(self):
         if not self.application_process_name:
-            get_application_process_name_script = \
-                'tell application "{sys_app}" \n set application_id to (get the id of application "{app_name}" as ' \
-                'string) \n set process_name to name of (application processes where bundle identifier is ' \
-                'application_id) \n end tell'.format(sys_app=self.system_level_application_name, app_name=self.app_name)
+            get_application_process_name_script = f"""
+            tell application "{self.system_level_application_name}"
+                if (name of processes) contains appName then
+                    set application_id to (get the id of application "{self.app_name}" as string)
+                    set process_name to name of (application processes where bundle identifier is application_id)
+                end if
+            end tell
+            """
             name = run_apple_script(get_application_process_name_script)
             if name:
                 logger.debug('Application process name is: {}'.format(name))
                 self.application_process_name = name.strip()
         return self.application_process_name
 
     def launch(self, arguments=None, timeout=60):
```

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/mac_input_control.py` & `pybenutils-3.3.0/pybenutils/os_operations/mac_input_control.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/mac_operations.py` & `pybenutils-3.3.0/pybenutils/os_operations/mac_operations.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/mac_popup_handler.py` & `pybenutils-3.3.0/pybenutils/os_operations/mac_popup_handler.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/process.py` & `pybenutils-3.3.0/pybenutils/os_operations/process.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/os_operations/window_operations.py` & `pybenutils-3.3.0/pybenutils/os_operations/window_operations.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/useful.py` & `pybenutils-3.3.0/pybenutils/useful.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils/utils_logger/config_logger.py` & `pybenutils-3.3.0/pybenutils/utils_logger/config_logger.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/pybenutils.egg-info/PKG-INFO` & `pybenutils-3.3.0/pybenutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: pybenutils
-Version: 3.2.3
+Version: 3.3.0
 Summary: PyBEN Utilities repository
 Home-page: https://github.com/DarkFlameBEN/pybenutils.git
 Author: Ben Moskovitch
 Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
 License: MIT License
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pybenutils
 PyBEN Utilities repository, Contains a variety of useful methods and classes designed to allow easy access to high level operations
```

### Comparing `pybenutils-3.2.3/pybenutils.egg-info/SOURCES.txt` & `pybenutils-3.3.0/pybenutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybenutils-3.2.3/setup.py` & `pybenutils-3.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
 from codecs import open
 import platform
 import pybenutils
+import os
 
 
+scriptFolder = os.path.dirname(os.path.realpath(__file__))
+os.chdir(scriptFolder)
+
 with open(r'requirements.txt') as req_file:
     requirements_list = [line.strip() for line in req_file.readlines() if
                          not line.strip().startswith('#') and not line.strip().startswith('-') and line.strip()]
 
 final_requirements_list = list(requirements_list)
 
 # XP workaround for psutil
@@ -32,24 +36,29 @@
     long_description_content_type='text/markdown',
     url='https://github.com/DarkFlameBEN/pybenutils.git',
     author=pybenutils.__author__,
     author_email=pybenutils.__author_email__,
     license='MIT License',
     classifiers=[
         # "Development Status :: 1 - Planning",
-        "Development Status :: 2 - Pre-Alpha",
-        # "Development Status :: 3 - Alpha",
+        # "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
         # "Development Status :: 6 - Mature",
         # "Development Status :: 7 - Inactive",
         "Intended Audience :: Developers",
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         # 'Programming Language :: Python :: 2.7',
+        'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=final_requirements_list,
     include_package_data=True,
     packages=find_packages(exclude=['tests']),
     python_requires='>3'
 )
```

