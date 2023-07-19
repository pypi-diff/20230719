# Comparing `tmp/zuicorn-1.0.0.tar.gz` & `tmp/zuicorn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuicorn-1.0.0.tar", last modified: Wed Jul 19 15:41:58 2023, max compression
+gzip compressed data, was "zuicorn-1.0.1.tar", last modified: Wed Jul 19 15:55:54 2023, max compression
```

## Comparing `zuicorn-1.0.0.tar` & `zuicorn-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-19 15:41:58.000732 zuicorn-1.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-07-19 15:41:58.000732 zuicorn-1.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-19 15:41:58.000732 zuicorn-1.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-07-19 15:41:40.000000 zuicorn-1.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-19 15:41:58.000732 zuicorn-1.0.0/zuicorn/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-19 15:33:30.000000 zuicorn-1.0.0/zuicorn/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8135 2023-07-19 15:08:30.000000 zuicorn-1.0.0/zuicorn/wsgi.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-19 15:41:58.000732 zuicorn-1.0.0/zuicorn.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-07-19 15:41:57.000000 zuicorn-1.0.0/zuicorn.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-07-19 15:41:57.000000 zuicorn-1.0.0/zuicorn.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-19 15:41:57.000000 zuicorn-1.0.0/zuicorn.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-19 15:41:57.000000 zuicorn-1.0.0/zuicorn.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-19 15:41:57.000000 zuicorn-1.0.0/zuicorn.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-19 15:55:53.998452 zuicorn-1.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-19 15:55:53.998452 zuicorn-1.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-19 15:55:53.998452 zuicorn-1.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      913 2023-07-19 15:55:20.000000 zuicorn-1.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-19 15:55:53.994451 zuicorn-1.0.1/zuicorn/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-19 15:53:54.000000 zuicorn-1.0.1/zuicorn/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8159 2023-07-19 15:52:32.000000 zuicorn-1.0.1/zuicorn/wsgi.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-19 15:55:53.998452 zuicorn-1.0.1/zuicorn.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-19 15:55:53.000000 zuicorn-1.0.1/zuicorn.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2023-07-19 15:55:53.000000 zuicorn-1.0.1/zuicorn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-19 15:55:53.000000 zuicorn-1.0.1/zuicorn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-19 15:55:53.000000 zuicorn-1.0.1/zuicorn.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-07-19 15:55:53.000000 zuicorn-1.0.1/zuicorn.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-19 15:55:53.000000 zuicorn-1.0.1/zuicorn.egg-info/top_level.txt
```

### Comparing `zuicorn-1.0.0/PKG-INFO` & `zuicorn-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: zuicorn
-Version: 1.0.0
+Version: 1.0.1
 Summary: A WSGI server designed & developed for ZYLO Python web Framework.
 Home-page: https://github.com/E491K7/zuicorn
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
```

### Comparing `zuicorn-1.0.0/setup.py` & `zuicorn-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zuicorn',
-    version='1.0.0',
+    version='1.0.1',
     description='A WSGI server designed & developed for ZYLO Python web Framework.',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zuicorn',
     packages=find_packages(),
     install_requires=['gevent', 'colorama', 'python-daemon', 'zylo-admin', 'zylo'],  
     classifiers=[
@@ -14,8 +14,14 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    python_requires=">=3.6",
+    entry_points={
+        "console_scripts": [
+            "zuicorn = zuicorn.wsgi:main"
+        ]
+    },
 )
```

### Comparing `zuicorn-1.0.0/zuicorn/wsgi.py` & `zuicorn-1.0.1/zuicorn/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,15 @@
     response_time = f"{response_time:.6f}" if response_time is not None else '-'
 
     log_line = f"{remote_addr} - - [{timestamp}] \"{method} {path} {protocol}\" {status} {content_length} {response_time}"
     colored_log_line = f"[{timestamp}] {Fore.CYAN}{log_line}{Style.RESET_ALL}"
 
     print(colored_log_line)
 
-
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser(description='WSGI server')
     parser.add_argument('app', help='The WSGI application object (e.g., module:app)')
     parser.add_argument('--workers', type=int, default=4, help='Number of worker processes (default: 4)')
     parser.add_argument('--concurrency', type=int, default=1000, help='Concurrency level (default: 1000)')
     parser.add_argument('--host', default='localhost', help='Host address (default: localhost)')
     parser.add_argument('--port', type=int, default=8000, help='Port number (default: 8000)')
     parser.add_argument('--config', help='Configuration file (default: None)')
@@ -209,7 +208,11 @@
         log_dir = os.path.join(os.getenv('APPDATA'), 'zyloWSGI', 'logs')
 
     os.makedirs(log_dir, exist_ok=True)
     log_path = os.path.join(log_dir, 'wsgi.json')
 
     server.save_logs(log_path)
 
+
+if __name__ == '__main__':
+    main()
+
```

### Comparing `zuicorn-1.0.0/zuicorn.egg-info/PKG-INFO` & `zuicorn-1.0.1/zuicorn.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: zuicorn
-Version: 1.0.0
+Version: 1.0.1
 Summary: A WSGI server designed & developed for ZYLO Python web Framework.
 Home-page: https://github.com/E491K7/zuicorn
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
```

